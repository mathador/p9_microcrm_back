# MicroCRM - Backend

[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=mathador_p9_microcrm_back&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=mathador_p9_microcrm_back)
[![Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=mathador_p9_microcrm_back&metric=vulnerabilities)](https://sonarcloud.io/summary/new_code?id=mathador_p9_microcrm_back)
[![Duplicated Lines (%)](https://sonarcloud.io/api/project_badges/measure?project=mathador_p9_microcrm_back&metric=duplicated_lines_density)](https://sonarcloud.io/summary/new_code?id=mathador_p9_microcrm_back)
[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=mathador_p9_microcrm_back&metric=coverage)](https://sonarcloud.io/summary/new_code?id=mathador_p9_microcrm_back)

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
