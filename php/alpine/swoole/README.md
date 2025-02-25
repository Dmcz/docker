# build command example
```bash
docker build . -t dmcz0/php:8.3-alpine-3.20-swoole-5.1.7 \
--build-arg ALPINE_VERSION=3.20 \
--build-arg PHP_VERSION=8.3 \
--build-arg SWOOLE_VERSION=5.1.7 \
--build-arg HTTP_PROXY=http://192.168.3.5:7890 \
--build-arg HTTPS_PROXY=http://192.168.3.5:7890
```
* 由于apline仅维护最新的z版本，所以每次都需要完整的安装php而无法维护一个公共的php镜像