FROM openjdk:11-jdk-slim

LABEL version = "1.0"

WORKDIR /progs_and_site/game-java

COPY . /progs_and_site/game-java/

RUN javac game.java

RUN apt-get update && apt-get install -y bash

CMD ["java", "-cp", "/progs_and_site/game-java", "game"] 