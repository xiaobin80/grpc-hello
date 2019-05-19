build:
	protoc -I. --go_out=plugins=grpc:. \
		proto/greeter.proto
	
run:
	go run main.go
