BT1:
docker run --name docker_btvn_1 -e MYSQL_DATABASE=docker_btvn_1 -e MYSQL_ROOT_PASSWORD=1234 -e MYSQL_USER=hoang-cao-long --cpus=0.5 --memory=256m -p 3307:3306 -d mysql:8.0 
jdbc:mysql://localhost:3307/docker_btvn_1?allowPublicKeyRetrieval=true&useSSL=false
docker ps -a
docker stats

BT2:
docker exec -it docker_btvn_1 mysql -u root -p
1234
show databases;
