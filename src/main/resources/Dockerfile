FROM openjdk:17-jdk-alpine
ARG JAR_FILE=target/*.jar
COPY target/backend-0.0.1-SNAPSHOT.jar /app.jar
COPY src/main/resources/application.yml /application.yml
RUN apk update && apk add mysql-client
ENTRYPOINT ["java","-jar","/app.jar"]
