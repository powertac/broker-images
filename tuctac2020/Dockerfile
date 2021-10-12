FROM openjdk:11-jre-slim
WORKDIR /opt/powertac/broker

RUN apt-get update \
    && apt-get -y install --no-install-recommends wget unzip \
    && apt-get -y autoremove \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*

RUN wget https://www.powertac.org/wiki/images/3/31/TUC_TAC.zip \
    && unzip -p TUC_TAC.zip TUC_TAC/TUC_TAC_2020.jar > TUC_TAC_2020.jar \
    && rm TUC_TAC.zip

ENTRYPOINT ["java", "-jar", "/opt/powertac/broker/TUC_TAC_2020.jar"]