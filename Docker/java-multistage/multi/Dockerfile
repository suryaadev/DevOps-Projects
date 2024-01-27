# Stage:1 compile java app

FROM openjdk:11-jdk AS builder

WORKDIR /app

COPY Calculator.java /app/

RUN javac Calculator.java

RUN jar -cvfe Calculator.jar Calculator Calculator.class

# Stage:2 Create runtime image

FROM gcr.io/distroless/java:11

WORKDIR /app

COPY --from=builder /app/Calculator.jar /app/

CMD ["Calculator.jar"]
