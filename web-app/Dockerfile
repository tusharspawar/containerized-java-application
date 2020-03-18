FROM oracle/openjdk:8

ARG APPLICATION_JAR=https://s3.amazonaws.com/tidal-fileshare-generic/187a5272-6044-4da6-af73-872efa342f1e/gs-spring-boot-0.1.0.jar
ENV NAME="${NAME:-unknown}" \
    SERVER_PORT="${SERVER_PORT:-80}"

WORKDIR /usr/src/app

RUN curl --output gs-spring-boot-0.1.0.jar $APPLICATION_JAR

EXPOSE $SERVER_PORT
CMD ["java", "-jar", "gs-spring-boot-0.1.0.jar"]
