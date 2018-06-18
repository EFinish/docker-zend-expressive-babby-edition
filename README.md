# docker-zend-expressive-babby-edition
A basic seed for setting up a zend expressive application within a local docker container.

Step 1. Clone/download this repo and go go into the primary folder in your cli.

Step 2. Run the following command. Replace "projectName" with the name you want for the application.
See https://docs.zendframework.com/zend-expressive/v3/getting-started/quick-start/ for more information.

composer create-project zendframework/zend-expressive-skeleton projectName

Step 3. Within docker/nginx/default.conf replace "projectName" in "root /var/www/html/projectName/public;" with whatever you named your project. 

For example:
If you did this,

composer create-project zendframework/zend-expressive-skeleton clockCountingApplication

then replace with the following in docker/nginx/default.conf

root /var/www/html/clockCountingApplication/public;

Step 4. Start Containers

With realtime request watching
docker-compose up

Without realtime request watching
docker-compose up -d

Shut down docker containers
docker-compose down