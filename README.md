# example-springboot-dockerfile
- springboot web app
- maven
- dockerfile

This example builds and deploys a SpringBoot inside Docker using Apache Maven

To build and run it:
mvn install -Ddocker.host=tcp://192.168.99.100:2376 -Pbuild-docker-image
docker run -t -i -p 9090:8080 jtpark-dockerimage/example-springboot-docker

http://192.168.99.100:9000/

