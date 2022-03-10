FROM openjdk:8-jre-alpine
WORKDIR /powertac/broker

RUN wget http://www.powertac.org/wiki/images/c/c1/AgentUDE17.zip \
    && unzip -p AgentUDE17.zip AgentUDE17/AgentUDE17.jar > AgentUDE17.jar \
    && rm AgentUDE17.zip

ENTRYPOINT ["java", "-jar", "/powertac/broker/AgentUDE17.jar"]