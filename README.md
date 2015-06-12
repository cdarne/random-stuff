# random-stuff

## md5 all files of a dir
```
$ find /you/path -type f -name "*.php" -exec md5sum {} + | sort
```

## md5 all files of a dir in one
```
$ find /you/path -type f -name "*.php" -exec md5sum {} + | awk '{print $1}' | sort | md5sum
```
