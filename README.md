# linux-cli

## List of Content
  - [systemctl](#systemctl)

### SEACRH FILE
1. find   :
2. locate :   

### FILE 
*capital letters is variables*
1. move file to directory  : mv FILENAME TUJUAN-DIRECTORY
2. COPY file               : cp FILENAME TUJUAN-DIRECTORY
3. change file name        : mv FILENAME(old) FILENAME(new)
4. create file             : touch FILENAME
5. create many file        : touch FILENAME{1..N}
6. delete file             : rm FILENAME
7. delete all file         : rm *
8. delete all file. tapi, akan dimintai izin dulu apakah file itu akan di hapus : rm -i *

### DIRECTORY
*-d : directory*
*-r : recursive*
1. delete directory kosong : rm -d DIRECTORY-NAME 
2. hapus folder beserta isinya : rm -r DIRECTORY-NAME
3. menampilkan isi folder : ls
4. menampilkan isi folder tertentu : l NAMAFILE / ls NAMAFILE?.txt

### systemctl
#### list
```
systemctl list-units --type=service
```
or
```
systemctl --type=service
```

### ENV
- create env : NAME_ENV=value-env -> export NAME_ENV 
> ![This is an image](/test.png)
- change env : NAME_ENV=value-env -> export NAME_ENV -> NAME_ENV=update
- create readonly env : readonly NAME_ENV=value-env -> export NAME_ENV
- check env : echo "$ENV-NAME"
