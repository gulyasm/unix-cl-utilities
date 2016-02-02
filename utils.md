# Utilities you should know

## find
Find files with filters. Use exec to execute commands on the the results.
```bash
find . -iname .git -type d -exec dirname {} \;
```

## locate
Find files using a DB. Very fast, but can't restrict queries like with `find`.
```bash
locate *.tar.gz | grep Downloads
```

## grep
Very powerful search text.
```bash
grep -A 5 -r "ERROR" *
```

## top
Minimalistic resource, process monitoring.
```bash
 top
```

## htop
Pumped version of top.
```bash
htop
```

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
Disk free utility.
```bash
df -h
```

## du
Disk usage utility
```bash
du -sh ~/* 2> /dev/null | sort -hr | head -20
```

## pgrep
Process grep.
```bash
pgrep chrome
```
## ps

## netstat
Network monitoring tool.
To check listening ports, use the following.
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
DNS utility. You can query DNS services with `dig`.
```bash
dig google.com +short A
dig google.com +stat
```

## seq
Generate numbers. Useful in pipelines, generating atttributes.
```bash
seq 20
```

## parallel
Run commands parallel. Great alternative in many cases for xargs, but you can run any command with parallel.
```bash
time seq 100 | curl --silent index.hu > /dev/null
time seq 100 | parallel -n0 curl --silent index.hu > /dev/null
```
To compress many files parallel:
```bash
parallel gunzip ::: *
```

## iotop

## uuidgen
```bash
uuidgen -r
```

## file
```bash
uuidgen > testfile && file testfile
```

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
```bash
curl -I http://cnn.com
```

## free
```bash
free -h
```
## cat
```bash
cat -E ~/.vimrc
```

## whatis
```bash
whatis tac
```

## which
```bash
which go
```

## whereis
```bash
whereis pip
```

## less
less is more than more

## more
more is less than less

## units
```bash
units "2.3 pounds" kg
```
```bash
function lbs { units "$1 lbs" kg; }
```

## ascii

## mtr

## cal
```bash
ncal -n3
```

## tac
Print file in reverse order.

## factor

## yes
```bash
yes yes | head -100 | slack --topic=offtopic
```

## nl
```bash
shuf -n 10 /usr/share/dict/words | nl
```

## expand

## dos2unix
Ever received file from a Windows user. dos2unix converts files from and to UNIX format.
```bash
dos2unix *
```

## whoami
```bash
less  /home/`whoami`/.vimrc
```

## diff

## sort

## uniq

## shuf
Random sample from file.

## last
```bash
last -5 -i
```

## tree

## stat
```bash
stat -f .vimrc -c %s*%a | bc | numfmt --to iec
```
```bash
stat .vimrc -c %U
```
```bash
stat -c %X .vimrc
```
## expr

## pv

## look
To find a word in the dictionary, use look:

## at

## convert

## lsb_release
```bash
lsb_release -is
```
```bash
lsb_release -ss
```

## uname
```bash
uname -o
```

## pdfunite

## base64

## tr

## apropos
# true
# false
# md5sum
# numfmt
# split

# realpath
```bash
realpath ../
```

# expand
Converts tabs to spaces.

# unexpand
Converts spaces to tabs.

# fmt
```bash
fmt -w 50 mytext
```
