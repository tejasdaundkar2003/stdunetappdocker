



FROM centos:7
RUN yum install java-11-openjdk -y 
ADD https://dlcdn.apache.org/tomcat/tomcat-8/v8.5.99/bin/apache-tomcat-8.5.99.tar.gz /opt/
RUN tar -xzvf /opt/apache-tomcat-8.5.99.tar.gz -C /opt/
COPY student.war webapps/student.war
COPY context.xml conf/context.xml
COPY mysql-connector.jar lib/mysql-connector.jar
EXPOSE 8082
CMD bin/catalina.sh start
