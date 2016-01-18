# Commands
- Cat with line endings
    `cat -E <filename>`

- Sort child directories and files by human readable size
    `du -ks * | sort -nr`

- Recursively install and download dependencies for offline use every maven project. 
    `find . -iname 'pom.xml' -execdir mvn install dependency:go-offline -f {} \;`

- Create temporary file
    `mktemp`

- Create temporary folder
    `mktemp -d`

- Changing every space to underscore recursively in file names
    `find $1 -depth -name "* *" -execdir rename 's/ /_/g' "{}" \;`
