# Imagen base con Java
FROM eclipse-temurin:17-jdk-alpine

# Carpeta de trabajo
WORKDIR /app

# Copiar el JAR compilado (asegúrate que exista en target/)
COPY target/jardin-api.jar /app/jardin-api.jar

# Exponer el puerto interno de Spring Boot
EXPOSE 8080

# Comando para ejecutar la API
CMD ["java", "-jar", "jardin-api.jar"]
