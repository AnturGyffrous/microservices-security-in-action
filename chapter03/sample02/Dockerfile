FROM maven:3.9.8-eclipse-temurin-11-focal

WORKDIR /app

COPY *.xml ./
COPY src ./src

RUN mvn clean install

EXPOSE 9090

ENTRYPOINT ["mvn", "spring-boot:run", "-Dspring-boot.run.profiles=docker"]
