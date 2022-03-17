## `kong:latest`

```console
$ docker pull kong@sha256:8d461dd0ad4b8589290c59833383eb58aa1f2ce2f63be1567922bf79cfb23c1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:latest` - linux; amd64

```console
$ docker pull kong@sha256:21236a4e662aea8cff7a62ad2d39f4c845a3ed5f44834bafcb8a7e07001466e8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49110785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c413c46038620ade201dd2d46194a758ad537e1c0b805142b43cce00455a9683`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 17 Mar 2022 04:01:58 GMT
ADD file:cf4b631a115c2bbfbd81cad2d3041bceb64a8136aac92ba8a63b6c51d60af764 in / 
# Thu, 17 Mar 2022 04:01:59 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 12:45:29 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 17 Mar 2022 12:45:29 GMT
ARG ASSET=ce
# Thu, 17 Mar 2022 12:45:30 GMT
ENV ASSET=ce
# Thu, 17 Mar 2022 12:45:30 GMT
ARG EE_PORTS
# Thu, 17 Mar 2022 12:45:30 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 17 Mar 2022 12:45:30 GMT
ARG KONG_VERSION=2.8.0
# Thu, 17 Mar 2022 12:45:30 GMT
ENV KONG_VERSION=2.8.0
# Thu, 17 Mar 2022 12:45:30 GMT
ARG KONG_AMD64_SHA=60ef680e0fc4d2cf52934758e6a0dc0f173d2a3b32aca49c7eb31ab478c24583
# Thu, 17 Mar 2022 12:45:30 GMT
ARG KONG_ARM64_SHA=5c23f448eeae1b363ece51d066405c13798ee08ca413097a23d9b5ccb49cbf35
# Thu, 17 Mar 2022 12:45:37 GMT
# ARGS: KONG_AMD64_SHA=60ef680e0fc4d2cf52934758e6a0dc0f173d2a3b32aca49c7eb31ab478c24583 KONG_ARM64_SHA=5c23f448eeae1b363ece51d066405c13798ee08ca413097a23d9b5ccb49cbf35
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 17 Mar 2022 12:45:38 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 17 Mar 2022 12:45:38 GMT
USER kong
# Thu, 17 Mar 2022 12:45:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Mar 2022 12:45:38 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 17 Mar 2022 12:45:38 GMT
STOPSIGNAL SIGQUIT
# Thu, 17 Mar 2022 12:45:38 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 17 Mar 2022 12:45:38 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:3d243047344378e9b7136d552d48feb7ea8b6fe14ce0990e0cc011d5e369626a`  
		Last Modified: Thu, 17 Mar 2022 04:02:41 GMT  
		Size: 2.8 MB (2812636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e3e05e1ea26f1f6f2bf1773cef7fddadbc475f528069e93e0c6ee25d2a9cd1`  
		Last Modified: Thu, 17 Mar 2022 12:46:30 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7d9b64b8a8870acc6d3d02360b77e5b0b21b1f03289a06bb4de681087df862e`  
		Last Modified: Thu, 17 Mar 2022 12:46:39 GMT  
		Size: 46.3 MB (46297137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85cf0f9d59c872d6017fdf14b8490fadf5a6e94d83cef15b4f70d56748318c2c`  
		Last Modified: Thu, 17 Mar 2022 12:46:30 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:latest` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:b96735d33c01557a3525c39ce1f01bd0a5a3a36e30767e4163bb1ca085984fbf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.3 MB (48303314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c42fa83c468eaec32dce2087b73e6334aa325b5097c194341f5396dcaba7c23`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Fri, 04 Feb 2022 20:40:18 GMT
LABEL maintainer=Kong <support@konghq.com>
# Fri, 04 Feb 2022 20:40:19 GMT
ARG ASSET=ce
# Fri, 04 Feb 2022 20:40:20 GMT
ENV ASSET=ce
# Fri, 04 Feb 2022 20:40:21 GMT
ARG EE_PORTS
# Fri, 04 Feb 2022 20:40:23 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 02 Mar 2022 19:51:54 GMT
ARG KONG_VERSION=2.8.0
# Wed, 02 Mar 2022 19:51:55 GMT
ENV KONG_VERSION=2.8.0
# Wed, 02 Mar 2022 19:51:56 GMT
ARG KONG_AMD64_SHA=60ef680e0fc4d2cf52934758e6a0dc0f173d2a3b32aca49c7eb31ab478c24583
# Wed, 02 Mar 2022 19:51:57 GMT
ARG KONG_ARM64_SHA=5c23f448eeae1b363ece51d066405c13798ee08ca413097a23d9b5ccb49cbf35
# Wed, 02 Mar 2022 19:52:29 GMT
# ARGS: KONG_AMD64_SHA=60ef680e0fc4d2cf52934758e6a0dc0f173d2a3b32aca49c7eb31ab478c24583 KONG_ARM64_SHA=5c23f448eeae1b363ece51d066405c13798ee08ca413097a23d9b5ccb49cbf35
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Wed, 02 Mar 2022 19:52:30 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 02 Mar 2022 19:52:30 GMT
USER kong
# Wed, 02 Mar 2022 19:52:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Mar 2022 19:52:32 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 02 Mar 2022 19:52:33 GMT
STOPSIGNAL SIGQUIT
# Wed, 02 Mar 2022 19:52:34 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 02 Mar 2022 19:52:35 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eae03c055040559b36a26ac32761328de07b80be76d8df38ca7192f8c5f5768`  
		Last Modified: Fri, 04 Feb 2022 20:46:52 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60148387cdde6488df89097c25b80e9735dd92124f940fe15bad0b85691bee69`  
		Last Modified: Wed, 02 Mar 2022 20:01:35 GMT  
		Size: 45.6 MB (45586868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c9e31595eeda74f4a57ca932c8c7500d4b4d704e22805fe95bf601ea698088`  
		Last Modified: Wed, 02 Mar 2022 20:01:26 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
