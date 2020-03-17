FROM oracle/openjdk:8

ARG APPLICATION_JAR
ENV NAME="${NAME:-unknown}" \
    SERVER_PORT="${SERVER_PORT:-80}"
    # APPLICATION_JAR="${APPLICATION_JAR}"

WORKDIR /usr/src/app

RUN curl --output gs-spring-boot-0.1.0.jar \
    $APPLICATION_JAR

EXPOSE $SERVER_PORT
CMD ["java", "-jar", "gs-spring-boot-0.1.0.jar"]
