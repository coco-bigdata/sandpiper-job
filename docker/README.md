```shell
mvn clean package

cd docker
sudo docker-compose up datax-web-mysql
sudo docker-compose up -d datax-web-mysql
sudo docker-compose down
sudo docker-compose up
sudo docker-compose up -d

sudo docker-compose build
sudo docker-compose build datax-web-admin
sudo docker-compose build datax-web-executor

sudo docker-compose up datax-web-admin
sudo docker-compose up -d datax-web-admin
sudo docker-compose stop datax-web-admin

sudo docker-compose up datax-web-executor
sudo docker-compose up -d datax-web-executor
sudo docker-compose stop datax-web-executor

mysql -h127.0.0.1 -uroot -p -P3312
root
create database dataxweb default character set utf8mb4 collate utf8mb4_unicode_ci;

mysql -h127.0.0.1 -uroot -p -P3312 dataxweb < bin/db/datax_web.sql

mvn clean package

cd docker
cp ../datax-admin/target/datax-admin-2.1.2.jar datax-fe/
cp ../datax-executor/target/datax-executor-2.1.2.jar datax-fe/

sudo docker-compose build
sudo docker-compose build datax-web-admin
sudo docker-compose build datax-web-executor

https://data1.yongchehang.com/index.html
admin
123456

https://sgcc.7otech.com/index.html
admin
123456

docker_datax-web-executor
docker_datax-web-admin

sudo docker tag docker_datax-web-admin:latest yiluxiangbei/centos7-bigdata-dataxweb-admin:latest
sudo docker tag docker_datax-web-executor:latest yiluxiangbei/centos7-bigdata-dataxweb-executor:latest

sudo docker push yiluxiangbei/centos7-bigdata-dataxweb-admin:latest
sudo docker push yiluxiangbei/centos7-bigdata-dataxweb-executor:latest

update job_jdbc_datasource set jdbc_username='yRjwDFuoPKlqya9h9H2Amg==' where id=4;
update job_jdbc_datasource set jdbc_username='XCYVpFosvZBBWobFzmLWvA==' where id=4;
update job_jdbc_datasource set jdbc_username='',jdbc_password='' where id=4;

yRjwDFuoPKlqya9h9H2Amg==
XCYVpFosvZBBWobFzmLWvA==
```
