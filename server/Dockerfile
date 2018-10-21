FROM resin/raspberrypi3-openjdk:latest

WORKDIR /usr/src/app

COPY build/distributions/server-1.0-SNAPSHOT.zip ./

RUN unzip server-1.0-SNAPSHOT.zip

# Enable systemd init system in container
ENV INITSYSTEM on

CMD ["./server-1.0-SNAPSHOT/bin/server"]
