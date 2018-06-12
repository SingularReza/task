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
5.
```
> useradd -u 4223 -p linux123 gabriel
```
6.
```
> tar -cvzf /tmp/var/archive.tar.bz etc/hosts
```
7.
```
> cat etc/services|grep udp>udp_services.txt
```
8.
```
> top -o+%CPU
```
9.
```
> echo -e "\nalias stat='uptime'" >> ~/.bashrc
```
10.
```
vim hello.txt
```
11.
```
> apt install firewalld
> firewall-cmd --get-default-zone
> firewall-cmd --set-default-zone=dmz
> firewall-cmd --get-zones>zones.txt
```
12.
```
> firewall-cmd --add-port=8080/tcp
> firewall-cmd --list-ports>>zones.txt
```
13.
```
> firewall-cmd --zone="public" --add-forward-port=port=80:proto=tcp:toport=8080
```
