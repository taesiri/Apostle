# Shadowsocks + Kcptun Docker

[Original Author](https://github.com/predatorray/shadowsocks-kcptun-docker)

## Quick Usage

```bash
docker run -d -p 8388:8388 -p 29900:29900/udp taesiri/apostle-ssskcptun
```

## Options

| Option | Description | Defaults |
| ------------- |:-------------:| -----:|
| --help | Help | - |
| -m, --ss-method METHOD | ShadowSocks encryption method | aes-256-cfb |
| -p, --ss-password PASSWORD | ShadowSocks passphrase | passw0rd |
| -s, --kcptun-secret PASSWORD | KCP Tunnel passphrase | it's a secrect |
| -c, --kcptun-crypt CRYPT | KCP Tunnel encryption method | aes |

```bash
docker run -d -p 8388:8388 -p 29900:29900/udp taesiri/apostle-ssskcptun -m 'aes-256-cfb' -p 'shadowsocks-passphrase' -s "kcp-secret" -c 'aes'
```

## Ports

| Service        | Port           | Type  |
| ------------- |:-------------:| -----:|
| Shadowsocks | 8388 | TCP |
| KCP Tunnel | 29900 | UDP |