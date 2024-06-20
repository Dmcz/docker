# docker hub images
## php alpine
* dmcz0/php:8.3-alpine-3.20
* dmcz0/php:8.3-alpine-3.20-swoole-5.1.3
## php dev
* dmcz0/php:8.1-dev-ubuntu-22.04
* dmcz0/php:8.2-dev-ubuntu-22.04
* dmcz0/php:8.2-dev-ubuntu-22.04-swow-1.3.1
* dmcz0/php:8.3-dev-ubuntu-22.04
* dmcz0/php:8.3-dev-ubuntu-24.04
* dmcz0/php:8.3-dev-ubuntu-24.04-swoole-5.1.2
* dmcz0/php:8.3-dev-ubuntu-24.04-swoole-5.1.2-python-3.11-phpy-1.0.5
* dmcz0/php:8.3-dev-ubuntu-24.04-swoole-5.1.2-python-3.12-phpy-1.0.4
* dmcz0/php:8.3-dev-ubuntu-24.04-swoole-5.1.2-python-3.12-phpy-1.0.5
* dmcz0/php:8.3-dev-ubuntu-24.04-swoole-5.1.3

# example of build command
```bash
docker build . -t dmcz0/php:8.3-dev-ubuntu-24.04 \
--build-arg UBUNTU_VERSION=24.04 \
--build-arg PHP_VERSION=8.3 \
--build-arg HTTP_PROXY=http://172.29.112.1:7890 \
--build-arg HTTPS_PROXY=http://172.29.112.1:7890
```
* 其中代理需要监听LAN，既非仅127.0.0.1
