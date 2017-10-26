# How to load XML Wikidump into SQL DB

# German dumps

https://dumps.wikimedia.org/dewiki

# Install MySQL

Start MySQL:

    docker run --name mysql -v mysql-data:/var/lib/mysql -p 3306:3306 -e MYSQL_ROOT_PASSWORD=123admin -d mysql:latest

Make myslq commandline tool available

    export PATH=$PATH:/Applications/MySQLWorkbench.app/Contents/MacOS

# Load dumps into database

For the first time: Generate DB Schema `wiki`

    mysql -h 123.0.0.1 -P 3306 -u root -p -v --force < mysql_wiki_tabellen.sql

Import dumps

    mysql -h 123.0.0.1 -P 3306 -u root -p -v --force wiki < dewiki-20171020-category.sql
