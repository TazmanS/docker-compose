# Time Application

Time application consists of the frontend and backend parts
Frontend is written with help of the Vue.js framework
Backend is written using Node.js and Express
Database is MySQL

docker ps 
docker images
docker container prune

docker exec -it e0f3dc9cb752 bash
docker run -v ${PWD}:/usr/share/nginx/html -p 8080:80 -d nginx
--rm -автомат удаление
\ - перенос строки

docker run \
  --name my-nginx \
  -v ${PWD}:/usr/share/nginx/html \
  -p 8080:80 \
  -d \
  --rm \
  nginx

  docker run `
  --name my-nginx `
  -v ${PWD}:/usr/share/nginx/html `
  -p 8080:80 `
  -d `
  --rm `
  nginx

docker container inspect 10dadc4ffa77

docker build . -t my-project:1.1.1  - создание образ (image)
docker run my-project


docker-compose up - запускает все сервисы
docker-compose down - stop and delete 
docker-compose up -d --build - запускает все сервисы в фоновом режиме и принудительно пересобирает образы перед запуском.
docker logs 0f86a1c3e15f

docker exec -it d21f145cb600 sh - зайти в контейнер через консоль
docker run -d -e MY_ENV_VARIABLE=test nginx - задать переменную

docker volume ls - посмотреть volumes
docker inspect volume_id