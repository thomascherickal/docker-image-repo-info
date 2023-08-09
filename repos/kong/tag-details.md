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
$ docker pull kong@sha256:f2d494d95098b74d9bb58741076db5d869d30b068389ef9a613d6cd7e73859ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.8` - linux; amd64

```console
$ docker pull kong@sha256:6ce3f41755a13032996be73e6a8d70facb125c245f7979465457e1ff0d99ba33
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49376140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3f8b070881af38984a3f093827b699ca405995b33c52e78b14b7935806e0edd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:31 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
# Mon, 07 Aug 2023 19:20:31 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 02:08:31 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 09 Aug 2023 02:08:31 GMT
ARG ASSET=ce
# Wed, 09 Aug 2023 02:08:31 GMT
ENV ASSET=ce
# Wed, 09 Aug 2023 02:08:31 GMT
ARG EE_PORTS
# Wed, 09 Aug 2023 02:08:32 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 09 Aug 2023 02:08:32 GMT
ARG KONG_VERSION=2.8.3
# Wed, 09 Aug 2023 02:08:32 GMT
ENV KONG_VERSION=2.8.3
# Wed, 09 Aug 2023 02:08:32 GMT
ARG KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa
# Wed, 09 Aug 2023 02:08:32 GMT
ARG KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
# Wed, 09 Aug 2023 02:08:39 GMT
# ARGS: KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Wed, 09 Aug 2023 02:08:39 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 09 Aug 2023 02:08:39 GMT
USER kong
# Wed, 09 Aug 2023 02:08:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 09 Aug 2023 02:08:40 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 09 Aug 2023 02:08:40 GMT
STOPSIGNAL SIGQUIT
# Wed, 09 Aug 2023 02:08:40 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 09 Aug 2023 02:08:40 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12bcd9b6be3062de5dcefc55569cea453f8eb5dffea3f0cc1d7f6b2f67c1681a`  
		Last Modified: Wed, 09 Aug 2023 02:10:10 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca9cc13002d9f4248549397b41afcc207e318a6e9f07123739a9bee9839174b`  
		Last Modified: Wed, 09 Aug 2023 02:10:18 GMT  
		Size: 46.6 MB (46567445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c614fc325c802d26e6d1c5560b68d6419c766adb2bdb7beeefd999d906ca0c7e`  
		Last Modified: Wed, 09 Aug 2023 02:10:10 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.8` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:e99f31fd874fb90b2e194f296456d363d2a1bad2ec3b8da21be8d7af654063ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.6 MB (48561884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a302312f91cd531f910fc1a3646ae44d5bbfc68f936e4a16a14d25568849be98`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:26 GMT
ADD file:cf85500a1f5b87a88587b279c8b8018eebeb3092f402b7e2cc4ad3873e078580 in / 
# Mon, 07 Aug 2023 19:39:26 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 00:48:58 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 09 Aug 2023 00:48:58 GMT
ARG ASSET=ce
# Wed, 09 Aug 2023 00:48:58 GMT
ENV ASSET=ce
# Wed, 09 Aug 2023 00:48:58 GMT
ARG EE_PORTS
# Wed, 09 Aug 2023 00:48:59 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 09 Aug 2023 00:48:59 GMT
ARG KONG_VERSION=2.8.3
# Wed, 09 Aug 2023 00:48:59 GMT
ENV KONG_VERSION=2.8.3
# Wed, 09 Aug 2023 00:48:59 GMT
ARG KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa
# Wed, 09 Aug 2023 00:48:59 GMT
ARG KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
# Wed, 09 Aug 2023 00:49:05 GMT
# ARGS: KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Wed, 09 Aug 2023 00:49:06 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 09 Aug 2023 00:49:06 GMT
USER kong
# Wed, 09 Aug 2023 00:49:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 09 Aug 2023 00:49:06 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 09 Aug 2023 00:49:06 GMT
STOPSIGNAL SIGQUIT
# Wed, 09 Aug 2023 00:49:06 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 09 Aug 2023 00:49:06 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:bdb2de7ba06c3a4e10b98f439a8c70afd63eee492c2ddc32342331a8e9ef4ff7`  
		Last Modified: Mon, 07 Aug 2023 19:40:08 GMT  
		Size: 2.7 MB (2708023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb1eecfa54964173b307c94487ea0af19f5e974b6398b3aa5a90f5cdf3868a9f`  
		Last Modified: Wed, 09 Aug 2023 00:50:06 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1351a66935df1b153fa2ed39f64538ccbcacf7b1e58445453b58a977287ad4c8`  
		Last Modified: Wed, 09 Aug 2023 00:50:13 GMT  
		Size: 45.9 MB (45852849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28fdd42e521b9b7be083f6d661af365af3fa72ec9637b6120d93db37f1932597`  
		Last Modified: Wed, 09 Aug 2023 00:50:06 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.8.3`

```console
$ docker pull kong@sha256:f2d494d95098b74d9bb58741076db5d869d30b068389ef9a613d6cd7e73859ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.8.3` - linux; amd64

```console
$ docker pull kong@sha256:6ce3f41755a13032996be73e6a8d70facb125c245f7979465457e1ff0d99ba33
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49376140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3f8b070881af38984a3f093827b699ca405995b33c52e78b14b7935806e0edd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:31 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
# Mon, 07 Aug 2023 19:20:31 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 02:08:31 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 09 Aug 2023 02:08:31 GMT
ARG ASSET=ce
# Wed, 09 Aug 2023 02:08:31 GMT
ENV ASSET=ce
# Wed, 09 Aug 2023 02:08:31 GMT
ARG EE_PORTS
# Wed, 09 Aug 2023 02:08:32 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 09 Aug 2023 02:08:32 GMT
ARG KONG_VERSION=2.8.3
# Wed, 09 Aug 2023 02:08:32 GMT
ENV KONG_VERSION=2.8.3
# Wed, 09 Aug 2023 02:08:32 GMT
ARG KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa
# Wed, 09 Aug 2023 02:08:32 GMT
ARG KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
# Wed, 09 Aug 2023 02:08:39 GMT
# ARGS: KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Wed, 09 Aug 2023 02:08:39 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 09 Aug 2023 02:08:39 GMT
USER kong
# Wed, 09 Aug 2023 02:08:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 09 Aug 2023 02:08:40 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 09 Aug 2023 02:08:40 GMT
STOPSIGNAL SIGQUIT
# Wed, 09 Aug 2023 02:08:40 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 09 Aug 2023 02:08:40 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12bcd9b6be3062de5dcefc55569cea453f8eb5dffea3f0cc1d7f6b2f67c1681a`  
		Last Modified: Wed, 09 Aug 2023 02:10:10 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca9cc13002d9f4248549397b41afcc207e318a6e9f07123739a9bee9839174b`  
		Last Modified: Wed, 09 Aug 2023 02:10:18 GMT  
		Size: 46.6 MB (46567445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c614fc325c802d26e6d1c5560b68d6419c766adb2bdb7beeefd999d906ca0c7e`  
		Last Modified: Wed, 09 Aug 2023 02:10:10 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.8.3` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:e99f31fd874fb90b2e194f296456d363d2a1bad2ec3b8da21be8d7af654063ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.6 MB (48561884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a302312f91cd531f910fc1a3646ae44d5bbfc68f936e4a16a14d25568849be98`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:26 GMT
ADD file:cf85500a1f5b87a88587b279c8b8018eebeb3092f402b7e2cc4ad3873e078580 in / 
# Mon, 07 Aug 2023 19:39:26 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 00:48:58 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 09 Aug 2023 00:48:58 GMT
ARG ASSET=ce
# Wed, 09 Aug 2023 00:48:58 GMT
ENV ASSET=ce
# Wed, 09 Aug 2023 00:48:58 GMT
ARG EE_PORTS
# Wed, 09 Aug 2023 00:48:59 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 09 Aug 2023 00:48:59 GMT
ARG KONG_VERSION=2.8.3
# Wed, 09 Aug 2023 00:48:59 GMT
ENV KONG_VERSION=2.8.3
# Wed, 09 Aug 2023 00:48:59 GMT
ARG KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa
# Wed, 09 Aug 2023 00:48:59 GMT
ARG KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
# Wed, 09 Aug 2023 00:49:05 GMT
# ARGS: KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Wed, 09 Aug 2023 00:49:06 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 09 Aug 2023 00:49:06 GMT
USER kong
# Wed, 09 Aug 2023 00:49:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 09 Aug 2023 00:49:06 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 09 Aug 2023 00:49:06 GMT
STOPSIGNAL SIGQUIT
# Wed, 09 Aug 2023 00:49:06 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 09 Aug 2023 00:49:06 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:bdb2de7ba06c3a4e10b98f439a8c70afd63eee492c2ddc32342331a8e9ef4ff7`  
		Last Modified: Mon, 07 Aug 2023 19:40:08 GMT  
		Size: 2.7 MB (2708023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb1eecfa54964173b307c94487ea0af19f5e974b6398b3aa5a90f5cdf3868a9f`  
		Last Modified: Wed, 09 Aug 2023 00:50:06 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1351a66935df1b153fa2ed39f64538ccbcacf7b1e58445453b58a977287ad4c8`  
		Last Modified: Wed, 09 Aug 2023 00:50:13 GMT  
		Size: 45.9 MB (45852849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28fdd42e521b9b7be083f6d661af365af3fa72ec9637b6120d93db37f1932597`  
		Last Modified: Wed, 09 Aug 2023 00:50:06 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.8.3-alpine`

```console
$ docker pull kong@sha256:f2d494d95098b74d9bb58741076db5d869d30b068389ef9a613d6cd7e73859ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.8.3-alpine` - linux; amd64

```console
$ docker pull kong@sha256:6ce3f41755a13032996be73e6a8d70facb125c245f7979465457e1ff0d99ba33
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49376140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3f8b070881af38984a3f093827b699ca405995b33c52e78b14b7935806e0edd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:31 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
# Mon, 07 Aug 2023 19:20:31 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 02:08:31 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 09 Aug 2023 02:08:31 GMT
ARG ASSET=ce
# Wed, 09 Aug 2023 02:08:31 GMT
ENV ASSET=ce
# Wed, 09 Aug 2023 02:08:31 GMT
ARG EE_PORTS
# Wed, 09 Aug 2023 02:08:32 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 09 Aug 2023 02:08:32 GMT
ARG KONG_VERSION=2.8.3
# Wed, 09 Aug 2023 02:08:32 GMT
ENV KONG_VERSION=2.8.3
# Wed, 09 Aug 2023 02:08:32 GMT
ARG KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa
# Wed, 09 Aug 2023 02:08:32 GMT
ARG KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
# Wed, 09 Aug 2023 02:08:39 GMT
# ARGS: KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Wed, 09 Aug 2023 02:08:39 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 09 Aug 2023 02:08:39 GMT
USER kong
# Wed, 09 Aug 2023 02:08:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 09 Aug 2023 02:08:40 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 09 Aug 2023 02:08:40 GMT
STOPSIGNAL SIGQUIT
# Wed, 09 Aug 2023 02:08:40 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 09 Aug 2023 02:08:40 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12bcd9b6be3062de5dcefc55569cea453f8eb5dffea3f0cc1d7f6b2f67c1681a`  
		Last Modified: Wed, 09 Aug 2023 02:10:10 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca9cc13002d9f4248549397b41afcc207e318a6e9f07123739a9bee9839174b`  
		Last Modified: Wed, 09 Aug 2023 02:10:18 GMT  
		Size: 46.6 MB (46567445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c614fc325c802d26e6d1c5560b68d6419c766adb2bdb7beeefd999d906ca0c7e`  
		Last Modified: Wed, 09 Aug 2023 02:10:10 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.8.3-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:e99f31fd874fb90b2e194f296456d363d2a1bad2ec3b8da21be8d7af654063ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.6 MB (48561884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a302312f91cd531f910fc1a3646ae44d5bbfc68f936e4a16a14d25568849be98`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:26 GMT
ADD file:cf85500a1f5b87a88587b279c8b8018eebeb3092f402b7e2cc4ad3873e078580 in / 
# Mon, 07 Aug 2023 19:39:26 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 00:48:58 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 09 Aug 2023 00:48:58 GMT
ARG ASSET=ce
# Wed, 09 Aug 2023 00:48:58 GMT
ENV ASSET=ce
# Wed, 09 Aug 2023 00:48:58 GMT
ARG EE_PORTS
# Wed, 09 Aug 2023 00:48:59 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 09 Aug 2023 00:48:59 GMT
ARG KONG_VERSION=2.8.3
# Wed, 09 Aug 2023 00:48:59 GMT
ENV KONG_VERSION=2.8.3
# Wed, 09 Aug 2023 00:48:59 GMT
ARG KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa
# Wed, 09 Aug 2023 00:48:59 GMT
ARG KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
# Wed, 09 Aug 2023 00:49:05 GMT
# ARGS: KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Wed, 09 Aug 2023 00:49:06 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 09 Aug 2023 00:49:06 GMT
USER kong
# Wed, 09 Aug 2023 00:49:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 09 Aug 2023 00:49:06 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 09 Aug 2023 00:49:06 GMT
STOPSIGNAL SIGQUIT
# Wed, 09 Aug 2023 00:49:06 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 09 Aug 2023 00:49:06 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:bdb2de7ba06c3a4e10b98f439a8c70afd63eee492c2ddc32342331a8e9ef4ff7`  
		Last Modified: Mon, 07 Aug 2023 19:40:08 GMT  
		Size: 2.7 MB (2708023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb1eecfa54964173b307c94487ea0af19f5e974b6398b3aa5a90f5cdf3868a9f`  
		Last Modified: Wed, 09 Aug 2023 00:50:06 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1351a66935df1b153fa2ed39f64538ccbcacf7b1e58445453b58a977287ad4c8`  
		Last Modified: Wed, 09 Aug 2023 00:50:13 GMT  
		Size: 45.9 MB (45852849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28fdd42e521b9b7be083f6d661af365af3fa72ec9637b6120d93db37f1932597`  
		Last Modified: Wed, 09 Aug 2023 00:50:06 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3`

```console
$ docker pull kong@sha256:88aad0fa3c603af1b2ced86f33f0c28f664bf7b53c92aec1256746136b8832ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3` - linux; amd64

```console
$ docker pull kong@sha256:42f6f9d446ef95ec15c5b923b427d1d388190873bed01acb629403a0c2beb900
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81309563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43e05bc78243dbb39affc720b41c1b6dc97c47b68399d685654f8564ba5083a3`
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
# Wed, 02 Aug 2023 23:20:11 GMT
ARG KONG_VERSION=3.3.1
# Wed, 02 Aug 2023 23:20:11 GMT
ENV KONG_VERSION=3.3.1
# Wed, 02 Aug 2023 23:20:11 GMT
ARG KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20
# Wed, 02 Aug 2023 23:20:12 GMT
ARG KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
# Wed, 02 Aug 2023 23:20:54 GMT
# ARGS: KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20 KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 02 Aug 2023 23:20:55 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Wed, 02 Aug 2023 23:20:55 GMT
USER kong
# Wed, 02 Aug 2023 23:20:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Aug 2023 23:20:55 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 02 Aug 2023 23:20:56 GMT
STOPSIGNAL SIGQUIT
# Wed, 02 Aug 2023 23:20:56 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 02 Aug 2023 23:20:56 GMT
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
	-	`sha256:4301c643ae4f3131c8c234c6df308c4a1c99774c6f5b2154e3220722bc7f9b80`  
		Last Modified: Wed, 02 Aug 2023 23:21:58 GMT  
		Size: 50.9 MB (50877055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4df5348ff8cc4eafe8037d9fe277c70fd1e6b53b748ef5c5b1e4b775b9171be2`  
		Last Modified: Wed, 02 Aug 2023 23:21:50 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:a8e1d2db1cb9b42a350e294d0fc4ddecd5efbf5d0866325a29e5fc1e21475a7d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75731094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1596ccb23ca7efed78b341971bd5298b5abd30766ca3fe3ed525494fb47f1a24`
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
# Wed, 02 Aug 2023 23:42:17 GMT
ARG KONG_VERSION=3.3.1
# Wed, 02 Aug 2023 23:42:17 GMT
ENV KONG_VERSION=3.3.1
# Wed, 02 Aug 2023 23:42:17 GMT
ARG KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20
# Wed, 02 Aug 2023 23:42:17 GMT
ARG KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
# Wed, 02 Aug 2023 23:43:09 GMT
# ARGS: KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20 KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 02 Aug 2023 23:43:10 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Wed, 02 Aug 2023 23:43:10 GMT
USER kong
# Wed, 02 Aug 2023 23:43:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Aug 2023 23:43:10 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 02 Aug 2023 23:43:10 GMT
STOPSIGNAL SIGQUIT
# Wed, 02 Aug 2023 23:43:10 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 02 Aug 2023 23:43:10 GMT
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
	-	`sha256:3bab189bfe11a0b3cde378bf325f026a1441ee41c576e1f18a0e5898cbb8971c`  
		Last Modified: Wed, 02 Aug 2023 23:43:44 GMT  
		Size: 47.3 MB (47338797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc59e46a8f641d2af00c285650418bde267ff3994e2cd0a837a58dddc2a6c8f3`  
		Last Modified: Wed, 02 Aug 2023 23:43:38 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.0`

```console
$ docker pull kong@sha256:2f790d4a2e14db6829fac4ce148f2ddad3d198975d668c20cc0047b51621cf26
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.0` - linux; amd64

```console
$ docker pull kong@sha256:b1238c932dc5625cf73957c1df3cefacf49d76e0e622993e9bea54b381a6ed5a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75643979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d759a3dd02d73352e56804e0c17cfea93c885520f6bb79e80c1921515a8fecf`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:31 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
# Mon, 07 Aug 2023 19:20:31 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 02:08:02 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 09 Aug 2023 02:08:17 GMT
ARG KONG_VERSION=3.0.2
# Wed, 09 Aug 2023 02:08:17 GMT
ENV KONG_VERSION=3.0.2
# Wed, 09 Aug 2023 02:08:17 GMT
ARG KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e
# Wed, 09 Aug 2023 02:08:17 GMT
ARG KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
# Wed, 09 Aug 2023 02:08:17 GMT
ARG ASSET=remote
# Wed, 09 Aug 2023 02:08:17 GMT
ARG EE_PORTS
# Wed, 09 Aug 2023 02:08:17 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Wed, 09 Aug 2023 02:08:25 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Wed, 09 Aug 2023 02:08:25 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 09 Aug 2023 02:08:25 GMT
USER kong
# Wed, 09 Aug 2023 02:08:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 09 Aug 2023 02:08:26 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 09 Aug 2023 02:08:26 GMT
STOPSIGNAL SIGQUIT
# Wed, 09 Aug 2023 02:08:26 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 09 Aug 2023 02:08:26 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2bf2292254bdeddece5fd5404142936305ac8ee1aa036f0763f25769357e348`  
		Last Modified: Wed, 09 Aug 2023 02:09:49 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfaf3cf1299c4fdc39877181f5644cb9499797b502580628438d5919c2f851af`  
		Last Modified: Wed, 09 Aug 2023 02:09:57 GMT  
		Size: 72.8 MB (72835283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd91f0e9fb94a9fc47753572b38053713073132fd2ba16fbc2f287c2c0de5af`  
		Last Modified: Wed, 09 Aug 2023 02:09:49 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.0` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:05f41961163b0668efbefb9817e9b6258d5060c3a6c7d4944c31827c21b91e2c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73631765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9027dcf27c785720d206d2f0b922e8794640b05d541a657a62f209cd42677f15`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:26 GMT
ADD file:cf85500a1f5b87a88587b279c8b8018eebeb3092f402b7e2cc4ad3873e078580 in / 
# Mon, 07 Aug 2023 19:39:26 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 00:48:35 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 09 Aug 2023 00:48:46 GMT
ARG KONG_VERSION=3.0.2
# Wed, 09 Aug 2023 00:48:46 GMT
ENV KONG_VERSION=3.0.2
# Wed, 09 Aug 2023 00:48:46 GMT
ARG KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e
# Wed, 09 Aug 2023 00:48:46 GMT
ARG KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
# Wed, 09 Aug 2023 00:48:46 GMT
ARG ASSET=remote
# Wed, 09 Aug 2023 00:48:46 GMT
ARG EE_PORTS
# Wed, 09 Aug 2023 00:48:46 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Wed, 09 Aug 2023 00:48:53 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Wed, 09 Aug 2023 00:48:54 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 09 Aug 2023 00:48:54 GMT
USER kong
# Wed, 09 Aug 2023 00:48:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 09 Aug 2023 00:48:54 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 09 Aug 2023 00:48:54 GMT
STOPSIGNAL SIGQUIT
# Wed, 09 Aug 2023 00:48:54 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 09 Aug 2023 00:48:54 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:bdb2de7ba06c3a4e10b98f439a8c70afd63eee492c2ddc32342331a8e9ef4ff7`  
		Last Modified: Mon, 07 Aug 2023 19:40:08 GMT  
		Size: 2.7 MB (2708023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0979f99a3bf24ca1ac26cec8bf995cd98638738fdd30bbac063af807d9b4fa`  
		Last Modified: Wed, 09 Aug 2023 00:49:46 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642faca89a4e609c1d30f22536faac2665b8c7a7999a54ffb3e3e8fbf8b0e74a`  
		Last Modified: Wed, 09 Aug 2023 00:49:53 GMT  
		Size: 70.9 MB (70922726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7e5c6493f3156245805619fab35c2f8b4e253717934a86070d48f1a25c8a11`  
		Last Modified: Wed, 09 Aug 2023 00:49:46 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.0-alpine`

```console
$ docker pull kong@sha256:2f790d4a2e14db6829fac4ce148f2ddad3d198975d668c20cc0047b51621cf26
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.0-alpine` - linux; amd64

```console
$ docker pull kong@sha256:b1238c932dc5625cf73957c1df3cefacf49d76e0e622993e9bea54b381a6ed5a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75643979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d759a3dd02d73352e56804e0c17cfea93c885520f6bb79e80c1921515a8fecf`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:31 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
# Mon, 07 Aug 2023 19:20:31 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 02:08:02 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 09 Aug 2023 02:08:17 GMT
ARG KONG_VERSION=3.0.2
# Wed, 09 Aug 2023 02:08:17 GMT
ENV KONG_VERSION=3.0.2
# Wed, 09 Aug 2023 02:08:17 GMT
ARG KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e
# Wed, 09 Aug 2023 02:08:17 GMT
ARG KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
# Wed, 09 Aug 2023 02:08:17 GMT
ARG ASSET=remote
# Wed, 09 Aug 2023 02:08:17 GMT
ARG EE_PORTS
# Wed, 09 Aug 2023 02:08:17 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Wed, 09 Aug 2023 02:08:25 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Wed, 09 Aug 2023 02:08:25 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 09 Aug 2023 02:08:25 GMT
USER kong
# Wed, 09 Aug 2023 02:08:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 09 Aug 2023 02:08:26 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 09 Aug 2023 02:08:26 GMT
STOPSIGNAL SIGQUIT
# Wed, 09 Aug 2023 02:08:26 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 09 Aug 2023 02:08:26 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2bf2292254bdeddece5fd5404142936305ac8ee1aa036f0763f25769357e348`  
		Last Modified: Wed, 09 Aug 2023 02:09:49 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfaf3cf1299c4fdc39877181f5644cb9499797b502580628438d5919c2f851af`  
		Last Modified: Wed, 09 Aug 2023 02:09:57 GMT  
		Size: 72.8 MB (72835283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd91f0e9fb94a9fc47753572b38053713073132fd2ba16fbc2f287c2c0de5af`  
		Last Modified: Wed, 09 Aug 2023 02:09:49 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.0-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:05f41961163b0668efbefb9817e9b6258d5060c3a6c7d4944c31827c21b91e2c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73631765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9027dcf27c785720d206d2f0b922e8794640b05d541a657a62f209cd42677f15`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:26 GMT
ADD file:cf85500a1f5b87a88587b279c8b8018eebeb3092f402b7e2cc4ad3873e078580 in / 
# Mon, 07 Aug 2023 19:39:26 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 00:48:35 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 09 Aug 2023 00:48:46 GMT
ARG KONG_VERSION=3.0.2
# Wed, 09 Aug 2023 00:48:46 GMT
ENV KONG_VERSION=3.0.2
# Wed, 09 Aug 2023 00:48:46 GMT
ARG KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e
# Wed, 09 Aug 2023 00:48:46 GMT
ARG KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
# Wed, 09 Aug 2023 00:48:46 GMT
ARG ASSET=remote
# Wed, 09 Aug 2023 00:48:46 GMT
ARG EE_PORTS
# Wed, 09 Aug 2023 00:48:46 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Wed, 09 Aug 2023 00:48:53 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Wed, 09 Aug 2023 00:48:54 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 09 Aug 2023 00:48:54 GMT
USER kong
# Wed, 09 Aug 2023 00:48:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 09 Aug 2023 00:48:54 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 09 Aug 2023 00:48:54 GMT
STOPSIGNAL SIGQUIT
# Wed, 09 Aug 2023 00:48:54 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 09 Aug 2023 00:48:54 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:bdb2de7ba06c3a4e10b98f439a8c70afd63eee492c2ddc32342331a8e9ef4ff7`  
		Last Modified: Mon, 07 Aug 2023 19:40:08 GMT  
		Size: 2.7 MB (2708023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0979f99a3bf24ca1ac26cec8bf995cd98638738fdd30bbac063af807d9b4fa`  
		Last Modified: Wed, 09 Aug 2023 00:49:46 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642faca89a4e609c1d30f22536faac2665b8c7a7999a54ffb3e3e8fbf8b0e74a`  
		Last Modified: Wed, 09 Aug 2023 00:49:53 GMT  
		Size: 70.9 MB (70922726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7e5c6493f3156245805619fab35c2f8b4e253717934a86070d48f1a25c8a11`  
		Last Modified: Wed, 09 Aug 2023 00:49:46 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.0-ubuntu`

```console
$ docker pull kong@sha256:3e8933b350ce45772ff2b892b3daa161118c383a00bbe72d62b2498c6528297c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.0-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:0cf391e1dc85b090eecf03656297cf12921b42a445d444a73d8c85037caab113
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101864240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a77ede46f9b18ee8387809124a5519ae792995ebc0dd725146c0ea95b8d8eca4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:42:06 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 03 Aug 2023 03:42:06 GMT
ARG ASSET=ce
# Thu, 03 Aug 2023 03:42:06 GMT
ENV ASSET=ce
# Thu, 03 Aug 2023 03:42:06 GMT
ARG EE_PORTS
# Thu, 03 Aug 2023 03:42:07 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Thu, 03 Aug 2023 03:42:43 GMT
ARG KONG_VERSION=3.0.2
# Thu, 03 Aug 2023 03:42:43 GMT
ENV KONG_VERSION=3.0.2
# Thu, 03 Aug 2023 03:42:43 GMT
ARG KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396
# Thu, 03 Aug 2023 03:42:43 GMT
ARG KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
# Thu, 03 Aug 2023 03:43:04 GMT
# ARGS: KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396 KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Thu, 03 Aug 2023 03:43:05 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 03 Aug 2023 03:43:05 GMT
USER kong
# Thu, 03 Aug 2023 03:43:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 03 Aug 2023 03:43:05 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 03 Aug 2023 03:43:05 GMT
STOPSIGNAL SIGQUIT
# Thu, 03 Aug 2023 03:43:05 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 03 Aug 2023 03:43:05 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bfd1947ef25bf9da0d9f28d7e2bdab76db562475f8fc009b0f8e23e22e43a77`  
		Last Modified: Thu, 03 Aug 2023 03:43:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81f2c73eb2df556b3d1fc424ed07da862b308575085f9de17acf9f1f240bd40`  
		Last Modified: Thu, 03 Aug 2023 03:44:07 GMT  
		Size: 73.3 MB (73282558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a6669cc3c843faf284f77cbd562093b6bae4b2d45b340c2d37fa04169f291c`  
		Last Modified: Thu, 03 Aug 2023 03:43:55 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.0-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:05469b5deccb56bf41c0e0dfe191554978f9e19905735f7ac50f3bfb75202cfc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99115576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e057fc80c51a933bc665a3a4ed4e451726eec8eb2c953005277127e1f324c54`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:56 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:57 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:21:03 GMT
ADD file:ef6e767091d76c1461d099d5bc7a18c526ec80834cf87280803ab6480192f766 in / 
# Tue, 01 Aug 2023 06:21:03 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 00:53:09 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 03 Aug 2023 00:53:09 GMT
ARG ASSET=ce
# Thu, 03 Aug 2023 00:53:09 GMT
ENV ASSET=ce
# Thu, 03 Aug 2023 00:53:09 GMT
ARG EE_PORTS
# Thu, 03 Aug 2023 00:53:09 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Thu, 03 Aug 2023 00:53:38 GMT
ARG KONG_VERSION=3.0.2
# Thu, 03 Aug 2023 00:53:38 GMT
ENV KONG_VERSION=3.0.2
# Thu, 03 Aug 2023 00:53:38 GMT
ARG KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396
# Thu, 03 Aug 2023 00:53:38 GMT
ARG KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
# Thu, 03 Aug 2023 00:53:56 GMT
# ARGS: KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396 KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Thu, 03 Aug 2023 00:53:57 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 03 Aug 2023 00:53:57 GMT
USER kong
# Thu, 03 Aug 2023 00:53:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 03 Aug 2023 00:53:57 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 03 Aug 2023 00:53:57 GMT
STOPSIGNAL SIGQUIT
# Thu, 03 Aug 2023 00:53:57 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 03 Aug 2023 00:53:57 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c77c845df3241dcbb0441d9831a8dc0b9570d2cbd930090da9ac2a3a95f8af`  
		Last Modified: Thu, 03 Aug 2023 00:54:24 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9926acb25dee6fafce9e3b3aa1416b6525e8ead593e70086a3268a6f4ffcb49`  
		Last Modified: Thu, 03 Aug 2023 00:54:51 GMT  
		Size: 71.9 MB (71913981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:428ed1e2df3af1bd43c5846307277056e32674577b0db3f7bc5aefeef78488e3`  
		Last Modified: Thu, 03 Aug 2023 00:54:42 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.0.2`

```console
$ docker pull kong@sha256:2f790d4a2e14db6829fac4ce148f2ddad3d198975d668c20cc0047b51621cf26
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.0.2` - linux; amd64

```console
$ docker pull kong@sha256:b1238c932dc5625cf73957c1df3cefacf49d76e0e622993e9bea54b381a6ed5a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75643979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d759a3dd02d73352e56804e0c17cfea93c885520f6bb79e80c1921515a8fecf`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:31 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
# Mon, 07 Aug 2023 19:20:31 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 02:08:02 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 09 Aug 2023 02:08:17 GMT
ARG KONG_VERSION=3.0.2
# Wed, 09 Aug 2023 02:08:17 GMT
ENV KONG_VERSION=3.0.2
# Wed, 09 Aug 2023 02:08:17 GMT
ARG KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e
# Wed, 09 Aug 2023 02:08:17 GMT
ARG KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
# Wed, 09 Aug 2023 02:08:17 GMT
ARG ASSET=remote
# Wed, 09 Aug 2023 02:08:17 GMT
ARG EE_PORTS
# Wed, 09 Aug 2023 02:08:17 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Wed, 09 Aug 2023 02:08:25 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Wed, 09 Aug 2023 02:08:25 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 09 Aug 2023 02:08:25 GMT
USER kong
# Wed, 09 Aug 2023 02:08:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 09 Aug 2023 02:08:26 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 09 Aug 2023 02:08:26 GMT
STOPSIGNAL SIGQUIT
# Wed, 09 Aug 2023 02:08:26 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 09 Aug 2023 02:08:26 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2bf2292254bdeddece5fd5404142936305ac8ee1aa036f0763f25769357e348`  
		Last Modified: Wed, 09 Aug 2023 02:09:49 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfaf3cf1299c4fdc39877181f5644cb9499797b502580628438d5919c2f851af`  
		Last Modified: Wed, 09 Aug 2023 02:09:57 GMT  
		Size: 72.8 MB (72835283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd91f0e9fb94a9fc47753572b38053713073132fd2ba16fbc2f287c2c0de5af`  
		Last Modified: Wed, 09 Aug 2023 02:09:49 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.0.2` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:05f41961163b0668efbefb9817e9b6258d5060c3a6c7d4944c31827c21b91e2c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73631765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9027dcf27c785720d206d2f0b922e8794640b05d541a657a62f209cd42677f15`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:26 GMT
ADD file:cf85500a1f5b87a88587b279c8b8018eebeb3092f402b7e2cc4ad3873e078580 in / 
# Mon, 07 Aug 2023 19:39:26 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 00:48:35 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 09 Aug 2023 00:48:46 GMT
ARG KONG_VERSION=3.0.2
# Wed, 09 Aug 2023 00:48:46 GMT
ENV KONG_VERSION=3.0.2
# Wed, 09 Aug 2023 00:48:46 GMT
ARG KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e
# Wed, 09 Aug 2023 00:48:46 GMT
ARG KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
# Wed, 09 Aug 2023 00:48:46 GMT
ARG ASSET=remote
# Wed, 09 Aug 2023 00:48:46 GMT
ARG EE_PORTS
# Wed, 09 Aug 2023 00:48:46 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Wed, 09 Aug 2023 00:48:53 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Wed, 09 Aug 2023 00:48:54 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 09 Aug 2023 00:48:54 GMT
USER kong
# Wed, 09 Aug 2023 00:48:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 09 Aug 2023 00:48:54 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 09 Aug 2023 00:48:54 GMT
STOPSIGNAL SIGQUIT
# Wed, 09 Aug 2023 00:48:54 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 09 Aug 2023 00:48:54 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:bdb2de7ba06c3a4e10b98f439a8c70afd63eee492c2ddc32342331a8e9ef4ff7`  
		Last Modified: Mon, 07 Aug 2023 19:40:08 GMT  
		Size: 2.7 MB (2708023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0979f99a3bf24ca1ac26cec8bf995cd98638738fdd30bbac063af807d9b4fa`  
		Last Modified: Wed, 09 Aug 2023 00:49:46 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642faca89a4e609c1d30f22536faac2665b8c7a7999a54ffb3e3e8fbf8b0e74a`  
		Last Modified: Wed, 09 Aug 2023 00:49:53 GMT  
		Size: 70.9 MB (70922726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7e5c6493f3156245805619fab35c2f8b4e253717934a86070d48f1a25c8a11`  
		Last Modified: Wed, 09 Aug 2023 00:49:46 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.0.2-alpine`

```console
$ docker pull kong@sha256:2f790d4a2e14db6829fac4ce148f2ddad3d198975d668c20cc0047b51621cf26
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.0.2-alpine` - linux; amd64

```console
$ docker pull kong@sha256:b1238c932dc5625cf73957c1df3cefacf49d76e0e622993e9bea54b381a6ed5a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75643979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d759a3dd02d73352e56804e0c17cfea93c885520f6bb79e80c1921515a8fecf`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:31 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
# Mon, 07 Aug 2023 19:20:31 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 02:08:02 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 09 Aug 2023 02:08:17 GMT
ARG KONG_VERSION=3.0.2
# Wed, 09 Aug 2023 02:08:17 GMT
ENV KONG_VERSION=3.0.2
# Wed, 09 Aug 2023 02:08:17 GMT
ARG KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e
# Wed, 09 Aug 2023 02:08:17 GMT
ARG KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
# Wed, 09 Aug 2023 02:08:17 GMT
ARG ASSET=remote
# Wed, 09 Aug 2023 02:08:17 GMT
ARG EE_PORTS
# Wed, 09 Aug 2023 02:08:17 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Wed, 09 Aug 2023 02:08:25 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Wed, 09 Aug 2023 02:08:25 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 09 Aug 2023 02:08:25 GMT
USER kong
# Wed, 09 Aug 2023 02:08:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 09 Aug 2023 02:08:26 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 09 Aug 2023 02:08:26 GMT
STOPSIGNAL SIGQUIT
# Wed, 09 Aug 2023 02:08:26 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 09 Aug 2023 02:08:26 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2bf2292254bdeddece5fd5404142936305ac8ee1aa036f0763f25769357e348`  
		Last Modified: Wed, 09 Aug 2023 02:09:49 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfaf3cf1299c4fdc39877181f5644cb9499797b502580628438d5919c2f851af`  
		Last Modified: Wed, 09 Aug 2023 02:09:57 GMT  
		Size: 72.8 MB (72835283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd91f0e9fb94a9fc47753572b38053713073132fd2ba16fbc2f287c2c0de5af`  
		Last Modified: Wed, 09 Aug 2023 02:09:49 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.0.2-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:05f41961163b0668efbefb9817e9b6258d5060c3a6c7d4944c31827c21b91e2c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73631765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9027dcf27c785720d206d2f0b922e8794640b05d541a657a62f209cd42677f15`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:26 GMT
ADD file:cf85500a1f5b87a88587b279c8b8018eebeb3092f402b7e2cc4ad3873e078580 in / 
# Mon, 07 Aug 2023 19:39:26 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 00:48:35 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 09 Aug 2023 00:48:46 GMT
ARG KONG_VERSION=3.0.2
# Wed, 09 Aug 2023 00:48:46 GMT
ENV KONG_VERSION=3.0.2
# Wed, 09 Aug 2023 00:48:46 GMT
ARG KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e
# Wed, 09 Aug 2023 00:48:46 GMT
ARG KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
# Wed, 09 Aug 2023 00:48:46 GMT
ARG ASSET=remote
# Wed, 09 Aug 2023 00:48:46 GMT
ARG EE_PORTS
# Wed, 09 Aug 2023 00:48:46 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Wed, 09 Aug 2023 00:48:53 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Wed, 09 Aug 2023 00:48:54 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 09 Aug 2023 00:48:54 GMT
USER kong
# Wed, 09 Aug 2023 00:48:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 09 Aug 2023 00:48:54 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 09 Aug 2023 00:48:54 GMT
STOPSIGNAL SIGQUIT
# Wed, 09 Aug 2023 00:48:54 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 09 Aug 2023 00:48:54 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:bdb2de7ba06c3a4e10b98f439a8c70afd63eee492c2ddc32342331a8e9ef4ff7`  
		Last Modified: Mon, 07 Aug 2023 19:40:08 GMT  
		Size: 2.7 MB (2708023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0979f99a3bf24ca1ac26cec8bf995cd98638738fdd30bbac063af807d9b4fa`  
		Last Modified: Wed, 09 Aug 2023 00:49:46 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:642faca89a4e609c1d30f22536faac2665b8c7a7999a54ffb3e3e8fbf8b0e74a`  
		Last Modified: Wed, 09 Aug 2023 00:49:53 GMT  
		Size: 70.9 MB (70922726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7e5c6493f3156245805619fab35c2f8b4e253717934a86070d48f1a25c8a11`  
		Last Modified: Wed, 09 Aug 2023 00:49:46 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.0.2-ubuntu`

```console
$ docker pull kong@sha256:3e8933b350ce45772ff2b892b3daa161118c383a00bbe72d62b2498c6528297c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.0.2-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:0cf391e1dc85b090eecf03656297cf12921b42a445d444a73d8c85037caab113
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101864240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a77ede46f9b18ee8387809124a5519ae792995ebc0dd725146c0ea95b8d8eca4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:42:06 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 03 Aug 2023 03:42:06 GMT
ARG ASSET=ce
# Thu, 03 Aug 2023 03:42:06 GMT
ENV ASSET=ce
# Thu, 03 Aug 2023 03:42:06 GMT
ARG EE_PORTS
# Thu, 03 Aug 2023 03:42:07 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Thu, 03 Aug 2023 03:42:43 GMT
ARG KONG_VERSION=3.0.2
# Thu, 03 Aug 2023 03:42:43 GMT
ENV KONG_VERSION=3.0.2
# Thu, 03 Aug 2023 03:42:43 GMT
ARG KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396
# Thu, 03 Aug 2023 03:42:43 GMT
ARG KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
# Thu, 03 Aug 2023 03:43:04 GMT
# ARGS: KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396 KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Thu, 03 Aug 2023 03:43:05 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 03 Aug 2023 03:43:05 GMT
USER kong
# Thu, 03 Aug 2023 03:43:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 03 Aug 2023 03:43:05 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 03 Aug 2023 03:43:05 GMT
STOPSIGNAL SIGQUIT
# Thu, 03 Aug 2023 03:43:05 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 03 Aug 2023 03:43:05 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bfd1947ef25bf9da0d9f28d7e2bdab76db562475f8fc009b0f8e23e22e43a77`  
		Last Modified: Thu, 03 Aug 2023 03:43:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81f2c73eb2df556b3d1fc424ed07da862b308575085f9de17acf9f1f240bd40`  
		Last Modified: Thu, 03 Aug 2023 03:44:07 GMT  
		Size: 73.3 MB (73282558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a6669cc3c843faf284f77cbd562093b6bae4b2d45b340c2d37fa04169f291c`  
		Last Modified: Thu, 03 Aug 2023 03:43:55 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.0.2-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:05469b5deccb56bf41c0e0dfe191554978f9e19905735f7ac50f3bfb75202cfc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99115576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e057fc80c51a933bc665a3a4ed4e451726eec8eb2c953005277127e1f324c54`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:56 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:57 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:21:03 GMT
ADD file:ef6e767091d76c1461d099d5bc7a18c526ec80834cf87280803ab6480192f766 in / 
# Tue, 01 Aug 2023 06:21:03 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 00:53:09 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 03 Aug 2023 00:53:09 GMT
ARG ASSET=ce
# Thu, 03 Aug 2023 00:53:09 GMT
ENV ASSET=ce
# Thu, 03 Aug 2023 00:53:09 GMT
ARG EE_PORTS
# Thu, 03 Aug 2023 00:53:09 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Thu, 03 Aug 2023 00:53:38 GMT
ARG KONG_VERSION=3.0.2
# Thu, 03 Aug 2023 00:53:38 GMT
ENV KONG_VERSION=3.0.2
# Thu, 03 Aug 2023 00:53:38 GMT
ARG KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396
# Thu, 03 Aug 2023 00:53:38 GMT
ARG KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
# Thu, 03 Aug 2023 00:53:56 GMT
# ARGS: KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396 KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Thu, 03 Aug 2023 00:53:57 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 03 Aug 2023 00:53:57 GMT
USER kong
# Thu, 03 Aug 2023 00:53:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 03 Aug 2023 00:53:57 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 03 Aug 2023 00:53:57 GMT
STOPSIGNAL SIGQUIT
# Thu, 03 Aug 2023 00:53:57 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 03 Aug 2023 00:53:57 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c77c845df3241dcbb0441d9831a8dc0b9570d2cbd930090da9ac2a3a95f8af`  
		Last Modified: Thu, 03 Aug 2023 00:54:24 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9926acb25dee6fafce9e3b3aa1416b6525e8ead593e70086a3268a6f4ffcb49`  
		Last Modified: Thu, 03 Aug 2023 00:54:51 GMT  
		Size: 71.9 MB (71913981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:428ed1e2df3af1bd43c5846307277056e32674577b0db3f7bc5aefeef78488e3`  
		Last Modified: Thu, 03 Aug 2023 00:54:42 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.1`

```console
$ docker pull kong@sha256:1343012088b39d8d537c2fe6458471a133f449f6204c8d7d70d8b8c0cfa8c8f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.1` - linux; amd64

```console
$ docker pull kong@sha256:d2472e234071c0cf3b05fca95a26aa5d99aaa7b41da3ce5a39316d878a1d641f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75688551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79572b5d2ffdb45a6352d276b15d7c2b8642d57b25b7148da866aa1393c8fcc1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:31 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
# Mon, 07 Aug 2023 19:20:31 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 02:08:02 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 09 Aug 2023 02:08:02 GMT
ARG KONG_VERSION=3.1.1
# Wed, 09 Aug 2023 02:08:02 GMT
ENV KONG_VERSION=3.1.1
# Wed, 09 Aug 2023 02:08:02 GMT
ARG KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c
# Wed, 09 Aug 2023 02:08:02 GMT
ARG KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
# Wed, 09 Aug 2023 02:08:02 GMT
ARG ASSET=remote
# Wed, 09 Aug 2023 02:08:02 GMT
ARG EE_PORTS
# Wed, 09 Aug 2023 02:08:02 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Wed, 09 Aug 2023 02:08:10 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Wed, 09 Aug 2023 02:08:10 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 09 Aug 2023 02:08:11 GMT
USER kong
# Wed, 09 Aug 2023 02:08:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 09 Aug 2023 02:08:11 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 09 Aug 2023 02:08:11 GMT
STOPSIGNAL SIGQUIT
# Wed, 09 Aug 2023 02:08:11 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 09 Aug 2023 02:08:11 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b3c55b434a1557b2a03f5de1da2c4c3a4797eeb296f72be90972d112de47f7`  
		Last Modified: Wed, 09 Aug 2023 02:09:31 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a819af6c9aa5601e8b2e2633640fd9b40ac32601daacc69444504a74902710`  
		Last Modified: Wed, 09 Aug 2023 02:09:38 GMT  
		Size: 72.9 MB (72879856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ea0410a4dddcfadf34f30856530d79c5f67b7f259991341443b9a7d012922f`  
		Last Modified: Wed, 09 Aug 2023 02:09:31 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.1` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:b7dfcf1d4c6b798d32aa52b9fc5b3d97ba1b99786e170cb9357f2993909dc87d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.7 MB (73705224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5164e03b97899461e1649290fa67a186dc23b884614c7189af52be54d0bad46e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:26 GMT
ADD file:cf85500a1f5b87a88587b279c8b8018eebeb3092f402b7e2cc4ad3873e078580 in / 
# Mon, 07 Aug 2023 19:39:26 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 00:48:35 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 09 Aug 2023 00:48:35 GMT
ARG KONG_VERSION=3.1.1
# Wed, 09 Aug 2023 00:48:35 GMT
ENV KONG_VERSION=3.1.1
# Wed, 09 Aug 2023 00:48:35 GMT
ARG KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c
# Wed, 09 Aug 2023 00:48:35 GMT
ARG KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
# Wed, 09 Aug 2023 00:48:35 GMT
ARG ASSET=remote
# Wed, 09 Aug 2023 00:48:35 GMT
ARG EE_PORTS
# Wed, 09 Aug 2023 00:48:35 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Wed, 09 Aug 2023 00:48:41 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Wed, 09 Aug 2023 00:48:42 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 09 Aug 2023 00:48:42 GMT
USER kong
# Wed, 09 Aug 2023 00:48:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 09 Aug 2023 00:48:42 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 09 Aug 2023 00:48:42 GMT
STOPSIGNAL SIGQUIT
# Wed, 09 Aug 2023 00:48:42 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 09 Aug 2023 00:48:43 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:bdb2de7ba06c3a4e10b98f439a8c70afd63eee492c2ddc32342331a8e9ef4ff7`  
		Last Modified: Mon, 07 Aug 2023 19:40:08 GMT  
		Size: 2.7 MB (2708023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6597708a938f08bd238a22418f37a3a106d1654ac0fa24ff747e6a8f8d991571`  
		Last Modified: Wed, 09 Aug 2023 00:49:26 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ead036cb321091d34aff3c37ef5ccc73ae4b602f7ff4e10ffb144e668a1ba2`  
		Last Modified: Wed, 09 Aug 2023 00:49:34 GMT  
		Size: 71.0 MB (70996187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f24009d19331e18ec2beb350bec21b9c1fa1e8649f40c20d5eb514857afadc3`  
		Last Modified: Wed, 09 Aug 2023 00:49:26 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.1-ubuntu`

```console
$ docker pull kong@sha256:084eac26e0e9a7ce27c6bf506d7436384f6675ba3d83a8d35bd937276dd428e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.1-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:20cfb317a05292ad29bd3985886cb664ab89b590d4bdfd626feedda08604ca8c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101884060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63c06083105862ff1d7cf2964be06e6987751e3c236665565f0b3d834caca2d4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:42:06 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 03 Aug 2023 03:42:06 GMT
ARG ASSET=ce
# Thu, 03 Aug 2023 03:42:06 GMT
ENV ASSET=ce
# Thu, 03 Aug 2023 03:42:06 GMT
ARG EE_PORTS
# Thu, 03 Aug 2023 03:42:07 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Thu, 03 Aug 2023 03:42:07 GMT
ARG KONG_VERSION=3.1.1
# Thu, 03 Aug 2023 03:42:07 GMT
ENV KONG_VERSION=3.1.1
# Thu, 03 Aug 2023 03:42:07 GMT
ARG KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b
# Thu, 03 Aug 2023 03:42:07 GMT
ARG KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
# Thu, 03 Aug 2023 03:42:36 GMT
# ARGS: KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Thu, 03 Aug 2023 03:42:37 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 03 Aug 2023 03:42:37 GMT
USER kong
# Thu, 03 Aug 2023 03:42:37 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 03 Aug 2023 03:42:37 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 03 Aug 2023 03:42:37 GMT
STOPSIGNAL SIGQUIT
# Thu, 03 Aug 2023 03:42:38 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 03 Aug 2023 03:42:38 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bfd1947ef25bf9da0d9f28d7e2bdab76db562475f8fc009b0f8e23e22e43a77`  
		Last Modified: Thu, 03 Aug 2023 03:43:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7da99a3a25d709198b7ba98018b890cdd4e41ee98e28695f4234f7724b9935`  
		Last Modified: Thu, 03 Aug 2023 03:43:46 GMT  
		Size: 73.3 MB (73302378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ea9c35517883794cce1ec10fe3aa0ae1ed5303555691e49bb49e4afe694a38`  
		Last Modified: Thu, 03 Aug 2023 03:43:35 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.1-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:0fbf5d11117887f1cc082d9175589e800401c27e0a8217a90d0a3247b3b57e44
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99145787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc06772006e5af39797b759b8cd34188e979f049b6d73ac5bba10fff7c126fab`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:56 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:57 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:21:03 GMT
ADD file:ef6e767091d76c1461d099d5bc7a18c526ec80834cf87280803ab6480192f766 in / 
# Tue, 01 Aug 2023 06:21:03 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 00:53:09 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 03 Aug 2023 00:53:09 GMT
ARG ASSET=ce
# Thu, 03 Aug 2023 00:53:09 GMT
ENV ASSET=ce
# Thu, 03 Aug 2023 00:53:09 GMT
ARG EE_PORTS
# Thu, 03 Aug 2023 00:53:09 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Thu, 03 Aug 2023 00:53:09 GMT
ARG KONG_VERSION=3.1.1
# Thu, 03 Aug 2023 00:53:09 GMT
ENV KONG_VERSION=3.1.1
# Thu, 03 Aug 2023 00:53:09 GMT
ARG KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b
# Thu, 03 Aug 2023 00:53:09 GMT
ARG KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
# Thu, 03 Aug 2023 00:53:31 GMT
# ARGS: KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Thu, 03 Aug 2023 00:53:32 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 03 Aug 2023 00:53:32 GMT
USER kong
# Thu, 03 Aug 2023 00:53:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 03 Aug 2023 00:53:33 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 03 Aug 2023 00:53:33 GMT
STOPSIGNAL SIGQUIT
# Thu, 03 Aug 2023 00:53:33 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 03 Aug 2023 00:53:33 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c77c845df3241dcbb0441d9831a8dc0b9570d2cbd930090da9ac2a3a95f8af`  
		Last Modified: Thu, 03 Aug 2023 00:54:24 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb00080b1dda76971934e260ad73f5e8b8259f5f26ba44293db189cba0e8db6d`  
		Last Modified: Thu, 03 Aug 2023 00:54:33 GMT  
		Size: 71.9 MB (71944192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006243dadd213bb59ff428fde4cd5c3445fac094643a85e55911c398f08b74b7`  
		Last Modified: Thu, 03 Aug 2023 00:54:24 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.1.1`

```console
$ docker pull kong@sha256:1343012088b39d8d537c2fe6458471a133f449f6204c8d7d70d8b8c0cfa8c8f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.1.1` - linux; amd64

```console
$ docker pull kong@sha256:d2472e234071c0cf3b05fca95a26aa5d99aaa7b41da3ce5a39316d878a1d641f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75688551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79572b5d2ffdb45a6352d276b15d7c2b8642d57b25b7148da866aa1393c8fcc1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:31 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
# Mon, 07 Aug 2023 19:20:31 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 02:08:02 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 09 Aug 2023 02:08:02 GMT
ARG KONG_VERSION=3.1.1
# Wed, 09 Aug 2023 02:08:02 GMT
ENV KONG_VERSION=3.1.1
# Wed, 09 Aug 2023 02:08:02 GMT
ARG KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c
# Wed, 09 Aug 2023 02:08:02 GMT
ARG KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
# Wed, 09 Aug 2023 02:08:02 GMT
ARG ASSET=remote
# Wed, 09 Aug 2023 02:08:02 GMT
ARG EE_PORTS
# Wed, 09 Aug 2023 02:08:02 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Wed, 09 Aug 2023 02:08:10 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Wed, 09 Aug 2023 02:08:10 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 09 Aug 2023 02:08:11 GMT
USER kong
# Wed, 09 Aug 2023 02:08:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 09 Aug 2023 02:08:11 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 09 Aug 2023 02:08:11 GMT
STOPSIGNAL SIGQUIT
# Wed, 09 Aug 2023 02:08:11 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 09 Aug 2023 02:08:11 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b3c55b434a1557b2a03f5de1da2c4c3a4797eeb296f72be90972d112de47f7`  
		Last Modified: Wed, 09 Aug 2023 02:09:31 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a819af6c9aa5601e8b2e2633640fd9b40ac32601daacc69444504a74902710`  
		Last Modified: Wed, 09 Aug 2023 02:09:38 GMT  
		Size: 72.9 MB (72879856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ea0410a4dddcfadf34f30856530d79c5f67b7f259991341443b9a7d012922f`  
		Last Modified: Wed, 09 Aug 2023 02:09:31 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.1.1` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:b7dfcf1d4c6b798d32aa52b9fc5b3d97ba1b99786e170cb9357f2993909dc87d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.7 MB (73705224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5164e03b97899461e1649290fa67a186dc23b884614c7189af52be54d0bad46e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:26 GMT
ADD file:cf85500a1f5b87a88587b279c8b8018eebeb3092f402b7e2cc4ad3873e078580 in / 
# Mon, 07 Aug 2023 19:39:26 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 00:48:35 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 09 Aug 2023 00:48:35 GMT
ARG KONG_VERSION=3.1.1
# Wed, 09 Aug 2023 00:48:35 GMT
ENV KONG_VERSION=3.1.1
# Wed, 09 Aug 2023 00:48:35 GMT
ARG KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c
# Wed, 09 Aug 2023 00:48:35 GMT
ARG KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
# Wed, 09 Aug 2023 00:48:35 GMT
ARG ASSET=remote
# Wed, 09 Aug 2023 00:48:35 GMT
ARG EE_PORTS
# Wed, 09 Aug 2023 00:48:35 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Wed, 09 Aug 2023 00:48:41 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Wed, 09 Aug 2023 00:48:42 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 09 Aug 2023 00:48:42 GMT
USER kong
# Wed, 09 Aug 2023 00:48:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 09 Aug 2023 00:48:42 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 09 Aug 2023 00:48:42 GMT
STOPSIGNAL SIGQUIT
# Wed, 09 Aug 2023 00:48:42 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 09 Aug 2023 00:48:43 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:bdb2de7ba06c3a4e10b98f439a8c70afd63eee492c2ddc32342331a8e9ef4ff7`  
		Last Modified: Mon, 07 Aug 2023 19:40:08 GMT  
		Size: 2.7 MB (2708023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6597708a938f08bd238a22418f37a3a106d1654ac0fa24ff747e6a8f8d991571`  
		Last Modified: Wed, 09 Aug 2023 00:49:26 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ead036cb321091d34aff3c37ef5ccc73ae4b602f7ff4e10ffb144e668a1ba2`  
		Last Modified: Wed, 09 Aug 2023 00:49:34 GMT  
		Size: 71.0 MB (70996187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f24009d19331e18ec2beb350bec21b9c1fa1e8649f40c20d5eb514857afadc3`  
		Last Modified: Wed, 09 Aug 2023 00:49:26 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.1.1-alpine`

```console
$ docker pull kong@sha256:1343012088b39d8d537c2fe6458471a133f449f6204c8d7d70d8b8c0cfa8c8f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.1.1-alpine` - linux; amd64

```console
$ docker pull kong@sha256:d2472e234071c0cf3b05fca95a26aa5d99aaa7b41da3ce5a39316d878a1d641f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75688551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79572b5d2ffdb45a6352d276b15d7c2b8642d57b25b7148da866aa1393c8fcc1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:31 GMT
ADD file:76d829bbce3dd420a8419919b0916c0fda917011d1e6752ca5b9e53d5ca890a6 in / 
# Mon, 07 Aug 2023 19:20:31 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 02:08:02 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 09 Aug 2023 02:08:02 GMT
ARG KONG_VERSION=3.1.1
# Wed, 09 Aug 2023 02:08:02 GMT
ENV KONG_VERSION=3.1.1
# Wed, 09 Aug 2023 02:08:02 GMT
ARG KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c
# Wed, 09 Aug 2023 02:08:02 GMT
ARG KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
# Wed, 09 Aug 2023 02:08:02 GMT
ARG ASSET=remote
# Wed, 09 Aug 2023 02:08:02 GMT
ARG EE_PORTS
# Wed, 09 Aug 2023 02:08:02 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Wed, 09 Aug 2023 02:08:10 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Wed, 09 Aug 2023 02:08:10 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 09 Aug 2023 02:08:11 GMT
USER kong
# Wed, 09 Aug 2023 02:08:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 09 Aug 2023 02:08:11 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 09 Aug 2023 02:08:11 GMT
STOPSIGNAL SIGQUIT
# Wed, 09 Aug 2023 02:08:11 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 09 Aug 2023 02:08:11 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:659d66d51139e8abad819d17e5d3c45eb82e88b9fc588c4de7711f251309b9d2`  
		Last Modified: Mon, 07 Aug 2023 19:21:19 GMT  
		Size: 2.8 MB (2807683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b3c55b434a1557b2a03f5de1da2c4c3a4797eeb296f72be90972d112de47f7`  
		Last Modified: Wed, 09 Aug 2023 02:09:31 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a819af6c9aa5601e8b2e2633640fd9b40ac32601daacc69444504a74902710`  
		Last Modified: Wed, 09 Aug 2023 02:09:38 GMT  
		Size: 72.9 MB (72879856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ea0410a4dddcfadf34f30856530d79c5f67b7f259991341443b9a7d012922f`  
		Last Modified: Wed, 09 Aug 2023 02:09:31 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.1.1-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:b7dfcf1d4c6b798d32aa52b9fc5b3d97ba1b99786e170cb9357f2993909dc87d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.7 MB (73705224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5164e03b97899461e1649290fa67a186dc23b884614c7189af52be54d0bad46e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:26 GMT
ADD file:cf85500a1f5b87a88587b279c8b8018eebeb3092f402b7e2cc4ad3873e078580 in / 
# Mon, 07 Aug 2023 19:39:26 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 00:48:35 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 09 Aug 2023 00:48:35 GMT
ARG KONG_VERSION=3.1.1
# Wed, 09 Aug 2023 00:48:35 GMT
ENV KONG_VERSION=3.1.1
# Wed, 09 Aug 2023 00:48:35 GMT
ARG KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c
# Wed, 09 Aug 2023 00:48:35 GMT
ARG KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
# Wed, 09 Aug 2023 00:48:35 GMT
ARG ASSET=remote
# Wed, 09 Aug 2023 00:48:35 GMT
ARG EE_PORTS
# Wed, 09 Aug 2023 00:48:35 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Wed, 09 Aug 2023 00:48:41 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Wed, 09 Aug 2023 00:48:42 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 09 Aug 2023 00:48:42 GMT
USER kong
# Wed, 09 Aug 2023 00:48:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 09 Aug 2023 00:48:42 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 09 Aug 2023 00:48:42 GMT
STOPSIGNAL SIGQUIT
# Wed, 09 Aug 2023 00:48:42 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 09 Aug 2023 00:48:43 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:bdb2de7ba06c3a4e10b98f439a8c70afd63eee492c2ddc32342331a8e9ef4ff7`  
		Last Modified: Mon, 07 Aug 2023 19:40:08 GMT  
		Size: 2.7 MB (2708023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6597708a938f08bd238a22418f37a3a106d1654ac0fa24ff747e6a8f8d991571`  
		Last Modified: Wed, 09 Aug 2023 00:49:26 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ead036cb321091d34aff3c37ef5ccc73ae4b602f7ff4e10ffb144e668a1ba2`  
		Last Modified: Wed, 09 Aug 2023 00:49:34 GMT  
		Size: 71.0 MB (70996187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f24009d19331e18ec2beb350bec21b9c1fa1e8649f40c20d5eb514857afadc3`  
		Last Modified: Wed, 09 Aug 2023 00:49:26 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.1.1-ubuntu`

```console
$ docker pull kong@sha256:084eac26e0e9a7ce27c6bf506d7436384f6675ba3d83a8d35bd937276dd428e7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.1.1-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:20cfb317a05292ad29bd3985886cb664ab89b590d4bdfd626feedda08604ca8c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101884060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63c06083105862ff1d7cf2964be06e6987751e3c236665565f0b3d834caca2d4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:42:06 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 03 Aug 2023 03:42:06 GMT
ARG ASSET=ce
# Thu, 03 Aug 2023 03:42:06 GMT
ENV ASSET=ce
# Thu, 03 Aug 2023 03:42:06 GMT
ARG EE_PORTS
# Thu, 03 Aug 2023 03:42:07 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Thu, 03 Aug 2023 03:42:07 GMT
ARG KONG_VERSION=3.1.1
# Thu, 03 Aug 2023 03:42:07 GMT
ENV KONG_VERSION=3.1.1
# Thu, 03 Aug 2023 03:42:07 GMT
ARG KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b
# Thu, 03 Aug 2023 03:42:07 GMT
ARG KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
# Thu, 03 Aug 2023 03:42:36 GMT
# ARGS: KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Thu, 03 Aug 2023 03:42:37 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 03 Aug 2023 03:42:37 GMT
USER kong
# Thu, 03 Aug 2023 03:42:37 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 03 Aug 2023 03:42:37 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 03 Aug 2023 03:42:37 GMT
STOPSIGNAL SIGQUIT
# Thu, 03 Aug 2023 03:42:38 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 03 Aug 2023 03:42:38 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bfd1947ef25bf9da0d9f28d7e2bdab76db562475f8fc009b0f8e23e22e43a77`  
		Last Modified: Thu, 03 Aug 2023 03:43:35 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7da99a3a25d709198b7ba98018b890cdd4e41ee98e28695f4234f7724b9935`  
		Last Modified: Thu, 03 Aug 2023 03:43:46 GMT  
		Size: 73.3 MB (73302378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ea9c35517883794cce1ec10fe3aa0ae1ed5303555691e49bb49e4afe694a38`  
		Last Modified: Thu, 03 Aug 2023 03:43:35 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.1.1-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:0fbf5d11117887f1cc082d9175589e800401c27e0a8217a90d0a3247b3b57e44
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99145787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc06772006e5af39797b759b8cd34188e979f049b6d73ac5bba10fff7c126fab`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:56 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:57 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:21:03 GMT
ADD file:ef6e767091d76c1461d099d5bc7a18c526ec80834cf87280803ab6480192f766 in / 
# Tue, 01 Aug 2023 06:21:03 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 00:53:09 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 03 Aug 2023 00:53:09 GMT
ARG ASSET=ce
# Thu, 03 Aug 2023 00:53:09 GMT
ENV ASSET=ce
# Thu, 03 Aug 2023 00:53:09 GMT
ARG EE_PORTS
# Thu, 03 Aug 2023 00:53:09 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Thu, 03 Aug 2023 00:53:09 GMT
ARG KONG_VERSION=3.1.1
# Thu, 03 Aug 2023 00:53:09 GMT
ENV KONG_VERSION=3.1.1
# Thu, 03 Aug 2023 00:53:09 GMT
ARG KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b
# Thu, 03 Aug 2023 00:53:09 GMT
ARG KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
# Thu, 03 Aug 2023 00:53:31 GMT
# ARGS: KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Thu, 03 Aug 2023 00:53:32 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 03 Aug 2023 00:53:32 GMT
USER kong
# Thu, 03 Aug 2023 00:53:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 03 Aug 2023 00:53:33 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 03 Aug 2023 00:53:33 GMT
STOPSIGNAL SIGQUIT
# Thu, 03 Aug 2023 00:53:33 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 03 Aug 2023 00:53:33 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c77c845df3241dcbb0441d9831a8dc0b9570d2cbd930090da9ac2a3a95f8af`  
		Last Modified: Thu, 03 Aug 2023 00:54:24 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb00080b1dda76971934e260ad73f5e8b8259f5f26ba44293db189cba0e8db6d`  
		Last Modified: Thu, 03 Aug 2023 00:54:33 GMT  
		Size: 71.9 MB (71944192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006243dadd213bb59ff428fde4cd5c3445fac094643a85e55911c398f08b74b7`  
		Last Modified: Thu, 03 Aug 2023 00:54:24 GMT  
		Size: 882.0 B  
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
$ docker pull kong@sha256:54784fbe110a9810921533854a89d06b42eaacb088e3eb92f7bba01928a38733
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:3.2.2-alpine` - linux; amd64

```console
$ docker pull kong@sha256:2bcb348f1e506db66d37fa2aeb19128fde0898c8e05e5a8041e5b09a7d0a6133
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.9 MB (36929739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e19dc1823bd86f40b0c4039b2cd0a704eb84d817e9b8b7c5ed8a77914fc77cc`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 02:07:36 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 09 Aug 2023 02:07:49 GMT
ARG KONG_VERSION=3.2.2
# Wed, 09 Aug 2023 02:07:49 GMT
ENV KONG_VERSION=3.2.2
# Wed, 09 Aug 2023 02:07:49 GMT
ARG KONG_SHA256=a07c3bc0307e2d8fe33acb8be5fe659f348279540eaa267bc6968005094835ef
# Wed, 09 Aug 2023 02:07:49 GMT
ARG KONG_PREFIX=/usr/local/kong
# Wed, 09 Aug 2023 02:07:49 GMT
ENV KONG_PREFIX=/usr/local/kong
# Wed, 09 Aug 2023 02:07:49 GMT
ARG ASSET=remote
# Wed, 09 Aug 2023 02:07:49 GMT
ARG EE_PORTS
# Wed, 09 Aug 2023 02:07:49 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Wed, 09 Aug 2023 02:07:55 GMT
# ARGS: ASSET=remote KONG_SHA256=a07c3bc0307e2d8fe33acb8be5fe659f348279540eaa267bc6968005094835ef
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     export ARCH='amd64';     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc perl tzdata libcap zlib zlib-dev bash yaml     && adduser -S kong     && addgroup -S kong     && mkdir -p "${KONG_PREFIX}"     && chown -R kong:0 ${KONG_PREFIX}     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u ${KONG_PREFIX}     && rm -rf /tmp/kong.apk.tar.gz     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Wed, 09 Aug 2023 02:07:56 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Wed, 09 Aug 2023 02:07:56 GMT
USER kong
# Wed, 09 Aug 2023 02:07:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 09 Aug 2023 02:07:56 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 09 Aug 2023 02:07:56 GMT
STOPSIGNAL SIGQUIT
# Wed, 09 Aug 2023 02:07:56 GMT
HEALTHCHECK &{["CMD-SHELL" "kong-health"] "1m0s" "10s" "0s" '\n'}
# Wed, 09 Aug 2023 02:07:56 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac031e089cfc50c29a8e0c1b930f962823136a6f64ccc838271520e3f9d76077`  
		Last Modified: Wed, 09 Aug 2023 02:09:18 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add0c2c9ad20db3b0aaf9257f81154fcc276dfea6aeeab2a9fce583c19954a9f`  
		Last Modified: Wed, 09 Aug 2023 02:09:23 GMT  
		Size: 33.5 MB (33549840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b636a0e14f5af89549dce48e0656c5ffce44bdfb1995c8e03066226bb9fcf89`  
		Last Modified: Wed, 09 Aug 2023 02:09:18 GMT  
		Size: 1.2 KB (1157 bytes)  
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
$ docker pull kong@sha256:88aad0fa3c603af1b2ced86f33f0c28f664bf7b53c92aec1256746136b8832ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.3` - linux; amd64

```console
$ docker pull kong@sha256:42f6f9d446ef95ec15c5b923b427d1d388190873bed01acb629403a0c2beb900
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81309563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43e05bc78243dbb39affc720b41c1b6dc97c47b68399d685654f8564ba5083a3`
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
# Wed, 02 Aug 2023 23:20:11 GMT
ARG KONG_VERSION=3.3.1
# Wed, 02 Aug 2023 23:20:11 GMT
ENV KONG_VERSION=3.3.1
# Wed, 02 Aug 2023 23:20:11 GMT
ARG KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20
# Wed, 02 Aug 2023 23:20:12 GMT
ARG KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
# Wed, 02 Aug 2023 23:20:54 GMT
# ARGS: KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20 KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 02 Aug 2023 23:20:55 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Wed, 02 Aug 2023 23:20:55 GMT
USER kong
# Wed, 02 Aug 2023 23:20:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Aug 2023 23:20:55 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 02 Aug 2023 23:20:56 GMT
STOPSIGNAL SIGQUIT
# Wed, 02 Aug 2023 23:20:56 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 02 Aug 2023 23:20:56 GMT
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
	-	`sha256:4301c643ae4f3131c8c234c6df308c4a1c99774c6f5b2154e3220722bc7f9b80`  
		Last Modified: Wed, 02 Aug 2023 23:21:58 GMT  
		Size: 50.9 MB (50877055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4df5348ff8cc4eafe8037d9fe277c70fd1e6b53b748ef5c5b1e4b775b9171be2`  
		Last Modified: Wed, 02 Aug 2023 23:21:50 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.3` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:a8e1d2db1cb9b42a350e294d0fc4ddecd5efbf5d0866325a29e5fc1e21475a7d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75731094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1596ccb23ca7efed78b341971bd5298b5abd30766ca3fe3ed525494fb47f1a24`
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
# Wed, 02 Aug 2023 23:42:17 GMT
ARG KONG_VERSION=3.3.1
# Wed, 02 Aug 2023 23:42:17 GMT
ENV KONG_VERSION=3.3.1
# Wed, 02 Aug 2023 23:42:17 GMT
ARG KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20
# Wed, 02 Aug 2023 23:42:17 GMT
ARG KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
# Wed, 02 Aug 2023 23:43:09 GMT
# ARGS: KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20 KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 02 Aug 2023 23:43:10 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Wed, 02 Aug 2023 23:43:10 GMT
USER kong
# Wed, 02 Aug 2023 23:43:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Aug 2023 23:43:10 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 02 Aug 2023 23:43:10 GMT
STOPSIGNAL SIGQUIT
# Wed, 02 Aug 2023 23:43:10 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 02 Aug 2023 23:43:10 GMT
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
	-	`sha256:3bab189bfe11a0b3cde378bf325f026a1441ee41c576e1f18a0e5898cbb8971c`  
		Last Modified: Wed, 02 Aug 2023 23:43:44 GMT  
		Size: 47.3 MB (47338797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc59e46a8f641d2af00c285650418bde267ff3994e2cd0a837a58dddc2a6c8f3`  
		Last Modified: Wed, 02 Aug 2023 23:43:38 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.3-ubuntu`

```console
$ docker pull kong@sha256:88aad0fa3c603af1b2ced86f33f0c28f664bf7b53c92aec1256746136b8832ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.3-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:42f6f9d446ef95ec15c5b923b427d1d388190873bed01acb629403a0c2beb900
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81309563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43e05bc78243dbb39affc720b41c1b6dc97c47b68399d685654f8564ba5083a3`
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
# Wed, 02 Aug 2023 23:20:11 GMT
ARG KONG_VERSION=3.3.1
# Wed, 02 Aug 2023 23:20:11 GMT
ENV KONG_VERSION=3.3.1
# Wed, 02 Aug 2023 23:20:11 GMT
ARG KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20
# Wed, 02 Aug 2023 23:20:12 GMT
ARG KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
# Wed, 02 Aug 2023 23:20:54 GMT
# ARGS: KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20 KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 02 Aug 2023 23:20:55 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Wed, 02 Aug 2023 23:20:55 GMT
USER kong
# Wed, 02 Aug 2023 23:20:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Aug 2023 23:20:55 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 02 Aug 2023 23:20:56 GMT
STOPSIGNAL SIGQUIT
# Wed, 02 Aug 2023 23:20:56 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 02 Aug 2023 23:20:56 GMT
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
	-	`sha256:4301c643ae4f3131c8c234c6df308c4a1c99774c6f5b2154e3220722bc7f9b80`  
		Last Modified: Wed, 02 Aug 2023 23:21:58 GMT  
		Size: 50.9 MB (50877055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4df5348ff8cc4eafe8037d9fe277c70fd1e6b53b748ef5c5b1e4b775b9171be2`  
		Last Modified: Wed, 02 Aug 2023 23:21:50 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.3-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:a8e1d2db1cb9b42a350e294d0fc4ddecd5efbf5d0866325a29e5fc1e21475a7d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75731094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1596ccb23ca7efed78b341971bd5298b5abd30766ca3fe3ed525494fb47f1a24`
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
# Wed, 02 Aug 2023 23:42:17 GMT
ARG KONG_VERSION=3.3.1
# Wed, 02 Aug 2023 23:42:17 GMT
ENV KONG_VERSION=3.3.1
# Wed, 02 Aug 2023 23:42:17 GMT
ARG KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20
# Wed, 02 Aug 2023 23:42:17 GMT
ARG KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
# Wed, 02 Aug 2023 23:43:09 GMT
# ARGS: KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20 KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 02 Aug 2023 23:43:10 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Wed, 02 Aug 2023 23:43:10 GMT
USER kong
# Wed, 02 Aug 2023 23:43:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Aug 2023 23:43:10 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 02 Aug 2023 23:43:10 GMT
STOPSIGNAL SIGQUIT
# Wed, 02 Aug 2023 23:43:10 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 02 Aug 2023 23:43:10 GMT
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
	-	`sha256:3bab189bfe11a0b3cde378bf325f026a1441ee41c576e1f18a0e5898cbb8971c`  
		Last Modified: Wed, 02 Aug 2023 23:43:44 GMT  
		Size: 47.3 MB (47338797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc59e46a8f641d2af00c285650418bde267ff3994e2cd0a837a58dddc2a6c8f3`  
		Last Modified: Wed, 02 Aug 2023 23:43:38 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.3.1`

```console
$ docker pull kong@sha256:88aad0fa3c603af1b2ced86f33f0c28f664bf7b53c92aec1256746136b8832ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.3.1` - linux; amd64

```console
$ docker pull kong@sha256:42f6f9d446ef95ec15c5b923b427d1d388190873bed01acb629403a0c2beb900
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81309563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43e05bc78243dbb39affc720b41c1b6dc97c47b68399d685654f8564ba5083a3`
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
# Wed, 02 Aug 2023 23:20:11 GMT
ARG KONG_VERSION=3.3.1
# Wed, 02 Aug 2023 23:20:11 GMT
ENV KONG_VERSION=3.3.1
# Wed, 02 Aug 2023 23:20:11 GMT
ARG KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20
# Wed, 02 Aug 2023 23:20:12 GMT
ARG KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
# Wed, 02 Aug 2023 23:20:54 GMT
# ARGS: KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20 KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 02 Aug 2023 23:20:55 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Wed, 02 Aug 2023 23:20:55 GMT
USER kong
# Wed, 02 Aug 2023 23:20:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Aug 2023 23:20:55 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 02 Aug 2023 23:20:56 GMT
STOPSIGNAL SIGQUIT
# Wed, 02 Aug 2023 23:20:56 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 02 Aug 2023 23:20:56 GMT
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
	-	`sha256:4301c643ae4f3131c8c234c6df308c4a1c99774c6f5b2154e3220722bc7f9b80`  
		Last Modified: Wed, 02 Aug 2023 23:21:58 GMT  
		Size: 50.9 MB (50877055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4df5348ff8cc4eafe8037d9fe277c70fd1e6b53b748ef5c5b1e4b775b9171be2`  
		Last Modified: Wed, 02 Aug 2023 23:21:50 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.3.1` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:a8e1d2db1cb9b42a350e294d0fc4ddecd5efbf5d0866325a29e5fc1e21475a7d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75731094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1596ccb23ca7efed78b341971bd5298b5abd30766ca3fe3ed525494fb47f1a24`
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
# Wed, 02 Aug 2023 23:42:17 GMT
ARG KONG_VERSION=3.3.1
# Wed, 02 Aug 2023 23:42:17 GMT
ENV KONG_VERSION=3.3.1
# Wed, 02 Aug 2023 23:42:17 GMT
ARG KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20
# Wed, 02 Aug 2023 23:42:17 GMT
ARG KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
# Wed, 02 Aug 2023 23:43:09 GMT
# ARGS: KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20 KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 02 Aug 2023 23:43:10 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Wed, 02 Aug 2023 23:43:10 GMT
USER kong
# Wed, 02 Aug 2023 23:43:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Aug 2023 23:43:10 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 02 Aug 2023 23:43:10 GMT
STOPSIGNAL SIGQUIT
# Wed, 02 Aug 2023 23:43:10 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 02 Aug 2023 23:43:10 GMT
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
	-	`sha256:3bab189bfe11a0b3cde378bf325f026a1441ee41c576e1f18a0e5898cbb8971c`  
		Last Modified: Wed, 02 Aug 2023 23:43:44 GMT  
		Size: 47.3 MB (47338797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc59e46a8f641d2af00c285650418bde267ff3994e2cd0a837a58dddc2a6c8f3`  
		Last Modified: Wed, 02 Aug 2023 23:43:38 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.3.1-alpine`

```console
$ docker pull kong@sha256:84e39757dea0738ed81050c2d52b5d98d6586382c32595c432cff5301ffbbac0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:3.3.1-alpine` - linux; amd64

```console
$ docker pull kong@sha256:f251e0548826872b2977d49f65455cedf5bf26cf3ab4a7ea113bcafa80a9e1cf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.2 MB (34225566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a066a357a70793c9f3561ea9490bfcd395a0635ad5c71750c145b124b02a63d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 02:07:36 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 09 Aug 2023 02:07:36 GMT
ARG KONG_VERSION=3.3.1
# Wed, 09 Aug 2023 02:07:36 GMT
ENV KONG_VERSION=3.3.1
# Wed, 09 Aug 2023 02:07:36 GMT
ARG KONG_AMD64_SHA=b544aa8d23b544b7ec48e943e3525f6c1f33b202522020eedf91784c87de1a3d
# Wed, 09 Aug 2023 02:07:36 GMT
ARG KONG_PREFIX=/usr/local/kong
# Wed, 09 Aug 2023 02:07:37 GMT
ENV KONG_PREFIX=/usr/local/kong
# Wed, 09 Aug 2023 02:07:37 GMT
ARG ASSET=remote
# Wed, 09 Aug 2023 02:07:37 GMT
ARG EE_PORTS
# Wed, 09 Aug 2023 02:07:37 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Wed, 09 Aug 2023 02:07:43 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=b544aa8d23b544b7ec48e943e3525f6c1f33b202522020eedf91784c87de1a3d
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     export ARCH='amd64';     KONG_SHA256=$KONG_AMD64_SHA ;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc perl tzdata libcap zlib zlib-dev bash yaml     && adduser -S kong     && addgroup -S kong     && mkdir -p "${KONG_PREFIX}"     && chown -R kong:0 ${KONG_PREFIX}     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u ${KONG_PREFIX}     && rm -rf /tmp/kong.apk.tar.gz     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Wed, 09 Aug 2023 02:07:43 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Wed, 09 Aug 2023 02:07:43 GMT
USER kong
# Wed, 09 Aug 2023 02:07:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 09 Aug 2023 02:07:44 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 09 Aug 2023 02:07:44 GMT
STOPSIGNAL SIGQUIT
# Wed, 09 Aug 2023 02:07:44 GMT
HEALTHCHECK &{["CMD-SHELL" "kong-health"] "1m0s" "10s" "0s" '\n'}
# Wed, 09 Aug 2023 02:07:44 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1255030893ba24db289fb90abbbf0db2482a41f41d63e0e742d11c2b66b9f75f`  
		Last Modified: Wed, 09 Aug 2023 02:09:02 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9d7b8775e303a2ddeffbaeb418a75a3227a6485fdd05db647121f284fc40cd`  
		Last Modified: Wed, 09 Aug 2023 02:09:07 GMT  
		Size: 30.8 MB (30845666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8181721c61c00a352e943a8b43fabd74ce58d8ed240bed5f2afca92b56e1a503`  
		Last Modified: Wed, 09 Aug 2023 02:09:02 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.3.1-ubuntu`

```console
$ docker pull kong@sha256:88aad0fa3c603af1b2ced86f33f0c28f664bf7b53c92aec1256746136b8832ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.3.1-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:42f6f9d446ef95ec15c5b923b427d1d388190873bed01acb629403a0c2beb900
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81309563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43e05bc78243dbb39affc720b41c1b6dc97c47b68399d685654f8564ba5083a3`
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
# Wed, 02 Aug 2023 23:20:11 GMT
ARG KONG_VERSION=3.3.1
# Wed, 02 Aug 2023 23:20:11 GMT
ENV KONG_VERSION=3.3.1
# Wed, 02 Aug 2023 23:20:11 GMT
ARG KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20
# Wed, 02 Aug 2023 23:20:12 GMT
ARG KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
# Wed, 02 Aug 2023 23:20:54 GMT
# ARGS: KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20 KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 02 Aug 2023 23:20:55 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Wed, 02 Aug 2023 23:20:55 GMT
USER kong
# Wed, 02 Aug 2023 23:20:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Aug 2023 23:20:55 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 02 Aug 2023 23:20:56 GMT
STOPSIGNAL SIGQUIT
# Wed, 02 Aug 2023 23:20:56 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 02 Aug 2023 23:20:56 GMT
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
	-	`sha256:4301c643ae4f3131c8c234c6df308c4a1c99774c6f5b2154e3220722bc7f9b80`  
		Last Modified: Wed, 02 Aug 2023 23:21:58 GMT  
		Size: 50.9 MB (50877055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4df5348ff8cc4eafe8037d9fe277c70fd1e6b53b748ef5c5b1e4b775b9171be2`  
		Last Modified: Wed, 02 Aug 2023 23:21:50 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.3.1-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:a8e1d2db1cb9b42a350e294d0fc4ddecd5efbf5d0866325a29e5fc1e21475a7d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75731094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1596ccb23ca7efed78b341971bd5298b5abd30766ca3fe3ed525494fb47f1a24`
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
# Wed, 02 Aug 2023 23:42:17 GMT
ARG KONG_VERSION=3.3.1
# Wed, 02 Aug 2023 23:42:17 GMT
ENV KONG_VERSION=3.3.1
# Wed, 02 Aug 2023 23:42:17 GMT
ARG KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20
# Wed, 02 Aug 2023 23:42:17 GMT
ARG KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
# Wed, 02 Aug 2023 23:43:09 GMT
# ARGS: KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20 KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 02 Aug 2023 23:43:10 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Wed, 02 Aug 2023 23:43:10 GMT
USER kong
# Wed, 02 Aug 2023 23:43:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Aug 2023 23:43:10 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 02 Aug 2023 23:43:10 GMT
STOPSIGNAL SIGQUIT
# Wed, 02 Aug 2023 23:43:10 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 02 Aug 2023 23:43:10 GMT
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
	-	`sha256:3bab189bfe11a0b3cde378bf325f026a1441ee41c576e1f18a0e5898cbb8971c`  
		Last Modified: Wed, 02 Aug 2023 23:43:44 GMT  
		Size: 47.3 MB (47338797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc59e46a8f641d2af00c285650418bde267ff3994e2cd0a837a58dddc2a6c8f3`  
		Last Modified: Wed, 02 Aug 2023 23:43:38 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:alpine`

```console
$ docker pull kong@sha256:84e39757dea0738ed81050c2d52b5d98d6586382c32595c432cff5301ffbbac0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:alpine` - linux; amd64

```console
$ docker pull kong@sha256:f251e0548826872b2977d49f65455cedf5bf26cf3ab4a7ea113bcafa80a9e1cf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.2 MB (34225566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a066a357a70793c9f3561ea9490bfcd395a0635ad5c71750c145b124b02a63d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 02:07:36 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 09 Aug 2023 02:07:36 GMT
ARG KONG_VERSION=3.3.1
# Wed, 09 Aug 2023 02:07:36 GMT
ENV KONG_VERSION=3.3.1
# Wed, 09 Aug 2023 02:07:36 GMT
ARG KONG_AMD64_SHA=b544aa8d23b544b7ec48e943e3525f6c1f33b202522020eedf91784c87de1a3d
# Wed, 09 Aug 2023 02:07:36 GMT
ARG KONG_PREFIX=/usr/local/kong
# Wed, 09 Aug 2023 02:07:37 GMT
ENV KONG_PREFIX=/usr/local/kong
# Wed, 09 Aug 2023 02:07:37 GMT
ARG ASSET=remote
# Wed, 09 Aug 2023 02:07:37 GMT
ARG EE_PORTS
# Wed, 09 Aug 2023 02:07:37 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Wed, 09 Aug 2023 02:07:43 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=b544aa8d23b544b7ec48e943e3525f6c1f33b202522020eedf91784c87de1a3d
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     export ARCH='amd64';     KONG_SHA256=$KONG_AMD64_SHA ;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc perl tzdata libcap zlib zlib-dev bash yaml     && adduser -S kong     && addgroup -S kong     && mkdir -p "${KONG_PREFIX}"     && chown -R kong:0 ${KONG_PREFIX}     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u ${KONG_PREFIX}     && rm -rf /tmp/kong.apk.tar.gz     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Wed, 09 Aug 2023 02:07:43 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Wed, 09 Aug 2023 02:07:43 GMT
USER kong
# Wed, 09 Aug 2023 02:07:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 09 Aug 2023 02:07:44 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 09 Aug 2023 02:07:44 GMT
STOPSIGNAL SIGQUIT
# Wed, 09 Aug 2023 02:07:44 GMT
HEALTHCHECK &{["CMD-SHELL" "kong-health"] "1m0s" "10s" "0s" '\n'}
# Wed, 09 Aug 2023 02:07:44 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1255030893ba24db289fb90abbbf0db2482a41f41d63e0e742d11c2b66b9f75f`  
		Last Modified: Wed, 09 Aug 2023 02:09:02 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9d7b8775e303a2ddeffbaeb418a75a3227a6485fdd05db647121f284fc40cd`  
		Last Modified: Wed, 09 Aug 2023 02:09:07 GMT  
		Size: 30.8 MB (30845666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8181721c61c00a352e943a8b43fabd74ce58d8ed240bed5f2afca92b56e1a503`  
		Last Modified: Wed, 09 Aug 2023 02:09:02 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:latest`

```console
$ docker pull kong@sha256:88aad0fa3c603af1b2ced86f33f0c28f664bf7b53c92aec1256746136b8832ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:latest` - linux; amd64

```console
$ docker pull kong@sha256:42f6f9d446ef95ec15c5b923b427d1d388190873bed01acb629403a0c2beb900
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81309563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43e05bc78243dbb39affc720b41c1b6dc97c47b68399d685654f8564ba5083a3`
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
# Wed, 02 Aug 2023 23:20:11 GMT
ARG KONG_VERSION=3.3.1
# Wed, 02 Aug 2023 23:20:11 GMT
ENV KONG_VERSION=3.3.1
# Wed, 02 Aug 2023 23:20:11 GMT
ARG KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20
# Wed, 02 Aug 2023 23:20:12 GMT
ARG KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
# Wed, 02 Aug 2023 23:20:54 GMT
# ARGS: KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20 KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 02 Aug 2023 23:20:55 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Wed, 02 Aug 2023 23:20:55 GMT
USER kong
# Wed, 02 Aug 2023 23:20:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Aug 2023 23:20:55 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 02 Aug 2023 23:20:56 GMT
STOPSIGNAL SIGQUIT
# Wed, 02 Aug 2023 23:20:56 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 02 Aug 2023 23:20:56 GMT
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
	-	`sha256:4301c643ae4f3131c8c234c6df308c4a1c99774c6f5b2154e3220722bc7f9b80`  
		Last Modified: Wed, 02 Aug 2023 23:21:58 GMT  
		Size: 50.9 MB (50877055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4df5348ff8cc4eafe8037d9fe277c70fd1e6b53b748ef5c5b1e4b775b9171be2`  
		Last Modified: Wed, 02 Aug 2023 23:21:50 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:latest` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:a8e1d2db1cb9b42a350e294d0fc4ddecd5efbf5d0866325a29e5fc1e21475a7d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75731094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1596ccb23ca7efed78b341971bd5298b5abd30766ca3fe3ed525494fb47f1a24`
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
# Wed, 02 Aug 2023 23:42:17 GMT
ARG KONG_VERSION=3.3.1
# Wed, 02 Aug 2023 23:42:17 GMT
ENV KONG_VERSION=3.3.1
# Wed, 02 Aug 2023 23:42:17 GMT
ARG KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20
# Wed, 02 Aug 2023 23:42:17 GMT
ARG KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
# Wed, 02 Aug 2023 23:43:09 GMT
# ARGS: KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20 KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 02 Aug 2023 23:43:10 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Wed, 02 Aug 2023 23:43:10 GMT
USER kong
# Wed, 02 Aug 2023 23:43:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Aug 2023 23:43:10 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 02 Aug 2023 23:43:10 GMT
STOPSIGNAL SIGQUIT
# Wed, 02 Aug 2023 23:43:10 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 02 Aug 2023 23:43:10 GMT
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
	-	`sha256:3bab189bfe11a0b3cde378bf325f026a1441ee41c576e1f18a0e5898cbb8971c`  
		Last Modified: Wed, 02 Aug 2023 23:43:44 GMT  
		Size: 47.3 MB (47338797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc59e46a8f641d2af00c285650418bde267ff3994e2cd0a837a58dddc2a6c8f3`  
		Last Modified: Wed, 02 Aug 2023 23:43:38 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:ubuntu`

```console
$ docker pull kong@sha256:88aad0fa3c603af1b2ced86f33f0c28f664bf7b53c92aec1256746136b8832ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:42f6f9d446ef95ec15c5b923b427d1d388190873bed01acb629403a0c2beb900
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81309563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43e05bc78243dbb39affc720b41c1b6dc97c47b68399d685654f8564ba5083a3`
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
# Wed, 02 Aug 2023 23:20:11 GMT
ARG KONG_VERSION=3.3.1
# Wed, 02 Aug 2023 23:20:11 GMT
ENV KONG_VERSION=3.3.1
# Wed, 02 Aug 2023 23:20:11 GMT
ARG KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20
# Wed, 02 Aug 2023 23:20:12 GMT
ARG KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
# Wed, 02 Aug 2023 23:20:54 GMT
# ARGS: KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20 KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 02 Aug 2023 23:20:55 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Wed, 02 Aug 2023 23:20:55 GMT
USER kong
# Wed, 02 Aug 2023 23:20:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Aug 2023 23:20:55 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 02 Aug 2023 23:20:56 GMT
STOPSIGNAL SIGQUIT
# Wed, 02 Aug 2023 23:20:56 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 02 Aug 2023 23:20:56 GMT
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
	-	`sha256:4301c643ae4f3131c8c234c6df308c4a1c99774c6f5b2154e3220722bc7f9b80`  
		Last Modified: Wed, 02 Aug 2023 23:21:58 GMT  
		Size: 50.9 MB (50877055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4df5348ff8cc4eafe8037d9fe277c70fd1e6b53b748ef5c5b1e4b775b9171be2`  
		Last Modified: Wed, 02 Aug 2023 23:21:50 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:a8e1d2db1cb9b42a350e294d0fc4ddecd5efbf5d0866325a29e5fc1e21475a7d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75731094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1596ccb23ca7efed78b341971bd5298b5abd30766ca3fe3ed525494fb47f1a24`
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
# Wed, 02 Aug 2023 23:42:17 GMT
ARG KONG_VERSION=3.3.1
# Wed, 02 Aug 2023 23:42:17 GMT
ENV KONG_VERSION=3.3.1
# Wed, 02 Aug 2023 23:42:17 GMT
ARG KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20
# Wed, 02 Aug 2023 23:42:17 GMT
ARG KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
# Wed, 02 Aug 2023 23:43:09 GMT
# ARGS: KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20 KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 02 Aug 2023 23:43:10 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Wed, 02 Aug 2023 23:43:10 GMT
USER kong
# Wed, 02 Aug 2023 23:43:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Aug 2023 23:43:10 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 02 Aug 2023 23:43:10 GMT
STOPSIGNAL SIGQUIT
# Wed, 02 Aug 2023 23:43:10 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 02 Aug 2023 23:43:10 GMT
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
	-	`sha256:3bab189bfe11a0b3cde378bf325f026a1441ee41c576e1f18a0e5898cbb8971c`  
		Last Modified: Wed, 02 Aug 2023 23:43:44 GMT  
		Size: 47.3 MB (47338797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc59e46a8f641d2af00c285650418bde267ff3994e2cd0a837a58dddc2a6c8f3`  
		Last Modified: Wed, 02 Aug 2023 23:43:38 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
