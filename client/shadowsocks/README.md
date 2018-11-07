# ShadowSocks Client

This image uses ``ENTRYPOINT`` to run the containers as an executable.

## Quick Start

``docker run -d -p 1080:1080 taesiri/sentinel-sslocal -b 0.0.0.0 -l 1080 -s 127.0.0.1 -p 10003 -k KeyPhrase  -m rc4-md5 --restart always``