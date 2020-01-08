# server
Docker support.

## Proxy
If you are trying to access Go from within China, please set proxy.
```
GOPROXY="https://gocenter.io"
export GO111MODULE=on
```

## Server
```bash
make build
make run
```