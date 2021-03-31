# grpc-hello
simple grpc-go demo.

## Host environment settings

### install ubuntu20.04(live)
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
down protobuf [v3.15.6](https://github.com/protocolbuffers/protobuf/releases/download/v3.15.6/protobuf-cpp-3.15.6.tar.gz).
```bash
pscp e:\docker-soft\protobuf-cpp-3.15.6.tar.gz tdtc@192.168.188.11:/home/tdtc/

pscp e:\docker-soft\go1.15.10.linux-amd64.tar.gz tdtc@192.168.188.11:/home/tdtc
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

### [install go on ubuntu](https://tecadmin.net/install-go-on-ubuntu/)

down [Go](https://dl.google.com/go/go1.15.10.linux-amd64.tar.gz)
```bash
sudo mkdir -p /usr/local/go
sudo tar zxvf go1.15.10.linux-amd64.tar.gz -C /usr/local/go
```
rename:
```bash
cd /usr/local/go
sudo mv go 1.15
```

#### set path
```bash
vi ~/.bashrc
```

```bash
export GOROOT=/usr/local/go/1.15

export GOPATH=/home/tdtc/go

PATH=$PATH:$GOROOT/bin:$GOPATH/bin
```

```bash
source ~/.bashrc
```

test:
```bash
go version
```

### set proxy(ubuntu)
```bash
export https_proxy="http://192.168.188.10:1080"
```

### lib
```bash
go get -u github.com/golang/protobuf/protoc-gen-go
```
