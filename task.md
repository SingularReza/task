1.
``` bash
> mkdir Audio
> touch song{1..10}.mp3
> mv song*.mp3 Music
> ln -s Music Audio
```
2.
```bash
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
