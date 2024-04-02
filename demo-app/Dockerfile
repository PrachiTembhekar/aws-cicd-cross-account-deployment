FROM 12345678910.dkr.ecr.us-east-1.amazonaws.com/demo-app:latest

RUN apt-get -y update
 
RUN apt-get install -y apache2 curl

EXPOSE 80

WORKDIR /var/www/html

COPY index.html /var/www/html/index.html 

ENTRYPOINT ["/usr/sbin/apache2ctl"]

CMD ["-D", "FOREGROUND"]
EXPOSE 80
