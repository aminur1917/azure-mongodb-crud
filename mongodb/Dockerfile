# Use an OpenJDK image
FROM openjdk:17-jdk-alpine

# Set the JAR file
ARG JAR_FILE=target/*.jar

# Copy the jar file into the container
COPY ${JAR_FILE} app.jar

# Run the jar file
ENTRYPOINT ["java", "-jar", "/app.jar"]