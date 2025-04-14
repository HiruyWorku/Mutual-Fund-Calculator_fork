# Use Maven image with Java 17
FROM maven:3.9.3-eclipse-temurin-17

# Set working directory
WORKDIR /app

# Copy all backend files
COPY . .

# Build the application and skip tests
RUN ./mvnw clean package -DskipTests

# Run the built Spring Boot app
CMD ["java", "-jar", "target/mutualfunds-0.0.1-SNAPSHOT.jar"]
