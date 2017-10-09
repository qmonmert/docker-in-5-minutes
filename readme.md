# Docker in 5 minutes

## Create a Web Server

* node index.js 

## Build docker

* docker build -t qmonmert/success .

## Run docker

* docker run -d -p 8626:8626 qmonmert/success

## Clean up

* docker stop $(docker ps -a -q --filter ancestor=qmonmert/success)  
* docker rm $(docker ps -a -q --filter status=exited)  
* docker rmi qmonmert/success

## Ref

* https://johnpapa.net/docker-in-5/
