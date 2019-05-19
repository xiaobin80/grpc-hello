build:
	protoc -I. --go_out=plugins=grpc:. \
		proto/greeter.proto
	GOOS=linux GOARCH=amd64 go build -o greeter && \
    sudo docker build -t greeter .
	
run:
	sudo docker run \
	       	-p 50051:50051 \
	     greeter
