# random-stuff

## Download and mirror locally a page
```bash
$ wget --convert-links --page-requisites --span-hosts --execute robots=off --user-agent=mozilla http://learnyousomeerlang.com
```

## Download and mirror locally a website
```bash
$ wget --mirror --backup-converted --adjust-extension --convert-links --random-wait --no-parent --limit-rate=200k --page-requisites --execute robots=off --user-agent=mozilla http://learnyousomeerlang.com
```

## md5 all files of a dir
```bash
$ find /you/path -type f -name "*.php" -exec md5sum {} + | sort
```

## md5 all files of a dir in one
```bash
$ find /you/path -type f -name "*.php" -exec md5sum {} + | awk '{print $1}' | sort | md5sum
```

## Get stats of the most expensive process
```bash
$ dstat -c --top-cpu -d --top-bio --top-latency
```

## Remove files older than 24h
```bash
$ find /path -type f -mmin +1440 -delete
```

## Remove empty directories
```bash
$ find /path -type d -empty -delete
```
