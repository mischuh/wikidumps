# How to load XML Wikidump into SQL DB

# German dumps

https://dumps.wikimedia.org/dewiki

# Install MySQL

docker run --name mysql -v [your data dir]:/var/lib/mysql -p 3306:3306 -e MYSQL_ROOT_PASSWORD=123admin -d mysql:latest
