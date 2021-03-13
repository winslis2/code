## docker启动容器并挂载数据和配置
```
docker run --name mysql-slave -e MYSQL_ROOT_PASSWORD=123456 -p 3307:3306 -v /Users/lis2/myservice/mysql/slave/data/:/var/lib/mysql -v /Users/lis2/myservice/mysql/slave/conf/my.cnf:/etc/mysql/conf.d/mysqld.conf -d mysql

``