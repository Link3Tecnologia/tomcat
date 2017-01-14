# link3tecnologia/tomcat:8
FROM link3tecnologia/centosjava8:7
ENV TOMCAT_VERSION=8.5.9
ENV TOMCAT_FILE=apache-tomcat-$TOMCAT_VERSION.tar.gz
ENV CATALINA_HOME=/opt/tomcat
WORKDIR  /opt
RUN wget http://mirror.nbtelecom.com.br/apache/tomcat/tomcat-8/v8.5.9/bin/$TOMCAT_FILE
RUN tar xzf $TOMCAT_FILE
EXPOSE 8080
RUN ln -s /opt/$TOMCAT_FILE /opt/tomcat
RUN ["rm", "-fr", "/opt/tomcat/webapps/ROOT"]
