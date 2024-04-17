FROM centos:7
WORKDIR /opt/
ADD https://dlcdn.apache.org/tomcat/tomcat-8/v8.5.99/bin/apache-tomcat-8.5.99.tar.gz ./
RUN tar -xzf apache-tomcat-8.5.99.tar.gz
RUN yum install java -y
ADD https://www.free-css.com/assets/files/free-css-templates/download/page296/healet.zip ./
RUN yum install unzip -y
RUN unzip healet.zip
RUN cp -rf ./healet-html/ ./apache-tomcat-8.5.99/webapps/
EXPOSE 8080
CMD ["./apache-tomcat-8.5.99/bin/catalina.sh","run"]
