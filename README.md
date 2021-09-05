# node-nats-streaming-server-practice

just playing around data streaming system

## Description

using nats streaming server as a mediator that transfers a message from a sender to a receiver. In this way, it provides a loosely coupled communication way between objects, services and applications.

## Installation

```bash
# using docker image
# pull image from docker hub
docker pull nats-streaming

# build and run a container
# port: 4223 for client
# port: 8223 for monitoring
docker run -p 4223:4223 -p 8223:8223 nats-streaming nats-streaming-server -p 4223 -m 8223
```
