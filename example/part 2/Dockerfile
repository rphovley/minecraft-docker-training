FROM  openjdk:8

WORKDIR /minecraft_server

RUN curl https://launcher.mojang.com/v1/objects/1b557e7b033b583cd9f66746b7a9ab1ec1673ced/server.jar --output minecraft.server.jar

COPY minecraft_config .

EXPOSE 25565 

CMD ["java", "-Xmx1024M", "-Xms1024M", "-jar", "minecraft.server.jar", "nogui"]