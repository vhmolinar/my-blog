

### Database creation
Execute at project's root folder in order to ensure volume path

```sh
docker run --name my-blog-mysql -d -p 3306:3306 -v ${PWD}/db/mysqld:/var/run/mysqld -e MYSQL_ROOT_PASSWORD=admin -e MYSQL_USER=vhmolinar -e MYSQL_PASSWORD=vhmolinar -e MYSQL_DATABASE=my-blog-db mysql:8.0.34
```