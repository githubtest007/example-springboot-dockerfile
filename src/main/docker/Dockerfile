FROM java:8
VOLUME /tmp
ADD example-springboot-docker-0.0.1-SNAPSHOT.jar app.jar
RUN bash -c 'touch /app.jar'
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-Dfile.encoding=utf-8","-Duser.timezone=GMT+09:00","-jar","/app.jar"]
