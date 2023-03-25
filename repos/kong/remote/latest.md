## `kong:latest`

```console
$ docker pull kong@sha256:5436a1fefaf877190571093034db91f82928d7492b372cc73a1755424bdf43b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:latest` - linux; amd64

```console
$ docker pull kong@sha256:36258c1d9dd6f5da8cc0403af4650f5d95296e48f83e330ec8f5fd3e3883f162
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75689080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b76469f8b580bfa16be2cce693e879f0c97cf21dab83dca21aa46b9597ed0747`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 13:59:53 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Sat, 11 Feb 2023 13:59:53 GMT
ARG KONG_VERSION=3.1.1
# Sat, 11 Feb 2023 13:59:53 GMT
ENV KONG_VERSION=3.1.1
# Sat, 11 Feb 2023 13:59:53 GMT
ARG KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c
# Sat, 11 Feb 2023 13:59:53 GMT
ARG KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
# Sat, 11 Feb 2023 13:59:53 GMT
ARG ASSET=remote
# Sat, 11 Feb 2023 13:59:53 GMT
ARG EE_PORTS
# Sat, 11 Feb 2023 13:59:53 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Sat, 11 Feb 2023 14:00:01 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Sat, 11 Feb 2023 14:00:01 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Sat, 11 Feb 2023 14:00:01 GMT
USER kong
# Sat, 11 Feb 2023 14:00:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 11 Feb 2023 14:00:01 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 11 Feb 2023 14:00:01 GMT
STOPSIGNAL SIGQUIT
# Sat, 11 Feb 2023 14:00:02 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Sat, 11 Feb 2023 14:00:02 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256d8d79435b0bcc04e2462111b09b5a21093f05b20ff38b484036c091891ff2`  
		Last Modified: Sat, 11 Feb 2023 14:01:47 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8a6c1e7dd831b077e9ed68a8dd90af0a86718c8e0873c8c3dd6f877dc08ded`  
		Last Modified: Sat, 11 Feb 2023 14:01:56 GMT  
		Size: 72.9 MB (72880307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce630ba9f4f76fa8c33b114ce2e01fe176acd00019a99c6e2c8d9f95c2157de`  
		Last Modified: Sat, 11 Feb 2023 14:01:47 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
