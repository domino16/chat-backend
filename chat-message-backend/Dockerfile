FROM openjdk:17-jdk-alpine
ARG JAR_FILE=target/*.jar
COPY /target/chat-message-backend-0.0.1-SNAPSHOT.jar /app.jar
COPY ./chat-app-396909-ea7f648f1e14.json .
ENV GOOGLE_APPLICATION_CREDENTIALS=./chat-app-396909-ea7f648f1e14.json
ENTRYPOINT ["java","-jar","/app.jar"]
EXPOSE 8080
