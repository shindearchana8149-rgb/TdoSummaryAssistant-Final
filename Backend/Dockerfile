FROM eclipse-temurin:17-jdk
WORKDIR /app
COPY todo-summary-assistant/. .
RUN chmod +x mvnw
RUN ./mvnw clean package -DskipTests
EXPOSE 8080
CMD ["java", "-jar", "target/todo-summary-assistant-0.0.1-SNAPSHOT.jar"]