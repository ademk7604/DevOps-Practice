# Getting Started
DOCKER
### ============= docker login =============
```
docker login   --username mimaraslan     --password 123456789
```
```
docker login   -u         mimaraslan     -p        123456789
```

### ============= nginx ============= DIŞ_PORT:İÇ_PORT

DIS_PORT.IC_PORT
```
docker run     -it     -d     -p 9991:80     --name my-nginx      nginx
```
http://localhost:9991

### ============= postgres =============
```
docker run  --name my-postgres   -p 9999:5432  -e POSTGRES_PASSWORD=123456789  -d  postgres
```
### ============= mysql =============
```
docker run  --name my-mysql      -p 9990:3306  -e MYSQL_ROOT_PASSWORD=123456789 -d  mysql
```
### ============= Docker container adını değiştirne =============
```
docker container rename my-app5 my-app1
```

### ============= kendi projemizi Docker image haline çevimek =============
docker build  --build-arg --tag
```
docker build  --build-arg JAR_FILE=target/devops-practice-01-1.0.1.jar   --tag    ademk7604/devops-practice-01:v001   .

docker build  --build-arg JAR_FILE=target/devops-practice-01-1.0.2.jar   --tag    ademk7604/devops-practice-01:v002   .

docker build  --build-arg JAR_FILE=target/devops-practice-01-1.0.2.jar   --tag    ademk7604/devops-practice-01:latest   .
```
docker container rename devops-practice07 devops-practice08

