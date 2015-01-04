- Sort child directories and files by human readable size

    `du -ks * | sort -nr`

- Recursively install and download dependencies for offline use every maven project. 

    `find . -iname 'pom.xml' -execdir mvn install dependency:go-offline -f {} \;`

