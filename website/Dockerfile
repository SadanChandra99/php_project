FROM ubuntu:22.04

RUN apt-get update 

RUN apt-get install apache2 -y

RUN apt-get install php8.1-common -y

RUN rm /var/www/html/index.html
 
COPY ./index.php /var/www/html

EXPOSE 80

CMD ["apachectl", "-D" ,"FOREGROUND"]