# Scala image

![sbt_version](https://img.shields.io/badge/sbt_version-1.2.8-blue.svg)

Image for running Scala projects using SBT.

[Docker Hub](https://hub.docker.com/r/diegoagd10/scala)

## Compiling your code

```
docker run --rm -v "$(pwd)":/app -w /app -v ~/.sbt:/root/.sbt -v ~/.ivy2:/root/.ivy2 diegoagd10/scala sh -c 'sbt clean compile'
```

## Running a Play Framework application

```
docker run -i -t --rm -v "$(pwd)":/app -w /app -v ~/.sbt:/root/.sbt -v ~/.ivy2:/root/.ivy2 -p 9000:9000 diegoagd10/scala sh -c 'sbt run'
```

## Building it locally

```
docker image build -t local/scala .
```