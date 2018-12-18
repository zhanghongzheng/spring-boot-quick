#FROM frolvlad/alpine-oraclejdk8:slim
#FROM java:alpine
#VOLUME /tmp
##WORKDIR /opt/app
#ADD quick-docker-1.0-SNAPSHOT.jar app.jar
#RUN sh -c 'touch /app.jar'
#ENV JAVA_OPTS=""
#EXPOSE 8080
#ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/quick-docker-1.0-SNAPSHOT.jar"]

FROM frolvlad/alpine-oraclejdk8:slim
VOLUME /tmp
ADD quick-docker-1.0-SNAPSHOT.jar app.jar
RUN sh -c 'touch /app.jar'
ENV JAVA_OPTS=""
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]