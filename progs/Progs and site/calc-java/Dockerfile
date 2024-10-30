FROM openjdk:11-jdk-slim

LABEL version = "1.0"

WORKDIR /progs_and_site/calc-java

COPY . /progs_and_site/calc-java/

RUN javac calc.java

RUN apt-get update && apt-get install -y bash

CMD ["java", "-cp", "/progs_and_site/calc-java", "calc"] 