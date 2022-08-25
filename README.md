# linux-cli

### FILE 
*capital letters is variables*
- move file to directory  : mv FILENAME ./dir
- change file name        : mv FILENAME(old) FILENAME(new)
- delete file             : rm FILENAME
- delete directory        : rm -d DIRECTORY-NAME

### ENV
![This is an image](/assets/env/Screen Shot 2022-08-25 at 23.27.10.png)
- create env : NAME_ENV=value-env -> export NAME_ENV
- change env : NAME_ENV=value-env -> export NAME_ENV -> NAME_ENV=update
- create readonly env : readonly NAME_ENV=value-env -> export NAME_ENV
- check env : echo "$ENV-NAME"
