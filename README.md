
Assignment1: 
Steps:
>Used an EC2 ubuntu free-tier host
>Installed docker
>Pulled an ubuntu image from DockerHub
>Installed apache2 on ubuntu container
>Created a custom image from the container.
>Pushed custom image to DockerHub repo 
"https://hub.docker.com/repository/docker/secabhk/ubuntu-apache2"


Assignment2: 

Dockerfile used: 

-----------------------

FROM ubuntu 
RUN apt-get update
RUN apt-get install -y apache2
ADD ./index.html /var/www/html
CMD apachectl -D FOREGROUND

-----------------------  

