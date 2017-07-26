# Docker frp
Docker image for [frp](https://github.com/fatedier/frp/).

## How to use
Run frp server:
```shell
docker run -d --name=frp-server -v /path/to/config:/opt/frp/config acrisliu/frp frps -c /opt/frp/config/frps.ini
```
Run frp client:
```shell
docker run -d --name=frp-client -v /path/to/config:/opt/frp/config acrisliu/frp frpc -c /opt/frp/config/frpc.ini
```
