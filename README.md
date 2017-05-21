# GoCD Docker Compose

To start GoCD
```
docker-compose up -d
```

To stop GoCD
```
docker-compose stop
```

To stop & remove GoCD
```
docker-compose down
```

## Build GoCD Worker with Go Lang support

```
docker build -f dockerfile-golang  -t gocd-agent-ubuntu-16.04-golang .
```

After building, you may replace the worker image with `gocd-agent-ubuntu-16.04-golang` instead of `gocd/gocd-agent-ubuntu-16.04:v17.4.0`