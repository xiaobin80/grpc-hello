# grpc-hello
simple grpc-go demo.
	
## Host environment settings

### install ubuntu18.04(live)
mirror:
https://mirrors.aliyun.com/ubuntu/

### install soft
```bash
sudo apt-get install ssh
sudo apt-get install build-essential
sudo apt-get install autoconf automake libtool curl make g++ unzip

sudo apt install docker.io
```
### putty(win)
down protobuf [v3.13.0](https://github.com/protocolbuffers/protobuf/releases/download/v3.13.0/protobuf-cpp-3.13.0.tar.gz).
```bash
pscp e:\docker-soft\protobuf-cpp-3.13.0.tar.gz tdtc@192.168.188.11:/home/tdtc/

pscp e:\docker-soft\go1.14.9.linux-amd64.tar.gz tdtc@192.168.188.11:/home/tdtc
```

## Protobuf
```bash
$ ./configure
$ make
$ make check
$ sudo make install
$ sudo ldconfig # refresh shared library cache.
```

## Down lib

### set proxy(ubuntu)
```bash
export https_proxy="http://192.168.188.10:1080"
```

### lib
```bash
go get -u github.com/golang/protobuf/protoc-gen-go
```
