# ShadowSocks Server
#
# VERSION 1.0.1

FROM ubuntu:18.10
LABEL maintainer="mtaesiri@gmail.com"

RUN apt update
RUN apt install -y python-pip libsodium23
RUN apt install -y git
RUN pip install -U git+https://github.com/shadowsocks/shadowsocks.git@master

ENV SERVER_ADDR     0.0.0.0
ENV SERVER_PORT     80
ENV PASSWORD        TheServerDude
ENV METHOD          aes-256-cfb
ENV TIMEOUT         300

EXPOSE $SERVER_PORT

CMD /usr/local/bin/ssserver -p $SERVER_PORT -k $PASSWORD -m $METHOD
