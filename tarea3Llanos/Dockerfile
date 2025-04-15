# Usa una imagen base de Java 21
FROM eclipse-temurin:21-jdk

# Copia el JAR generado al contenedor
ARG JAR_FILE=target/*.jar
COPY ${JAR_FILE} app.jar

# Expone el puerto donde corre Spring Boot
EXPOSE 8080

# Comando para ejecutar la app
ENTRYPOINT ["java", "-jar", "app.jar"]
