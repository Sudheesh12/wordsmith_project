FROM ubuntu:latest

WORKDIR /app

RUN apt-get update && apt-get install -y maven

COPY . /app/

RUN mvn verify

CMD ["java", "-Xmx8m", "-Xms8m", "-jar", "target/words.jar" ]

EXPOSE 8080