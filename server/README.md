# server
Docker support.

## Proxy
If you are trying to access Go from within China, please set proxy.
> v1.13+
```bash
go env -w GO111MODULE=on
go env -w GOPROXY=https://goproxy.io,direct
```

## docker image(china)

### edit json
> sudo vi /etc/docker/daemon.json

```bash
{
    "registry-mirrors":["https://almtd3fa.mirror.aliyuncs.com"]
}
```

### restart docker
```bash
sudo service docker restart
```

## Server
```bash
make build
make run
```