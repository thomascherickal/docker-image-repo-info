## `kong:alpine`

```console
$ docker pull kong@sha256:e4581fb9fc2d382b21ce570836edf39e66230d51babf4e41505114500f28fe7f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:alpine` - linux; amd64

```console
$ docker pull kong@sha256:652a2b60d6dddfa1eb275ba8f600500e6ca3040e21962c70f614ef3dc2bd1553
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.2 MB (34221565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ae2092c73c42e1857cb516fdf98fb785a331571a797f4dee6df608d22fb50a7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:24:27 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 02 Aug 2023 23:19:59 GMT
ARG KONG_VERSION=3.3.1
# Wed, 02 Aug 2023 23:19:59 GMT
ENV KONG_VERSION=3.3.1
# Wed, 02 Aug 2023 23:19:59 GMT
ARG KONG_AMD64_SHA=b544aa8d23b544b7ec48e943e3525f6c1f33b202522020eedf91784c87de1a3d
# Wed, 02 Aug 2023 23:19:59 GMT
ARG KONG_PREFIX=/usr/local/kong
# Wed, 02 Aug 2023 23:19:59 GMT
ENV KONG_PREFIX=/usr/local/kong
# Wed, 02 Aug 2023 23:19:59 GMT
ARG ASSET=remote
# Wed, 02 Aug 2023 23:19:59 GMT
ARG EE_PORTS
# Wed, 02 Aug 2023 23:20:00 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Wed, 02 Aug 2023 23:20:06 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=b544aa8d23b544b7ec48e943e3525f6c1f33b202522020eedf91784c87de1a3d
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     export ARCH='amd64';     KONG_SHA256=$KONG_AMD64_SHA ;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc perl tzdata libcap zlib zlib-dev bash yaml     && adduser -S kong     && addgroup -S kong     && mkdir -p "${KONG_PREFIX}"     && chown -R kong:0 ${KONG_PREFIX}     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u ${KONG_PREFIX}     && rm -rf /tmp/kong.apk.tar.gz     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Wed, 02 Aug 2023 23:20:07 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Wed, 02 Aug 2023 23:20:07 GMT
USER kong
# Wed, 02 Aug 2023 23:20:07 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Aug 2023 23:20:07 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 02 Aug 2023 23:20:07 GMT
STOPSIGNAL SIGQUIT
# Wed, 02 Aug 2023 23:20:07 GMT
HEALTHCHECK &{["CMD-SHELL" "kong-health"] "1m0s" "10s" "0s" '\n'}
# Wed, 02 Aug 2023 23:20:07 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f73e69d72915283fe5a8c6a68e9e1764c1adb0d4f9521fd4d44b8040564cb6`  
		Last Modified: Wed, 02 Aug 2023 23:21:35 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93542fef104993f298735ed04a090df4ec1e7e245048ec2e8171111744dec6dd`  
		Last Modified: Wed, 02 Aug 2023 23:21:40 GMT  
		Size: 30.8 MB (30845560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94709bcb36b141a70e0545aaea10a347e9c265e27e6260429fbfedfc6455f37a`  
		Last Modified: Wed, 02 Aug 2023 23:21:35 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
