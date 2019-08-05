#This sample docker for testapp front end
FROM centos:7
MAINTAINER deepu19t@gmail.com
RUN yum -y update ;yum -y install httpd 
#COPY code/index.html /var/www/html
ADD code/index.html /var/www/html
ENV BACKENLB=test
EXPOSE 80
CMD ["apachectl", "-D", "FOREGROUND"]
COPY config/httpd-foreground /usr/bin
RUN chmod 755 /usr/bin/httpd-foreground
CMD ["httpd-foreground"]chmod