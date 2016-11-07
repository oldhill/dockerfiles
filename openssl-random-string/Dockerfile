FROM debian:latest

ENV LEN 100

RUN apt-get update && apt-get install -y openssl

ENTRYPOINT openssl rand -base64 ${LEN}
