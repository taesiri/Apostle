# KCP Tun Client
#
# VERSION 1.0.0

FROM ubuntu:18.10
LABEL maintainer="mtaesiri@gmail.com"

RUN apt update && \
    apt install -y wget
RUN wget "https://github.com/xtaci/kcptun/releases/download/v20181002/kcptun-linux-amd64-20181002.tar.gz"
RUN tar xzf "kcptun-linux-amd64-20181002.tar.gz"

# Increasing the number of open files on server
RUN ulimit -n 65535

# Configure container to run as an executable
ENTRYPOINT ["./server_linux_amd64"]