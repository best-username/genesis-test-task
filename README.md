# Hello there! 
It is test case for https://github.com/AndriiPopovych/gses/blob/main/gses2swagger.yaml 

by Andrii Yarosh

### How to launch project:

1. Create a folder for new project and paste:

git clone git@github.com:best-username/genesis-test-task.git .

2. Make sure that you have proper .env file

cp .env.example .env

and change some staff there:

MAIL_MAILER=log

3. Build app

docker-compose build app

4. Up containers

docker-compose up -d

5. Go inside the container and make some staff

docker-compose exec app composer install

docker-compose exec app php artisan key:generate

6. Use Swagger to check that everything fine

Go to: https://editor.swagger.io/ and paste there https://github.com/AndriiPopovych/gses/blob/main/gses2swagger.yaml and change host: "gses2.app" to "127.0.0.1:8000"
