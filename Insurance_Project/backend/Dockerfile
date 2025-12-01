FROM eclipse-temurin:17-jdk-alpine

WORKDIR /app

# Copy JAR file
COPY target/CrudOperation-0.0.1-SNAPSHOT.jar CrudOperation-0.0.1-SNAPSHOT.jar

# Add environment variables for MySQL
ENV SPRING_DATASOURCE_URL=jdbc:mysql://mysql:3306/mydb?useSSL=false&allowPublicKeyRetrieval=true&createDatabaseIfNotExist=true
ENV SPRING_DATASOURCE_USERNAME=root
ENV SPRING_DATASOURCE_PASSWORD=root

# Expose backend port
EXPOSE 8089

# Start the application
ENTRYPOINT ["java", "-jar", "CrudOperation-0.0.1-SNAPSHOT.jar"]

