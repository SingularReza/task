1.
```
> mkdir Audio
> touch song{1..10}.mp3
> mv song*.mp3 Music
> ln -s Music Audio
```
2.
```
> sudo -i
> groupadd sysadmin
> groupadd manager
> useradd -m bob -p linux123
> useradd -m rob -p linux123
> useradd -m max -p linux123
> usermod -a -G sysadmin, manager bob
> usermod -a -G sysadmin, manager rob
> usermod -a -G sysadmin max
``` 
3.
```
> chage -E `date -d "30 days" +"%Y-%m-%d"` max
> chage -d 0 bob
```
4.
```
> mkdir /home/manager 
> chgrp manager /home/manager 
> chmod 755 -R /home/manager 
```
