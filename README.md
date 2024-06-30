# MoviePilot 微信转发代理 Docker

[![Build Status](https://github.com/sq1018/mp-wxproxy/actions/workflows/docker-image.yml/badge.svg)](https://github.com/sq1018/mp-wxproxy/actions/workflows/docker-image.yml)[![Build Status](https://github.com/sq1018/mp-wxproxy/actions/workflows/docker-push.yml/badge.svg)](https://github.com/sq1018/mp-wxproxy/actions/workflows/docker-push.yml)

```bash
docker run -d \
    --name mp-wxproxy \
    --restart=always \
    -p 9080:80 \
    sq101817/mp-wxproxy:latest
```

```yaml
version: '3.3'
services:
    mp-wxproxy:
        container_name: mp-wxproxy
        restart: always
        ports:
            - '9080:80'
        image: 'sq101817/mp-wxproxy:latest'
```
