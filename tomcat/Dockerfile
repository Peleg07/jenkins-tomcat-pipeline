FROM tomcat:latest

COPY ./webapp/app.war /usr/local/tomcat/webapps/
COPY context.xml /usr/local/tomcat/conf/Catalina/localhost/
COPY context.xml /usr/local/tomcat/webapps.dist/manager/META-INF/
COPY context.xml /usr/local/tomcat/webapps.dist/host-manager/META-INF/
COPY tomcat-users.xml /usr/local/tomcat/conf/

CMD ["catalina.sh", "run"]
