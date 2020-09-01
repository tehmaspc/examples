我是光年实验室高级招聘经理。
我在github上访问了你的开源项目，你的代码超赞。你最近有没有在看工作机会，我们在招软件开发工程师，拉钩和BOSS等招聘网站也发布了相关岗位，有公司和职位的详细信息。
我们公司在杭州，业务主要做流量增长，是很多大型互联网公司的流量顾问。公司弹性工作制，福利齐全，发展潜力大，良好的办公环境和学习氛围。
公司官网是http://www.gnlab.com,公司地址是杭州市西湖区古墩路紫金广场B座，若你感兴趣，欢迎与我联系，
电话是0571-88839161，手机号：18668131388，微信号：echo 'bGhsaGxoMTEyNAo='|base64 -D ,静待佳音。如有打扰，还请见谅，祝生活愉快工作顺利。

# Micro Examples  [![Travis CI](https://travis-ci.org/micro/examples.svg?branch=master)](https://travis-ci.org/micro/examples) [![Go Report Card](https://goreportcard.com/badge/micro/examples)](https://goreportcard.com/report/github.com/micro/examples)

This is a repository for micro examples. Feel free to contribute.

## Contents

- [api](api) - Provides API usage examples
- [booking](booking) - A booking.com demo application
- [broker](broker) - A example of using Broker for Publish and Subscribing.
- [client](client) - Usage of the Client package to call a service.
- [command](command) - An example of bot commands as micro services
- [event](event) - Using the API Gateway event handler
- [flags](flags) - Using command line flags with a service
- [form](form) - How to parse a form behind the micro api
- [function](function) - Example of using Function programming model
- [graceful](graceful) - Demonstrates graceful shutdown of a service
- [greeter](greeter) - A complete greeter example (includes python, ruby examples)
- [heartbeat](heartbeat) - Make services heartbeat with discovery for high availability
- [helloworld](helloworld) - Hello world using micro
- [metadata](metadata) - Extracting metadata from context of a request
- [options](options) - Setting options in the go-micro framework
- [plugins](plugins) - How to use plugins
- [pubsub](pubsub) - Example of using pubsub at the client/server level
- [grpc](grpc) - Examples of how to use [go-grpc](https://github.com/micro/go-grpc)
- [redirect](redirect) - An example of how to http redirect using an API service
- [roundrobin](roundrobin) - A stateful client wrapper for true round robin of requests
- [secure](secure) - Demonstrates use of transport secure option for self signed certs
- [server](server) - Use of the Server package directly to server requests.
- [service](service) - Example of the top level Service in go-micro.
- [sharding](sharding) - An example of how to shard requests or use session affinity
- [shutdown](shutdown) - Demonstrates graceful shutdown via context cancellation
- [sidecar](sidecar) - Greeter service using the sidecar with multiple languages
- [stream](stream) - An example of a streaming service and client
- [template](template) - Api, web and srv service templates generated with the 'micro new' command
- [waitgroup](waitgroup) - Demonstrates how to use a waitgroup with a service
- [wrapper](wrapper) - A simple example of using a log wrapper

## External

- [auth-srv](https://github.com/micro/auth-srv) - An Oauth2 authentication service
- [geo-srv](https://github.com/micro/geo-srv) - Geolocation tracking service using hailocab/go-geoindex
- [geo-web](https://github.com/micro/geo-web) - Web demo for the geo srv
- [geo-api](https://github.com/micro/geo-api) - API for the geo srv
- [discovery-srv](https://github.com/micro/discovery-srv) - A discovery in the micro platform
- [geocode-srv](https://github.com/micro/geocode-srv) - A geocoding service using the Google Geocoding API
- [hailo-srv](https://github.com/micro/hailo-srv) - A service for the hailo taxi service developer api
- [monitor-srv](https://github.com/micro/monitor-srv) - A monitoring service for Micro services
- [place-srv](https://github.com/micro/place-srv) - A microservice to store and retrieve places (includes Google Place Search API)
- [slack-srv](https://github.com/micro/slack-srv) - The slack bot API as a go-micro RPC service
- [trace-srv](https://github.com/micro/trace-srv) - A distributed tracing microservice in the realm of dapper, zipkin, etc
- [twitter-srv](https://github.com/micro/twitter-srv) - A microservice for the twitter API
- [user-srv](https://github.com/micro/user-srv)	- A microservice for user management and authentication

## Community

Find contributions from the community via the [explorer](https://micro.mu/explore/)

- [go-shopping](https://github.com/autodidaddict/go-shopping) - A sample product with a suite of services

## Dependencies

### Service Discovery

All services require service discovery. The default is Consul or MDNS.

#### Consul

Install
```
brew install consul
```

Run
```
consul agent -dev
```

#### Multicast DNS

Use flag `--registry=mdns` for a zero dependency configuration

### Protobuf

Protobuf is used for code generation of message types and client/hander stubs.

If making changes recompile the protos.

#### Install

Install [protoc](https://github.com/google/protobuf) for your environment. Then:

```shell
go get github.com/golang/protobuf/{proto,protoc-gen-go}
```

```shell
go get github.com/micro/protoc-gen-micro
```

#### Compile Proto

```shell
protoc --proto_path=$GOPATH/src:. --micro_out=. --go_out=. path/to/proto
```

