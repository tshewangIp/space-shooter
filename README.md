# space-shooter

## build the image for gaming site
$ docker build -t space-shooter:latest .

## run the gaming site on container
$ docker run -d -P space-shooter:latest

## check the container port and browse the site 
http://x.x.x.x:xxxx


In order to make this as docker-compse add the file called docker-compose.yml with the content
version: '3'
services:
  sapcegame:
    build: .
    ports:
     - "80"
     
     then 
run using docker-compose
$ docker-compose up -d

check the container port and browse the site
http://x.x.x.x:xxxx

