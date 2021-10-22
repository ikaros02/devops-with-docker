FROM openjdk:8-oracle
WORKDIR /src/usr/app/
COPY ./spring-example-project .
RUN ./mvnw package
CMD ["java", "-jar" "./target/docker-example-1.1.3.jar"]
EXPOSE 8080