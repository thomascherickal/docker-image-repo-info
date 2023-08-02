<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kong`

-	[`kong:2.8`](#kong28)
-	[`kong:2.8.3`](#kong283)
-	[`kong:2.8.3-alpine`](#kong283-alpine)
-	[`kong:3`](#kong3)
-	[`kong:3.0`](#kong30)
-	[`kong:3.0-alpine`](#kong30-alpine)
-	[`kong:3.0-ubuntu`](#kong30-ubuntu)
-	[`kong:3.0.2`](#kong302)
-	[`kong:3.0.2-alpine`](#kong302-alpine)
-	[`kong:3.0.2-ubuntu`](#kong302-ubuntu)
-	[`kong:3.1`](#kong31)
-	[`kong:3.1-ubuntu`](#kong31-ubuntu)
-	[`kong:3.1.1`](#kong311)
-	[`kong:3.1.1-alpine`](#kong311-alpine)
-	[`kong:3.1.1-ubuntu`](#kong311-ubuntu)
-	[`kong:3.2`](#kong32)
-	[`kong:3.2-ubuntu`](#kong32-ubuntu)
-	[`kong:3.2.2`](#kong322)
-	[`kong:3.2.2-alpine`](#kong322-alpine)
-	[`kong:3.2.2-ubuntu`](#kong322-ubuntu)
-	[`kong:3.3`](#kong33)
-	[`kong:3.3-ubuntu`](#kong33-ubuntu)
-	[`kong:3.3.1`](#kong331)
-	[`kong:3.3.1-alpine`](#kong331-alpine)
-	[`kong:3.3.1-ubuntu`](#kong331-ubuntu)
-	[`kong:alpine`](#kongalpine)
-	[`kong:latest`](#konglatest)
-	[`kong:ubuntu`](#kongubuntu)

## `kong:2.8`

```console
$ docker pull kong@sha256:333d0f4d22ca495e9e376a590bb24d134e6b59175e5e77d2e11322d263b3ce21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.8` - linux; amd64

```console
$ docker pull kong@sha256:713789b93a0fa4081776691c27e4a9712b4c163f3c6fc3d0d8f20e988267f5e6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49373331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6aa1f074244b99d59199674239b3125eed26146726d39803b7c432541c618e2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:09 GMT
ADD file:4af69326e088b3c0f82320e9cd97b60c28bf019b984787c6f1c22489e6221f29 in / 
# Wed, 14 Jun 2023 20:42:09 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:25:19 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 15 Jun 2023 06:25:19 GMT
ARG ASSET=ce
# Thu, 15 Jun 2023 06:25:20 GMT
ENV ASSET=ce
# Thu, 15 Jun 2023 06:25:20 GMT
ARG EE_PORTS
# Thu, 15 Jun 2023 06:25:20 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 15 Jun 2023 06:25:20 GMT
ARG KONG_VERSION=2.8.3
# Thu, 15 Jun 2023 06:25:20 GMT
ENV KONG_VERSION=2.8.3
# Thu, 15 Jun 2023 06:25:20 GMT
ARG KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa
# Thu, 15 Jun 2023 06:25:20 GMT
ARG KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
# Thu, 15 Jun 2023 06:25:27 GMT
# ARGS: KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 15 Jun 2023 06:25:27 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 15 Jun 2023 06:25:27 GMT
USER kong
# Thu, 15 Jun 2023 06:25:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Jun 2023 06:25:27 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 15 Jun 2023 06:25:27 GMT
STOPSIGNAL SIGQUIT
# Thu, 15 Jun 2023 06:25:28 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 15 Jun 2023 06:25:28 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:c1d6d1b2d5a367259e6e51a7f4d1ccd66a28cc9940d6599d8a8ea9544dd4b4a8`  
		Last Modified: Wed, 14 Jun 2023 20:42:45 GMT  
		Size: 2.8 MB (2807669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a3cffc76b093ccc58db04ef3355333d93f40ac3c60304ac3c451740f20380e`  
		Last Modified: Thu, 15 Jun 2023 06:27:00 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b68e3c47dd4a95fb01daf0c3f21056dbb306c43005ed97c9c8d537edf2ce84`  
		Last Modified: Thu, 15 Jun 2023 06:27:07 GMT  
		Size: 46.6 MB (46564649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf89364b9c0039a1ccd22f01467d98fec4250f7e4a1fd94385971ab4e1de6e67`  
		Last Modified: Thu, 15 Jun 2023 06:27:00 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.8` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:0453ddb662f69b61f3e7dc9599818aa7086c5e1a79406e48ad2dc24de1973446
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.6 MB (48558546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e83fb576cec3804f46d1ac467a47660530f4995293951b475a4bc5422df0e96`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:07 GMT
ADD file:e80eabe59d1f87ef41634428d9f8fdeb633c2128ac97564f96f5495ef6bf2c72 in / 
# Wed, 14 Jun 2023 20:49:07 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:42:20 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 15 Jun 2023 00:42:20 GMT
ARG ASSET=ce
# Thu, 15 Jun 2023 00:42:20 GMT
ENV ASSET=ce
# Thu, 15 Jun 2023 00:42:20 GMT
ARG EE_PORTS
# Thu, 15 Jun 2023 00:42:20 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 15 Jun 2023 00:42:20 GMT
ARG KONG_VERSION=2.8.3
# Thu, 15 Jun 2023 00:42:21 GMT
ENV KONG_VERSION=2.8.3
# Thu, 15 Jun 2023 00:42:21 GMT
ARG KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa
# Thu, 15 Jun 2023 00:42:21 GMT
ARG KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
# Thu, 15 Jun 2023 00:42:27 GMT
# ARGS: KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 15 Jun 2023 00:42:28 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 15 Jun 2023 00:42:28 GMT
USER kong
# Thu, 15 Jun 2023 00:42:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Jun 2023 00:42:28 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 15 Jun 2023 00:42:28 GMT
STOPSIGNAL SIGQUIT
# Thu, 15 Jun 2023 00:42:28 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 15 Jun 2023 00:42:28 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:a880266d3b77f75696023df2da1ef66c3c565e0f70596242395c9e68de955c7c`  
		Last Modified: Wed, 14 Jun 2023 20:49:43 GMT  
		Size: 2.7 MB (2707906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dab1b35d2d75cdc60cacfe207a2fc28581512d1e48b38519945b8d95d45cb2b`  
		Last Modified: Thu, 15 Jun 2023 00:43:29 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb8719519dc06ae4474af38360433cae6d3875191a3fa3f99f09ac32b31c9a7b`  
		Last Modified: Thu, 15 Jun 2023 00:43:36 GMT  
		Size: 45.8 MB (45849631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb2e7eaca4a2e90378e3725946eaabe938e5babee334d3482a78a36ad6eb276d`  
		Last Modified: Thu, 15 Jun 2023 00:43:29 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.8.3`

```console
$ docker pull kong@sha256:333d0f4d22ca495e9e376a590bb24d134e6b59175e5e77d2e11322d263b3ce21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.8.3` - linux; amd64

```console
$ docker pull kong@sha256:713789b93a0fa4081776691c27e4a9712b4c163f3c6fc3d0d8f20e988267f5e6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49373331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6aa1f074244b99d59199674239b3125eed26146726d39803b7c432541c618e2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:09 GMT
ADD file:4af69326e088b3c0f82320e9cd97b60c28bf019b984787c6f1c22489e6221f29 in / 
# Wed, 14 Jun 2023 20:42:09 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:25:19 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 15 Jun 2023 06:25:19 GMT
ARG ASSET=ce
# Thu, 15 Jun 2023 06:25:20 GMT
ENV ASSET=ce
# Thu, 15 Jun 2023 06:25:20 GMT
ARG EE_PORTS
# Thu, 15 Jun 2023 06:25:20 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 15 Jun 2023 06:25:20 GMT
ARG KONG_VERSION=2.8.3
# Thu, 15 Jun 2023 06:25:20 GMT
ENV KONG_VERSION=2.8.3
# Thu, 15 Jun 2023 06:25:20 GMT
ARG KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa
# Thu, 15 Jun 2023 06:25:20 GMT
ARG KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
# Thu, 15 Jun 2023 06:25:27 GMT
# ARGS: KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 15 Jun 2023 06:25:27 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 15 Jun 2023 06:25:27 GMT
USER kong
# Thu, 15 Jun 2023 06:25:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Jun 2023 06:25:27 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 15 Jun 2023 06:25:27 GMT
STOPSIGNAL SIGQUIT
# Thu, 15 Jun 2023 06:25:28 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 15 Jun 2023 06:25:28 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:c1d6d1b2d5a367259e6e51a7f4d1ccd66a28cc9940d6599d8a8ea9544dd4b4a8`  
		Last Modified: Wed, 14 Jun 2023 20:42:45 GMT  
		Size: 2.8 MB (2807669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a3cffc76b093ccc58db04ef3355333d93f40ac3c60304ac3c451740f20380e`  
		Last Modified: Thu, 15 Jun 2023 06:27:00 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b68e3c47dd4a95fb01daf0c3f21056dbb306c43005ed97c9c8d537edf2ce84`  
		Last Modified: Thu, 15 Jun 2023 06:27:07 GMT  
		Size: 46.6 MB (46564649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf89364b9c0039a1ccd22f01467d98fec4250f7e4a1fd94385971ab4e1de6e67`  
		Last Modified: Thu, 15 Jun 2023 06:27:00 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.8.3` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:0453ddb662f69b61f3e7dc9599818aa7086c5e1a79406e48ad2dc24de1973446
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.6 MB (48558546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e83fb576cec3804f46d1ac467a47660530f4995293951b475a4bc5422df0e96`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:07 GMT
ADD file:e80eabe59d1f87ef41634428d9f8fdeb633c2128ac97564f96f5495ef6bf2c72 in / 
# Wed, 14 Jun 2023 20:49:07 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:42:20 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 15 Jun 2023 00:42:20 GMT
ARG ASSET=ce
# Thu, 15 Jun 2023 00:42:20 GMT
ENV ASSET=ce
# Thu, 15 Jun 2023 00:42:20 GMT
ARG EE_PORTS
# Thu, 15 Jun 2023 00:42:20 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 15 Jun 2023 00:42:20 GMT
ARG KONG_VERSION=2.8.3
# Thu, 15 Jun 2023 00:42:21 GMT
ENV KONG_VERSION=2.8.3
# Thu, 15 Jun 2023 00:42:21 GMT
ARG KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa
# Thu, 15 Jun 2023 00:42:21 GMT
ARG KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
# Thu, 15 Jun 2023 00:42:27 GMT
# ARGS: KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 15 Jun 2023 00:42:28 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 15 Jun 2023 00:42:28 GMT
USER kong
# Thu, 15 Jun 2023 00:42:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Jun 2023 00:42:28 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 15 Jun 2023 00:42:28 GMT
STOPSIGNAL SIGQUIT
# Thu, 15 Jun 2023 00:42:28 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 15 Jun 2023 00:42:28 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:a880266d3b77f75696023df2da1ef66c3c565e0f70596242395c9e68de955c7c`  
		Last Modified: Wed, 14 Jun 2023 20:49:43 GMT  
		Size: 2.7 MB (2707906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dab1b35d2d75cdc60cacfe207a2fc28581512d1e48b38519945b8d95d45cb2b`  
		Last Modified: Thu, 15 Jun 2023 00:43:29 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb8719519dc06ae4474af38360433cae6d3875191a3fa3f99f09ac32b31c9a7b`  
		Last Modified: Thu, 15 Jun 2023 00:43:36 GMT  
		Size: 45.8 MB (45849631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb2e7eaca4a2e90378e3725946eaabe938e5babee334d3482a78a36ad6eb276d`  
		Last Modified: Thu, 15 Jun 2023 00:43:29 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.8.3-alpine`

```console
$ docker pull kong@sha256:333d0f4d22ca495e9e376a590bb24d134e6b59175e5e77d2e11322d263b3ce21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.8.3-alpine` - linux; amd64

```console
$ docker pull kong@sha256:713789b93a0fa4081776691c27e4a9712b4c163f3c6fc3d0d8f20e988267f5e6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49373331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6aa1f074244b99d59199674239b3125eed26146726d39803b7c432541c618e2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:09 GMT
ADD file:4af69326e088b3c0f82320e9cd97b60c28bf019b984787c6f1c22489e6221f29 in / 
# Wed, 14 Jun 2023 20:42:09 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:25:19 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 15 Jun 2023 06:25:19 GMT
ARG ASSET=ce
# Thu, 15 Jun 2023 06:25:20 GMT
ENV ASSET=ce
# Thu, 15 Jun 2023 06:25:20 GMT
ARG EE_PORTS
# Thu, 15 Jun 2023 06:25:20 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 15 Jun 2023 06:25:20 GMT
ARG KONG_VERSION=2.8.3
# Thu, 15 Jun 2023 06:25:20 GMT
ENV KONG_VERSION=2.8.3
# Thu, 15 Jun 2023 06:25:20 GMT
ARG KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa
# Thu, 15 Jun 2023 06:25:20 GMT
ARG KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
# Thu, 15 Jun 2023 06:25:27 GMT
# ARGS: KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 15 Jun 2023 06:25:27 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 15 Jun 2023 06:25:27 GMT
USER kong
# Thu, 15 Jun 2023 06:25:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Jun 2023 06:25:27 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 15 Jun 2023 06:25:27 GMT
STOPSIGNAL SIGQUIT
# Thu, 15 Jun 2023 06:25:28 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 15 Jun 2023 06:25:28 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:c1d6d1b2d5a367259e6e51a7f4d1ccd66a28cc9940d6599d8a8ea9544dd4b4a8`  
		Last Modified: Wed, 14 Jun 2023 20:42:45 GMT  
		Size: 2.8 MB (2807669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a3cffc76b093ccc58db04ef3355333d93f40ac3c60304ac3c451740f20380e`  
		Last Modified: Thu, 15 Jun 2023 06:27:00 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b68e3c47dd4a95fb01daf0c3f21056dbb306c43005ed97c9c8d537edf2ce84`  
		Last Modified: Thu, 15 Jun 2023 06:27:07 GMT  
		Size: 46.6 MB (46564649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf89364b9c0039a1ccd22f01467d98fec4250f7e4a1fd94385971ab4e1de6e67`  
		Last Modified: Thu, 15 Jun 2023 06:27:00 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.8.3-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:0453ddb662f69b61f3e7dc9599818aa7086c5e1a79406e48ad2dc24de1973446
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.6 MB (48558546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e83fb576cec3804f46d1ac467a47660530f4995293951b475a4bc5422df0e96`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:07 GMT
ADD file:e80eabe59d1f87ef41634428d9f8fdeb633c2128ac97564f96f5495ef6bf2c72 in / 
# Wed, 14 Jun 2023 20:49:07 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:42:20 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 15 Jun 2023 00:42:20 GMT
ARG ASSET=ce
# Thu, 15 Jun 2023 00:42:20 GMT
ENV ASSET=ce
# Thu, 15 Jun 2023 00:42:20 GMT
ARG EE_PORTS
# Thu, 15 Jun 2023 00:42:20 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 15 Jun 2023 00:42:20 GMT
ARG KONG_VERSION=2.8.3
# Thu, 15 Jun 2023 00:42:21 GMT
ENV KONG_VERSION=2.8.3
# Thu, 15 Jun 2023 00:42:21 GMT
ARG KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa
# Thu, 15 Jun 2023 00:42:21 GMT
ARG KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
# Thu, 15 Jun 2023 00:42:27 GMT
# ARGS: KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 15 Jun 2023 00:42:28 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 15 Jun 2023 00:42:28 GMT
USER kong
# Thu, 15 Jun 2023 00:42:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Jun 2023 00:42:28 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 15 Jun 2023 00:42:28 GMT
STOPSIGNAL SIGQUIT
# Thu, 15 Jun 2023 00:42:28 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 15 Jun 2023 00:42:28 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:a880266d3b77f75696023df2da1ef66c3c565e0f70596242395c9e68de955c7c`  
		Last Modified: Wed, 14 Jun 2023 20:49:43 GMT  
		Size: 2.7 MB (2707906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dab1b35d2d75cdc60cacfe207a2fc28581512d1e48b38519945b8d95d45cb2b`  
		Last Modified: Thu, 15 Jun 2023 00:43:29 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb8719519dc06ae4474af38360433cae6d3875191a3fa3f99f09ac32b31c9a7b`  
		Last Modified: Thu, 15 Jun 2023 00:43:36 GMT  
		Size: 45.8 MB (45849631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb2e7eaca4a2e90378e3725946eaabe938e5babee334d3482a78a36ad6eb276d`  
		Last Modified: Thu, 15 Jun 2023 00:43:29 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3`

```console
$ docker pull kong@sha256:6901d658a7fe670a285c85fb41b6dfca465b3bf97b1f488b2f4a04518ec46567
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3` - linux; amd64

```console
$ docker pull kong@sha256:f305f85491b60c6139464ead7fe0b7289d3469a45224f4fada8ba16e909ce8ef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81308072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27891b72fb11814512dfd7f819d980b9af44f35dc071846c7bed9d2315c8818b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:22:10 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Tue, 04 Jul 2023 18:22:10 GMT
ARG ASSET=ce
# Tue, 04 Jul 2023 18:22:10 GMT
ENV ASSET=ce
# Tue, 04 Jul 2023 18:22:10 GMT
ARG EE_PORTS
# Tue, 04 Jul 2023 18:22:11 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Tue, 04 Jul 2023 18:22:11 GMT
ARG KONG_VERSION=3.3.0
# Tue, 04 Jul 2023 18:22:11 GMT
ENV KONG_VERSION=3.3.0
# Tue, 04 Jul 2023 18:22:11 GMT
ARG KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b
# Tue, 04 Jul 2023 18:22:11 GMT
ARG KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
# Tue, 04 Jul 2023 18:23:00 GMT
# ARGS: KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 04 Jul 2023 18:23:00 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Tue, 04 Jul 2023 18:23:00 GMT
USER kong
# Tue, 04 Jul 2023 18:23:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 18:23:01 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 04 Jul 2023 18:23:01 GMT
STOPSIGNAL SIGQUIT
# Tue, 04 Jul 2023 18:23:01 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 04 Jul 2023 18:23:01 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95d715c451393bf53843bdb2d56f67f9228685e8a5467f1581eb7dbd1555e40`  
		Last Modified: Tue, 04 Jul 2023 18:25:40 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0485449e03859344d0d3afc6a0e5d0ac35cd50deb2c2c3cb8cc6114b503c1ed`  
		Last Modified: Tue, 04 Jul 2023 18:25:48 GMT  
		Size: 50.9 MB (50875561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb811f70b9c3e6e52149298e8491972444909b64a67a7549200fdcf841b8f0c`  
		Last Modified: Tue, 04 Jul 2023 18:25:40 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:1af0841022124e34b06deef7223695918912f31bac0d41a5b973b57f235e9f0f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75729473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43979f607227bbb2b07e6de8a0352138b806c807dcfc885c007f7d6235c368ff`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 15:56:30 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Tue, 04 Jul 2023 15:56:30 GMT
ARG ASSET=ce
# Tue, 04 Jul 2023 15:56:30 GMT
ENV ASSET=ce
# Tue, 04 Jul 2023 15:56:31 GMT
ARG EE_PORTS
# Tue, 04 Jul 2023 15:56:31 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Tue, 04 Jul 2023 15:56:31 GMT
ARG KONG_VERSION=3.3.0
# Tue, 04 Jul 2023 15:56:31 GMT
ENV KONG_VERSION=3.3.0
# Tue, 04 Jul 2023 15:56:31 GMT
ARG KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b
# Tue, 04 Jul 2023 15:56:31 GMT
ARG KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
# Tue, 04 Jul 2023 15:56:55 GMT
# ARGS: KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 04 Jul 2023 15:56:55 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Tue, 04 Jul 2023 15:56:55 GMT
USER kong
# Tue, 04 Jul 2023 15:56:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 15:56:55 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 04 Jul 2023 15:56:55 GMT
STOPSIGNAL SIGQUIT
# Tue, 04 Jul 2023 15:56:55 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 04 Jul 2023 15:56:56 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323749330ae28b00c28d5d9426a6340ac8c0950f884d5f86035845592177af50`  
		Last Modified: Tue, 04 Jul 2023 15:58:27 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0838f7579b4383b8de9c9ba94ea92f5e8bf54501aad19ff3c7b20a69d3e9601c`  
		Last Modified: Tue, 04 Jul 2023 15:58:33 GMT  
		Size: 47.3 MB (47337178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86236cf6ed5d8a29939463122de34686c5333330b978ec314bb8718c4bf9f92d`  
		Last Modified: Tue, 04 Jul 2023 15:58:27 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.0`

```console
$ docker pull kong@sha256:c16f02938ab7ae019576dfc17a72e0408393b74ef5a363eb1d9f4d673bffa8f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.0` - linux; amd64

```console
$ docker pull kong@sha256:dbdab62f9949e0843b7d8a46740b805940c6214a78bdab5bf61d169075affbc5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75644403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cde42fd180357ec474d41db513f1f83b601663b89a41dedd1b04abb9543e8fd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:09 GMT
ADD file:4af69326e088b3c0f82320e9cd97b60c28bf019b984787c6f1c22489e6221f29 in / 
# Wed, 14 Jun 2023 20:42:09 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:24:51 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 15 Jun 2023 06:25:05 GMT
ARG KONG_VERSION=3.0.2
# Thu, 15 Jun 2023 06:25:05 GMT
ENV KONG_VERSION=3.0.2
# Thu, 15 Jun 2023 06:25:05 GMT
ARG KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e
# Thu, 15 Jun 2023 06:25:06 GMT
ARG KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
# Thu, 15 Jun 2023 06:25:06 GMT
ARG ASSET=remote
# Thu, 15 Jun 2023 06:25:06 GMT
ARG EE_PORTS
# Thu, 15 Jun 2023 06:25:06 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Thu, 15 Jun 2023 06:25:14 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Thu, 15 Jun 2023 06:25:14 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 15 Jun 2023 06:25:14 GMT
USER kong
# Thu, 15 Jun 2023 06:25:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Jun 2023 06:25:15 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 15 Jun 2023 06:25:15 GMT
STOPSIGNAL SIGQUIT
# Thu, 15 Jun 2023 06:25:15 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 15 Jun 2023 06:25:15 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:c1d6d1b2d5a367259e6e51a7f4d1ccd66a28cc9940d6599d8a8ea9544dd4b4a8`  
		Last Modified: Wed, 14 Jun 2023 20:42:45 GMT  
		Size: 2.8 MB (2807669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eb51f944ac07d5786d81ea9e5223532bd0fc2724b596128d6c6bfb4622548e7`  
		Last Modified: Thu, 15 Jun 2023 06:26:40 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0ea639b18a7afef1350cd95f2c2c066cca2f54a3df6e97a7e86483e91566e9`  
		Last Modified: Thu, 15 Jun 2023 06:26:47 GMT  
		Size: 72.8 MB (72835718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63061c0a2f964430e9d29a86c8866f9b64a4d76c4102fb4508b66d2eb354f7d`  
		Last Modified: Thu, 15 Jun 2023 06:26:40 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.0` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:440179860d6592ac71ab2aa38baa3b43da04a46e1b8c398f46d23bc1298f8f66
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73631302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66027ffeec8745797878c3e3898ddb0355ff120ecb2634833b84d17c22ece6d4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:07 GMT
ADD file:e80eabe59d1f87ef41634428d9f8fdeb633c2128ac97564f96f5495ef6bf2c72 in / 
# Wed, 14 Jun 2023 20:49:07 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:41:55 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 15 Jun 2023 00:42:07 GMT
ARG KONG_VERSION=3.0.2
# Thu, 15 Jun 2023 00:42:07 GMT
ENV KONG_VERSION=3.0.2
# Thu, 15 Jun 2023 00:42:08 GMT
ARG KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e
# Thu, 15 Jun 2023 00:42:08 GMT
ARG KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
# Thu, 15 Jun 2023 00:42:08 GMT
ARG ASSET=remote
# Thu, 15 Jun 2023 00:42:08 GMT
ARG EE_PORTS
# Thu, 15 Jun 2023 00:42:08 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Thu, 15 Jun 2023 00:42:15 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Thu, 15 Jun 2023 00:42:16 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 15 Jun 2023 00:42:16 GMT
USER kong
# Thu, 15 Jun 2023 00:42:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Jun 2023 00:42:16 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 15 Jun 2023 00:42:16 GMT
STOPSIGNAL SIGQUIT
# Thu, 15 Jun 2023 00:42:16 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 15 Jun 2023 00:42:16 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:a880266d3b77f75696023df2da1ef66c3c565e0f70596242395c9e68de955c7c`  
		Last Modified: Wed, 14 Jun 2023 20:49:43 GMT  
		Size: 2.7 MB (2707906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940d9fed445e052edcf4526f82739dd13d3f896eee44d0e7f5ebee7ef05bcc3b`  
		Last Modified: Thu, 15 Jun 2023 00:43:10 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ef0525a80cd2df99acdab00fb0d3a3c1990e46f334a3a78d96509a5ba1535f`  
		Last Modified: Thu, 15 Jun 2023 00:43:17 GMT  
		Size: 70.9 MB (70922382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e236f022db4cf2d3a5525147f6383071ab5184218e5dcd71a4c6754190fdd8a`  
		Last Modified: Thu, 15 Jun 2023 00:43:10 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.0-alpine`

```console
$ docker pull kong@sha256:c16f02938ab7ae019576dfc17a72e0408393b74ef5a363eb1d9f4d673bffa8f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.0-alpine` - linux; amd64

```console
$ docker pull kong@sha256:dbdab62f9949e0843b7d8a46740b805940c6214a78bdab5bf61d169075affbc5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75644403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cde42fd180357ec474d41db513f1f83b601663b89a41dedd1b04abb9543e8fd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:09 GMT
ADD file:4af69326e088b3c0f82320e9cd97b60c28bf019b984787c6f1c22489e6221f29 in / 
# Wed, 14 Jun 2023 20:42:09 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:24:51 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 15 Jun 2023 06:25:05 GMT
ARG KONG_VERSION=3.0.2
# Thu, 15 Jun 2023 06:25:05 GMT
ENV KONG_VERSION=3.0.2
# Thu, 15 Jun 2023 06:25:05 GMT
ARG KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e
# Thu, 15 Jun 2023 06:25:06 GMT
ARG KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
# Thu, 15 Jun 2023 06:25:06 GMT
ARG ASSET=remote
# Thu, 15 Jun 2023 06:25:06 GMT
ARG EE_PORTS
# Thu, 15 Jun 2023 06:25:06 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Thu, 15 Jun 2023 06:25:14 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Thu, 15 Jun 2023 06:25:14 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 15 Jun 2023 06:25:14 GMT
USER kong
# Thu, 15 Jun 2023 06:25:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Jun 2023 06:25:15 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 15 Jun 2023 06:25:15 GMT
STOPSIGNAL SIGQUIT
# Thu, 15 Jun 2023 06:25:15 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 15 Jun 2023 06:25:15 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:c1d6d1b2d5a367259e6e51a7f4d1ccd66a28cc9940d6599d8a8ea9544dd4b4a8`  
		Last Modified: Wed, 14 Jun 2023 20:42:45 GMT  
		Size: 2.8 MB (2807669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eb51f944ac07d5786d81ea9e5223532bd0fc2724b596128d6c6bfb4622548e7`  
		Last Modified: Thu, 15 Jun 2023 06:26:40 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0ea639b18a7afef1350cd95f2c2c066cca2f54a3df6e97a7e86483e91566e9`  
		Last Modified: Thu, 15 Jun 2023 06:26:47 GMT  
		Size: 72.8 MB (72835718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63061c0a2f964430e9d29a86c8866f9b64a4d76c4102fb4508b66d2eb354f7d`  
		Last Modified: Thu, 15 Jun 2023 06:26:40 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.0-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:440179860d6592ac71ab2aa38baa3b43da04a46e1b8c398f46d23bc1298f8f66
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73631302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66027ffeec8745797878c3e3898ddb0355ff120ecb2634833b84d17c22ece6d4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:07 GMT
ADD file:e80eabe59d1f87ef41634428d9f8fdeb633c2128ac97564f96f5495ef6bf2c72 in / 
# Wed, 14 Jun 2023 20:49:07 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:41:55 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 15 Jun 2023 00:42:07 GMT
ARG KONG_VERSION=3.0.2
# Thu, 15 Jun 2023 00:42:07 GMT
ENV KONG_VERSION=3.0.2
# Thu, 15 Jun 2023 00:42:08 GMT
ARG KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e
# Thu, 15 Jun 2023 00:42:08 GMT
ARG KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
# Thu, 15 Jun 2023 00:42:08 GMT
ARG ASSET=remote
# Thu, 15 Jun 2023 00:42:08 GMT
ARG EE_PORTS
# Thu, 15 Jun 2023 00:42:08 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Thu, 15 Jun 2023 00:42:15 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Thu, 15 Jun 2023 00:42:16 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 15 Jun 2023 00:42:16 GMT
USER kong
# Thu, 15 Jun 2023 00:42:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Jun 2023 00:42:16 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 15 Jun 2023 00:42:16 GMT
STOPSIGNAL SIGQUIT
# Thu, 15 Jun 2023 00:42:16 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 15 Jun 2023 00:42:16 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:a880266d3b77f75696023df2da1ef66c3c565e0f70596242395c9e68de955c7c`  
		Last Modified: Wed, 14 Jun 2023 20:49:43 GMT  
		Size: 2.7 MB (2707906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940d9fed445e052edcf4526f82739dd13d3f896eee44d0e7f5ebee7ef05bcc3b`  
		Last Modified: Thu, 15 Jun 2023 00:43:10 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ef0525a80cd2df99acdab00fb0d3a3c1990e46f334a3a78d96509a5ba1535f`  
		Last Modified: Thu, 15 Jun 2023 00:43:17 GMT  
		Size: 70.9 MB (70922382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e236f022db4cf2d3a5525147f6383071ab5184218e5dcd71a4c6754190fdd8a`  
		Last Modified: Thu, 15 Jun 2023 00:43:10 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.0-ubuntu`

```console
$ docker pull kong@sha256:24cbbbacd3296528e5104559a1b6254e0298052ad485db989bc51cbe13288228
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.0-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:a9b00e2e5bedfec98b8905c13c06fbbef1b53049694673103127af0f7cf1ec90
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101885117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd6b71146c02236181face2ea79de967b9f35501c04573e755fbc4f5d3535b0e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 28 Jun 2023 09:59:08 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:59:08 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:59:10 GMT
ADD file:12f97b7b044d0d1166dd59408c67f5610a764127aa8a01bc57db23bee48911af in / 
# Wed, 28 Jun 2023 09:59:10 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:23:37 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Tue, 04 Jul 2023 18:23:37 GMT
ARG ASSET=ce
# Tue, 04 Jul 2023 18:23:37 GMT
ENV ASSET=ce
# Tue, 04 Jul 2023 18:23:37 GMT
ARG EE_PORTS
# Tue, 04 Jul 2023 18:23:37 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Tue, 04 Jul 2023 18:24:49 GMT
ARG KONG_VERSION=3.0.2
# Tue, 04 Jul 2023 18:24:49 GMT
ENV KONG_VERSION=3.0.2
# Tue, 04 Jul 2023 18:24:49 GMT
ARG KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396
# Tue, 04 Jul 2023 18:24:49 GMT
ARG KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
# Tue, 04 Jul 2023 18:25:10 GMT
# ARGS: KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396 KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 04 Jul 2023 18:25:11 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 04 Jul 2023 18:25:11 GMT
USER kong
# Tue, 04 Jul 2023 18:25:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 18:25:11 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 04 Jul 2023 18:25:11 GMT
STOPSIGNAL SIGQUIT
# Tue, 04 Jul 2023 18:25:11 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 04 Jul 2023 18:25:11 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:0fb668748fc8bb961f4580895692ae741be788857ac2e8220adc2265ffb38e10`  
		Last Modified: Wed, 28 Jun 2023 18:43:28 GMT  
		Size: 28.6 MB (28580012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca31fff16a0a8495754877d21bacf3beb7dc174663d74198527b2743b2adce15`  
		Last Modified: Tue, 04 Jul 2023 18:26:25 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd1f5efc6380ca9e4fd5ebb97213b912e2a19b1ea2c396a316adc9c1a4e87d9`  
		Last Modified: Tue, 04 Jul 2023 18:26:57 GMT  
		Size: 73.3 MB (73304098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0929b62935f73a03cbf0575be3783bdc4570ac590f94eee71a66ac219dc72c`  
		Last Modified: Tue, 04 Jul 2023 18:26:46 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.0-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:08ff21e4a18fe387491cbfa824a842f4ff7066e76b305ad2226fad52988245a8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99132279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db8f116e754610c28dd7752a1b21f729577da19790a35075df99d5f5482c34b3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 28 Jun 2023 09:54:46 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:54:46 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:54:48 GMT
ADD file:a6db9f7789e57b7119f68e4e4ec9ec5aab8c3c8bd53fd932f3c59c54b1c20a26 in / 
# Wed, 28 Jun 2023 09:54:49 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 15:57:19 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Tue, 04 Jul 2023 15:57:19 GMT
ARG ASSET=ce
# Tue, 04 Jul 2023 15:57:19 GMT
ENV ASSET=ce
# Tue, 04 Jul 2023 15:57:19 GMT
ARG EE_PORTS
# Tue, 04 Jul 2023 15:57:19 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Tue, 04 Jul 2023 15:57:44 GMT
ARG KONG_VERSION=3.0.2
# Tue, 04 Jul 2023 15:57:44 GMT
ENV KONG_VERSION=3.0.2
# Tue, 04 Jul 2023 15:57:44 GMT
ARG KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396
# Tue, 04 Jul 2023 15:57:44 GMT
ARG KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
# Tue, 04 Jul 2023 15:58:01 GMT
# ARGS: KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396 KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 04 Jul 2023 15:58:02 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 04 Jul 2023 15:58:02 GMT
USER kong
# Tue, 04 Jul 2023 15:58:02 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 15:58:02 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 04 Jul 2023 15:58:02 GMT
STOPSIGNAL SIGQUIT
# Tue, 04 Jul 2023 15:58:02 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 04 Jul 2023 15:58:03 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:1e77eb131c5c9032ce8e6e512f601714ce7ba48e296f5b7a5191703bdcbc904d`  
		Last Modified: Tue, 04 Jul 2023 04:05:23 GMT  
		Size: 27.2 MB (27198330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ba1ec8088b9154bcb845d99ec7e2e7637af31579cf013dd8dbc7b2afaa1b66`  
		Last Modified: Tue, 04 Jul 2023 15:59:10 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09dd273bc6475225d0fc285678961850026f2b9bd180b6bd7873e5973684007a`  
		Last Modified: Tue, 04 Jul 2023 15:59:38 GMT  
		Size: 71.9 MB (71932944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5417de850f805d56546080bf475ef43d52508160f9c037540678ba5a4b3d1ca1`  
		Last Modified: Tue, 04 Jul 2023 15:59:29 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.0.2`

```console
$ docker pull kong@sha256:c16f02938ab7ae019576dfc17a72e0408393b74ef5a363eb1d9f4d673bffa8f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.0.2` - linux; amd64

```console
$ docker pull kong@sha256:dbdab62f9949e0843b7d8a46740b805940c6214a78bdab5bf61d169075affbc5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75644403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cde42fd180357ec474d41db513f1f83b601663b89a41dedd1b04abb9543e8fd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:09 GMT
ADD file:4af69326e088b3c0f82320e9cd97b60c28bf019b984787c6f1c22489e6221f29 in / 
# Wed, 14 Jun 2023 20:42:09 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:24:51 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 15 Jun 2023 06:25:05 GMT
ARG KONG_VERSION=3.0.2
# Thu, 15 Jun 2023 06:25:05 GMT
ENV KONG_VERSION=3.0.2
# Thu, 15 Jun 2023 06:25:05 GMT
ARG KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e
# Thu, 15 Jun 2023 06:25:06 GMT
ARG KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
# Thu, 15 Jun 2023 06:25:06 GMT
ARG ASSET=remote
# Thu, 15 Jun 2023 06:25:06 GMT
ARG EE_PORTS
# Thu, 15 Jun 2023 06:25:06 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Thu, 15 Jun 2023 06:25:14 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Thu, 15 Jun 2023 06:25:14 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 15 Jun 2023 06:25:14 GMT
USER kong
# Thu, 15 Jun 2023 06:25:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Jun 2023 06:25:15 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 15 Jun 2023 06:25:15 GMT
STOPSIGNAL SIGQUIT
# Thu, 15 Jun 2023 06:25:15 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 15 Jun 2023 06:25:15 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:c1d6d1b2d5a367259e6e51a7f4d1ccd66a28cc9940d6599d8a8ea9544dd4b4a8`  
		Last Modified: Wed, 14 Jun 2023 20:42:45 GMT  
		Size: 2.8 MB (2807669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eb51f944ac07d5786d81ea9e5223532bd0fc2724b596128d6c6bfb4622548e7`  
		Last Modified: Thu, 15 Jun 2023 06:26:40 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0ea639b18a7afef1350cd95f2c2c066cca2f54a3df6e97a7e86483e91566e9`  
		Last Modified: Thu, 15 Jun 2023 06:26:47 GMT  
		Size: 72.8 MB (72835718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63061c0a2f964430e9d29a86c8866f9b64a4d76c4102fb4508b66d2eb354f7d`  
		Last Modified: Thu, 15 Jun 2023 06:26:40 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.0.2` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:440179860d6592ac71ab2aa38baa3b43da04a46e1b8c398f46d23bc1298f8f66
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73631302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66027ffeec8745797878c3e3898ddb0355ff120ecb2634833b84d17c22ece6d4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:07 GMT
ADD file:e80eabe59d1f87ef41634428d9f8fdeb633c2128ac97564f96f5495ef6bf2c72 in / 
# Wed, 14 Jun 2023 20:49:07 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:41:55 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 15 Jun 2023 00:42:07 GMT
ARG KONG_VERSION=3.0.2
# Thu, 15 Jun 2023 00:42:07 GMT
ENV KONG_VERSION=3.0.2
# Thu, 15 Jun 2023 00:42:08 GMT
ARG KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e
# Thu, 15 Jun 2023 00:42:08 GMT
ARG KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
# Thu, 15 Jun 2023 00:42:08 GMT
ARG ASSET=remote
# Thu, 15 Jun 2023 00:42:08 GMT
ARG EE_PORTS
# Thu, 15 Jun 2023 00:42:08 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Thu, 15 Jun 2023 00:42:15 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Thu, 15 Jun 2023 00:42:16 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 15 Jun 2023 00:42:16 GMT
USER kong
# Thu, 15 Jun 2023 00:42:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Jun 2023 00:42:16 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 15 Jun 2023 00:42:16 GMT
STOPSIGNAL SIGQUIT
# Thu, 15 Jun 2023 00:42:16 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 15 Jun 2023 00:42:16 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:a880266d3b77f75696023df2da1ef66c3c565e0f70596242395c9e68de955c7c`  
		Last Modified: Wed, 14 Jun 2023 20:49:43 GMT  
		Size: 2.7 MB (2707906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940d9fed445e052edcf4526f82739dd13d3f896eee44d0e7f5ebee7ef05bcc3b`  
		Last Modified: Thu, 15 Jun 2023 00:43:10 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ef0525a80cd2df99acdab00fb0d3a3c1990e46f334a3a78d96509a5ba1535f`  
		Last Modified: Thu, 15 Jun 2023 00:43:17 GMT  
		Size: 70.9 MB (70922382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e236f022db4cf2d3a5525147f6383071ab5184218e5dcd71a4c6754190fdd8a`  
		Last Modified: Thu, 15 Jun 2023 00:43:10 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.0.2-alpine`

```console
$ docker pull kong@sha256:c16f02938ab7ae019576dfc17a72e0408393b74ef5a363eb1d9f4d673bffa8f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.0.2-alpine` - linux; amd64

```console
$ docker pull kong@sha256:dbdab62f9949e0843b7d8a46740b805940c6214a78bdab5bf61d169075affbc5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75644403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cde42fd180357ec474d41db513f1f83b601663b89a41dedd1b04abb9543e8fd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:09 GMT
ADD file:4af69326e088b3c0f82320e9cd97b60c28bf019b984787c6f1c22489e6221f29 in / 
# Wed, 14 Jun 2023 20:42:09 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:24:51 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 15 Jun 2023 06:25:05 GMT
ARG KONG_VERSION=3.0.2
# Thu, 15 Jun 2023 06:25:05 GMT
ENV KONG_VERSION=3.0.2
# Thu, 15 Jun 2023 06:25:05 GMT
ARG KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e
# Thu, 15 Jun 2023 06:25:06 GMT
ARG KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
# Thu, 15 Jun 2023 06:25:06 GMT
ARG ASSET=remote
# Thu, 15 Jun 2023 06:25:06 GMT
ARG EE_PORTS
# Thu, 15 Jun 2023 06:25:06 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Thu, 15 Jun 2023 06:25:14 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Thu, 15 Jun 2023 06:25:14 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 15 Jun 2023 06:25:14 GMT
USER kong
# Thu, 15 Jun 2023 06:25:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Jun 2023 06:25:15 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 15 Jun 2023 06:25:15 GMT
STOPSIGNAL SIGQUIT
# Thu, 15 Jun 2023 06:25:15 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 15 Jun 2023 06:25:15 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:c1d6d1b2d5a367259e6e51a7f4d1ccd66a28cc9940d6599d8a8ea9544dd4b4a8`  
		Last Modified: Wed, 14 Jun 2023 20:42:45 GMT  
		Size: 2.8 MB (2807669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eb51f944ac07d5786d81ea9e5223532bd0fc2724b596128d6c6bfb4622548e7`  
		Last Modified: Thu, 15 Jun 2023 06:26:40 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0ea639b18a7afef1350cd95f2c2c066cca2f54a3df6e97a7e86483e91566e9`  
		Last Modified: Thu, 15 Jun 2023 06:26:47 GMT  
		Size: 72.8 MB (72835718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f63061c0a2f964430e9d29a86c8866f9b64a4d76c4102fb4508b66d2eb354f7d`  
		Last Modified: Thu, 15 Jun 2023 06:26:40 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.0.2-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:440179860d6592ac71ab2aa38baa3b43da04a46e1b8c398f46d23bc1298f8f66
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73631302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66027ffeec8745797878c3e3898ddb0355ff120ecb2634833b84d17c22ece6d4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:07 GMT
ADD file:e80eabe59d1f87ef41634428d9f8fdeb633c2128ac97564f96f5495ef6bf2c72 in / 
# Wed, 14 Jun 2023 20:49:07 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:41:55 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 15 Jun 2023 00:42:07 GMT
ARG KONG_VERSION=3.0.2
# Thu, 15 Jun 2023 00:42:07 GMT
ENV KONG_VERSION=3.0.2
# Thu, 15 Jun 2023 00:42:08 GMT
ARG KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e
# Thu, 15 Jun 2023 00:42:08 GMT
ARG KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
# Thu, 15 Jun 2023 00:42:08 GMT
ARG ASSET=remote
# Thu, 15 Jun 2023 00:42:08 GMT
ARG EE_PORTS
# Thu, 15 Jun 2023 00:42:08 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Thu, 15 Jun 2023 00:42:15 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Thu, 15 Jun 2023 00:42:16 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 15 Jun 2023 00:42:16 GMT
USER kong
# Thu, 15 Jun 2023 00:42:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Jun 2023 00:42:16 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 15 Jun 2023 00:42:16 GMT
STOPSIGNAL SIGQUIT
# Thu, 15 Jun 2023 00:42:16 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 15 Jun 2023 00:42:16 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:a880266d3b77f75696023df2da1ef66c3c565e0f70596242395c9e68de955c7c`  
		Last Modified: Wed, 14 Jun 2023 20:49:43 GMT  
		Size: 2.7 MB (2707906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940d9fed445e052edcf4526f82739dd13d3f896eee44d0e7f5ebee7ef05bcc3b`  
		Last Modified: Thu, 15 Jun 2023 00:43:10 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ef0525a80cd2df99acdab00fb0d3a3c1990e46f334a3a78d96509a5ba1535f`  
		Last Modified: Thu, 15 Jun 2023 00:43:17 GMT  
		Size: 70.9 MB (70922382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e236f022db4cf2d3a5525147f6383071ab5184218e5dcd71a4c6754190fdd8a`  
		Last Modified: Thu, 15 Jun 2023 00:43:10 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.0.2-ubuntu`

```console
$ docker pull kong@sha256:24cbbbacd3296528e5104559a1b6254e0298052ad485db989bc51cbe13288228
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.0.2-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:a9b00e2e5bedfec98b8905c13c06fbbef1b53049694673103127af0f7cf1ec90
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101885117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd6b71146c02236181face2ea79de967b9f35501c04573e755fbc4f5d3535b0e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 28 Jun 2023 09:59:08 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:59:08 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:59:10 GMT
ADD file:12f97b7b044d0d1166dd59408c67f5610a764127aa8a01bc57db23bee48911af in / 
# Wed, 28 Jun 2023 09:59:10 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:23:37 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Tue, 04 Jul 2023 18:23:37 GMT
ARG ASSET=ce
# Tue, 04 Jul 2023 18:23:37 GMT
ENV ASSET=ce
# Tue, 04 Jul 2023 18:23:37 GMT
ARG EE_PORTS
# Tue, 04 Jul 2023 18:23:37 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Tue, 04 Jul 2023 18:24:49 GMT
ARG KONG_VERSION=3.0.2
# Tue, 04 Jul 2023 18:24:49 GMT
ENV KONG_VERSION=3.0.2
# Tue, 04 Jul 2023 18:24:49 GMT
ARG KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396
# Tue, 04 Jul 2023 18:24:49 GMT
ARG KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
# Tue, 04 Jul 2023 18:25:10 GMT
# ARGS: KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396 KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 04 Jul 2023 18:25:11 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 04 Jul 2023 18:25:11 GMT
USER kong
# Tue, 04 Jul 2023 18:25:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 18:25:11 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 04 Jul 2023 18:25:11 GMT
STOPSIGNAL SIGQUIT
# Tue, 04 Jul 2023 18:25:11 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 04 Jul 2023 18:25:11 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:0fb668748fc8bb961f4580895692ae741be788857ac2e8220adc2265ffb38e10`  
		Last Modified: Wed, 28 Jun 2023 18:43:28 GMT  
		Size: 28.6 MB (28580012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca31fff16a0a8495754877d21bacf3beb7dc174663d74198527b2743b2adce15`  
		Last Modified: Tue, 04 Jul 2023 18:26:25 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd1f5efc6380ca9e4fd5ebb97213b912e2a19b1ea2c396a316adc9c1a4e87d9`  
		Last Modified: Tue, 04 Jul 2023 18:26:57 GMT  
		Size: 73.3 MB (73304098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0929b62935f73a03cbf0575be3783bdc4570ac590f94eee71a66ac219dc72c`  
		Last Modified: Tue, 04 Jul 2023 18:26:46 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.0.2-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:08ff21e4a18fe387491cbfa824a842f4ff7066e76b305ad2226fad52988245a8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99132279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db8f116e754610c28dd7752a1b21f729577da19790a35075df99d5f5482c34b3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 28 Jun 2023 09:54:46 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:54:46 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:54:48 GMT
ADD file:a6db9f7789e57b7119f68e4e4ec9ec5aab8c3c8bd53fd932f3c59c54b1c20a26 in / 
# Wed, 28 Jun 2023 09:54:49 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 15:57:19 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Tue, 04 Jul 2023 15:57:19 GMT
ARG ASSET=ce
# Tue, 04 Jul 2023 15:57:19 GMT
ENV ASSET=ce
# Tue, 04 Jul 2023 15:57:19 GMT
ARG EE_PORTS
# Tue, 04 Jul 2023 15:57:19 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Tue, 04 Jul 2023 15:57:44 GMT
ARG KONG_VERSION=3.0.2
# Tue, 04 Jul 2023 15:57:44 GMT
ENV KONG_VERSION=3.0.2
# Tue, 04 Jul 2023 15:57:44 GMT
ARG KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396
# Tue, 04 Jul 2023 15:57:44 GMT
ARG KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
# Tue, 04 Jul 2023 15:58:01 GMT
# ARGS: KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396 KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 04 Jul 2023 15:58:02 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 04 Jul 2023 15:58:02 GMT
USER kong
# Tue, 04 Jul 2023 15:58:02 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 15:58:02 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 04 Jul 2023 15:58:02 GMT
STOPSIGNAL SIGQUIT
# Tue, 04 Jul 2023 15:58:02 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 04 Jul 2023 15:58:03 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:1e77eb131c5c9032ce8e6e512f601714ce7ba48e296f5b7a5191703bdcbc904d`  
		Last Modified: Tue, 04 Jul 2023 04:05:23 GMT  
		Size: 27.2 MB (27198330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ba1ec8088b9154bcb845d99ec7e2e7637af31579cf013dd8dbc7b2afaa1b66`  
		Last Modified: Tue, 04 Jul 2023 15:59:10 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09dd273bc6475225d0fc285678961850026f2b9bd180b6bd7873e5973684007a`  
		Last Modified: Tue, 04 Jul 2023 15:59:38 GMT  
		Size: 71.9 MB (71932944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5417de850f805d56546080bf475ef43d52508160f9c037540678ba5a4b3d1ca1`  
		Last Modified: Tue, 04 Jul 2023 15:59:29 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.1`

```console
$ docker pull kong@sha256:f8a5fbd18b2aa19765201e26c1104def41a8ec6177a80840939307062270fbf0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.1` - linux; amd64

```console
$ docker pull kong@sha256:69b75ed0bdb6ba6e81d90d2aedcab947d67f9565644d64fc112b56cdc1500d97
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75688911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8929f3c41e7e38ceda54c16364709ce8fa22846a410d5eb933ce5bd8d1d4966`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:09 GMT
ADD file:4af69326e088b3c0f82320e9cd97b60c28bf019b984787c6f1c22489e6221f29 in / 
# Wed, 14 Jun 2023 20:42:09 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:24:51 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 15 Jun 2023 06:24:51 GMT
ARG KONG_VERSION=3.1.1
# Thu, 15 Jun 2023 06:24:51 GMT
ENV KONG_VERSION=3.1.1
# Thu, 15 Jun 2023 06:24:52 GMT
ARG KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c
# Thu, 15 Jun 2023 06:24:52 GMT
ARG KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
# Thu, 15 Jun 2023 06:24:52 GMT
ARG ASSET=remote
# Thu, 15 Jun 2023 06:24:52 GMT
ARG EE_PORTS
# Thu, 15 Jun 2023 06:24:52 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Thu, 15 Jun 2023 06:24:59 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Thu, 15 Jun 2023 06:24:59 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 15 Jun 2023 06:24:59 GMT
USER kong
# Thu, 15 Jun 2023 06:24:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Jun 2023 06:24:59 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 15 Jun 2023 06:25:00 GMT
STOPSIGNAL SIGQUIT
# Thu, 15 Jun 2023 06:25:00 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 15 Jun 2023 06:25:00 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:c1d6d1b2d5a367259e6e51a7f4d1ccd66a28cc9940d6599d8a8ea9544dd4b4a8`  
		Last Modified: Wed, 14 Jun 2023 20:42:45 GMT  
		Size: 2.8 MB (2807669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5cc8882a14901bbac226d538a5a1189bc09c6051ce266e3796316d2fd5c06b`  
		Last Modified: Thu, 15 Jun 2023 06:26:20 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63d89016896ec2b5175ddfe42106245e95d33efcd4521f46d7eaebb0ad30f13`  
		Last Modified: Thu, 15 Jun 2023 06:26:28 GMT  
		Size: 72.9 MB (72880224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46f4698ce39118443bf7df323b3355fc755e901a7217156d40f920f5297fada`  
		Last Modified: Thu, 15 Jun 2023 06:26:20 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.1` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:23d3a20180d1bf763ad7360b7c9ed51d222953736b5d672ddc4921dba8daab74
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.7 MB (73704647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be03fcbc57b0bccedc31292d3be6d1c56896251b5aebf0a86f74fe3bf8a1ed1b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:07 GMT
ADD file:e80eabe59d1f87ef41634428d9f8fdeb633c2128ac97564f96f5495ef6bf2c72 in / 
# Wed, 14 Jun 2023 20:49:07 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:41:55 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 15 Jun 2023 00:41:55 GMT
ARG KONG_VERSION=3.1.1
# Thu, 15 Jun 2023 00:41:55 GMT
ENV KONG_VERSION=3.1.1
# Thu, 15 Jun 2023 00:41:55 GMT
ARG KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c
# Thu, 15 Jun 2023 00:41:55 GMT
ARG KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
# Thu, 15 Jun 2023 00:41:55 GMT
ARG ASSET=remote
# Thu, 15 Jun 2023 00:41:55 GMT
ARG EE_PORTS
# Thu, 15 Jun 2023 00:41:55 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Thu, 15 Jun 2023 00:42:02 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Thu, 15 Jun 2023 00:42:02 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 15 Jun 2023 00:42:02 GMT
USER kong
# Thu, 15 Jun 2023 00:42:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Jun 2023 00:42:03 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 15 Jun 2023 00:42:03 GMT
STOPSIGNAL SIGQUIT
# Thu, 15 Jun 2023 00:42:03 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 15 Jun 2023 00:42:03 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:a880266d3b77f75696023df2da1ef66c3c565e0f70596242395c9e68de955c7c`  
		Last Modified: Wed, 14 Jun 2023 20:49:43 GMT  
		Size: 2.7 MB (2707906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9e3e57ed4acbf2d9f596b31a20c6341d8172233d7291253d484be6a57df0c9f`  
		Last Modified: Thu, 15 Jun 2023 00:42:52 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e50a11265ca59622b21c480195c8d6017270abaa14e97d0ba2db719a8364f4e`  
		Last Modified: Thu, 15 Jun 2023 00:42:59 GMT  
		Size: 71.0 MB (70995728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497a79f5e6a72fce6df0f2ec91f63cce422cdd5e233cb3889cb83127d0c9effc`  
		Last Modified: Thu, 15 Jun 2023 00:42:52 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.1-ubuntu`

```console
$ docker pull kong@sha256:0f757da173431431a4f118db9faa885159d8b8c42f88a6a5a9bf925e95c23ccd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.1-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:3fe1c4e4880f3033ba6a419f5a3879f87a6b684fd9dfb7535b83e8f6a82ff01e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101909355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56754fb0001a2925811ea8f84eb2bd6f57cdc914df677b297738f2a482181956`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 28 Jun 2023 09:59:08 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:59:08 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:59:10 GMT
ADD file:12f97b7b044d0d1166dd59408c67f5610a764127aa8a01bc57db23bee48911af in / 
# Wed, 28 Jun 2023 09:59:10 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:23:37 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Tue, 04 Jul 2023 18:23:37 GMT
ARG ASSET=ce
# Tue, 04 Jul 2023 18:23:37 GMT
ENV ASSET=ce
# Tue, 04 Jul 2023 18:23:37 GMT
ARG EE_PORTS
# Tue, 04 Jul 2023 18:23:37 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Tue, 04 Jul 2023 18:23:38 GMT
ARG KONG_VERSION=3.1.1
# Tue, 04 Jul 2023 18:23:38 GMT
ENV KONG_VERSION=3.1.1
# Tue, 04 Jul 2023 18:23:38 GMT
ARG KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b
# Tue, 04 Jul 2023 18:23:38 GMT
ARG KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
# Tue, 04 Jul 2023 18:24:34 GMT
# ARGS: KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 04 Jul 2023 18:24:35 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 04 Jul 2023 18:24:35 GMT
USER kong
# Tue, 04 Jul 2023 18:24:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 18:24:35 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 04 Jul 2023 18:24:35 GMT
STOPSIGNAL SIGQUIT
# Tue, 04 Jul 2023 18:24:35 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 04 Jul 2023 18:24:35 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:0fb668748fc8bb961f4580895692ae741be788857ac2e8220adc2265ffb38e10`  
		Last Modified: Wed, 28 Jun 2023 18:43:28 GMT  
		Size: 28.6 MB (28580012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca31fff16a0a8495754877d21bacf3beb7dc174663d74198527b2743b2adce15`  
		Last Modified: Tue, 04 Jul 2023 18:26:25 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7faf7329a8b33ac2647d06da7b6220b6057d486a75f93bad2677994bb13d25`  
		Last Modified: Tue, 04 Jul 2023 18:26:37 GMT  
		Size: 73.3 MB (73328336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c233133e90400e8ccdb4db1b93e9c81fcf32b48755f4a8985f904f02cdee881a`  
		Last Modified: Tue, 04 Jul 2023 18:26:25 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.1-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:c82681ab3ea123ad4ef6e025bd4a5689d2126d1376367cb32f9927173f9cf3d4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99164836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23131b26255ed1b3841bd4f322fe3d005c6c4549f2dceaf2af1e63a87eccd124`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 28 Jun 2023 09:54:46 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:54:46 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:54:48 GMT
ADD file:a6db9f7789e57b7119f68e4e4ec9ec5aab8c3c8bd53fd932f3c59c54b1c20a26 in / 
# Wed, 28 Jun 2023 09:54:49 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 15:57:19 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Tue, 04 Jul 2023 15:57:19 GMT
ARG ASSET=ce
# Tue, 04 Jul 2023 15:57:19 GMT
ENV ASSET=ce
# Tue, 04 Jul 2023 15:57:19 GMT
ARG EE_PORTS
# Tue, 04 Jul 2023 15:57:19 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Tue, 04 Jul 2023 15:57:19 GMT
ARG KONG_VERSION=3.1.1
# Tue, 04 Jul 2023 15:57:19 GMT
ENV KONG_VERSION=3.1.1
# Tue, 04 Jul 2023 15:57:19 GMT
ARG KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b
# Tue, 04 Jul 2023 15:57:20 GMT
ARG KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
# Tue, 04 Jul 2023 15:57:38 GMT
# ARGS: KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 04 Jul 2023 15:57:39 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 04 Jul 2023 15:57:39 GMT
USER kong
# Tue, 04 Jul 2023 15:57:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 15:57:39 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 04 Jul 2023 15:57:39 GMT
STOPSIGNAL SIGQUIT
# Tue, 04 Jul 2023 15:57:39 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 04 Jul 2023 15:57:39 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:1e77eb131c5c9032ce8e6e512f601714ce7ba48e296f5b7a5191703bdcbc904d`  
		Last Modified: Tue, 04 Jul 2023 04:05:23 GMT  
		Size: 27.2 MB (27198330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ba1ec8088b9154bcb845d99ec7e2e7637af31579cf013dd8dbc7b2afaa1b66`  
		Last Modified: Tue, 04 Jul 2023 15:59:10 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c0446f9290d8256310c24bda8d8333889e72c5aa4bced69d1decff330c1c00`  
		Last Modified: Tue, 04 Jul 2023 15:59:19 GMT  
		Size: 72.0 MB (71965501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca06d4f66f0ce183149a3f415d7645008872a0431059625c8064c241a0445ce`  
		Last Modified: Tue, 04 Jul 2023 15:59:10 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.1.1`

```console
$ docker pull kong@sha256:f8a5fbd18b2aa19765201e26c1104def41a8ec6177a80840939307062270fbf0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.1.1` - linux; amd64

```console
$ docker pull kong@sha256:69b75ed0bdb6ba6e81d90d2aedcab947d67f9565644d64fc112b56cdc1500d97
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75688911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8929f3c41e7e38ceda54c16364709ce8fa22846a410d5eb933ce5bd8d1d4966`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:09 GMT
ADD file:4af69326e088b3c0f82320e9cd97b60c28bf019b984787c6f1c22489e6221f29 in / 
# Wed, 14 Jun 2023 20:42:09 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:24:51 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 15 Jun 2023 06:24:51 GMT
ARG KONG_VERSION=3.1.1
# Thu, 15 Jun 2023 06:24:51 GMT
ENV KONG_VERSION=3.1.1
# Thu, 15 Jun 2023 06:24:52 GMT
ARG KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c
# Thu, 15 Jun 2023 06:24:52 GMT
ARG KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
# Thu, 15 Jun 2023 06:24:52 GMT
ARG ASSET=remote
# Thu, 15 Jun 2023 06:24:52 GMT
ARG EE_PORTS
# Thu, 15 Jun 2023 06:24:52 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Thu, 15 Jun 2023 06:24:59 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Thu, 15 Jun 2023 06:24:59 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 15 Jun 2023 06:24:59 GMT
USER kong
# Thu, 15 Jun 2023 06:24:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Jun 2023 06:24:59 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 15 Jun 2023 06:25:00 GMT
STOPSIGNAL SIGQUIT
# Thu, 15 Jun 2023 06:25:00 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 15 Jun 2023 06:25:00 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:c1d6d1b2d5a367259e6e51a7f4d1ccd66a28cc9940d6599d8a8ea9544dd4b4a8`  
		Last Modified: Wed, 14 Jun 2023 20:42:45 GMT  
		Size: 2.8 MB (2807669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5cc8882a14901bbac226d538a5a1189bc09c6051ce266e3796316d2fd5c06b`  
		Last Modified: Thu, 15 Jun 2023 06:26:20 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63d89016896ec2b5175ddfe42106245e95d33efcd4521f46d7eaebb0ad30f13`  
		Last Modified: Thu, 15 Jun 2023 06:26:28 GMT  
		Size: 72.9 MB (72880224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46f4698ce39118443bf7df323b3355fc755e901a7217156d40f920f5297fada`  
		Last Modified: Thu, 15 Jun 2023 06:26:20 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.1.1` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:23d3a20180d1bf763ad7360b7c9ed51d222953736b5d672ddc4921dba8daab74
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.7 MB (73704647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be03fcbc57b0bccedc31292d3be6d1c56896251b5aebf0a86f74fe3bf8a1ed1b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:07 GMT
ADD file:e80eabe59d1f87ef41634428d9f8fdeb633c2128ac97564f96f5495ef6bf2c72 in / 
# Wed, 14 Jun 2023 20:49:07 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:41:55 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 15 Jun 2023 00:41:55 GMT
ARG KONG_VERSION=3.1.1
# Thu, 15 Jun 2023 00:41:55 GMT
ENV KONG_VERSION=3.1.1
# Thu, 15 Jun 2023 00:41:55 GMT
ARG KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c
# Thu, 15 Jun 2023 00:41:55 GMT
ARG KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
# Thu, 15 Jun 2023 00:41:55 GMT
ARG ASSET=remote
# Thu, 15 Jun 2023 00:41:55 GMT
ARG EE_PORTS
# Thu, 15 Jun 2023 00:41:55 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Thu, 15 Jun 2023 00:42:02 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Thu, 15 Jun 2023 00:42:02 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 15 Jun 2023 00:42:02 GMT
USER kong
# Thu, 15 Jun 2023 00:42:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Jun 2023 00:42:03 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 15 Jun 2023 00:42:03 GMT
STOPSIGNAL SIGQUIT
# Thu, 15 Jun 2023 00:42:03 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 15 Jun 2023 00:42:03 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:a880266d3b77f75696023df2da1ef66c3c565e0f70596242395c9e68de955c7c`  
		Last Modified: Wed, 14 Jun 2023 20:49:43 GMT  
		Size: 2.7 MB (2707906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9e3e57ed4acbf2d9f596b31a20c6341d8172233d7291253d484be6a57df0c9f`  
		Last Modified: Thu, 15 Jun 2023 00:42:52 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e50a11265ca59622b21c480195c8d6017270abaa14e97d0ba2db719a8364f4e`  
		Last Modified: Thu, 15 Jun 2023 00:42:59 GMT  
		Size: 71.0 MB (70995728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497a79f5e6a72fce6df0f2ec91f63cce422cdd5e233cb3889cb83127d0c9effc`  
		Last Modified: Thu, 15 Jun 2023 00:42:52 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.1.1-alpine`

```console
$ docker pull kong@sha256:f8a5fbd18b2aa19765201e26c1104def41a8ec6177a80840939307062270fbf0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.1.1-alpine` - linux; amd64

```console
$ docker pull kong@sha256:69b75ed0bdb6ba6e81d90d2aedcab947d67f9565644d64fc112b56cdc1500d97
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75688911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8929f3c41e7e38ceda54c16364709ce8fa22846a410d5eb933ce5bd8d1d4966`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:09 GMT
ADD file:4af69326e088b3c0f82320e9cd97b60c28bf019b984787c6f1c22489e6221f29 in / 
# Wed, 14 Jun 2023 20:42:09 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:24:51 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 15 Jun 2023 06:24:51 GMT
ARG KONG_VERSION=3.1.1
# Thu, 15 Jun 2023 06:24:51 GMT
ENV KONG_VERSION=3.1.1
# Thu, 15 Jun 2023 06:24:52 GMT
ARG KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c
# Thu, 15 Jun 2023 06:24:52 GMT
ARG KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
# Thu, 15 Jun 2023 06:24:52 GMT
ARG ASSET=remote
# Thu, 15 Jun 2023 06:24:52 GMT
ARG EE_PORTS
# Thu, 15 Jun 2023 06:24:52 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Thu, 15 Jun 2023 06:24:59 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Thu, 15 Jun 2023 06:24:59 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 15 Jun 2023 06:24:59 GMT
USER kong
# Thu, 15 Jun 2023 06:24:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Jun 2023 06:24:59 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 15 Jun 2023 06:25:00 GMT
STOPSIGNAL SIGQUIT
# Thu, 15 Jun 2023 06:25:00 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 15 Jun 2023 06:25:00 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:c1d6d1b2d5a367259e6e51a7f4d1ccd66a28cc9940d6599d8a8ea9544dd4b4a8`  
		Last Modified: Wed, 14 Jun 2023 20:42:45 GMT  
		Size: 2.8 MB (2807669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5cc8882a14901bbac226d538a5a1189bc09c6051ce266e3796316d2fd5c06b`  
		Last Modified: Thu, 15 Jun 2023 06:26:20 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63d89016896ec2b5175ddfe42106245e95d33efcd4521f46d7eaebb0ad30f13`  
		Last Modified: Thu, 15 Jun 2023 06:26:28 GMT  
		Size: 72.9 MB (72880224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b46f4698ce39118443bf7df323b3355fc755e901a7217156d40f920f5297fada`  
		Last Modified: Thu, 15 Jun 2023 06:26:20 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.1.1-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:23d3a20180d1bf763ad7360b7c9ed51d222953736b5d672ddc4921dba8daab74
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.7 MB (73704647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be03fcbc57b0bccedc31292d3be6d1c56896251b5aebf0a86f74fe3bf8a1ed1b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:07 GMT
ADD file:e80eabe59d1f87ef41634428d9f8fdeb633c2128ac97564f96f5495ef6bf2c72 in / 
# Wed, 14 Jun 2023 20:49:07 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:41:55 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 15 Jun 2023 00:41:55 GMT
ARG KONG_VERSION=3.1.1
# Thu, 15 Jun 2023 00:41:55 GMT
ENV KONG_VERSION=3.1.1
# Thu, 15 Jun 2023 00:41:55 GMT
ARG KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c
# Thu, 15 Jun 2023 00:41:55 GMT
ARG KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
# Thu, 15 Jun 2023 00:41:55 GMT
ARG ASSET=remote
# Thu, 15 Jun 2023 00:41:55 GMT
ARG EE_PORTS
# Thu, 15 Jun 2023 00:41:55 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Thu, 15 Jun 2023 00:42:02 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Thu, 15 Jun 2023 00:42:02 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 15 Jun 2023 00:42:02 GMT
USER kong
# Thu, 15 Jun 2023 00:42:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Jun 2023 00:42:03 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 15 Jun 2023 00:42:03 GMT
STOPSIGNAL SIGQUIT
# Thu, 15 Jun 2023 00:42:03 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 15 Jun 2023 00:42:03 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:a880266d3b77f75696023df2da1ef66c3c565e0f70596242395c9e68de955c7c`  
		Last Modified: Wed, 14 Jun 2023 20:49:43 GMT  
		Size: 2.7 MB (2707906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9e3e57ed4acbf2d9f596b31a20c6341d8172233d7291253d484be6a57df0c9f`  
		Last Modified: Thu, 15 Jun 2023 00:42:52 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e50a11265ca59622b21c480195c8d6017270abaa14e97d0ba2db719a8364f4e`  
		Last Modified: Thu, 15 Jun 2023 00:42:59 GMT  
		Size: 71.0 MB (70995728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497a79f5e6a72fce6df0f2ec91f63cce422cdd5e233cb3889cb83127d0c9effc`  
		Last Modified: Thu, 15 Jun 2023 00:42:52 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.1.1-ubuntu`

```console
$ docker pull kong@sha256:0f757da173431431a4f118db9faa885159d8b8c42f88a6a5a9bf925e95c23ccd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.1.1-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:3fe1c4e4880f3033ba6a419f5a3879f87a6b684fd9dfb7535b83e8f6a82ff01e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101909355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56754fb0001a2925811ea8f84eb2bd6f57cdc914df677b297738f2a482181956`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 28 Jun 2023 09:59:08 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:59:08 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:59:10 GMT
ADD file:12f97b7b044d0d1166dd59408c67f5610a764127aa8a01bc57db23bee48911af in / 
# Wed, 28 Jun 2023 09:59:10 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:23:37 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Tue, 04 Jul 2023 18:23:37 GMT
ARG ASSET=ce
# Tue, 04 Jul 2023 18:23:37 GMT
ENV ASSET=ce
# Tue, 04 Jul 2023 18:23:37 GMT
ARG EE_PORTS
# Tue, 04 Jul 2023 18:23:37 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Tue, 04 Jul 2023 18:23:38 GMT
ARG KONG_VERSION=3.1.1
# Tue, 04 Jul 2023 18:23:38 GMT
ENV KONG_VERSION=3.1.1
# Tue, 04 Jul 2023 18:23:38 GMT
ARG KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b
# Tue, 04 Jul 2023 18:23:38 GMT
ARG KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
# Tue, 04 Jul 2023 18:24:34 GMT
# ARGS: KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 04 Jul 2023 18:24:35 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 04 Jul 2023 18:24:35 GMT
USER kong
# Tue, 04 Jul 2023 18:24:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 18:24:35 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 04 Jul 2023 18:24:35 GMT
STOPSIGNAL SIGQUIT
# Tue, 04 Jul 2023 18:24:35 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 04 Jul 2023 18:24:35 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:0fb668748fc8bb961f4580895692ae741be788857ac2e8220adc2265ffb38e10`  
		Last Modified: Wed, 28 Jun 2023 18:43:28 GMT  
		Size: 28.6 MB (28580012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca31fff16a0a8495754877d21bacf3beb7dc174663d74198527b2743b2adce15`  
		Last Modified: Tue, 04 Jul 2023 18:26:25 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7faf7329a8b33ac2647d06da7b6220b6057d486a75f93bad2677994bb13d25`  
		Last Modified: Tue, 04 Jul 2023 18:26:37 GMT  
		Size: 73.3 MB (73328336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c233133e90400e8ccdb4db1b93e9c81fcf32b48755f4a8985f904f02cdee881a`  
		Last Modified: Tue, 04 Jul 2023 18:26:25 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.1.1-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:c82681ab3ea123ad4ef6e025bd4a5689d2126d1376367cb32f9927173f9cf3d4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99164836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23131b26255ed1b3841bd4f322fe3d005c6c4549f2dceaf2af1e63a87eccd124`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 28 Jun 2023 09:54:46 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:54:46 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:54:48 GMT
ADD file:a6db9f7789e57b7119f68e4e4ec9ec5aab8c3c8bd53fd932f3c59c54b1c20a26 in / 
# Wed, 28 Jun 2023 09:54:49 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 15:57:19 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Tue, 04 Jul 2023 15:57:19 GMT
ARG ASSET=ce
# Tue, 04 Jul 2023 15:57:19 GMT
ENV ASSET=ce
# Tue, 04 Jul 2023 15:57:19 GMT
ARG EE_PORTS
# Tue, 04 Jul 2023 15:57:19 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Tue, 04 Jul 2023 15:57:19 GMT
ARG KONG_VERSION=3.1.1
# Tue, 04 Jul 2023 15:57:19 GMT
ENV KONG_VERSION=3.1.1
# Tue, 04 Jul 2023 15:57:19 GMT
ARG KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b
# Tue, 04 Jul 2023 15:57:20 GMT
ARG KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
# Tue, 04 Jul 2023 15:57:38 GMT
# ARGS: KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 04 Jul 2023 15:57:39 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 04 Jul 2023 15:57:39 GMT
USER kong
# Tue, 04 Jul 2023 15:57:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 15:57:39 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 04 Jul 2023 15:57:39 GMT
STOPSIGNAL SIGQUIT
# Tue, 04 Jul 2023 15:57:39 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 04 Jul 2023 15:57:39 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:1e77eb131c5c9032ce8e6e512f601714ce7ba48e296f5b7a5191703bdcbc904d`  
		Last Modified: Tue, 04 Jul 2023 04:05:23 GMT  
		Size: 27.2 MB (27198330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ba1ec8088b9154bcb845d99ec7e2e7637af31579cf013dd8dbc7b2afaa1b66`  
		Last Modified: Tue, 04 Jul 2023 15:59:10 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c0446f9290d8256310c24bda8d8333889e72c5aa4bced69d1decff330c1c00`  
		Last Modified: Tue, 04 Jul 2023 15:59:19 GMT  
		Size: 72.0 MB (71965501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca06d4f66f0ce183149a3f415d7645008872a0431059625c8064c241a0445ce`  
		Last Modified: Tue, 04 Jul 2023 15:59:10 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.2`

```console
$ docker pull kong@sha256:a021eb2214d23758ca57ae0f9afa0d2f447cbaa0e9852da03a4806d3d672e5c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.2` - linux; amd64

```console
$ docker pull kong@sha256:e0b522fee00498db98ad4961411b0cca00589cb26ea62cbd6eee5800c75b68f2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.5 MB (74455340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9ab1bb01aff7b69946af3bf899036dac3968dc04f3d6540d6ba9120715c5017`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:22:10 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Tue, 04 Jul 2023 18:22:10 GMT
ARG ASSET=ce
# Tue, 04 Jul 2023 18:22:10 GMT
ENV ASSET=ce
# Tue, 04 Jul 2023 18:22:10 GMT
ARG EE_PORTS
# Tue, 04 Jul 2023 18:22:11 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Tue, 04 Jul 2023 18:23:11 GMT
ARG KONG_VERSION=3.2.2
# Tue, 04 Jul 2023 18:23:11 GMT
ENV KONG_VERSION=3.2.2
# Tue, 04 Jul 2023 18:23:11 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Tue, 04 Jul 2023 18:23:11 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Tue, 04 Jul 2023 18:23:28 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 04 Jul 2023 18:23:28 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Tue, 04 Jul 2023 18:23:28 GMT
USER kong
# Tue, 04 Jul 2023 18:23:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 18:23:29 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 04 Jul 2023 18:23:29 GMT
STOPSIGNAL SIGQUIT
# Tue, 04 Jul 2023 18:23:29 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 04 Jul 2023 18:23:29 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95d715c451393bf53843bdb2d56f67f9228685e8a5467f1581eb7dbd1555e40`  
		Last Modified: Tue, 04 Jul 2023 18:25:40 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1646c4360da56b2965cc1e8193d338352966992fc54f7ec7fe372befd31fbfd8`  
		Last Modified: Tue, 04 Jul 2023 18:26:13 GMT  
		Size: 44.0 MB (44022829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe2a8b6aa5fd47013d1cc3020cdae81b5645fffbf64294a91fceb53f567d615e`  
		Last Modified: Tue, 04 Jul 2023 18:26:06 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.2` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:9a7241232bb449f94c45ed396748d83107123553fbf12fa70afcf6876621e438
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.6 MB (78579187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ffe76a7b5bdfae321129262d26cd6f8f8b0b464f1f39544b5e9c12ee0331f4f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 15:56:30 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Tue, 04 Jul 2023 15:56:30 GMT
ARG ASSET=ce
# Tue, 04 Jul 2023 15:56:30 GMT
ENV ASSET=ce
# Tue, 04 Jul 2023 15:56:31 GMT
ARG EE_PORTS
# Tue, 04 Jul 2023 15:56:31 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Tue, 04 Jul 2023 15:56:58 GMT
ARG KONG_VERSION=3.2.2
# Tue, 04 Jul 2023 15:56:58 GMT
ENV KONG_VERSION=3.2.2
# Tue, 04 Jul 2023 15:56:58 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Tue, 04 Jul 2023 15:56:58 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Tue, 04 Jul 2023 15:57:14 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 04 Jul 2023 15:57:14 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Tue, 04 Jul 2023 15:57:14 GMT
USER kong
# Tue, 04 Jul 2023 15:57:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 15:57:14 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 04 Jul 2023 15:57:15 GMT
STOPSIGNAL SIGQUIT
# Tue, 04 Jul 2023 15:57:15 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 04 Jul 2023 15:57:15 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323749330ae28b00c28d5d9426a6340ac8c0950f884d5f86035845592177af50`  
		Last Modified: Tue, 04 Jul 2023 15:58:27 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23aaa8161d4b96a8946d95bbfc0fd69fea9319244013027fdcc5c4850cf88091`  
		Last Modified: Tue, 04 Jul 2023 15:58:56 GMT  
		Size: 50.2 MB (50186891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5e57ac29025fffa301531d54b858aa32d495a664a8b9bd221f134bb600adcee`  
		Last Modified: Tue, 04 Jul 2023 15:58:50 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.2-ubuntu`

```console
$ docker pull kong@sha256:a021eb2214d23758ca57ae0f9afa0d2f447cbaa0e9852da03a4806d3d672e5c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.2-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:e0b522fee00498db98ad4961411b0cca00589cb26ea62cbd6eee5800c75b68f2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.5 MB (74455340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9ab1bb01aff7b69946af3bf899036dac3968dc04f3d6540d6ba9120715c5017`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:22:10 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Tue, 04 Jul 2023 18:22:10 GMT
ARG ASSET=ce
# Tue, 04 Jul 2023 18:22:10 GMT
ENV ASSET=ce
# Tue, 04 Jul 2023 18:22:10 GMT
ARG EE_PORTS
# Tue, 04 Jul 2023 18:22:11 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Tue, 04 Jul 2023 18:23:11 GMT
ARG KONG_VERSION=3.2.2
# Tue, 04 Jul 2023 18:23:11 GMT
ENV KONG_VERSION=3.2.2
# Tue, 04 Jul 2023 18:23:11 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Tue, 04 Jul 2023 18:23:11 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Tue, 04 Jul 2023 18:23:28 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 04 Jul 2023 18:23:28 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Tue, 04 Jul 2023 18:23:28 GMT
USER kong
# Tue, 04 Jul 2023 18:23:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 18:23:29 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 04 Jul 2023 18:23:29 GMT
STOPSIGNAL SIGQUIT
# Tue, 04 Jul 2023 18:23:29 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 04 Jul 2023 18:23:29 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95d715c451393bf53843bdb2d56f67f9228685e8a5467f1581eb7dbd1555e40`  
		Last Modified: Tue, 04 Jul 2023 18:25:40 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1646c4360da56b2965cc1e8193d338352966992fc54f7ec7fe372befd31fbfd8`  
		Last Modified: Tue, 04 Jul 2023 18:26:13 GMT  
		Size: 44.0 MB (44022829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe2a8b6aa5fd47013d1cc3020cdae81b5645fffbf64294a91fceb53f567d615e`  
		Last Modified: Tue, 04 Jul 2023 18:26:06 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.2-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:9a7241232bb449f94c45ed396748d83107123553fbf12fa70afcf6876621e438
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.6 MB (78579187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ffe76a7b5bdfae321129262d26cd6f8f8b0b464f1f39544b5e9c12ee0331f4f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 15:56:30 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Tue, 04 Jul 2023 15:56:30 GMT
ARG ASSET=ce
# Tue, 04 Jul 2023 15:56:30 GMT
ENV ASSET=ce
# Tue, 04 Jul 2023 15:56:31 GMT
ARG EE_PORTS
# Tue, 04 Jul 2023 15:56:31 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Tue, 04 Jul 2023 15:56:58 GMT
ARG KONG_VERSION=3.2.2
# Tue, 04 Jul 2023 15:56:58 GMT
ENV KONG_VERSION=3.2.2
# Tue, 04 Jul 2023 15:56:58 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Tue, 04 Jul 2023 15:56:58 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Tue, 04 Jul 2023 15:57:14 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 04 Jul 2023 15:57:14 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Tue, 04 Jul 2023 15:57:14 GMT
USER kong
# Tue, 04 Jul 2023 15:57:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 15:57:14 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 04 Jul 2023 15:57:15 GMT
STOPSIGNAL SIGQUIT
# Tue, 04 Jul 2023 15:57:15 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 04 Jul 2023 15:57:15 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323749330ae28b00c28d5d9426a6340ac8c0950f884d5f86035845592177af50`  
		Last Modified: Tue, 04 Jul 2023 15:58:27 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23aaa8161d4b96a8946d95bbfc0fd69fea9319244013027fdcc5c4850cf88091`  
		Last Modified: Tue, 04 Jul 2023 15:58:56 GMT  
		Size: 50.2 MB (50186891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5e57ac29025fffa301531d54b858aa32d495a664a8b9bd221f134bb600adcee`  
		Last Modified: Tue, 04 Jul 2023 15:58:50 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.2.2`

```console
$ docker pull kong@sha256:a021eb2214d23758ca57ae0f9afa0d2f447cbaa0e9852da03a4806d3d672e5c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.2.2` - linux; amd64

```console
$ docker pull kong@sha256:e0b522fee00498db98ad4961411b0cca00589cb26ea62cbd6eee5800c75b68f2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.5 MB (74455340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9ab1bb01aff7b69946af3bf899036dac3968dc04f3d6540d6ba9120715c5017`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:22:10 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Tue, 04 Jul 2023 18:22:10 GMT
ARG ASSET=ce
# Tue, 04 Jul 2023 18:22:10 GMT
ENV ASSET=ce
# Tue, 04 Jul 2023 18:22:10 GMT
ARG EE_PORTS
# Tue, 04 Jul 2023 18:22:11 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Tue, 04 Jul 2023 18:23:11 GMT
ARG KONG_VERSION=3.2.2
# Tue, 04 Jul 2023 18:23:11 GMT
ENV KONG_VERSION=3.2.2
# Tue, 04 Jul 2023 18:23:11 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Tue, 04 Jul 2023 18:23:11 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Tue, 04 Jul 2023 18:23:28 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 04 Jul 2023 18:23:28 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Tue, 04 Jul 2023 18:23:28 GMT
USER kong
# Tue, 04 Jul 2023 18:23:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 18:23:29 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 04 Jul 2023 18:23:29 GMT
STOPSIGNAL SIGQUIT
# Tue, 04 Jul 2023 18:23:29 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 04 Jul 2023 18:23:29 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95d715c451393bf53843bdb2d56f67f9228685e8a5467f1581eb7dbd1555e40`  
		Last Modified: Tue, 04 Jul 2023 18:25:40 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1646c4360da56b2965cc1e8193d338352966992fc54f7ec7fe372befd31fbfd8`  
		Last Modified: Tue, 04 Jul 2023 18:26:13 GMT  
		Size: 44.0 MB (44022829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe2a8b6aa5fd47013d1cc3020cdae81b5645fffbf64294a91fceb53f567d615e`  
		Last Modified: Tue, 04 Jul 2023 18:26:06 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.2.2` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:9a7241232bb449f94c45ed396748d83107123553fbf12fa70afcf6876621e438
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.6 MB (78579187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ffe76a7b5bdfae321129262d26cd6f8f8b0b464f1f39544b5e9c12ee0331f4f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 15:56:30 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Tue, 04 Jul 2023 15:56:30 GMT
ARG ASSET=ce
# Tue, 04 Jul 2023 15:56:30 GMT
ENV ASSET=ce
# Tue, 04 Jul 2023 15:56:31 GMT
ARG EE_PORTS
# Tue, 04 Jul 2023 15:56:31 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Tue, 04 Jul 2023 15:56:58 GMT
ARG KONG_VERSION=3.2.2
# Tue, 04 Jul 2023 15:56:58 GMT
ENV KONG_VERSION=3.2.2
# Tue, 04 Jul 2023 15:56:58 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Tue, 04 Jul 2023 15:56:58 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Tue, 04 Jul 2023 15:57:14 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 04 Jul 2023 15:57:14 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Tue, 04 Jul 2023 15:57:14 GMT
USER kong
# Tue, 04 Jul 2023 15:57:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 15:57:14 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 04 Jul 2023 15:57:15 GMT
STOPSIGNAL SIGQUIT
# Tue, 04 Jul 2023 15:57:15 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 04 Jul 2023 15:57:15 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323749330ae28b00c28d5d9426a6340ac8c0950f884d5f86035845592177af50`  
		Last Modified: Tue, 04 Jul 2023 15:58:27 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23aaa8161d4b96a8946d95bbfc0fd69fea9319244013027fdcc5c4850cf88091`  
		Last Modified: Tue, 04 Jul 2023 15:58:56 GMT  
		Size: 50.2 MB (50186891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5e57ac29025fffa301531d54b858aa32d495a664a8b9bd221f134bb600adcee`  
		Last Modified: Tue, 04 Jul 2023 15:58:50 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.2.2-alpine`

```console
$ docker pull kong@sha256:f985adcc9ed18baa749e0601ab373795579d2cbb23d982cd5bd14eb30adcdca0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:3.2.2-alpine` - linux; amd64

```console
$ docker pull kong@sha256:6c508876f692c8df3346e63119e36ac1a237384c8c44f02fefcb2b74cea99f36
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.9 MB (36925700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96642dab3c1c86110eb73e5d6013381cf90df6c6dd50c5295ea3fb7cd1f0a08f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:24:27 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 15 Jun 2023 06:24:39 GMT
ARG KONG_VERSION=3.2.2
# Thu, 15 Jun 2023 06:24:39 GMT
ENV KONG_VERSION=3.2.2
# Thu, 15 Jun 2023 06:24:39 GMT
ARG KONG_SHA256=a07c3bc0307e2d8fe33acb8be5fe659f348279540eaa267bc6968005094835ef
# Thu, 15 Jun 2023 06:24:40 GMT
ARG KONG_PREFIX=/usr/local/kong
# Thu, 15 Jun 2023 06:24:40 GMT
ENV KONG_PREFIX=/usr/local/kong
# Thu, 15 Jun 2023 06:24:40 GMT
ARG ASSET=remote
# Thu, 15 Jun 2023 06:24:40 GMT
ARG EE_PORTS
# Thu, 15 Jun 2023 06:24:40 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Thu, 15 Jun 2023 06:24:46 GMT
# ARGS: ASSET=remote KONG_SHA256=a07c3bc0307e2d8fe33acb8be5fe659f348279540eaa267bc6968005094835ef
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     export ARCH='amd64';     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc perl tzdata libcap zlib zlib-dev bash yaml     && adduser -S kong     && addgroup -S kong     && mkdir -p "${KONG_PREFIX}"     && chown -R kong:0 ${KONG_PREFIX}     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u ${KONG_PREFIX}     && rm -rf /tmp/kong.apk.tar.gz     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Thu, 15 Jun 2023 06:24:47 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Thu, 15 Jun 2023 06:24:47 GMT
USER kong
# Thu, 15 Jun 2023 06:24:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Jun 2023 06:24:47 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 15 Jun 2023 06:24:47 GMT
STOPSIGNAL SIGQUIT
# Thu, 15 Jun 2023 06:24:47 GMT
HEALTHCHECK &{["CMD-SHELL" "kong-health"] "1m0s" "10s" "0s" '\n'}
# Thu, 15 Jun 2023 06:24:47 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd039fb5ac2e17d182f72cb499825604a85321aa36a51fbdbb3f9fc226d114a9`  
		Last Modified: Thu, 15 Jun 2023 06:26:08 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef7ad483e17ea0283b93716e78b8f3397f1b187880b68963b0e7e5db7753481`  
		Last Modified: Thu, 15 Jun 2023 06:26:13 GMT  
		Size: 33.5 MB (33549698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ee442fb6c11d14c18f89e7c6d930d5c62b13d91a5a2af2fb628c49554b44b0`  
		Last Modified: Thu, 15 Jun 2023 06:26:08 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.2.2-ubuntu`

```console
$ docker pull kong@sha256:a021eb2214d23758ca57ae0f9afa0d2f447cbaa0e9852da03a4806d3d672e5c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.2.2-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:e0b522fee00498db98ad4961411b0cca00589cb26ea62cbd6eee5800c75b68f2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.5 MB (74455340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9ab1bb01aff7b69946af3bf899036dac3968dc04f3d6540d6ba9120715c5017`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:22:10 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Tue, 04 Jul 2023 18:22:10 GMT
ARG ASSET=ce
# Tue, 04 Jul 2023 18:22:10 GMT
ENV ASSET=ce
# Tue, 04 Jul 2023 18:22:10 GMT
ARG EE_PORTS
# Tue, 04 Jul 2023 18:22:11 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Tue, 04 Jul 2023 18:23:11 GMT
ARG KONG_VERSION=3.2.2
# Tue, 04 Jul 2023 18:23:11 GMT
ENV KONG_VERSION=3.2.2
# Tue, 04 Jul 2023 18:23:11 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Tue, 04 Jul 2023 18:23:11 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Tue, 04 Jul 2023 18:23:28 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 04 Jul 2023 18:23:28 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Tue, 04 Jul 2023 18:23:28 GMT
USER kong
# Tue, 04 Jul 2023 18:23:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 18:23:29 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 04 Jul 2023 18:23:29 GMT
STOPSIGNAL SIGQUIT
# Tue, 04 Jul 2023 18:23:29 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 04 Jul 2023 18:23:29 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95d715c451393bf53843bdb2d56f67f9228685e8a5467f1581eb7dbd1555e40`  
		Last Modified: Tue, 04 Jul 2023 18:25:40 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1646c4360da56b2965cc1e8193d338352966992fc54f7ec7fe372befd31fbfd8`  
		Last Modified: Tue, 04 Jul 2023 18:26:13 GMT  
		Size: 44.0 MB (44022829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe2a8b6aa5fd47013d1cc3020cdae81b5645fffbf64294a91fceb53f567d615e`  
		Last Modified: Tue, 04 Jul 2023 18:26:06 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.2.2-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:9a7241232bb449f94c45ed396748d83107123553fbf12fa70afcf6876621e438
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.6 MB (78579187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ffe76a7b5bdfae321129262d26cd6f8f8b0b464f1f39544b5e9c12ee0331f4f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 15:56:30 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Tue, 04 Jul 2023 15:56:30 GMT
ARG ASSET=ce
# Tue, 04 Jul 2023 15:56:30 GMT
ENV ASSET=ce
# Tue, 04 Jul 2023 15:56:31 GMT
ARG EE_PORTS
# Tue, 04 Jul 2023 15:56:31 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Tue, 04 Jul 2023 15:56:58 GMT
ARG KONG_VERSION=3.2.2
# Tue, 04 Jul 2023 15:56:58 GMT
ENV KONG_VERSION=3.2.2
# Tue, 04 Jul 2023 15:56:58 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Tue, 04 Jul 2023 15:56:58 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Tue, 04 Jul 2023 15:57:14 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 04 Jul 2023 15:57:14 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Tue, 04 Jul 2023 15:57:14 GMT
USER kong
# Tue, 04 Jul 2023 15:57:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 15:57:14 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 04 Jul 2023 15:57:15 GMT
STOPSIGNAL SIGQUIT
# Tue, 04 Jul 2023 15:57:15 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 04 Jul 2023 15:57:15 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323749330ae28b00c28d5d9426a6340ac8c0950f884d5f86035845592177af50`  
		Last Modified: Tue, 04 Jul 2023 15:58:27 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23aaa8161d4b96a8946d95bbfc0fd69fea9319244013027fdcc5c4850cf88091`  
		Last Modified: Tue, 04 Jul 2023 15:58:56 GMT  
		Size: 50.2 MB (50186891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5e57ac29025fffa301531d54b858aa32d495a664a8b9bd221f134bb600adcee`  
		Last Modified: Tue, 04 Jul 2023 15:58:50 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.3`

```console
$ docker pull kong@sha256:6901d658a7fe670a285c85fb41b6dfca465b3bf97b1f488b2f4a04518ec46567
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.3` - linux; amd64

```console
$ docker pull kong@sha256:f305f85491b60c6139464ead7fe0b7289d3469a45224f4fada8ba16e909ce8ef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81308072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27891b72fb11814512dfd7f819d980b9af44f35dc071846c7bed9d2315c8818b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:22:10 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Tue, 04 Jul 2023 18:22:10 GMT
ARG ASSET=ce
# Tue, 04 Jul 2023 18:22:10 GMT
ENV ASSET=ce
# Tue, 04 Jul 2023 18:22:10 GMT
ARG EE_PORTS
# Tue, 04 Jul 2023 18:22:11 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Tue, 04 Jul 2023 18:22:11 GMT
ARG KONG_VERSION=3.3.0
# Tue, 04 Jul 2023 18:22:11 GMT
ENV KONG_VERSION=3.3.0
# Tue, 04 Jul 2023 18:22:11 GMT
ARG KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b
# Tue, 04 Jul 2023 18:22:11 GMT
ARG KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
# Tue, 04 Jul 2023 18:23:00 GMT
# ARGS: KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 04 Jul 2023 18:23:00 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Tue, 04 Jul 2023 18:23:00 GMT
USER kong
# Tue, 04 Jul 2023 18:23:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 18:23:01 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 04 Jul 2023 18:23:01 GMT
STOPSIGNAL SIGQUIT
# Tue, 04 Jul 2023 18:23:01 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 04 Jul 2023 18:23:01 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95d715c451393bf53843bdb2d56f67f9228685e8a5467f1581eb7dbd1555e40`  
		Last Modified: Tue, 04 Jul 2023 18:25:40 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0485449e03859344d0d3afc6a0e5d0ac35cd50deb2c2c3cb8cc6114b503c1ed`  
		Last Modified: Tue, 04 Jul 2023 18:25:48 GMT  
		Size: 50.9 MB (50875561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb811f70b9c3e6e52149298e8491972444909b64a67a7549200fdcf841b8f0c`  
		Last Modified: Tue, 04 Jul 2023 18:25:40 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.3` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:1af0841022124e34b06deef7223695918912f31bac0d41a5b973b57f235e9f0f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75729473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43979f607227bbb2b07e6de8a0352138b806c807dcfc885c007f7d6235c368ff`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 15:56:30 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Tue, 04 Jul 2023 15:56:30 GMT
ARG ASSET=ce
# Tue, 04 Jul 2023 15:56:30 GMT
ENV ASSET=ce
# Tue, 04 Jul 2023 15:56:31 GMT
ARG EE_PORTS
# Tue, 04 Jul 2023 15:56:31 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Tue, 04 Jul 2023 15:56:31 GMT
ARG KONG_VERSION=3.3.0
# Tue, 04 Jul 2023 15:56:31 GMT
ENV KONG_VERSION=3.3.0
# Tue, 04 Jul 2023 15:56:31 GMT
ARG KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b
# Tue, 04 Jul 2023 15:56:31 GMT
ARG KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
# Tue, 04 Jul 2023 15:56:55 GMT
# ARGS: KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 04 Jul 2023 15:56:55 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Tue, 04 Jul 2023 15:56:55 GMT
USER kong
# Tue, 04 Jul 2023 15:56:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 15:56:55 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 04 Jul 2023 15:56:55 GMT
STOPSIGNAL SIGQUIT
# Tue, 04 Jul 2023 15:56:55 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 04 Jul 2023 15:56:56 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323749330ae28b00c28d5d9426a6340ac8c0950f884d5f86035845592177af50`  
		Last Modified: Tue, 04 Jul 2023 15:58:27 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0838f7579b4383b8de9c9ba94ea92f5e8bf54501aad19ff3c7b20a69d3e9601c`  
		Last Modified: Tue, 04 Jul 2023 15:58:33 GMT  
		Size: 47.3 MB (47337178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86236cf6ed5d8a29939463122de34686c5333330b978ec314bb8718c4bf9f92d`  
		Last Modified: Tue, 04 Jul 2023 15:58:27 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.3-ubuntu`

```console
$ docker pull kong@sha256:6901d658a7fe670a285c85fb41b6dfca465b3bf97b1f488b2f4a04518ec46567
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.3-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:f305f85491b60c6139464ead7fe0b7289d3469a45224f4fada8ba16e909ce8ef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81308072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27891b72fb11814512dfd7f819d980b9af44f35dc071846c7bed9d2315c8818b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:22:10 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Tue, 04 Jul 2023 18:22:10 GMT
ARG ASSET=ce
# Tue, 04 Jul 2023 18:22:10 GMT
ENV ASSET=ce
# Tue, 04 Jul 2023 18:22:10 GMT
ARG EE_PORTS
# Tue, 04 Jul 2023 18:22:11 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Tue, 04 Jul 2023 18:22:11 GMT
ARG KONG_VERSION=3.3.0
# Tue, 04 Jul 2023 18:22:11 GMT
ENV KONG_VERSION=3.3.0
# Tue, 04 Jul 2023 18:22:11 GMT
ARG KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b
# Tue, 04 Jul 2023 18:22:11 GMT
ARG KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
# Tue, 04 Jul 2023 18:23:00 GMT
# ARGS: KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 04 Jul 2023 18:23:00 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Tue, 04 Jul 2023 18:23:00 GMT
USER kong
# Tue, 04 Jul 2023 18:23:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 18:23:01 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 04 Jul 2023 18:23:01 GMT
STOPSIGNAL SIGQUIT
# Tue, 04 Jul 2023 18:23:01 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 04 Jul 2023 18:23:01 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95d715c451393bf53843bdb2d56f67f9228685e8a5467f1581eb7dbd1555e40`  
		Last Modified: Tue, 04 Jul 2023 18:25:40 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0485449e03859344d0d3afc6a0e5d0ac35cd50deb2c2c3cb8cc6114b503c1ed`  
		Last Modified: Tue, 04 Jul 2023 18:25:48 GMT  
		Size: 50.9 MB (50875561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb811f70b9c3e6e52149298e8491972444909b64a67a7549200fdcf841b8f0c`  
		Last Modified: Tue, 04 Jul 2023 18:25:40 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.3-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:1af0841022124e34b06deef7223695918912f31bac0d41a5b973b57f235e9f0f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75729473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43979f607227bbb2b07e6de8a0352138b806c807dcfc885c007f7d6235c368ff`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 15:56:30 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Tue, 04 Jul 2023 15:56:30 GMT
ARG ASSET=ce
# Tue, 04 Jul 2023 15:56:30 GMT
ENV ASSET=ce
# Tue, 04 Jul 2023 15:56:31 GMT
ARG EE_PORTS
# Tue, 04 Jul 2023 15:56:31 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Tue, 04 Jul 2023 15:56:31 GMT
ARG KONG_VERSION=3.3.0
# Tue, 04 Jul 2023 15:56:31 GMT
ENV KONG_VERSION=3.3.0
# Tue, 04 Jul 2023 15:56:31 GMT
ARG KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b
# Tue, 04 Jul 2023 15:56:31 GMT
ARG KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
# Tue, 04 Jul 2023 15:56:55 GMT
# ARGS: KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 04 Jul 2023 15:56:55 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Tue, 04 Jul 2023 15:56:55 GMT
USER kong
# Tue, 04 Jul 2023 15:56:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 15:56:55 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 04 Jul 2023 15:56:55 GMT
STOPSIGNAL SIGQUIT
# Tue, 04 Jul 2023 15:56:55 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 04 Jul 2023 15:56:56 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323749330ae28b00c28d5d9426a6340ac8c0950f884d5f86035845592177af50`  
		Last Modified: Tue, 04 Jul 2023 15:58:27 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0838f7579b4383b8de9c9ba94ea92f5e8bf54501aad19ff3c7b20a69d3e9601c`  
		Last Modified: Tue, 04 Jul 2023 15:58:33 GMT  
		Size: 47.3 MB (47337178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86236cf6ed5d8a29939463122de34686c5333330b978ec314bb8718c4bf9f92d`  
		Last Modified: Tue, 04 Jul 2023 15:58:27 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.3.1`

**does not exist** (yet?)

## `kong:3.3.1-alpine`

**does not exist** (yet?)

## `kong:3.3.1-ubuntu`

**does not exist** (yet?)

## `kong:alpine`

```console
$ docker pull kong@sha256:aae539892ee4f08d979274768504d5e592928b1d57a824e3436d627a8588fe6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:alpine` - linux; amd64

```console
$ docker pull kong@sha256:0259087c5093b770b34ca17d3be227a9264e2c5658c58563c01283b12d7c49ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.2 MB (34222118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90459c3fc97f37b85cb1fa39db3539cc1cbaf0ac2c8d9b58ad9e033f95165008`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:24:27 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 15 Jun 2023 06:24:27 GMT
ARG KONG_VERSION=3.3.0
# Thu, 15 Jun 2023 06:24:27 GMT
ENV KONG_VERSION=3.3.0
# Thu, 15 Jun 2023 06:24:27 GMT
ARG KONG_AMD64_SHA=494522d5ef9baf674272bbb7075e406a4515a7475253fd3026cc7ca9451612a2
# Thu, 15 Jun 2023 06:24:27 GMT
ARG KONG_PREFIX=/usr/local/kong
# Thu, 15 Jun 2023 06:24:27 GMT
ENV KONG_PREFIX=/usr/local/kong
# Thu, 15 Jun 2023 06:24:27 GMT
ARG ASSET=remote
# Thu, 15 Jun 2023 06:24:28 GMT
ARG EE_PORTS
# Thu, 15 Jun 2023 06:24:28 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Thu, 15 Jun 2023 06:24:34 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=494522d5ef9baf674272bbb7075e406a4515a7475253fd3026cc7ca9451612a2
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     export ARCH='amd64';     KONG_SHA256=$KONG_AMD64_SHA ;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc perl tzdata libcap zlib zlib-dev bash yaml     && adduser -S kong     && addgroup -S kong     && mkdir -p "${KONG_PREFIX}"     && chown -R kong:0 ${KONG_PREFIX}     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u ${KONG_PREFIX}     && rm -rf /tmp/kong.apk.tar.gz     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Thu, 15 Jun 2023 06:24:34 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Thu, 15 Jun 2023 06:24:34 GMT
USER kong
# Thu, 15 Jun 2023 06:24:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Jun 2023 06:24:34 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 15 Jun 2023 06:24:34 GMT
STOPSIGNAL SIGQUIT
# Thu, 15 Jun 2023 06:24:34 GMT
HEALTHCHECK &{["CMD-SHELL" "kong-health"] "1m0s" "10s" "0s" '\n'}
# Thu, 15 Jun 2023 06:24:34 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71bf8f4939b0d0d869272046c9d70b9159d8da43fcbe49aa3db948aeec25ccc4`  
		Last Modified: Thu, 15 Jun 2023 06:25:53 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b72589f98cfb44bd3f9dca2c93d93173361a0ac30a8d5a5a11639bafaecba65e`  
		Last Modified: Thu, 15 Jun 2023 06:25:58 GMT  
		Size: 30.8 MB (30846114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd32791a2d9c85fcb9b2a8553438aa66214a402cd38b29453bbc9b72bf4f76e`  
		Last Modified: Thu, 15 Jun 2023 06:25:53 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:latest`

```console
$ docker pull kong@sha256:6901d658a7fe670a285c85fb41b6dfca465b3bf97b1f488b2f4a04518ec46567
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:latest` - linux; amd64

```console
$ docker pull kong@sha256:f305f85491b60c6139464ead7fe0b7289d3469a45224f4fada8ba16e909ce8ef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81308072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27891b72fb11814512dfd7f819d980b9af44f35dc071846c7bed9d2315c8818b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:22:10 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Tue, 04 Jul 2023 18:22:10 GMT
ARG ASSET=ce
# Tue, 04 Jul 2023 18:22:10 GMT
ENV ASSET=ce
# Tue, 04 Jul 2023 18:22:10 GMT
ARG EE_PORTS
# Tue, 04 Jul 2023 18:22:11 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Tue, 04 Jul 2023 18:22:11 GMT
ARG KONG_VERSION=3.3.0
# Tue, 04 Jul 2023 18:22:11 GMT
ENV KONG_VERSION=3.3.0
# Tue, 04 Jul 2023 18:22:11 GMT
ARG KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b
# Tue, 04 Jul 2023 18:22:11 GMT
ARG KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
# Tue, 04 Jul 2023 18:23:00 GMT
# ARGS: KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 04 Jul 2023 18:23:00 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Tue, 04 Jul 2023 18:23:00 GMT
USER kong
# Tue, 04 Jul 2023 18:23:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 18:23:01 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 04 Jul 2023 18:23:01 GMT
STOPSIGNAL SIGQUIT
# Tue, 04 Jul 2023 18:23:01 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 04 Jul 2023 18:23:01 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95d715c451393bf53843bdb2d56f67f9228685e8a5467f1581eb7dbd1555e40`  
		Last Modified: Tue, 04 Jul 2023 18:25:40 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0485449e03859344d0d3afc6a0e5d0ac35cd50deb2c2c3cb8cc6114b503c1ed`  
		Last Modified: Tue, 04 Jul 2023 18:25:48 GMT  
		Size: 50.9 MB (50875561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb811f70b9c3e6e52149298e8491972444909b64a67a7549200fdcf841b8f0c`  
		Last Modified: Tue, 04 Jul 2023 18:25:40 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:latest` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:1af0841022124e34b06deef7223695918912f31bac0d41a5b973b57f235e9f0f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75729473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43979f607227bbb2b07e6de8a0352138b806c807dcfc885c007f7d6235c368ff`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 15:56:30 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Tue, 04 Jul 2023 15:56:30 GMT
ARG ASSET=ce
# Tue, 04 Jul 2023 15:56:30 GMT
ENV ASSET=ce
# Tue, 04 Jul 2023 15:56:31 GMT
ARG EE_PORTS
# Tue, 04 Jul 2023 15:56:31 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Tue, 04 Jul 2023 15:56:31 GMT
ARG KONG_VERSION=3.3.0
# Tue, 04 Jul 2023 15:56:31 GMT
ENV KONG_VERSION=3.3.0
# Tue, 04 Jul 2023 15:56:31 GMT
ARG KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b
# Tue, 04 Jul 2023 15:56:31 GMT
ARG KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
# Tue, 04 Jul 2023 15:56:55 GMT
# ARGS: KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 04 Jul 2023 15:56:55 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Tue, 04 Jul 2023 15:56:55 GMT
USER kong
# Tue, 04 Jul 2023 15:56:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 15:56:55 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 04 Jul 2023 15:56:55 GMT
STOPSIGNAL SIGQUIT
# Tue, 04 Jul 2023 15:56:55 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 04 Jul 2023 15:56:56 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323749330ae28b00c28d5d9426a6340ac8c0950f884d5f86035845592177af50`  
		Last Modified: Tue, 04 Jul 2023 15:58:27 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0838f7579b4383b8de9c9ba94ea92f5e8bf54501aad19ff3c7b20a69d3e9601c`  
		Last Modified: Tue, 04 Jul 2023 15:58:33 GMT  
		Size: 47.3 MB (47337178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86236cf6ed5d8a29939463122de34686c5333330b978ec314bb8718c4bf9f92d`  
		Last Modified: Tue, 04 Jul 2023 15:58:27 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:ubuntu`

```console
$ docker pull kong@sha256:6901d658a7fe670a285c85fb41b6dfca465b3bf97b1f488b2f4a04518ec46567
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:f305f85491b60c6139464ead7fe0b7289d3469a45224f4fada8ba16e909ce8ef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81308072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27891b72fb11814512dfd7f819d980b9af44f35dc071846c7bed9d2315c8818b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 18:22:10 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Tue, 04 Jul 2023 18:22:10 GMT
ARG ASSET=ce
# Tue, 04 Jul 2023 18:22:10 GMT
ENV ASSET=ce
# Tue, 04 Jul 2023 18:22:10 GMT
ARG EE_PORTS
# Tue, 04 Jul 2023 18:22:11 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Tue, 04 Jul 2023 18:22:11 GMT
ARG KONG_VERSION=3.3.0
# Tue, 04 Jul 2023 18:22:11 GMT
ENV KONG_VERSION=3.3.0
# Tue, 04 Jul 2023 18:22:11 GMT
ARG KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b
# Tue, 04 Jul 2023 18:22:11 GMT
ARG KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
# Tue, 04 Jul 2023 18:23:00 GMT
# ARGS: KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 04 Jul 2023 18:23:00 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Tue, 04 Jul 2023 18:23:00 GMT
USER kong
# Tue, 04 Jul 2023 18:23:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 18:23:01 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 04 Jul 2023 18:23:01 GMT
STOPSIGNAL SIGQUIT
# Tue, 04 Jul 2023 18:23:01 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 04 Jul 2023 18:23:01 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95d715c451393bf53843bdb2d56f67f9228685e8a5467f1581eb7dbd1555e40`  
		Last Modified: Tue, 04 Jul 2023 18:25:40 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0485449e03859344d0d3afc6a0e5d0ac35cd50deb2c2c3cb8cc6114b503c1ed`  
		Last Modified: Tue, 04 Jul 2023 18:25:48 GMT  
		Size: 50.9 MB (50875561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb811f70b9c3e6e52149298e8491972444909b64a67a7549200fdcf841b8f0c`  
		Last Modified: Tue, 04 Jul 2023 18:25:40 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:1af0841022124e34b06deef7223695918912f31bac0d41a5b973b57f235e9f0f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75729473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43979f607227bbb2b07e6de8a0352138b806c807dcfc885c007f7d6235c368ff`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 15:56:30 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Tue, 04 Jul 2023 15:56:30 GMT
ARG ASSET=ce
# Tue, 04 Jul 2023 15:56:30 GMT
ENV ASSET=ce
# Tue, 04 Jul 2023 15:56:31 GMT
ARG EE_PORTS
# Tue, 04 Jul 2023 15:56:31 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Tue, 04 Jul 2023 15:56:31 GMT
ARG KONG_VERSION=3.3.0
# Tue, 04 Jul 2023 15:56:31 GMT
ENV KONG_VERSION=3.3.0
# Tue, 04 Jul 2023 15:56:31 GMT
ARG KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b
# Tue, 04 Jul 2023 15:56:31 GMT
ARG KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
# Tue, 04 Jul 2023 15:56:55 GMT
# ARGS: KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 04 Jul 2023 15:56:55 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Tue, 04 Jul 2023 15:56:55 GMT
USER kong
# Tue, 04 Jul 2023 15:56:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 04 Jul 2023 15:56:55 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 04 Jul 2023 15:56:55 GMT
STOPSIGNAL SIGQUIT
# Tue, 04 Jul 2023 15:56:55 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 04 Jul 2023 15:56:56 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323749330ae28b00c28d5d9426a6340ac8c0950f884d5f86035845592177af50`  
		Last Modified: Tue, 04 Jul 2023 15:58:27 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0838f7579b4383b8de9c9ba94ea92f5e8bf54501aad19ff3c7b20a69d3e9601c`  
		Last Modified: Tue, 04 Jul 2023 15:58:33 GMT  
		Size: 47.3 MB (47337178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86236cf6ed5d8a29939463122de34686c5333330b978ec314bb8718c4bf9f92d`  
		Last Modified: Tue, 04 Jul 2023 15:58:27 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
