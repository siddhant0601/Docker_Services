FROM ubuntu:latest #base image 
LABEL "author "="rana"
LABEL "project"="htmlFromTOOPlate"
ENV DEBIAN_FRONTEND=noninteractive
RUN apt update && install apache2 -y
CMD ["/usr/sbin/apache2ctl","-D","FOREGROUND"]
EXPOSE 80 
WORKDIR /var/www/html
VOLUME /var/log/apache2
ADD nano.tar.gz /var/www/html #also extract the tar
#COPY nano.tar.gx /var/www/html only copy the tar without extracting 