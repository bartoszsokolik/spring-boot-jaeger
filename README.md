##Usage
Pull jaeger from docker hub
```
docker pull jaegertracing/all-in-one
```
and run
```
docker run --rm -it --network=host jaegertracing/all-in-one
```

Jaeger UI will be available at `http://localhost:16686`

Run spring-boot application
```
./mvnw spring-boot:run
```

and curl one of the endpoints
```
curl -v http://localhost:8080/hello
```

```
curl -v http://localhost:8080/chaining
```
