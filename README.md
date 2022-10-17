# linux-cli

## List of Content
  - [systemctl/systemd](#systemctl)
  - [check currently installed programs](#currently-installed-programs)
  - [uninstall program installed ubuntu](#uninstall-program-installed-ubuntu)
  - [Directory](#directory)
  - [File](#file)
  - [Search File](#search-file)
  - [ssh-keygen](#ssh-keygen)

### Search File
1. find   :
2. locate :   

### File 
*capital letters is variables*
1. move file to directory  : mv FILENAME TUJUAN-DIRECTORY
2. COPY file               : cp FILENAME TUJUAN-DIRECTORY
3. change file name        : mv FILENAME(old) FILENAME(new)
4. create file             : touch FILENAME
5. create many file        : touch FILENAME{1..N}
6. delete file             : rm FILENAME
7. delete all file         : rm *
8. delete all file. tapi, akan dimintai izin dulu apakah file itu akan di hapus : rm -i *

### Directory
*-d : directory*
*-r : recursive*
1. delete directory kosong : rm -d DIRECTORY-NAME 
2. hapus folder beserta isinya : rm -rf DIRECTORY-NAME
3. menampilkan isi folder : ls
4. menampilkan isi folder tertentu : l NAMAFILE / ls NAMAFILE?.txt
5. copy : cp -r [DIRECTORY-NAME] [DIRECTORY-TUJUAN]

### ssh-keygen
| **TYPE** | **SYNTAX** |
| --- | --- |
| rsa | ssh-keygen -t rsa -C "[EMAIL-NAME]" |
| ed25519 | ssh-keygen -t ed25519 -C "[EMAIL-NAME]" |
| known_hosts | ssh-keyscan [DOMAIN-NAME] >> ~/.ssh/known_hosts |


### systemctl
example :
```
[Unit]
Description=userapp

[Service]
Type=simple
Restart=always
RestartSec=5s
EnvironmentFile=/home/bobby.irawan/app/src/userapp/.env
ExecStart=/home/bobby.irawan/app/src/userapp/userapp

[Install]
WantedBy=multi-user.target
```

reference :
1. https://www.youtube.com/watch?v=N1vgvhiyq0E&t=674s
2. https://www.digitalocean.com/community/tutorials/systemd-essentials-working-with-services-units-and-the-journal
3. https://wiki.archlinux.org/title/systemd#Using_units
4. https://ma.ttias.be/auto-restart-crashed-service-systemd/
5. https://marik-marek.medium.com/systemd-service-error-handling-and-automatic-restarting-a07726717191
6. https://serverfault.com/questions/730239/start-n-processes-with-one-systemd-service-file
7. https://www.jenkins.io/doc/book/system-administration/systemd-services/


#### list [reference](https://www.tecmint.com/list-all-running-services-under-systemd-in-linux/)
```
systemctl list-units --type=service
```
or
```
systemctl --type=service
```

### currently installed programs
```
dpkg --list
```

### uninstall program installed ubuntu
```
sudo apt-get --purge remove program
```

### ENV
- create env : NAME_ENV=value-env -> export NAME_ENV 
> ![This is an image](/test.png)
- change env : NAME_ENV=value-env -> export NAME_ENV -> NAME_ENV=update
- create readonly env : readonly NAME_ENV=value-env -> export NAME_ENV
- check env : echo "$ENV-NAME"
