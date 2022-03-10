FROM openjdk:8-jre-alpine
WORKDIR /powertac/broker

RUN wget http://www.powertac.org/wiki/images/f/f3/SPOT17-Binary-Release.zip \
    && unzip -p SPOT17-Binary-Release.zip SPOT17-Binary_Release/SPOT17.jar > SPOT17.jar \
    && rm SPOT17-Binary-Release.zip

ENTRYPOINT ["java", "-jar", "/powertac/broker/SPOT17.jar"]