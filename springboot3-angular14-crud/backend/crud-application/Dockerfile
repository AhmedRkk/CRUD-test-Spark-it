# Base image
FROM openjdk:17-jdk-alpine

# Set the working directory
WORKDIR /app

# Copy the project files to the container
COPY . .

RUN apk add --no-cache maven

# Build the application
RUN mvn package -DskipTests

EXPOSE 9080
# Set the command to run the application
CMD ["java", "-jar", "target/crud-application-0.0.1-SNAPSHOT.jar"]
