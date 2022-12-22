# Docker_homework

скачиваем nginx

docker pull nginx

Зпускаем используя порт 8000

docker run --name some-nginx -d -p 8000:80 nginx 

по адресу localhost:8000 видим оригинальную страницу

Создаем образ
В папке в которой находится Dockerfile вводим команду

docker image build .

в ответ получаем id образа

запускаем контейнер используя порт 8001

docker run -d -p 8001:80 --name docker-homework < id образа >

в браузере по адресу localhost:8001 видим измененную страницу
