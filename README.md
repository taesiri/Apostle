# Apostle

## 🔥 Experimental Section 🔥

A set of toolsets that helps me browse the Internet!

## Components

There are serveral components in this project. this includes ``Tor Gun``, ``ShadowSocks``, ``KCP Tunnel`` and ``RedSocks``. I personally don't like/use ``OpenVPN``, ``IPSec LT2P`` nor ``IKEV2``, so I did not include neither of them in this project. There are lots of pre-built docker images for these types of VPNs, you can use them 😊.

## Server Setup

Server setup is easy, every configuration has its own `Dockerfile`.

## Client Setup

There are 5+1 different clients to use. for MacOS, iOS, Linux, Android and Windows.

### MacOS, Linux, Windows

I'll use sweet ``docker-compose`` to automate everything!

### iOS

The best iOS client you can get is [Potatso Lite](https://itunes.apple.com/us/app/potatso-lite/id1239860606?mt=8), It's free, fast and supports a wide variety of protocols.

### Android

There is an official [ShadowSocks client](https://play.google.com/store/apps/details?id=com.github.shadowsocks&hl=en_US) out there, but sadly it lacks the ShadowSocksR support and a few other things. The best client I've been found so far is [ShadowsocksR Android](https://github.com/shadowsocksr-backup/shadowsocksr-android/releases)

### Mips and Mipsle

There are no immediate plans to support these architectures!