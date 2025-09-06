# Start with a lightweight JDK base image
FROM openjdk:17-jdk-slim

# Add a volume for logs
VOLUME /tmp

# Copy the JAR from target to container
ARG JAR_FILE=target/retail-pipeline-demo-0.0.1-SNAPSHOT.jar
COPY ${JAR_FILE} app.jar

# Run the JAR
ENTRYPOINT ["java","-jar","/app.jar"]
