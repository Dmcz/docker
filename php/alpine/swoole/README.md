# build command example
```bash
docker build . -t dmcz0/php:8.3-alpine-3.20-swoole-5.1.4 \
--build-arg ALPINE_VERSION=3.20 \
--build-arg PHP_VERSION=8.3 \
--build-arg SWOOLE_VERSION=5.1.4 \
--build-arg HTTP_PROXY=http://172.29.112.1:7890 \
--build-arg HTTPS_PROXY=http://172.29.112.1:7890
```