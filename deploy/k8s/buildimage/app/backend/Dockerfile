# Use an OpenJDK base image for Java
FROM ubi8/openjdk-17-runtime

# Use ADD to download the JAR directly from GitHub
ADD --chmod=755 https://github.com/kisaro247/spring-boot-reactjs-app-ow/raw/refs/heads/main/backend/target/weather-0.0.1-SNAPSHOT.jar /home/jboss/main.jar
EXPOSE 7890
CMD ["java", "-Dserver.port=7890", "-jar", "main.jar"]
