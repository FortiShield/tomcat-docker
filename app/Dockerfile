# Use a base image for Java
FROM openjdk:11-jre-slim

# Set the working directory
WORKDIR /app

# Copy the JAR file and JDBC driver into the container
COPY your-app.jar /app/your-app.jar
COPY mysql-connector-java.jar /app/mysql-connector-java.jar

# Copy the optional initialization SQL script (if using)
COPY ../db/init.sql /app/init.sql

# Set the command to run your JAR file
ENTRYPOINT ["java", "-cp", "your-app.jar:mysql-connector-java.jar", "your.package.MainClass"]
