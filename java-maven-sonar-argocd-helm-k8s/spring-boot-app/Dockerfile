# Use Java 17 instead of Java 11
FROM eclipse-temurin:17-jdk-alpine

# Path to your built jar
ARG artifact=target/spring-boot-web.jar

WORKDIR /opt/app

COPY ${artifact} app.jar

# Run the app
ENTRYPOINT ["java","-jar","app.jar"]
