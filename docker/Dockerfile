# Use OpenJDK 17 as base image (recommended for modern apps)
FROM openjdk:17-jdk-slim

# Set the working directory in the container
WORKDIR /usr/src/app

# Expose port used by the Spring Boot application
EXPOSE 8070

# Copy the compiled JAR from the target folder into the image
COPY target/shopping-cart-0.0.1-SNAPSHOT.jar app.jar

# Run the JAR file
ENTRYPOINT ["java", "-jar", "app.jar"]
