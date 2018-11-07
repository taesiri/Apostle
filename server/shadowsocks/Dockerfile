# ShadowSocks Server
#
# VERSION 1.0.0

FROM ubuntu:18.10
LABEL maintainer="mtaesiri@gmail.com"

RUN apt update
RUN apt install -y python-pip libsodium18
RUN pip install shadowsocks

# Configure container to run as an executable
ENTRYPOINT ["/usr/local/bin/ssserver"]