FROM golang:1.12 as builder

RUN mkdir /app
WORKDIR /app

ENV GO111MODULE=on
ENV GOPROXY=https://goproxy.io

COPY . .

RUN CGO_ENABLED=0 GOOS=linux go build -a -installsuffix cgo -o greeter

FROM ubuntu:18.04

RUN mkdir /app
WORKDIR /app
COPY --from=builder /app/greeter .

CMD ["./greeter"]
