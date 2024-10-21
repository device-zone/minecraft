# minecraft
RPM packaging for the Minecraft java server

# build instructions
This depends on the Minecraft server jar published by [Mojang](https://www.minecraft.net/en-us/download/server). After downloading
the server, import into your maven repository as follows:

```
mvn install:install-file -Dfile=server.jar -DgroupId=com.mojang -DartifactId=minecraft-server -Dversion=1.21.1 -Dpackaging=jar -DgeneratePom=true
```

To produce the RPM, run:

```
mmvn install
```

