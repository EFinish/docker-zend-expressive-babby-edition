# docker-zend-expressive-babby-edition
basic structure for setting up a zend expressive application within a local docker container

Step 1. Clone this repo somewhere and go to it in your cli.

Step 2. Install dependencies via composer () (TODO flusht his out more)

composer install

Step 3. Create a Zend expressive skeleton via composer.

composer create-project zendframework/zend-expressive-skeleton expressive

See https://docs.zendframework.com/zend-expressive/v3/getting-started/quick-start/ for more information.

Step 4. Start Containers

With realtime request watching
docker-compose up

Without realtime request watching
docker-compose up -d

Shut down docker containers
docker-compose down