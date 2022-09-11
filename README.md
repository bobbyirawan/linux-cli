# linux-cli

### FILE 
*capital letters is variables*
1. move file to directory  : mv FILENAME TUJUAN-DIRECTORY
2. COPY file               : cp FILENAME TUJUAN-DIRECTORY
3. change file name        : mv FILENAME(old) FILENAME(new)
4. delete file             : rm FILENAME

### DIRECTORY
* -d : directory
* -r : recursive
1. delete directory kosong : rm -d DIRECTORY-NAME 
2. hapus folder beserta isinya : rm -r DIRECTORY-NAME


### ENV
- create env : NAME_ENV=value-env -> export NAME_ENV 
> ![This is an image](/test.png)
- change env : NAME_ENV=value-env -> export NAME_ENV -> NAME_ENV=update
- create readonly env : readonly NAME_ENV=value-env -> export NAME_ENV
- check env : echo "$ENV-NAME"
