FROM 192.168.1.101:5000/public/web_base
MAINTAINER songhaitao
	
VOLUME /tmp
COPY target/*.jar /opt/
WORKDIR /opt
RUN rm -rf start-site.jar && rm -rf *docker-info.jar && mkdir /opt/webserver && mv *.jar /opt/webserver/app.jar
EXPOSE 8080
ENTRYPOINT ["java","-jar","/opt/webserver/app.jar"]
