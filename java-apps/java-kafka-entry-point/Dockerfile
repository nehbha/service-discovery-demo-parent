FROM openjdk:8-jdk-slim
EXPOSE 8114
COPY target/java-kafka-entry-point.jar java-kafka-entry-point.jar
COPY start.sh start.sh
RUN chmod +x start.sh
RUN apt-get update
RUN apt-get install wget unzip -y
CMD ./start.sh