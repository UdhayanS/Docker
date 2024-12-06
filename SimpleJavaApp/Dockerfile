# Use an official OpenJDK image with JDK 17
FROM openjdk:21-jdk-slim

# Set the working directory inside the container
WORKDIR /app

# Copy the compiled Java class to the container
COPY Main.class .

# Command to run the Java application
CMD ["java", "Main"]
