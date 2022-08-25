# linux-cli

### FILE 
*kapital is variable
- move file to directory  : mv FILENAME ./dir
- change file name        : mv FILENAME(old) FILENAME(new)
- delete file             : rm FILENAME
- delete directory        : rm -d DIRECTORY-NAME

### ENV
- create env : NAME_ENV=value-env -> export NAME_ENV
- change env : NAME_ENV=value-env -> export NAME_ENV -> NAME_ENV=update
- create readonly env : readonly NAME_ENV=value-env -> export NAME_ENV
- check env : echo "$ENV-NAME"
