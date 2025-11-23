FROM bellsoft/liberica-openjdk-debian:17
WORKDIR /app
COPY target/*.jar backend.jar
EXPOSE 8089 
ENTRYPOINT ["java", "-jar", "backend.jar"]

