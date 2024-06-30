# MoviePilot 微信转发代理 Docker

[![Build](https://github.com/sq1018/mp-wxproxy/actions/workflows/build.yml/badge.svg)](https://github.com/sq1018/mp-wxproxy/actions/workflows/build.yml) [![Docker readme update](https://github.com/sq1018/mp-wxproxy/actions/workflows/readme_update.yml/badge.svg)](https://github.com/sq1018/mp-wxproxy/actions/workflows/readme_update.yml)

```bash
docker run -d \
    --name wxchat \
    --restart=always \
    -p 9080:80 \
    sq101817/wxproxy:latest
```

```yaml
version: '3.3'
services:
    wxproxy:
        container_name: wxproxy
        restart: always
        ports:
            - '9080:80'
        image: 'sq101817/wxproxy:latest'
```
