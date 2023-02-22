# Base image
FROM maven:3.8.4-openjdk-17-slim

# Set the working directory
WORKDIR /app

# Copy the project files to the container
COPY . .


# Build the application
RUN mvn package -DskipTests

EXPOSE 9080
# Set the command to run the application
CMD ["java", "-jar", "target/crud-application-0.0.1-SNAPSHOT.jar"]
