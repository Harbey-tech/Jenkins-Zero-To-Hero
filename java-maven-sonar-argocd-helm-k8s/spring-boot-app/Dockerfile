# Use OpenJDK 17 Alpine JRE as base image
FROM eclipse-temurin:17-jre-alpine

# Set the artifact path (from Maven build)
ARG artifact=target/spring-boot-web.jar

# Set the working directory inside the container
WORKDIR /opt/app

# Copy the JAR file into the image
COPY ${artifact} app.jar

# Start the Java application when the container starts
ENTRYPOINT ["java", "-jar", "app.jar"]
