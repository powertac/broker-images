FROM openjdk:8-jre-alpine
WORKDIR /powertac/broker

RUN apk add p7zip

RUN wget -O SPOT19.7z "https://drive.google.com/u/0/uc?id=1U3FHCkMmzECGRxJrlZx5lg4ezwUn0lpu&export=download&confirm=t" \
    && p7zip -d SPOT19.7z \
    && mv SPOT19/* . \
    && rm -rf SPOT19

ENTRYPOINT ["java", "-jar", "/powertac/broker/spot-broker-1.6.0.jar"]