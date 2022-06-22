```
Author: lightsavers
Created: 06222022
```

# Enable Network on CentOS 7 Minimal

 - Check if ethernet cards are connected to the internet
```
[yourusername@localhost ~]# nmcli d
```

 - Open network manager to configure or edit connection
```
[yourusername@localhost ~]# nmtui
```

 - Choose your network interface (using tab and space bar)
```
 -----------------------------
| Ethernet     |   <Add>      |
|	 enp0s3    |   <Edit...>  |
|	           |   <Delete>   |
|              |              |

```

 - Choose "Automatic" next to IPv4 (using tab and space bar), then tick box bext to "Automatically connect". Finally <OK>
```
            Profile name enp0s3
			      Device 00:00:27:ED:7C:42 (enp0s3) 

- ETHERNET                                        <Show>

- IPv4 CONFIGURATION <Automatic>                  <Show>
- IPv6 CONFIGURATION <Automatic>                  <Show>

[X] Automatically  connect
[X] Available to all users

                                                  <Cancel> <OK>

```

 - Reset network services (Sudo power may be needed)
```
[yourusername@localhost ~]# service network restart
```



