FROM centos:latest
RUN yum -y update && yum -y install php-gd php php-mysql httpd
ADD code /var/www/html
ENV MY_DB_NAME=test MY_DB_USER=test MY_DB_PASS=test MY_DB_HOST=test
ENV BACKENDLB = backend
cmd ["apachectl","-D","FOREGROUND"]
