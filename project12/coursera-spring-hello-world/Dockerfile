# Stage 01: BUILD
FROM maven:3.9.15-eclipse-temurin-21 AS build

WORKDIR /build

COPY ./pom.xml ./
COPY ./src ./src

RUN mvn clean package -DskipTests


# Stage 02: PRODUCTION
FROM eclipse-temurin:21-jre

WORKDIR /app

COPY --from=build /build/target/*.jar app.jar

EXPOSE 8080

CMD [ "java", "-jar", "app.jar" ]
