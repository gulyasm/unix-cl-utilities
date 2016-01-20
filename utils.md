# Utilities you should know
## find
```bash
find . -iname .git -type d -exec dirname {} \;
```
## locate
```bash
locate *.tar.gz
```
## grep
```bash
grep -A 5 -r "ERROR" *
```
## top

## htop

## mktemp
```bash
vim `mktemp`
```
Temporary directory
```bash
mktemp -d
```
## mkdir
```bash
mkdir -p photos/{2005..2016}/{1..12}
```

## fuser
```bash
ps l | grep `fuser /tmp`
```
## sed

## df
```bash
df -h
```
## du
```bash
du -sh ~/* 2> /dev/null | sort -hr | head -20
```
## pgrep
```bash
pgrep chrome
```
## ps

## netstat
```bash
sudo netstat -tulnp
```
## lsof

## tcpdump

## fg
With `Ctrl-z` you can send programs back to background. With `fg` you bring them back.

## tailf
Same as `tail -f`.
```bash
tailf /var/log/mysql.log
```

## dig
```bash
dig google.com +short A
dig google.com +stat
```

## seq
```bash
seq 20
```

## xargs

## parallel
```bash
seq 100 | curl --silent index.hu > /dev/null
```

## iotop

## file

## tee

## script

## watch
```bash
watch -n 1 tree -L 1
```

## xargs

## pwd
Prints the working directory

## basename
Prints the filename from any path.

## dirname
Strips the last component from a path.

## wget

## curl

## free
```bash
free -h
```
## cat

## whatis

## which

## whereis

## locate

## less

## more

## units

## ascii

## mtr

## cal

## tac

## factor

## yes

## nl

## expand

## dos2unix

## whoami

## diff

## file

## sort

## uniq

## shuf

## last

## tree

## stat

## expr

## pv

## look

## at

## convert

## lsb_release

## uname

## pdfunite

## base64

## tr

## apropos
```bash
apropos -a docker run
```

## truncate

## scp

## rsync
