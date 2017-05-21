# GoCD Docker Compose

This is a docker-compose script to run [GoCD-Server](https://github.com/gocd/docker-gocd-server) and one [GoCD-Worker (Ubuntu 16.04)](https://github.com/gocd/docker-gocd-agent-ubuntu-16.04) together.

## Getting Started

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