FROM centos:7
LABEL OWER ="TEJAS"
RUN yum install httpd -y 
COPY index.html /var/www/html/
RUN chmod 777 -r /var/*
EXPOSE 80
CMD httpd -DFOREGROUND