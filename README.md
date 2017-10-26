# How to load XML Wikidump into SQL DB

# German dumps

https://dumps.wikimedia.org/dewiki

# Install MySQL

docker run --name mysql -v mysql-data:/var/lib/mysql -p 3306:3306 -e MYSQL_ROOT_PASSWORD=123admin -d mysql:latest
export PATH=$PATH:/Applications/MySQLWorkbench.app/Contents/MacOS
