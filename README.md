# random-stuff

## Download and mirror locally a website
```bash
$ wget --mirror --backup-converted --adjust-extension --random-wait --no-parent --limit-rate=200k --page-requisites --execute robots=off --user-agent=mozilla http://learnyousomeerlang.com
```

## md5 all files of a dir
```bash
$ find /you/path -type f -name "*.php" -exec md5sum {} + | sort
```

## md5 all files of a dir in one
```bash
$ find /you/path -type f -name "*.php" -exec md5sum {} + | awk '{print $1}' | sort | md5sum
```
