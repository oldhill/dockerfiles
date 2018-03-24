FROM golang:latest

RUN apt-get update && apt-get install -y man tree htop vim

WORKDIR /go/src/helloworld

COPY hello_world.go /go/src/helloworld

RUN go build hello_world.go

CMD ["./hello_world"]
