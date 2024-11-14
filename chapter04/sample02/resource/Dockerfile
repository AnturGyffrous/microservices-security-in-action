FROM maven:3.9.8-eclipse-temurin-11-focal

WORKDIR /app

COPY *.xml ./
COPY src ./src

RUN mvn clean install

EXPOSE 8080

ENTRYPOINT ["mvn", "spring-boot:run"]
