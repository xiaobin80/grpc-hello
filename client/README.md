# client
    simple grpc client demo.

## dependencies

### golang.org - x
```bash
git clone https://github.com/golang/net.git $GOPATH/src/golang.org/x/net
git clone https://github.com/golang/sys.git $GOPATH/src/golang.org/x/sys
git clone https://github.com/golang/text.git $GOPATH/src/golang.org/x/text
```

### google.golang.org
```bash
git clone https://github.com/grpc/grpc-go.git $GOPATH/src/google.golang.org/grpc
git clone https://github.com/google/go-genproto.git $GOPATH/src/google.golang.org/genproto
```

## run
```bash
make build
make run
```