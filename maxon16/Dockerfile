FROM openjdk:8-jre-alpine
WORKDIR /powertac/broker

RUN wget http://www.powertac.org/wiki/images/c/c4/Maxon16.zip \
    && unzip -p Maxon16.zip maxon16.jar > maxon16.jar \
    && rm Maxon16.zip

ENTRYPOINT ["java", "-jar", "/powertac/broker/maxon16.jar"]