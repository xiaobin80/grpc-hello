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
down protobuf [v3.11.2](https://github.com/protocolbuffers/protobuf/releases/download/v3.11.2/protobuf-cpp-3.11.2.tar.gz).
```bash
scp f:\docker-soft\protobuf-cpp-3.11.2.tar.gz tdtc@192.168.188.11:/home/tdtc/

scp f:\docker-soft\go1.13.5.linux-amd64.tar.gz tdtc@192.168.188.11:/home/tdtc
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
```bash
go get -u github.com/golang/protobuf/protoc-gen-go
```
