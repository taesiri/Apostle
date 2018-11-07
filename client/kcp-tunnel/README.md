# KCP Tunnel Client

This image uses ``ENTRYPOINT`` to run the containers as an executable.

## Quick Start

How to Run:

``docker run -d -p 10003:10003 taesiri/sentinel-kcp -l 0.0.0.0:10003 -r SERVER-ADDRESS:47437 --crypt aes-192 --key SECUREPASSWORD --restart always``
