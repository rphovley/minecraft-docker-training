FROM openjdk:8-alpine

RUN apk --no-cache add curl

RUN curl https://launcher.mojang.com/v1/objects/1b557e7b033b583cd9f66746b7a9ab1ec1673ced/server.jar \
  --output minecraft_server.1.16.5.jar

COPY minecraft_config .

CMD ["java", "-Xmx1024M", "-Xms1024M", "-jar" ,"/minecraft_server.1.16.5.jar", "nogui"]
