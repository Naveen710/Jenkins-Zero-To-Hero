# Use Java 17 base image
FROM eclipse-temurin:17-jre-alpine

# Define the build artifact
ARG artifact=target/spring-boot-web.jar

# Set the working directory inside the container
WORKDIR /opt/app

# Copy the JAR into the container
COPY ${artifact} app.jar

# Run the app
ENTRYPOINT ["java","-jar","app.jar"]
