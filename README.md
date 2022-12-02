<div align="center">
# Metadata Formatter API

<i>Formats and validates QBiC project metadata for different public repositories </i>

[![Build Maven Package](https://github.com/qbicsoftware/metadata-formatter-api/actions/workflows/build_package.yml/badge.svg)](https://github.com/qbicsoftware/metadata-formatter-api/actions/workflows/build_package.yml)
[![Run Maven Tests](https://github.com/qbicsoftware/metadata-formatter-api/actions/workflows/run_tests.yml/badge.svg)](https://github.com/qbicsoftware/metadata-formatter-api/actions/workflows/run_tests.yml)
[![CodeQL](https://github.com/qbicsoftware/metadata-formatter-api/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/qbicsoftware/metadata-formatter-api/actions/workflows/codeql-analysis.yml)
[![release](https://img.shields.io/github/v/release/qbicsoftware/metadata-formatter-api?include_prereleases)](https://github.com/qbicsoftware/metadata-formatter-api/releases)

[![license](https://img.shields.io/github/license/qbicsoftware/metadata-formatter-api)](https://github.com/qbicsoftware/metadata-formatter-api/blob/main/LICENSE)
![language](https://img.shields.io/badge/language-java-blue.svg)

</div>

## How to run

Create a runable version of this code with maven and java 8:

```
mvn clean package
```

The JAR file will be created in the ``/target`` folder

## How to use

This library is not hosted on maven central. To use it, you have to include our artifact repository to your pom.

```xml
<repositories>
    <repository>
        <releases>
            <enabled>true</enabled>
            <updatePolicy>always</updatePolicy>
            <checksumPolicy>fail</checksumPolicy>
        </releases>
        <snapshots>
            <enabled>false</enabled>
        </snapshots>
        <id>nexus-releases</id>
        <name>QBiC Releases</name>
        <url>https://qbic-repo.qbic.uni-tuebingen.de/repository/maven-releases</url>
    </repository>
</repositories>
```

Then include this library as an artifact.
```xml
<dependency>
    <groupId>life.qbic</groupId>
    <artifactId>metadata-formatter-api</artifactId>
    <version>[version-number]</version>
</dependency>
```

## Data Models and Examples

