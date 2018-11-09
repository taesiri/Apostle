# ShadowSocks Client
#
# VERSION 1.0.0

FROM ubuntu:18.10
LABEL maintainer="mtaesiri@gmail.com"

RUN apt update
RUN apt install -y python-pip libsodium23
RUN apt install -y git
RUN pip install -U git+https://github.com/shadowsocks/shadowsocks.git@master

# Configure container to run as an executable
ENTRYPOINT ["/usr/local/bin/sslocal"]