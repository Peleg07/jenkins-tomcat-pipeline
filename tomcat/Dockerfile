FROM tomcat:latest

ARG TOMCAT_PASSWORD
ARG TOMCAT_USERNAME

RUN mv /usr/local/tomcat/webapps.dist/* /usr/local/tomcat/webapps/
COPY ./webapp/ /usr/local/tomcat/webapps/
COPY tomcat-users.xml /usr/local/tomcat/conf/
COPY context.xml /usr/local/tomcat/conf/
COPY context.xml /usr/local/tomcat/webapps/manager/META-INF/
COPY context.xml /usr/local/tomcat/webapps/host-manager/META-INF/

EXPOSE 8080

CMD ["catalina.sh", "run"]
