# Docker frp
Docker image for [frp](https://github.com/zoranke/docker-frp-arm/), based on Alpine Linux.

Current frp version: v0.27.0

## How to use
Run frp server:
```shell
docker run -d -p 7000:7000 --name=frps --restart=always -v /path/to/config:/etc/frp zoranke/docker-frp-arm
```

Run frp client:
```shell
docker run -d --name=frpc --restart=always -v /path/to/config:/etc/frp zoranke/docker-frp-arm frpc -c /etc/frp/frpc.ini
```
