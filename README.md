# mc-bukkit-server-repos

<!-- ABOUT THE PROJECT -->
## About The Project

This repos serves the bukkit jar and the craftbukkit jar in order to use them via maven. The goal was to have an easy access to those jars to install them 
into your local maven repository or include them via maven as a dependency.

## Getting Started

Clone this repository onto your local machine and execute the following 2 commands in order to install them into your local maven repository
```sh
mvn install:install-file -Dfile=./bukkit-1.14.4-R0.1-SNAPSHOT.jar -DgroupId=<group-id> -DartifactId=<artifact-id> -Dversion=<version> -Dpackaging=jar
mvn install:install-file -Dfile=./craftbukkit-1.14.4-R0.1-SNAPSHOT.jar -DgroupId=<group-id> -DartifactId=<artifact-id> -Dversion=<version> -Dpackaging=jar
```
You can then use them in your maven project as usual 
```xml
<dependency>
    <groupId>test</groupId>
    <artifactId>bukkit-mc</artifactId>
    <version>1.14.4</version>
</dependency>

<dependency>
    <groupId>test</groupId>
    <artifactId>craftbukkit-mc</artifactId>
    <version>1.14.4</version>
</dependency>
```

## License
I hereby declare that I do not own the rights to those jars / sources. All rights belong to the owner. No Copyright Infringement Intended.
