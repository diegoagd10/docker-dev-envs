
```
docker image build -t local/scala-alpine .
```

```
docker run --rm -v "$(pwd)":/app -w /app -v ~/.sbt:/root/.sbt -v ~/.ivy2:/root/.ivy2 diegoagd10/scala-alpine sh -c 'sbt clean compile'
```