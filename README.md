# MicroCRM - Backend

Ce projet est la partie Backend de l'application MicroCRM, développée avec Spring Boot (Java 17).

## Prérequis

- JDK 17
- Gradle 8+

## Compilation et Tests


1. Construire le JAR:

   ```shell
   # Sur Linux
   ./gradlew build

   # Sur Windows
   .\gradlew.bat build
   ```

2. Démarrer le service:

   ```shell
   java -jar build/libs/microcrm-0.0.1-SNAPSHOT.jar
   ```

Puis ouvrir l'URL http://localhost:8080 dans votre navigateur.


Dans votre terminal:

```shell
.\gradlew.bat test
```
Le résultat du test sont situé dans:
```
build\reports\tests\test\index.html
```

#### Image Docker

##### Construire l'image

```shell
docker build -t orion-microcrm-back:latest .
```

##### Exécuter l'image

```shell
docker run -it --rm -p 8080:8080 orion-microcrm-back:latest
```

L'API sera disponible sur http://localhost:8080.
