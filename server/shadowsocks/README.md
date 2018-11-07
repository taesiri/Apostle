# ShadowSocks Server

This image uses ``ENTRYPOINT`` to run the containers as an executable.

## Quick Start

``docker run -d -p 10003:10003 taesiri/apostle-ssserver -p 10003 -k KeyPhrase -m rc4-md5 --restart always``
