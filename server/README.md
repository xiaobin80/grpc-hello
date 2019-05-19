# server
Docker support.

## Down lib
```bash
go get -u github.com/golang/protobuf/protoc-gen-go
```
If you are trying to access grpc-go from within China, please see the [FAQ](https://github.com/grpc/grpc-go#FAQ) below.
### google.golang.org
```bash
git clone https://github.com/grpc/grpc-go.git $GOPATH/src/google.golang.org/grpc
git clone https://github.com/google/go-genproto.git $GOPATH/src/google.golang.org/genproto
```
### golang.org - x
```bash
git clone https://github.com/golang/net.git
git clone https://github.com/golang/sys.git
git clone https://github.com/golang/text.git
```

## Server
```bash
make build
make run
```