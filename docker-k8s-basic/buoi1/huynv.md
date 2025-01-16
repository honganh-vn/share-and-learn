
 Bài 1:
 docker run -d \
 --name limited-mysql \
 -e MYSQL_ROOT_PASSWORD=strongpassword123 \
 -e MYSQL_DATABASE=myapp_database \
 --cpus="0.5" \
 --memory="256m" \
 -p 3306:3306 \
 mysql:latest
 
Bài 2:
docker ps -a 
docker exec -it limited-mysql mysql -u root -p strongpassword123