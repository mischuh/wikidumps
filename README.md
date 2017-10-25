# How to load XML Wikidump into SQL DB

# Install MySQL

docker run --name mysql -v /Users/mirko/src/private/wiki/mysql-data:/var/lib/mysql -p 3306:3306 -e MYSQL_ROOT_PASSWORD=123admin -d mysql:latest
