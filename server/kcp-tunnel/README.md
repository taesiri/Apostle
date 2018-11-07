# KCP Tunnel Server

This image uses ``ENTRYPOINT`` to run the containers as an executable.

## Quick Start

How to Run:

``docker run -d -p 47437:47437 taesiri/apostle-kcp -l 0.0.0.0:47437 -t 127.0.0.1:10003 --crypt aes-192 --key SECUREPASSWORD --restart always``

## Improving performance

According to [this](https://github.com/xtaci/kcptun), it is possible to improve the performance by increasing of the OS UDP buffers.

```bash
sudo sysctl -w net.core.rmem_max=26214400
sudo sysctl -w net.core.rmem_default=26214400
```
