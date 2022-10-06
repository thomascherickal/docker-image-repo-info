<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kong`

-	[`kong:2.5`](#kong25)
-	[`kong:2.5-ubuntu`](#kong25-ubuntu)
-	[`kong:2.5.2`](#kong252)
-	[`kong:2.5.2-alpine`](#kong252-alpine)
-	[`kong:2.5.2-ubuntu`](#kong252-ubuntu)
-	[`kong:2.6`](#kong26)
-	[`kong:2.6-ubuntu`](#kong26-ubuntu)
-	[`kong:2.6.1`](#kong261)
-	[`kong:2.6.1-alpine`](#kong261-alpine)
-	[`kong:2.6.1-ubuntu`](#kong261-ubuntu)
-	[`kong:2.7`](#kong27)
-	[`kong:2.7-ubuntu`](#kong27-ubuntu)
-	[`kong:2.7.2`](#kong272)
-	[`kong:2.7.2-alpine`](#kong272-alpine)
-	[`kong:2.7.2-ubuntu`](#kong272-ubuntu)
-	[`kong:2.8`](#kong28)
-	[`kong:2.8-ubuntu`](#kong28-ubuntu)
-	[`kong:2.8.1`](#kong281)
-	[`kong:2.8.1-alpine`](#kong281-alpine)
-	[`kong:2.8.1-ubuntu`](#kong281-ubuntu)
-	[`kong:3.0`](#kong30)
-	[`kong:3.0-ubuntu`](#kong30-ubuntu)
-	[`kong:3.0.0`](#kong300)
-	[`kong:3.0.0-alpine`](#kong300-alpine)
-	[`kong:3.0.0-ubuntu`](#kong300-ubuntu)
-	[`kong:alpine`](#kongalpine)
-	[`kong:latest`](#konglatest)
-	[`kong:ubuntu`](#kongubuntu)

## `kong:2.5`

```console
$ docker pull kong@sha256:260dca99ebf93758f5495afa0b108875069f2a00170bad30ed1c96849a54d10f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.5` - linux; amd64

```console
$ docker pull kong@sha256:05289c41fbd1aca217f6db0d25fbb2865b062e209743ac04119daea13015654f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49212370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53b83ca7b49ebd6c41ab1dd1eff15083f2ce7cc7ce42ae1da19a4e13e02ee035`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 23:01:23 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 06 Oct 2022 23:01:23 GMT
ARG ASSET=ce
# Thu, 06 Oct 2022 23:01:23 GMT
ENV ASSET=ce
# Thu, 06 Oct 2022 23:01:23 GMT
ARG EE_PORTS
# Thu, 06 Oct 2022 23:01:23 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 06 Oct 2022 23:01:50 GMT
ARG KONG_VERSION=2.5.2
# Thu, 06 Oct 2022 23:01:50 GMT
ENV KONG_VERSION=2.5.2
# Thu, 06 Oct 2022 23:01:50 GMT
ARG KONG_AMD64_SHA=d4bc93bcb14cce8c37ced136632a290b441050c540db779e742bcd88e5cfd70d
# Thu, 06 Oct 2022 23:01:50 GMT
ARG KONG_ARM64_SHA=691e1dc29e96d6a95b60674513932c4f7547773014685ce0130549f980c1c46e
# Thu, 06 Oct 2022 23:01:57 GMT
# ARGS: KONG_AMD64_SHA=d4bc93bcb14cce8c37ced136632a290b441050c540db779e742bcd88e5cfd70d KONG_ARM64_SHA=691e1dc29e96d6a95b60674513932c4f7547773014685ce0130549f980c1c46e
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 06 Oct 2022 23:01:58 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 06 Oct 2022 23:01:58 GMT
USER kong
# Thu, 06 Oct 2022 23:01:58 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Oct 2022 23:01:58 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 06 Oct 2022 23:01:58 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Oct 2022 23:01:58 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 06 Oct 2022 23:01:58 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29712f9007996b849b4ca5751d9caac52946d8e35200fe77a0e58b376287bbbd`  
		Last Modified: Thu, 06 Oct 2022 23:03:14 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669c28460b5bfedf1255235b6e1a6b33b6be4927235fd60cb1e16bd6a0ff29f9`  
		Last Modified: Thu, 06 Oct 2022 23:04:02 GMT  
		Size: 46.4 MB (46387849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b879cb95f5a94f57e19a2f23ee6511900441e380da40ee1c2ace9ded3136ee4f`  
		Last Modified: Thu, 06 Oct 2022 23:03:54 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.5` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:bc7a5e4fe0db2842373c4db51e061bd5e1b7ed86b70ccb4a7ce7d50fa1a667ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.4 MB (48411983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbf73c9f8e850e136aa9461c18f0b55418d4f95223abf6529ada186dc6351603`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 22:25:07 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 06 Oct 2022 22:25:07 GMT
ARG ASSET=ce
# Thu, 06 Oct 2022 22:25:08 GMT
ENV ASSET=ce
# Thu, 06 Oct 2022 22:25:09 GMT
ARG EE_PORTS
# Thu, 06 Oct 2022 22:25:11 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 06 Oct 2022 22:26:05 GMT
ARG KONG_VERSION=2.5.2
# Thu, 06 Oct 2022 22:26:06 GMT
ENV KONG_VERSION=2.5.2
# Thu, 06 Oct 2022 22:26:07 GMT
ARG KONG_AMD64_SHA=d4bc93bcb14cce8c37ced136632a290b441050c540db779e742bcd88e5cfd70d
# Thu, 06 Oct 2022 22:26:08 GMT
ARG KONG_ARM64_SHA=691e1dc29e96d6a95b60674513932c4f7547773014685ce0130549f980c1c46e
# Thu, 06 Oct 2022 22:26:33 GMT
# ARGS: KONG_AMD64_SHA=d4bc93bcb14cce8c37ced136632a290b441050c540db779e742bcd88e5cfd70d KONG_ARM64_SHA=691e1dc29e96d6a95b60674513932c4f7547773014685ce0130549f980c1c46e
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 06 Oct 2022 22:26:34 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 06 Oct 2022 22:26:34 GMT
USER kong
# Thu, 06 Oct 2022 22:26:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Oct 2022 22:26:36 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 06 Oct 2022 22:26:37 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Oct 2022 22:26:38 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 06 Oct 2022 22:26:39 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be38426b84d987a4cd0ee5faa0e7209d36689d721c007c605f5d82a9b874ab1`  
		Last Modified: Thu, 06 Oct 2022 22:28:36 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c3d9bb0728f99d45cea6475b191d1c9b47443a4e63933097953bfb84e6ae989`  
		Last Modified: Thu, 06 Oct 2022 22:29:32 GMT  
		Size: 45.7 MB (45692531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf1b0d68fbf1491a23a82146ffea1bcf67111e738d7f4e492065b8d9c266abd`  
		Last Modified: Thu, 06 Oct 2022 22:29:24 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.5-ubuntu`

```console
$ docker pull kong@sha256:7e94157233cb982e62211e4fd8b53994057d8dcfcc7dc27ad9b0f1a27b3f363a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.5-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:e632ff086a0398c2e689ad15179a4c1a21a52bf97eae02e9cbe9bcbc8bc41453
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121373747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12bc344365a9680adcc5a9b5f47c0fa586d0277ce2dcf80b2c63ee0c015530c6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 18:04:26 GMT
ARG ASSET=ce
# Wed, 05 Oct 2022 18:04:26 GMT
ENV ASSET=ce
# Wed, 05 Oct 2022 18:04:26 GMT
ARG EE_PORTS
# Wed, 05 Oct 2022 18:04:26 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 05 Oct 2022 18:05:56 GMT
ARG KONG_VERSION=2.5.2
# Wed, 05 Oct 2022 18:05:56 GMT
ENV KONG_VERSION=2.5.2
# Wed, 05 Oct 2022 18:05:56 GMT
ARG KONG_AMD64_SHA=ae65ac9eb35f682768abfb080c61581440347db8dafd0a495639ff666a406a96
# Wed, 05 Oct 2022 18:05:56 GMT
ARG KONG_ARM64_SHA=b4720e3d0831d13364cc749200c77df356a2145478f6a55fd48618a9aa1967d9
# Wed, 05 Oct 2022 18:06:17 GMT
# ARGS: KONG_AMD64_SHA=ae65ac9eb35f682768abfb080c61581440347db8dafd0a495639ff666a406a96 KONG_ARM64_SHA=b4720e3d0831d13364cc749200c77df356a2145478f6a55fd48618a9aa1967d9
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 05 Oct 2022 18:06:18 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 05 Oct 2022 18:06:18 GMT
USER kong
# Wed, 05 Oct 2022 18:06:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 18:06:19 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 05 Oct 2022 18:06:19 GMT
STOPSIGNAL SIGQUIT
# Wed, 05 Oct 2022 18:06:19 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 05 Oct 2022 18:06:19 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af493d1a174862c166e0d67b32f1bb9d93e2304a59209a55e08cd858d032d8b`  
		Last Modified: Wed, 05 Oct 2022 18:07:23 GMT  
		Size: 25.1 MB (25081963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feafaa2914aeeed8aa4de482bc243e365ed0f4ed3e2fbae0768c8a361cb9754c`  
		Last Modified: Wed, 05 Oct 2022 18:08:48 GMT  
		Size: 67.7 MB (67716453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a07f475cc0994afcdbe19a018a9413c11861f5a8e22c3cb7d88a87b158083ef`  
		Last Modified: Wed, 05 Oct 2022 18:08:36 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.5-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:e28154aea3d28adb56e330635c326316b54b2f2ac5e22d110b1172949b711196
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118404412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:412dd6500807518ad61eb53f7f67b3438a9986e525b6e88d8e817438e8aae3d6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:00:20 GMT
ARG ASSET=ce
# Wed, 05 Oct 2022 16:00:20 GMT
ENV ASSET=ce
# Wed, 05 Oct 2022 16:00:21 GMT
ARG EE_PORTS
# Wed, 05 Oct 2022 16:00:23 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 05 Oct 2022 16:03:17 GMT
ARG KONG_VERSION=2.5.2
# Wed, 05 Oct 2022 16:03:18 GMT
ENV KONG_VERSION=2.5.2
# Wed, 05 Oct 2022 16:03:19 GMT
ARG KONG_AMD64_SHA=ae65ac9eb35f682768abfb080c61581440347db8dafd0a495639ff666a406a96
# Wed, 05 Oct 2022 16:03:20 GMT
ARG KONG_ARM64_SHA=b4720e3d0831d13364cc749200c77df356a2145478f6a55fd48618a9aa1967d9
# Wed, 05 Oct 2022 16:03:48 GMT
# ARGS: KONG_AMD64_SHA=ae65ac9eb35f682768abfb080c61581440347db8dafd0a495639ff666a406a96 KONG_ARM64_SHA=b4720e3d0831d13364cc749200c77df356a2145478f6a55fd48618a9aa1967d9
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 05 Oct 2022 16:03:50 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 05 Oct 2022 16:03:50 GMT
USER kong
# Wed, 05 Oct 2022 16:03:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 16:03:52 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 05 Oct 2022 16:03:53 GMT
STOPSIGNAL SIGQUIT
# Wed, 05 Oct 2022 16:03:54 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 05 Oct 2022 16:03:55 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f20e2ab08e0103d6be14c1b3d377ca9e5f15a0a1256d9621c287546c1b9f4de`  
		Last Modified: Wed, 05 Oct 2022 16:05:25 GMT  
		Size: 25.1 MB (25081964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c4103eb0376b976fac8b1121dc604af20917888625ae4e224e466f81fa68336`  
		Last Modified: Wed, 05 Oct 2022 16:06:49 GMT  
		Size: 66.1 MB (66129945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6b39b4604dfdcc6c6ceb5bc14d7771450cf8cf6e23a18fcb97c51ab33ce1af`  
		Last Modified: Wed, 05 Oct 2022 16:06:38 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.5.2`

```console
$ docker pull kong@sha256:260dca99ebf93758f5495afa0b108875069f2a00170bad30ed1c96849a54d10f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.5.2` - linux; amd64

```console
$ docker pull kong@sha256:05289c41fbd1aca217f6db0d25fbb2865b062e209743ac04119daea13015654f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49212370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53b83ca7b49ebd6c41ab1dd1eff15083f2ce7cc7ce42ae1da19a4e13e02ee035`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 23:01:23 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 06 Oct 2022 23:01:23 GMT
ARG ASSET=ce
# Thu, 06 Oct 2022 23:01:23 GMT
ENV ASSET=ce
# Thu, 06 Oct 2022 23:01:23 GMT
ARG EE_PORTS
# Thu, 06 Oct 2022 23:01:23 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 06 Oct 2022 23:01:50 GMT
ARG KONG_VERSION=2.5.2
# Thu, 06 Oct 2022 23:01:50 GMT
ENV KONG_VERSION=2.5.2
# Thu, 06 Oct 2022 23:01:50 GMT
ARG KONG_AMD64_SHA=d4bc93bcb14cce8c37ced136632a290b441050c540db779e742bcd88e5cfd70d
# Thu, 06 Oct 2022 23:01:50 GMT
ARG KONG_ARM64_SHA=691e1dc29e96d6a95b60674513932c4f7547773014685ce0130549f980c1c46e
# Thu, 06 Oct 2022 23:01:57 GMT
# ARGS: KONG_AMD64_SHA=d4bc93bcb14cce8c37ced136632a290b441050c540db779e742bcd88e5cfd70d KONG_ARM64_SHA=691e1dc29e96d6a95b60674513932c4f7547773014685ce0130549f980c1c46e
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 06 Oct 2022 23:01:58 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 06 Oct 2022 23:01:58 GMT
USER kong
# Thu, 06 Oct 2022 23:01:58 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Oct 2022 23:01:58 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 06 Oct 2022 23:01:58 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Oct 2022 23:01:58 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 06 Oct 2022 23:01:58 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29712f9007996b849b4ca5751d9caac52946d8e35200fe77a0e58b376287bbbd`  
		Last Modified: Thu, 06 Oct 2022 23:03:14 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669c28460b5bfedf1255235b6e1a6b33b6be4927235fd60cb1e16bd6a0ff29f9`  
		Last Modified: Thu, 06 Oct 2022 23:04:02 GMT  
		Size: 46.4 MB (46387849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b879cb95f5a94f57e19a2f23ee6511900441e380da40ee1c2ace9ded3136ee4f`  
		Last Modified: Thu, 06 Oct 2022 23:03:54 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.5.2` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:bc7a5e4fe0db2842373c4db51e061bd5e1b7ed86b70ccb4a7ce7d50fa1a667ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.4 MB (48411983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbf73c9f8e850e136aa9461c18f0b55418d4f95223abf6529ada186dc6351603`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 22:25:07 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 06 Oct 2022 22:25:07 GMT
ARG ASSET=ce
# Thu, 06 Oct 2022 22:25:08 GMT
ENV ASSET=ce
# Thu, 06 Oct 2022 22:25:09 GMT
ARG EE_PORTS
# Thu, 06 Oct 2022 22:25:11 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 06 Oct 2022 22:26:05 GMT
ARG KONG_VERSION=2.5.2
# Thu, 06 Oct 2022 22:26:06 GMT
ENV KONG_VERSION=2.5.2
# Thu, 06 Oct 2022 22:26:07 GMT
ARG KONG_AMD64_SHA=d4bc93bcb14cce8c37ced136632a290b441050c540db779e742bcd88e5cfd70d
# Thu, 06 Oct 2022 22:26:08 GMT
ARG KONG_ARM64_SHA=691e1dc29e96d6a95b60674513932c4f7547773014685ce0130549f980c1c46e
# Thu, 06 Oct 2022 22:26:33 GMT
# ARGS: KONG_AMD64_SHA=d4bc93bcb14cce8c37ced136632a290b441050c540db779e742bcd88e5cfd70d KONG_ARM64_SHA=691e1dc29e96d6a95b60674513932c4f7547773014685ce0130549f980c1c46e
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 06 Oct 2022 22:26:34 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 06 Oct 2022 22:26:34 GMT
USER kong
# Thu, 06 Oct 2022 22:26:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Oct 2022 22:26:36 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 06 Oct 2022 22:26:37 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Oct 2022 22:26:38 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 06 Oct 2022 22:26:39 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be38426b84d987a4cd0ee5faa0e7209d36689d721c007c605f5d82a9b874ab1`  
		Last Modified: Thu, 06 Oct 2022 22:28:36 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c3d9bb0728f99d45cea6475b191d1c9b47443a4e63933097953bfb84e6ae989`  
		Last Modified: Thu, 06 Oct 2022 22:29:32 GMT  
		Size: 45.7 MB (45692531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf1b0d68fbf1491a23a82146ffea1bcf67111e738d7f4e492065b8d9c266abd`  
		Last Modified: Thu, 06 Oct 2022 22:29:24 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.5.2-alpine`

```console
$ docker pull kong@sha256:260dca99ebf93758f5495afa0b108875069f2a00170bad30ed1c96849a54d10f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.5.2-alpine` - linux; amd64

```console
$ docker pull kong@sha256:05289c41fbd1aca217f6db0d25fbb2865b062e209743ac04119daea13015654f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49212370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53b83ca7b49ebd6c41ab1dd1eff15083f2ce7cc7ce42ae1da19a4e13e02ee035`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 23:01:23 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 06 Oct 2022 23:01:23 GMT
ARG ASSET=ce
# Thu, 06 Oct 2022 23:01:23 GMT
ENV ASSET=ce
# Thu, 06 Oct 2022 23:01:23 GMT
ARG EE_PORTS
# Thu, 06 Oct 2022 23:01:23 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 06 Oct 2022 23:01:50 GMT
ARG KONG_VERSION=2.5.2
# Thu, 06 Oct 2022 23:01:50 GMT
ENV KONG_VERSION=2.5.2
# Thu, 06 Oct 2022 23:01:50 GMT
ARG KONG_AMD64_SHA=d4bc93bcb14cce8c37ced136632a290b441050c540db779e742bcd88e5cfd70d
# Thu, 06 Oct 2022 23:01:50 GMT
ARG KONG_ARM64_SHA=691e1dc29e96d6a95b60674513932c4f7547773014685ce0130549f980c1c46e
# Thu, 06 Oct 2022 23:01:57 GMT
# ARGS: KONG_AMD64_SHA=d4bc93bcb14cce8c37ced136632a290b441050c540db779e742bcd88e5cfd70d KONG_ARM64_SHA=691e1dc29e96d6a95b60674513932c4f7547773014685ce0130549f980c1c46e
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 06 Oct 2022 23:01:58 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 06 Oct 2022 23:01:58 GMT
USER kong
# Thu, 06 Oct 2022 23:01:58 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Oct 2022 23:01:58 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 06 Oct 2022 23:01:58 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Oct 2022 23:01:58 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 06 Oct 2022 23:01:58 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29712f9007996b849b4ca5751d9caac52946d8e35200fe77a0e58b376287bbbd`  
		Last Modified: Thu, 06 Oct 2022 23:03:14 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669c28460b5bfedf1255235b6e1a6b33b6be4927235fd60cb1e16bd6a0ff29f9`  
		Last Modified: Thu, 06 Oct 2022 23:04:02 GMT  
		Size: 46.4 MB (46387849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b879cb95f5a94f57e19a2f23ee6511900441e380da40ee1c2ace9ded3136ee4f`  
		Last Modified: Thu, 06 Oct 2022 23:03:54 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.5.2-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:bc7a5e4fe0db2842373c4db51e061bd5e1b7ed86b70ccb4a7ce7d50fa1a667ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.4 MB (48411983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbf73c9f8e850e136aa9461c18f0b55418d4f95223abf6529ada186dc6351603`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 22:25:07 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 06 Oct 2022 22:25:07 GMT
ARG ASSET=ce
# Thu, 06 Oct 2022 22:25:08 GMT
ENV ASSET=ce
# Thu, 06 Oct 2022 22:25:09 GMT
ARG EE_PORTS
# Thu, 06 Oct 2022 22:25:11 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 06 Oct 2022 22:26:05 GMT
ARG KONG_VERSION=2.5.2
# Thu, 06 Oct 2022 22:26:06 GMT
ENV KONG_VERSION=2.5.2
# Thu, 06 Oct 2022 22:26:07 GMT
ARG KONG_AMD64_SHA=d4bc93bcb14cce8c37ced136632a290b441050c540db779e742bcd88e5cfd70d
# Thu, 06 Oct 2022 22:26:08 GMT
ARG KONG_ARM64_SHA=691e1dc29e96d6a95b60674513932c4f7547773014685ce0130549f980c1c46e
# Thu, 06 Oct 2022 22:26:33 GMT
# ARGS: KONG_AMD64_SHA=d4bc93bcb14cce8c37ced136632a290b441050c540db779e742bcd88e5cfd70d KONG_ARM64_SHA=691e1dc29e96d6a95b60674513932c4f7547773014685ce0130549f980c1c46e
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 06 Oct 2022 22:26:34 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 06 Oct 2022 22:26:34 GMT
USER kong
# Thu, 06 Oct 2022 22:26:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Oct 2022 22:26:36 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 06 Oct 2022 22:26:37 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Oct 2022 22:26:38 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 06 Oct 2022 22:26:39 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be38426b84d987a4cd0ee5faa0e7209d36689d721c007c605f5d82a9b874ab1`  
		Last Modified: Thu, 06 Oct 2022 22:28:36 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c3d9bb0728f99d45cea6475b191d1c9b47443a4e63933097953bfb84e6ae989`  
		Last Modified: Thu, 06 Oct 2022 22:29:32 GMT  
		Size: 45.7 MB (45692531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf1b0d68fbf1491a23a82146ffea1bcf67111e738d7f4e492065b8d9c266abd`  
		Last Modified: Thu, 06 Oct 2022 22:29:24 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.5.2-ubuntu`

```console
$ docker pull kong@sha256:7e94157233cb982e62211e4fd8b53994057d8dcfcc7dc27ad9b0f1a27b3f363a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.5.2-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:e632ff086a0398c2e689ad15179a4c1a21a52bf97eae02e9cbe9bcbc8bc41453
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121373747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12bc344365a9680adcc5a9b5f47c0fa586d0277ce2dcf80b2c63ee0c015530c6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 18:04:26 GMT
ARG ASSET=ce
# Wed, 05 Oct 2022 18:04:26 GMT
ENV ASSET=ce
# Wed, 05 Oct 2022 18:04:26 GMT
ARG EE_PORTS
# Wed, 05 Oct 2022 18:04:26 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 05 Oct 2022 18:05:56 GMT
ARG KONG_VERSION=2.5.2
# Wed, 05 Oct 2022 18:05:56 GMT
ENV KONG_VERSION=2.5.2
# Wed, 05 Oct 2022 18:05:56 GMT
ARG KONG_AMD64_SHA=ae65ac9eb35f682768abfb080c61581440347db8dafd0a495639ff666a406a96
# Wed, 05 Oct 2022 18:05:56 GMT
ARG KONG_ARM64_SHA=b4720e3d0831d13364cc749200c77df356a2145478f6a55fd48618a9aa1967d9
# Wed, 05 Oct 2022 18:06:17 GMT
# ARGS: KONG_AMD64_SHA=ae65ac9eb35f682768abfb080c61581440347db8dafd0a495639ff666a406a96 KONG_ARM64_SHA=b4720e3d0831d13364cc749200c77df356a2145478f6a55fd48618a9aa1967d9
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 05 Oct 2022 18:06:18 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 05 Oct 2022 18:06:18 GMT
USER kong
# Wed, 05 Oct 2022 18:06:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 18:06:19 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 05 Oct 2022 18:06:19 GMT
STOPSIGNAL SIGQUIT
# Wed, 05 Oct 2022 18:06:19 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 05 Oct 2022 18:06:19 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af493d1a174862c166e0d67b32f1bb9d93e2304a59209a55e08cd858d032d8b`  
		Last Modified: Wed, 05 Oct 2022 18:07:23 GMT  
		Size: 25.1 MB (25081963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feafaa2914aeeed8aa4de482bc243e365ed0f4ed3e2fbae0768c8a361cb9754c`  
		Last Modified: Wed, 05 Oct 2022 18:08:48 GMT  
		Size: 67.7 MB (67716453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a07f475cc0994afcdbe19a018a9413c11861f5a8e22c3cb7d88a87b158083ef`  
		Last Modified: Wed, 05 Oct 2022 18:08:36 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.5.2-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:e28154aea3d28adb56e330635c326316b54b2f2ac5e22d110b1172949b711196
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118404412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:412dd6500807518ad61eb53f7f67b3438a9986e525b6e88d8e817438e8aae3d6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:00:20 GMT
ARG ASSET=ce
# Wed, 05 Oct 2022 16:00:20 GMT
ENV ASSET=ce
# Wed, 05 Oct 2022 16:00:21 GMT
ARG EE_PORTS
# Wed, 05 Oct 2022 16:00:23 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 05 Oct 2022 16:03:17 GMT
ARG KONG_VERSION=2.5.2
# Wed, 05 Oct 2022 16:03:18 GMT
ENV KONG_VERSION=2.5.2
# Wed, 05 Oct 2022 16:03:19 GMT
ARG KONG_AMD64_SHA=ae65ac9eb35f682768abfb080c61581440347db8dafd0a495639ff666a406a96
# Wed, 05 Oct 2022 16:03:20 GMT
ARG KONG_ARM64_SHA=b4720e3d0831d13364cc749200c77df356a2145478f6a55fd48618a9aa1967d9
# Wed, 05 Oct 2022 16:03:48 GMT
# ARGS: KONG_AMD64_SHA=ae65ac9eb35f682768abfb080c61581440347db8dafd0a495639ff666a406a96 KONG_ARM64_SHA=b4720e3d0831d13364cc749200c77df356a2145478f6a55fd48618a9aa1967d9
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 05 Oct 2022 16:03:50 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 05 Oct 2022 16:03:50 GMT
USER kong
# Wed, 05 Oct 2022 16:03:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 16:03:52 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 05 Oct 2022 16:03:53 GMT
STOPSIGNAL SIGQUIT
# Wed, 05 Oct 2022 16:03:54 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 05 Oct 2022 16:03:55 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f20e2ab08e0103d6be14c1b3d377ca9e5f15a0a1256d9621c287546c1b9f4de`  
		Last Modified: Wed, 05 Oct 2022 16:05:25 GMT  
		Size: 25.1 MB (25081964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c4103eb0376b976fac8b1121dc604af20917888625ae4e224e466f81fa68336`  
		Last Modified: Wed, 05 Oct 2022 16:06:49 GMT  
		Size: 66.1 MB (66129945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6b39b4604dfdcc6c6ceb5bc14d7771450cf8cf6e23a18fcb97c51ab33ce1af`  
		Last Modified: Wed, 05 Oct 2022 16:06:38 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.6`

```console
$ docker pull kong@sha256:3d48c2c6d9262b5949b40df4f1b1a459a0e4b7676d03b7c6c94a4c0289d22ae3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.6` - linux; amd64

```console
$ docker pull kong@sha256:8b976b5e1f07a06c0d337ac2548b48147b0180b92e3b4aad8de6f47b02177f1a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50233005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88dda4b3d1de7ee2ca6ebe5ec1f2c84f6784f10ee8c8f10f0525738aa67b191d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 23:01:23 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 06 Oct 2022 23:01:23 GMT
ARG ASSET=ce
# Thu, 06 Oct 2022 23:01:23 GMT
ENV ASSET=ce
# Thu, 06 Oct 2022 23:01:23 GMT
ARG EE_PORTS
# Thu, 06 Oct 2022 23:01:23 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 06 Oct 2022 23:01:37 GMT
ARG KONG_VERSION=2.6.1
# Thu, 06 Oct 2022 23:01:37 GMT
ENV KONG_VERSION=2.6.1
# Thu, 06 Oct 2022 23:01:37 GMT
ARG KONG_AMD64_SHA=9e7618ad06c148ed216be8bbf65a9c7cb95301e5349ef61b996fbb55ec4cfa87
# Thu, 06 Oct 2022 23:01:37 GMT
ARG KONG_ARM64_SHA=0fbf008685c6eac510d221595172e9e7bd51a846d410972d6950d9207cf400de
# Thu, 06 Oct 2022 23:01:44 GMT
# ARGS: KONG_AMD64_SHA=9e7618ad06c148ed216be8bbf65a9c7cb95301e5349ef61b996fbb55ec4cfa87 KONG_ARM64_SHA=0fbf008685c6eac510d221595172e9e7bd51a846d410972d6950d9207cf400de
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 06 Oct 2022 23:01:44 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 06 Oct 2022 23:01:44 GMT
USER kong
# Thu, 06 Oct 2022 23:01:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Oct 2022 23:01:45 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 06 Oct 2022 23:01:45 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Oct 2022 23:01:45 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 06 Oct 2022 23:01:45 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29712f9007996b849b4ca5751d9caac52946d8e35200fe77a0e58b376287bbbd`  
		Last Modified: Thu, 06 Oct 2022 23:03:14 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfba4240422e95f3476c90d92e9255cfa6695fb3af89710a50538a16141d797`  
		Last Modified: Thu, 06 Oct 2022 23:03:42 GMT  
		Size: 47.4 MB (47408484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9417a3349224dae27cda5dddd34c1f1da6015d5eaa81560431b42c522e6fbb0f`  
		Last Modified: Thu, 06 Oct 2022 23:03:34 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.6` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:2d3ff01b942487e8d8121c6794a79435fc5a358be321ed46728456616cb87c82
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49647010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15fb761959084d34c7b2a6fd9c843365d30cf061af02bd3eda9f06071a130f2e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 22:25:07 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 06 Oct 2022 22:25:07 GMT
ARG ASSET=ce
# Thu, 06 Oct 2022 22:25:08 GMT
ENV ASSET=ce
# Thu, 06 Oct 2022 22:25:09 GMT
ARG EE_PORTS
# Thu, 06 Oct 2022 22:25:11 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 06 Oct 2022 22:25:38 GMT
ARG KONG_VERSION=2.6.1
# Thu, 06 Oct 2022 22:25:39 GMT
ENV KONG_VERSION=2.6.1
# Thu, 06 Oct 2022 22:25:40 GMT
ARG KONG_AMD64_SHA=9e7618ad06c148ed216be8bbf65a9c7cb95301e5349ef61b996fbb55ec4cfa87
# Thu, 06 Oct 2022 22:25:41 GMT
ARG KONG_ARM64_SHA=0fbf008685c6eac510d221595172e9e7bd51a846d410972d6950d9207cf400de
# Thu, 06 Oct 2022 22:25:49 GMT
# ARGS: KONG_AMD64_SHA=9e7618ad06c148ed216be8bbf65a9c7cb95301e5349ef61b996fbb55ec4cfa87 KONG_ARM64_SHA=0fbf008685c6eac510d221595172e9e7bd51a846d410972d6950d9207cf400de
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 06 Oct 2022 22:25:50 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 06 Oct 2022 22:25:50 GMT
USER kong
# Thu, 06 Oct 2022 22:25:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Oct 2022 22:25:52 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 06 Oct 2022 22:25:53 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Oct 2022 22:25:54 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 06 Oct 2022 22:25:55 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be38426b84d987a4cd0ee5faa0e7209d36689d721c007c605f5d82a9b874ab1`  
		Last Modified: Thu, 06 Oct 2022 22:28:36 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38892d82a1c574e8aeaf86b4904b79581a9074fbcf59a3be1600159d30debace`  
		Last Modified: Thu, 06 Oct 2022 22:29:09 GMT  
		Size: 46.9 MB (46927558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131735889baefb1009dca31f80d16416f766b321a45264d22854c737ed3d60a8`  
		Last Modified: Thu, 06 Oct 2022 22:29:00 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.6-ubuntu`

```console
$ docker pull kong@sha256:80764058c7bfed69eace499cb52ccf6efecfc54585835e2a3a88a02cde257df0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.6-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:62f0eb7ee8aecf4d9ae88517c0b54e9401f2a992719e7f38d592650d443e4370
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128258108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8466c81f7e147ef5ef114b87cf3a53fe0bf59eaa7df8336d594fadf88cf56e83`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 18:04:26 GMT
ARG ASSET=ce
# Wed, 05 Oct 2022 18:04:26 GMT
ENV ASSET=ce
# Wed, 05 Oct 2022 18:04:26 GMT
ARG EE_PORTS
# Wed, 05 Oct 2022 18:04:26 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 05 Oct 2022 18:05:26 GMT
ARG KONG_VERSION=2.6.1
# Wed, 05 Oct 2022 18:05:26 GMT
ENV KONG_VERSION=2.6.1
# Wed, 05 Oct 2022 18:05:26 GMT
ARG KONG_AMD64_SHA=f70757f9317a1d40316f0187ae6e91c0c94b5b4346e564f7ae8430775bf7ad7e
# Wed, 05 Oct 2022 18:05:26 GMT
ARG KONG_ARM64_SHA=5cba6e7e28685fb7d80b77b70586cfb92c1de4b5198a6218bb1ca0c7f2502c89
# Wed, 05 Oct 2022 18:05:48 GMT
# ARGS: KONG_AMD64_SHA=f70757f9317a1d40316f0187ae6e91c0c94b5b4346e564f7ae8430775bf7ad7e KONG_ARM64_SHA=5cba6e7e28685fb7d80b77b70586cfb92c1de4b5198a6218bb1ca0c7f2502c89
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 05 Oct 2022 18:05:49 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 05 Oct 2022 18:05:49 GMT
USER kong
# Wed, 05 Oct 2022 18:05:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 18:05:49 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 05 Oct 2022 18:05:49 GMT
STOPSIGNAL SIGQUIT
# Wed, 05 Oct 2022 18:05:49 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 05 Oct 2022 18:05:49 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af493d1a174862c166e0d67b32f1bb9d93e2304a59209a55e08cd858d032d8b`  
		Last Modified: Wed, 05 Oct 2022 18:07:23 GMT  
		Size: 25.1 MB (25081963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399e993696815ce3a452cb95ab776e9c62ff68517f43710256e73e840cffb96e`  
		Last Modified: Wed, 05 Oct 2022 18:08:25 GMT  
		Size: 74.6 MB (74600814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eedb74a132762f4f4e3c5e5039de49d10ffd3c81369242eb4030c36ad9517bfa`  
		Last Modified: Wed, 05 Oct 2022 18:08:08 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.6-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:7959dfdbadbe22048a6bfe42c860367e3ee46e87f0355482761ebb2bd6344249
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125291886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04e14163bb9b74116b6a4088c99cc27460c5472c05ccce60f9e27cbdad999033`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:00:20 GMT
ARG ASSET=ce
# Wed, 05 Oct 2022 16:00:20 GMT
ENV ASSET=ce
# Wed, 05 Oct 2022 16:00:21 GMT
ARG EE_PORTS
# Wed, 05 Oct 2022 16:00:23 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 05 Oct 2022 16:02:12 GMT
ARG KONG_VERSION=2.6.1
# Wed, 05 Oct 2022 16:02:13 GMT
ENV KONG_VERSION=2.6.1
# Wed, 05 Oct 2022 16:02:14 GMT
ARG KONG_AMD64_SHA=f70757f9317a1d40316f0187ae6e91c0c94b5b4346e564f7ae8430775bf7ad7e
# Wed, 05 Oct 2022 16:02:15 GMT
ARG KONG_ARM64_SHA=5cba6e7e28685fb7d80b77b70586cfb92c1de4b5198a6218bb1ca0c7f2502c89
# Wed, 05 Oct 2022 16:02:54 GMT
# ARGS: KONG_AMD64_SHA=f70757f9317a1d40316f0187ae6e91c0c94b5b4346e564f7ae8430775bf7ad7e KONG_ARM64_SHA=5cba6e7e28685fb7d80b77b70586cfb92c1de4b5198a6218bb1ca0c7f2502c89
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 05 Oct 2022 16:02:56 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 05 Oct 2022 16:02:56 GMT
USER kong
# Wed, 05 Oct 2022 16:02:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 16:02:58 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 05 Oct 2022 16:02:59 GMT
STOPSIGNAL SIGQUIT
# Wed, 05 Oct 2022 16:03:00 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 05 Oct 2022 16:03:01 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f20e2ab08e0103d6be14c1b3d377ca9e5f15a0a1256d9621c287546c1b9f4de`  
		Last Modified: Wed, 05 Oct 2022 16:05:25 GMT  
		Size: 25.1 MB (25081964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334cec1feb82f9fb166e93c65b4850f9091ddc92322466174a41619467d0f4e3`  
		Last Modified: Wed, 05 Oct 2022 16:06:25 GMT  
		Size: 73.0 MB (73017419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381756fc3ea950cdfe10255dc06998b14a9e521385d86d838bf0fc9fdbb2b163`  
		Last Modified: Wed, 05 Oct 2022 16:06:13 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.6.1`

```console
$ docker pull kong@sha256:3d48c2c6d9262b5949b40df4f1b1a459a0e4b7676d03b7c6c94a4c0289d22ae3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.6.1` - linux; amd64

```console
$ docker pull kong@sha256:8b976b5e1f07a06c0d337ac2548b48147b0180b92e3b4aad8de6f47b02177f1a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50233005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88dda4b3d1de7ee2ca6ebe5ec1f2c84f6784f10ee8c8f10f0525738aa67b191d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 23:01:23 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 06 Oct 2022 23:01:23 GMT
ARG ASSET=ce
# Thu, 06 Oct 2022 23:01:23 GMT
ENV ASSET=ce
# Thu, 06 Oct 2022 23:01:23 GMT
ARG EE_PORTS
# Thu, 06 Oct 2022 23:01:23 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 06 Oct 2022 23:01:37 GMT
ARG KONG_VERSION=2.6.1
# Thu, 06 Oct 2022 23:01:37 GMT
ENV KONG_VERSION=2.6.1
# Thu, 06 Oct 2022 23:01:37 GMT
ARG KONG_AMD64_SHA=9e7618ad06c148ed216be8bbf65a9c7cb95301e5349ef61b996fbb55ec4cfa87
# Thu, 06 Oct 2022 23:01:37 GMT
ARG KONG_ARM64_SHA=0fbf008685c6eac510d221595172e9e7bd51a846d410972d6950d9207cf400de
# Thu, 06 Oct 2022 23:01:44 GMT
# ARGS: KONG_AMD64_SHA=9e7618ad06c148ed216be8bbf65a9c7cb95301e5349ef61b996fbb55ec4cfa87 KONG_ARM64_SHA=0fbf008685c6eac510d221595172e9e7bd51a846d410972d6950d9207cf400de
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 06 Oct 2022 23:01:44 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 06 Oct 2022 23:01:44 GMT
USER kong
# Thu, 06 Oct 2022 23:01:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Oct 2022 23:01:45 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 06 Oct 2022 23:01:45 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Oct 2022 23:01:45 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 06 Oct 2022 23:01:45 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29712f9007996b849b4ca5751d9caac52946d8e35200fe77a0e58b376287bbbd`  
		Last Modified: Thu, 06 Oct 2022 23:03:14 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfba4240422e95f3476c90d92e9255cfa6695fb3af89710a50538a16141d797`  
		Last Modified: Thu, 06 Oct 2022 23:03:42 GMT  
		Size: 47.4 MB (47408484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9417a3349224dae27cda5dddd34c1f1da6015d5eaa81560431b42c522e6fbb0f`  
		Last Modified: Thu, 06 Oct 2022 23:03:34 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.6.1` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:2d3ff01b942487e8d8121c6794a79435fc5a358be321ed46728456616cb87c82
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49647010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15fb761959084d34c7b2a6fd9c843365d30cf061af02bd3eda9f06071a130f2e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 22:25:07 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 06 Oct 2022 22:25:07 GMT
ARG ASSET=ce
# Thu, 06 Oct 2022 22:25:08 GMT
ENV ASSET=ce
# Thu, 06 Oct 2022 22:25:09 GMT
ARG EE_PORTS
# Thu, 06 Oct 2022 22:25:11 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 06 Oct 2022 22:25:38 GMT
ARG KONG_VERSION=2.6.1
# Thu, 06 Oct 2022 22:25:39 GMT
ENV KONG_VERSION=2.6.1
# Thu, 06 Oct 2022 22:25:40 GMT
ARG KONG_AMD64_SHA=9e7618ad06c148ed216be8bbf65a9c7cb95301e5349ef61b996fbb55ec4cfa87
# Thu, 06 Oct 2022 22:25:41 GMT
ARG KONG_ARM64_SHA=0fbf008685c6eac510d221595172e9e7bd51a846d410972d6950d9207cf400de
# Thu, 06 Oct 2022 22:25:49 GMT
# ARGS: KONG_AMD64_SHA=9e7618ad06c148ed216be8bbf65a9c7cb95301e5349ef61b996fbb55ec4cfa87 KONG_ARM64_SHA=0fbf008685c6eac510d221595172e9e7bd51a846d410972d6950d9207cf400de
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 06 Oct 2022 22:25:50 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 06 Oct 2022 22:25:50 GMT
USER kong
# Thu, 06 Oct 2022 22:25:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Oct 2022 22:25:52 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 06 Oct 2022 22:25:53 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Oct 2022 22:25:54 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 06 Oct 2022 22:25:55 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be38426b84d987a4cd0ee5faa0e7209d36689d721c007c605f5d82a9b874ab1`  
		Last Modified: Thu, 06 Oct 2022 22:28:36 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38892d82a1c574e8aeaf86b4904b79581a9074fbcf59a3be1600159d30debace`  
		Last Modified: Thu, 06 Oct 2022 22:29:09 GMT  
		Size: 46.9 MB (46927558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131735889baefb1009dca31f80d16416f766b321a45264d22854c737ed3d60a8`  
		Last Modified: Thu, 06 Oct 2022 22:29:00 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.6.1-alpine`

```console
$ docker pull kong@sha256:3d48c2c6d9262b5949b40df4f1b1a459a0e4b7676d03b7c6c94a4c0289d22ae3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.6.1-alpine` - linux; amd64

```console
$ docker pull kong@sha256:8b976b5e1f07a06c0d337ac2548b48147b0180b92e3b4aad8de6f47b02177f1a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50233005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88dda4b3d1de7ee2ca6ebe5ec1f2c84f6784f10ee8c8f10f0525738aa67b191d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 23:01:23 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 06 Oct 2022 23:01:23 GMT
ARG ASSET=ce
# Thu, 06 Oct 2022 23:01:23 GMT
ENV ASSET=ce
# Thu, 06 Oct 2022 23:01:23 GMT
ARG EE_PORTS
# Thu, 06 Oct 2022 23:01:23 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 06 Oct 2022 23:01:37 GMT
ARG KONG_VERSION=2.6.1
# Thu, 06 Oct 2022 23:01:37 GMT
ENV KONG_VERSION=2.6.1
# Thu, 06 Oct 2022 23:01:37 GMT
ARG KONG_AMD64_SHA=9e7618ad06c148ed216be8bbf65a9c7cb95301e5349ef61b996fbb55ec4cfa87
# Thu, 06 Oct 2022 23:01:37 GMT
ARG KONG_ARM64_SHA=0fbf008685c6eac510d221595172e9e7bd51a846d410972d6950d9207cf400de
# Thu, 06 Oct 2022 23:01:44 GMT
# ARGS: KONG_AMD64_SHA=9e7618ad06c148ed216be8bbf65a9c7cb95301e5349ef61b996fbb55ec4cfa87 KONG_ARM64_SHA=0fbf008685c6eac510d221595172e9e7bd51a846d410972d6950d9207cf400de
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 06 Oct 2022 23:01:44 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 06 Oct 2022 23:01:44 GMT
USER kong
# Thu, 06 Oct 2022 23:01:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Oct 2022 23:01:45 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 06 Oct 2022 23:01:45 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Oct 2022 23:01:45 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 06 Oct 2022 23:01:45 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29712f9007996b849b4ca5751d9caac52946d8e35200fe77a0e58b376287bbbd`  
		Last Modified: Thu, 06 Oct 2022 23:03:14 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfba4240422e95f3476c90d92e9255cfa6695fb3af89710a50538a16141d797`  
		Last Modified: Thu, 06 Oct 2022 23:03:42 GMT  
		Size: 47.4 MB (47408484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9417a3349224dae27cda5dddd34c1f1da6015d5eaa81560431b42c522e6fbb0f`  
		Last Modified: Thu, 06 Oct 2022 23:03:34 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.6.1-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:2d3ff01b942487e8d8121c6794a79435fc5a358be321ed46728456616cb87c82
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49647010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15fb761959084d34c7b2a6fd9c843365d30cf061af02bd3eda9f06071a130f2e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 22:25:07 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 06 Oct 2022 22:25:07 GMT
ARG ASSET=ce
# Thu, 06 Oct 2022 22:25:08 GMT
ENV ASSET=ce
# Thu, 06 Oct 2022 22:25:09 GMT
ARG EE_PORTS
# Thu, 06 Oct 2022 22:25:11 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 06 Oct 2022 22:25:38 GMT
ARG KONG_VERSION=2.6.1
# Thu, 06 Oct 2022 22:25:39 GMT
ENV KONG_VERSION=2.6.1
# Thu, 06 Oct 2022 22:25:40 GMT
ARG KONG_AMD64_SHA=9e7618ad06c148ed216be8bbf65a9c7cb95301e5349ef61b996fbb55ec4cfa87
# Thu, 06 Oct 2022 22:25:41 GMT
ARG KONG_ARM64_SHA=0fbf008685c6eac510d221595172e9e7bd51a846d410972d6950d9207cf400de
# Thu, 06 Oct 2022 22:25:49 GMT
# ARGS: KONG_AMD64_SHA=9e7618ad06c148ed216be8bbf65a9c7cb95301e5349ef61b996fbb55ec4cfa87 KONG_ARM64_SHA=0fbf008685c6eac510d221595172e9e7bd51a846d410972d6950d9207cf400de
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 06 Oct 2022 22:25:50 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 06 Oct 2022 22:25:50 GMT
USER kong
# Thu, 06 Oct 2022 22:25:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Oct 2022 22:25:52 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 06 Oct 2022 22:25:53 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Oct 2022 22:25:54 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 06 Oct 2022 22:25:55 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be38426b84d987a4cd0ee5faa0e7209d36689d721c007c605f5d82a9b874ab1`  
		Last Modified: Thu, 06 Oct 2022 22:28:36 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38892d82a1c574e8aeaf86b4904b79581a9074fbcf59a3be1600159d30debace`  
		Last Modified: Thu, 06 Oct 2022 22:29:09 GMT  
		Size: 46.9 MB (46927558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131735889baefb1009dca31f80d16416f766b321a45264d22854c737ed3d60a8`  
		Last Modified: Thu, 06 Oct 2022 22:29:00 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.6.1-ubuntu`

```console
$ docker pull kong@sha256:80764058c7bfed69eace499cb52ccf6efecfc54585835e2a3a88a02cde257df0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.6.1-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:62f0eb7ee8aecf4d9ae88517c0b54e9401f2a992719e7f38d592650d443e4370
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128258108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8466c81f7e147ef5ef114b87cf3a53fe0bf59eaa7df8336d594fadf88cf56e83`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 18:04:26 GMT
ARG ASSET=ce
# Wed, 05 Oct 2022 18:04:26 GMT
ENV ASSET=ce
# Wed, 05 Oct 2022 18:04:26 GMT
ARG EE_PORTS
# Wed, 05 Oct 2022 18:04:26 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 05 Oct 2022 18:05:26 GMT
ARG KONG_VERSION=2.6.1
# Wed, 05 Oct 2022 18:05:26 GMT
ENV KONG_VERSION=2.6.1
# Wed, 05 Oct 2022 18:05:26 GMT
ARG KONG_AMD64_SHA=f70757f9317a1d40316f0187ae6e91c0c94b5b4346e564f7ae8430775bf7ad7e
# Wed, 05 Oct 2022 18:05:26 GMT
ARG KONG_ARM64_SHA=5cba6e7e28685fb7d80b77b70586cfb92c1de4b5198a6218bb1ca0c7f2502c89
# Wed, 05 Oct 2022 18:05:48 GMT
# ARGS: KONG_AMD64_SHA=f70757f9317a1d40316f0187ae6e91c0c94b5b4346e564f7ae8430775bf7ad7e KONG_ARM64_SHA=5cba6e7e28685fb7d80b77b70586cfb92c1de4b5198a6218bb1ca0c7f2502c89
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 05 Oct 2022 18:05:49 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 05 Oct 2022 18:05:49 GMT
USER kong
# Wed, 05 Oct 2022 18:05:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 18:05:49 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 05 Oct 2022 18:05:49 GMT
STOPSIGNAL SIGQUIT
# Wed, 05 Oct 2022 18:05:49 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 05 Oct 2022 18:05:49 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af493d1a174862c166e0d67b32f1bb9d93e2304a59209a55e08cd858d032d8b`  
		Last Modified: Wed, 05 Oct 2022 18:07:23 GMT  
		Size: 25.1 MB (25081963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399e993696815ce3a452cb95ab776e9c62ff68517f43710256e73e840cffb96e`  
		Last Modified: Wed, 05 Oct 2022 18:08:25 GMT  
		Size: 74.6 MB (74600814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eedb74a132762f4f4e3c5e5039de49d10ffd3c81369242eb4030c36ad9517bfa`  
		Last Modified: Wed, 05 Oct 2022 18:08:08 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.6.1-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:7959dfdbadbe22048a6bfe42c860367e3ee46e87f0355482761ebb2bd6344249
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125291886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04e14163bb9b74116b6a4088c99cc27460c5472c05ccce60f9e27cbdad999033`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:00:20 GMT
ARG ASSET=ce
# Wed, 05 Oct 2022 16:00:20 GMT
ENV ASSET=ce
# Wed, 05 Oct 2022 16:00:21 GMT
ARG EE_PORTS
# Wed, 05 Oct 2022 16:00:23 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 05 Oct 2022 16:02:12 GMT
ARG KONG_VERSION=2.6.1
# Wed, 05 Oct 2022 16:02:13 GMT
ENV KONG_VERSION=2.6.1
# Wed, 05 Oct 2022 16:02:14 GMT
ARG KONG_AMD64_SHA=f70757f9317a1d40316f0187ae6e91c0c94b5b4346e564f7ae8430775bf7ad7e
# Wed, 05 Oct 2022 16:02:15 GMT
ARG KONG_ARM64_SHA=5cba6e7e28685fb7d80b77b70586cfb92c1de4b5198a6218bb1ca0c7f2502c89
# Wed, 05 Oct 2022 16:02:54 GMT
# ARGS: KONG_AMD64_SHA=f70757f9317a1d40316f0187ae6e91c0c94b5b4346e564f7ae8430775bf7ad7e KONG_ARM64_SHA=5cba6e7e28685fb7d80b77b70586cfb92c1de4b5198a6218bb1ca0c7f2502c89
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 05 Oct 2022 16:02:56 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 05 Oct 2022 16:02:56 GMT
USER kong
# Wed, 05 Oct 2022 16:02:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 16:02:58 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 05 Oct 2022 16:02:59 GMT
STOPSIGNAL SIGQUIT
# Wed, 05 Oct 2022 16:03:00 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 05 Oct 2022 16:03:01 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f20e2ab08e0103d6be14c1b3d377ca9e5f15a0a1256d9621c287546c1b9f4de`  
		Last Modified: Wed, 05 Oct 2022 16:05:25 GMT  
		Size: 25.1 MB (25081964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334cec1feb82f9fb166e93c65b4850f9091ddc92322466174a41619467d0f4e3`  
		Last Modified: Wed, 05 Oct 2022 16:06:25 GMT  
		Size: 73.0 MB (73017419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381756fc3ea950cdfe10255dc06998b14a9e521385d86d838bf0fc9fdbb2b163`  
		Last Modified: Wed, 05 Oct 2022 16:06:13 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.7`

```console
$ docker pull kong@sha256:d27fc998bea14e427e52897a043c83a3818caf9e47a227ee51724be3afe41a3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.7` - linux; amd64

```console
$ docker pull kong@sha256:8d092fb34ec241f32d28a847c523d8343acc6fd124d9c741a345af7006b7f6df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50140063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b7c0c4fabfb88b737b0346cad01366cd42c2ef0c01af6933b23bcc68f275eeb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 23:01:23 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 06 Oct 2022 23:01:23 GMT
ARG ASSET=ce
# Thu, 06 Oct 2022 23:01:23 GMT
ENV ASSET=ce
# Thu, 06 Oct 2022 23:01:23 GMT
ARG EE_PORTS
# Thu, 06 Oct 2022 23:01:23 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 06 Oct 2022 23:01:24 GMT
ARG KONG_VERSION=2.7.2
# Thu, 06 Oct 2022 23:01:24 GMT
ENV KONG_VERSION=2.7.2
# Thu, 06 Oct 2022 23:01:24 GMT
ARG KONG_AMD64_SHA=16990765aee26fc194992f0f90fc81e78a46d77cd0fc1e6670f3b2f797c1fe6b
# Thu, 06 Oct 2022 23:01:24 GMT
ARG KONG_ARM64_SHA=3e5dde2479d53299e81dd903a04e30302108b0864c996a3662fda24ca7aee9f6
# Thu, 06 Oct 2022 23:01:31 GMT
# ARGS: KONG_AMD64_SHA=16990765aee26fc194992f0f90fc81e78a46d77cd0fc1e6670f3b2f797c1fe6b KONG_ARM64_SHA=3e5dde2479d53299e81dd903a04e30302108b0864c996a3662fda24ca7aee9f6
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 06 Oct 2022 23:01:31 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 06 Oct 2022 23:01:31 GMT
USER kong
# Thu, 06 Oct 2022 23:01:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Oct 2022 23:01:32 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 06 Oct 2022 23:01:32 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Oct 2022 23:01:32 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 06 Oct 2022 23:01:32 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29712f9007996b849b4ca5751d9caac52946d8e35200fe77a0e58b376287bbbd`  
		Last Modified: Thu, 06 Oct 2022 23:03:14 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acde767c288c65146a32b71e68d2c25ff1803ac881577a77f6bfc3bdc82630e5`  
		Last Modified: Thu, 06 Oct 2022 23:03:22 GMT  
		Size: 47.3 MB (47315542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e54051d48e8ce97f13a7d5496d56b730a129bd4a03e80cc4eabb0f39010d55a`  
		Last Modified: Thu, 06 Oct 2022 23:03:14 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.7` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:c051abf2704134fd72edd144de58cfbab85a814122eedaaf20ee0ade3325073c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49566759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cd326fbdf9fb58a424fa28a53c05872dc6fb2ace9b44ba0cc5cbd14d3fad437`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 22:25:07 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 06 Oct 2022 22:25:07 GMT
ARG ASSET=ce
# Thu, 06 Oct 2022 22:25:08 GMT
ENV ASSET=ce
# Thu, 06 Oct 2022 22:25:09 GMT
ARG EE_PORTS
# Thu, 06 Oct 2022 22:25:11 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 06 Oct 2022 22:25:11 GMT
ARG KONG_VERSION=2.7.2
# Thu, 06 Oct 2022 22:25:12 GMT
ENV KONG_VERSION=2.7.2
# Thu, 06 Oct 2022 22:25:13 GMT
ARG KONG_AMD64_SHA=16990765aee26fc194992f0f90fc81e78a46d77cd0fc1e6670f3b2f797c1fe6b
# Thu, 06 Oct 2022 22:25:14 GMT
ARG KONG_ARM64_SHA=3e5dde2479d53299e81dd903a04e30302108b0864c996a3662fda24ca7aee9f6
# Thu, 06 Oct 2022 22:25:22 GMT
# ARGS: KONG_AMD64_SHA=16990765aee26fc194992f0f90fc81e78a46d77cd0fc1e6670f3b2f797c1fe6b KONG_ARM64_SHA=3e5dde2479d53299e81dd903a04e30302108b0864c996a3662fda24ca7aee9f6
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 06 Oct 2022 22:25:23 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 06 Oct 2022 22:25:23 GMT
USER kong
# Thu, 06 Oct 2022 22:25:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Oct 2022 22:25:25 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 06 Oct 2022 22:25:26 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Oct 2022 22:25:27 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 06 Oct 2022 22:25:28 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be38426b84d987a4cd0ee5faa0e7209d36689d721c007c605f5d82a9b874ab1`  
		Last Modified: Thu, 06 Oct 2022 22:28:36 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f3815d3f00770132abed1234a30423ab0d8608ce6270699cfcaad15cdcaf0f`  
		Last Modified: Thu, 06 Oct 2022 22:28:45 GMT  
		Size: 46.8 MB (46847307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b5792839796c17b24eb0075d1ed2687c3dabe1c7c4dbe4a544e45ab62ebaa4`  
		Last Modified: Thu, 06 Oct 2022 22:28:36 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.7-ubuntu`

```console
$ docker pull kong@sha256:e62e53ba5181f05c27d18d2edbb97272510d4565c2725a63c735c0289c7b3b72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.7-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:1b3b987b13fc81da2bc6d633049a829a93edc97c864045ef7face0cf839ef55b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128168397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d71cac7eed8a53d0cc9fbe23a14c1512174123d29c4c74b29476d5576424a20e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 18:04:26 GMT
ARG ASSET=ce
# Wed, 05 Oct 2022 18:04:26 GMT
ENV ASSET=ce
# Wed, 05 Oct 2022 18:04:26 GMT
ARG EE_PORTS
# Wed, 05 Oct 2022 18:04:26 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 05 Oct 2022 18:04:56 GMT
ARG KONG_VERSION=2.7.2
# Wed, 05 Oct 2022 18:04:56 GMT
ENV KONG_VERSION=2.7.2
# Wed, 05 Oct 2022 18:04:56 GMT
ARG KONG_AMD64_SHA=8124ddbfe80a1627b19a54e14b20ff0e176549699491cf5c61a4f0355470f8fc
# Wed, 05 Oct 2022 18:04:56 GMT
ARG KONG_ARM64_SHA=f40e616539ab64cb4fd333d19895ec9768b742bc25e5f2dbcb7f162bf90421d8
# Wed, 05 Oct 2022 18:05:18 GMT
# ARGS: KONG_AMD64_SHA=8124ddbfe80a1627b19a54e14b20ff0e176549699491cf5c61a4f0355470f8fc KONG_ARM64_SHA=f40e616539ab64cb4fd333d19895ec9768b742bc25e5f2dbcb7f162bf90421d8
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 05 Oct 2022 18:05:19 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 05 Oct 2022 18:05:19 GMT
USER kong
# Wed, 05 Oct 2022 18:05:19 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 18:05:19 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 05 Oct 2022 18:05:19 GMT
STOPSIGNAL SIGQUIT
# Wed, 05 Oct 2022 18:05:19 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 05 Oct 2022 18:05:19 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af493d1a174862c166e0d67b32f1bb9d93e2304a59209a55e08cd858d032d8b`  
		Last Modified: Wed, 05 Oct 2022 18:07:23 GMT  
		Size: 25.1 MB (25081963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073853ff82a5607beb1a0cc44c91ba59a4d1122dcb52322cc1a5531bd62a43a2`  
		Last Modified: Wed, 05 Oct 2022 18:07:57 GMT  
		Size: 74.5 MB (74511102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2450b04737255f8e696efca60087f8daa06ac4202cd42d03d8fb4990a420f22`  
		Last Modified: Wed, 05 Oct 2022 18:07:45 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.7-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:eb157fb45b7513a34ee7346bcf101f51a723878f681d734da59af1209f779749
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125203448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e71a2b9ea24ebf4b91396b4c41fa8f777f1d33e9bdd1af1500f355864b060b2f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:00:20 GMT
ARG ASSET=ce
# Wed, 05 Oct 2022 16:00:20 GMT
ENV ASSET=ce
# Wed, 05 Oct 2022 16:00:21 GMT
ARG EE_PORTS
# Wed, 05 Oct 2022 16:00:23 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 05 Oct 2022 16:01:16 GMT
ARG KONG_VERSION=2.7.2
# Wed, 05 Oct 2022 16:01:16 GMT
ENV KONG_VERSION=2.7.2
# Wed, 05 Oct 2022 16:01:17 GMT
ARG KONG_AMD64_SHA=8124ddbfe80a1627b19a54e14b20ff0e176549699491cf5c61a4f0355470f8fc
# Wed, 05 Oct 2022 16:01:18 GMT
ARG KONG_ARM64_SHA=f40e616539ab64cb4fd333d19895ec9768b742bc25e5f2dbcb7f162bf90421d8
# Wed, 05 Oct 2022 16:01:56 GMT
# ARGS: KONG_AMD64_SHA=8124ddbfe80a1627b19a54e14b20ff0e176549699491cf5c61a4f0355470f8fc KONG_ARM64_SHA=f40e616539ab64cb4fd333d19895ec9768b742bc25e5f2dbcb7f162bf90421d8
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 05 Oct 2022 16:01:57 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 05 Oct 2022 16:01:57 GMT
USER kong
# Wed, 05 Oct 2022 16:01:58 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 16:01:59 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 05 Oct 2022 16:02:00 GMT
STOPSIGNAL SIGQUIT
# Wed, 05 Oct 2022 16:02:01 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 05 Oct 2022 16:02:02 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f20e2ab08e0103d6be14c1b3d377ca9e5f15a0a1256d9621c287546c1b9f4de`  
		Last Modified: Wed, 05 Oct 2022 16:05:25 GMT  
		Size: 25.1 MB (25081964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d123530c8c055d40c36f39c6cb0709ac2140afc0abe75c3da0a05f7ed45d24`  
		Last Modified: Wed, 05 Oct 2022 16:05:59 GMT  
		Size: 72.9 MB (72928980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c5796061e5648ed60d7642e8c3816d5bf4e148e98f1002f28297ebac309241`  
		Last Modified: Wed, 05 Oct 2022 16:05:48 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.7.2`

```console
$ docker pull kong@sha256:d27fc998bea14e427e52897a043c83a3818caf9e47a227ee51724be3afe41a3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.7.2` - linux; amd64

```console
$ docker pull kong@sha256:8d092fb34ec241f32d28a847c523d8343acc6fd124d9c741a345af7006b7f6df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50140063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b7c0c4fabfb88b737b0346cad01366cd42c2ef0c01af6933b23bcc68f275eeb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 23:01:23 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 06 Oct 2022 23:01:23 GMT
ARG ASSET=ce
# Thu, 06 Oct 2022 23:01:23 GMT
ENV ASSET=ce
# Thu, 06 Oct 2022 23:01:23 GMT
ARG EE_PORTS
# Thu, 06 Oct 2022 23:01:23 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 06 Oct 2022 23:01:24 GMT
ARG KONG_VERSION=2.7.2
# Thu, 06 Oct 2022 23:01:24 GMT
ENV KONG_VERSION=2.7.2
# Thu, 06 Oct 2022 23:01:24 GMT
ARG KONG_AMD64_SHA=16990765aee26fc194992f0f90fc81e78a46d77cd0fc1e6670f3b2f797c1fe6b
# Thu, 06 Oct 2022 23:01:24 GMT
ARG KONG_ARM64_SHA=3e5dde2479d53299e81dd903a04e30302108b0864c996a3662fda24ca7aee9f6
# Thu, 06 Oct 2022 23:01:31 GMT
# ARGS: KONG_AMD64_SHA=16990765aee26fc194992f0f90fc81e78a46d77cd0fc1e6670f3b2f797c1fe6b KONG_ARM64_SHA=3e5dde2479d53299e81dd903a04e30302108b0864c996a3662fda24ca7aee9f6
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 06 Oct 2022 23:01:31 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 06 Oct 2022 23:01:31 GMT
USER kong
# Thu, 06 Oct 2022 23:01:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Oct 2022 23:01:32 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 06 Oct 2022 23:01:32 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Oct 2022 23:01:32 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 06 Oct 2022 23:01:32 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29712f9007996b849b4ca5751d9caac52946d8e35200fe77a0e58b376287bbbd`  
		Last Modified: Thu, 06 Oct 2022 23:03:14 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acde767c288c65146a32b71e68d2c25ff1803ac881577a77f6bfc3bdc82630e5`  
		Last Modified: Thu, 06 Oct 2022 23:03:22 GMT  
		Size: 47.3 MB (47315542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e54051d48e8ce97f13a7d5496d56b730a129bd4a03e80cc4eabb0f39010d55a`  
		Last Modified: Thu, 06 Oct 2022 23:03:14 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.7.2` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:c051abf2704134fd72edd144de58cfbab85a814122eedaaf20ee0ade3325073c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49566759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cd326fbdf9fb58a424fa28a53c05872dc6fb2ace9b44ba0cc5cbd14d3fad437`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 22:25:07 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 06 Oct 2022 22:25:07 GMT
ARG ASSET=ce
# Thu, 06 Oct 2022 22:25:08 GMT
ENV ASSET=ce
# Thu, 06 Oct 2022 22:25:09 GMT
ARG EE_PORTS
# Thu, 06 Oct 2022 22:25:11 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 06 Oct 2022 22:25:11 GMT
ARG KONG_VERSION=2.7.2
# Thu, 06 Oct 2022 22:25:12 GMT
ENV KONG_VERSION=2.7.2
# Thu, 06 Oct 2022 22:25:13 GMT
ARG KONG_AMD64_SHA=16990765aee26fc194992f0f90fc81e78a46d77cd0fc1e6670f3b2f797c1fe6b
# Thu, 06 Oct 2022 22:25:14 GMT
ARG KONG_ARM64_SHA=3e5dde2479d53299e81dd903a04e30302108b0864c996a3662fda24ca7aee9f6
# Thu, 06 Oct 2022 22:25:22 GMT
# ARGS: KONG_AMD64_SHA=16990765aee26fc194992f0f90fc81e78a46d77cd0fc1e6670f3b2f797c1fe6b KONG_ARM64_SHA=3e5dde2479d53299e81dd903a04e30302108b0864c996a3662fda24ca7aee9f6
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 06 Oct 2022 22:25:23 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 06 Oct 2022 22:25:23 GMT
USER kong
# Thu, 06 Oct 2022 22:25:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Oct 2022 22:25:25 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 06 Oct 2022 22:25:26 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Oct 2022 22:25:27 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 06 Oct 2022 22:25:28 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be38426b84d987a4cd0ee5faa0e7209d36689d721c007c605f5d82a9b874ab1`  
		Last Modified: Thu, 06 Oct 2022 22:28:36 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f3815d3f00770132abed1234a30423ab0d8608ce6270699cfcaad15cdcaf0f`  
		Last Modified: Thu, 06 Oct 2022 22:28:45 GMT  
		Size: 46.8 MB (46847307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b5792839796c17b24eb0075d1ed2687c3dabe1c7c4dbe4a544e45ab62ebaa4`  
		Last Modified: Thu, 06 Oct 2022 22:28:36 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.7.2-alpine`

```console
$ docker pull kong@sha256:d27fc998bea14e427e52897a043c83a3818caf9e47a227ee51724be3afe41a3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.7.2-alpine` - linux; amd64

```console
$ docker pull kong@sha256:8d092fb34ec241f32d28a847c523d8343acc6fd124d9c741a345af7006b7f6df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50140063 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b7c0c4fabfb88b737b0346cad01366cd42c2ef0c01af6933b23bcc68f275eeb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 23:01:23 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 06 Oct 2022 23:01:23 GMT
ARG ASSET=ce
# Thu, 06 Oct 2022 23:01:23 GMT
ENV ASSET=ce
# Thu, 06 Oct 2022 23:01:23 GMT
ARG EE_PORTS
# Thu, 06 Oct 2022 23:01:23 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 06 Oct 2022 23:01:24 GMT
ARG KONG_VERSION=2.7.2
# Thu, 06 Oct 2022 23:01:24 GMT
ENV KONG_VERSION=2.7.2
# Thu, 06 Oct 2022 23:01:24 GMT
ARG KONG_AMD64_SHA=16990765aee26fc194992f0f90fc81e78a46d77cd0fc1e6670f3b2f797c1fe6b
# Thu, 06 Oct 2022 23:01:24 GMT
ARG KONG_ARM64_SHA=3e5dde2479d53299e81dd903a04e30302108b0864c996a3662fda24ca7aee9f6
# Thu, 06 Oct 2022 23:01:31 GMT
# ARGS: KONG_AMD64_SHA=16990765aee26fc194992f0f90fc81e78a46d77cd0fc1e6670f3b2f797c1fe6b KONG_ARM64_SHA=3e5dde2479d53299e81dd903a04e30302108b0864c996a3662fda24ca7aee9f6
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 06 Oct 2022 23:01:31 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 06 Oct 2022 23:01:31 GMT
USER kong
# Thu, 06 Oct 2022 23:01:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Oct 2022 23:01:32 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 06 Oct 2022 23:01:32 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Oct 2022 23:01:32 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 06 Oct 2022 23:01:32 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29712f9007996b849b4ca5751d9caac52946d8e35200fe77a0e58b376287bbbd`  
		Last Modified: Thu, 06 Oct 2022 23:03:14 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acde767c288c65146a32b71e68d2c25ff1803ac881577a77f6bfc3bdc82630e5`  
		Last Modified: Thu, 06 Oct 2022 23:03:22 GMT  
		Size: 47.3 MB (47315542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e54051d48e8ce97f13a7d5496d56b730a129bd4a03e80cc4eabb0f39010d55a`  
		Last Modified: Thu, 06 Oct 2022 23:03:14 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.7.2-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:c051abf2704134fd72edd144de58cfbab85a814122eedaaf20ee0ade3325073c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49566759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cd326fbdf9fb58a424fa28a53c05872dc6fb2ace9b44ba0cc5cbd14d3fad437`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 22:25:07 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 06 Oct 2022 22:25:07 GMT
ARG ASSET=ce
# Thu, 06 Oct 2022 22:25:08 GMT
ENV ASSET=ce
# Thu, 06 Oct 2022 22:25:09 GMT
ARG EE_PORTS
# Thu, 06 Oct 2022 22:25:11 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 06 Oct 2022 22:25:11 GMT
ARG KONG_VERSION=2.7.2
# Thu, 06 Oct 2022 22:25:12 GMT
ENV KONG_VERSION=2.7.2
# Thu, 06 Oct 2022 22:25:13 GMT
ARG KONG_AMD64_SHA=16990765aee26fc194992f0f90fc81e78a46d77cd0fc1e6670f3b2f797c1fe6b
# Thu, 06 Oct 2022 22:25:14 GMT
ARG KONG_ARM64_SHA=3e5dde2479d53299e81dd903a04e30302108b0864c996a3662fda24ca7aee9f6
# Thu, 06 Oct 2022 22:25:22 GMT
# ARGS: KONG_AMD64_SHA=16990765aee26fc194992f0f90fc81e78a46d77cd0fc1e6670f3b2f797c1fe6b KONG_ARM64_SHA=3e5dde2479d53299e81dd903a04e30302108b0864c996a3662fda24ca7aee9f6
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 06 Oct 2022 22:25:23 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 06 Oct 2022 22:25:23 GMT
USER kong
# Thu, 06 Oct 2022 22:25:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Oct 2022 22:25:25 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 06 Oct 2022 22:25:26 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Oct 2022 22:25:27 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 06 Oct 2022 22:25:28 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be38426b84d987a4cd0ee5faa0e7209d36689d721c007c605f5d82a9b874ab1`  
		Last Modified: Thu, 06 Oct 2022 22:28:36 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f3815d3f00770132abed1234a30423ab0d8608ce6270699cfcaad15cdcaf0f`  
		Last Modified: Thu, 06 Oct 2022 22:28:45 GMT  
		Size: 46.8 MB (46847307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b5792839796c17b24eb0075d1ed2687c3dabe1c7c4dbe4a544e45ab62ebaa4`  
		Last Modified: Thu, 06 Oct 2022 22:28:36 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.7.2-ubuntu`

```console
$ docker pull kong@sha256:e62e53ba5181f05c27d18d2edbb97272510d4565c2725a63c735c0289c7b3b72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.7.2-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:1b3b987b13fc81da2bc6d633049a829a93edc97c864045ef7face0cf839ef55b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128168397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d71cac7eed8a53d0cc9fbe23a14c1512174123d29c4c74b29476d5576424a20e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 18:04:26 GMT
ARG ASSET=ce
# Wed, 05 Oct 2022 18:04:26 GMT
ENV ASSET=ce
# Wed, 05 Oct 2022 18:04:26 GMT
ARG EE_PORTS
# Wed, 05 Oct 2022 18:04:26 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 05 Oct 2022 18:04:56 GMT
ARG KONG_VERSION=2.7.2
# Wed, 05 Oct 2022 18:04:56 GMT
ENV KONG_VERSION=2.7.2
# Wed, 05 Oct 2022 18:04:56 GMT
ARG KONG_AMD64_SHA=8124ddbfe80a1627b19a54e14b20ff0e176549699491cf5c61a4f0355470f8fc
# Wed, 05 Oct 2022 18:04:56 GMT
ARG KONG_ARM64_SHA=f40e616539ab64cb4fd333d19895ec9768b742bc25e5f2dbcb7f162bf90421d8
# Wed, 05 Oct 2022 18:05:18 GMT
# ARGS: KONG_AMD64_SHA=8124ddbfe80a1627b19a54e14b20ff0e176549699491cf5c61a4f0355470f8fc KONG_ARM64_SHA=f40e616539ab64cb4fd333d19895ec9768b742bc25e5f2dbcb7f162bf90421d8
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 05 Oct 2022 18:05:19 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 05 Oct 2022 18:05:19 GMT
USER kong
# Wed, 05 Oct 2022 18:05:19 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 18:05:19 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 05 Oct 2022 18:05:19 GMT
STOPSIGNAL SIGQUIT
# Wed, 05 Oct 2022 18:05:19 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 05 Oct 2022 18:05:19 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af493d1a174862c166e0d67b32f1bb9d93e2304a59209a55e08cd858d032d8b`  
		Last Modified: Wed, 05 Oct 2022 18:07:23 GMT  
		Size: 25.1 MB (25081963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073853ff82a5607beb1a0cc44c91ba59a4d1122dcb52322cc1a5531bd62a43a2`  
		Last Modified: Wed, 05 Oct 2022 18:07:57 GMT  
		Size: 74.5 MB (74511102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2450b04737255f8e696efca60087f8daa06ac4202cd42d03d8fb4990a420f22`  
		Last Modified: Wed, 05 Oct 2022 18:07:45 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.7.2-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:eb157fb45b7513a34ee7346bcf101f51a723878f681d734da59af1209f779749
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125203448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e71a2b9ea24ebf4b91396b4c41fa8f777f1d33e9bdd1af1500f355864b060b2f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:00:20 GMT
ARG ASSET=ce
# Wed, 05 Oct 2022 16:00:20 GMT
ENV ASSET=ce
# Wed, 05 Oct 2022 16:00:21 GMT
ARG EE_PORTS
# Wed, 05 Oct 2022 16:00:23 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 05 Oct 2022 16:01:16 GMT
ARG KONG_VERSION=2.7.2
# Wed, 05 Oct 2022 16:01:16 GMT
ENV KONG_VERSION=2.7.2
# Wed, 05 Oct 2022 16:01:17 GMT
ARG KONG_AMD64_SHA=8124ddbfe80a1627b19a54e14b20ff0e176549699491cf5c61a4f0355470f8fc
# Wed, 05 Oct 2022 16:01:18 GMT
ARG KONG_ARM64_SHA=f40e616539ab64cb4fd333d19895ec9768b742bc25e5f2dbcb7f162bf90421d8
# Wed, 05 Oct 2022 16:01:56 GMT
# ARGS: KONG_AMD64_SHA=8124ddbfe80a1627b19a54e14b20ff0e176549699491cf5c61a4f0355470f8fc KONG_ARM64_SHA=f40e616539ab64cb4fd333d19895ec9768b742bc25e5f2dbcb7f162bf90421d8
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 05 Oct 2022 16:01:57 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 05 Oct 2022 16:01:57 GMT
USER kong
# Wed, 05 Oct 2022 16:01:58 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 16:01:59 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 05 Oct 2022 16:02:00 GMT
STOPSIGNAL SIGQUIT
# Wed, 05 Oct 2022 16:02:01 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 05 Oct 2022 16:02:02 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f20e2ab08e0103d6be14c1b3d377ca9e5f15a0a1256d9621c287546c1b9f4de`  
		Last Modified: Wed, 05 Oct 2022 16:05:25 GMT  
		Size: 25.1 MB (25081964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d123530c8c055d40c36f39c6cb0709ac2140afc0abe75c3da0a05f7ed45d24`  
		Last Modified: Wed, 05 Oct 2022 16:05:59 GMT  
		Size: 72.9 MB (72928980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c5796061e5648ed60d7642e8c3816d5bf4e148e98f1002f28297ebac309241`  
		Last Modified: Wed, 05 Oct 2022 16:05:48 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.8`

```console
$ docker pull kong@sha256:421e3813782a6773eb5642e60ed68135e40556b7abeac2fd9cf95b131abd59ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.8` - linux; amd64

```console
$ docker pull kong@sha256:e21b0b793879ab96720ed4188f9441260273f4bf775bcbff8d435e019ffb759a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49335657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cefb958bcd694597b65adc00053a762b1f9a6df3c6031af528d052d75a64e1a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 23:01:09 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 06 Oct 2022 23:01:10 GMT
ARG ASSET=ce
# Thu, 06 Oct 2022 23:01:10 GMT
ENV ASSET=ce
# Thu, 06 Oct 2022 23:01:10 GMT
ARG EE_PORTS
# Thu, 06 Oct 2022 23:01:10 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 06 Oct 2022 23:01:10 GMT
ARG KONG_VERSION=2.8.1
# Thu, 06 Oct 2022 23:01:10 GMT
ENV KONG_VERSION=2.8.1
# Thu, 06 Oct 2022 23:01:10 GMT
ARG KONG_AMD64_SHA=ccda33bf02803b6b8dd46b22990f92265fe61d900ba94e3e0fa26db0433098c0
# Thu, 06 Oct 2022 23:01:10 GMT
ARG KONG_ARM64_SHA=d21690332a89adf9900f7266e083f41f565eb009f2771ef112f3564878eeff53
# Thu, 06 Oct 2022 23:01:17 GMT
# ARGS: KONG_AMD64_SHA=ccda33bf02803b6b8dd46b22990f92265fe61d900ba94e3e0fa26db0433098c0 KONG_ARM64_SHA=d21690332a89adf9900f7266e083f41f565eb009f2771ef112f3564878eeff53
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 06 Oct 2022 23:01:18 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 06 Oct 2022 23:01:18 GMT
USER kong
# Thu, 06 Oct 2022 23:01:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Oct 2022 23:01:18 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 06 Oct 2022 23:01:18 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Oct 2022 23:01:18 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 06 Oct 2022 23:01:18 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70653f7a2d526d9024e271d864947f47000d34d971f36a44665b51e8c3b739c`  
		Last Modified: Thu, 06 Oct 2022 23:02:55 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531e3bd93090d08ef911bb2c8320f2fef2428ef96597535a55111fda18efde52`  
		Last Modified: Thu, 06 Oct 2022 23:03:02 GMT  
		Size: 46.5 MB (46528590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814dd06d26c72ec884803b7dd47e90f8855d4df9267025e9eb33d22aaa061e88`  
		Last Modified: Thu, 06 Oct 2022 23:02:55 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.8` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:ec9f01d724d09f67df585a96cc37203ab49bc15272f366eeec8f955324126202
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.5 MB (48534031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb476397266ce1811aad8dfb066804f5a235252247151be53548358254714a5d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 22:24:19 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 06 Oct 2022 22:24:20 GMT
ARG ASSET=ce
# Thu, 06 Oct 2022 22:24:21 GMT
ENV ASSET=ce
# Thu, 06 Oct 2022 22:24:22 GMT
ARG EE_PORTS
# Thu, 06 Oct 2022 22:24:24 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 06 Oct 2022 22:24:24 GMT
ARG KONG_VERSION=2.8.1
# Thu, 06 Oct 2022 22:24:25 GMT
ENV KONG_VERSION=2.8.1
# Thu, 06 Oct 2022 22:24:26 GMT
ARG KONG_AMD64_SHA=ccda33bf02803b6b8dd46b22990f92265fe61d900ba94e3e0fa26db0433098c0
# Thu, 06 Oct 2022 22:24:27 GMT
ARG KONG_ARM64_SHA=d21690332a89adf9900f7266e083f41f565eb009f2771ef112f3564878eeff53
# Thu, 06 Oct 2022 22:24:47 GMT
# ARGS: KONG_AMD64_SHA=ccda33bf02803b6b8dd46b22990f92265fe61d900ba94e3e0fa26db0433098c0 KONG_ARM64_SHA=d21690332a89adf9900f7266e083f41f565eb009f2771ef112f3564878eeff53
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 06 Oct 2022 22:24:48 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 06 Oct 2022 22:24:48 GMT
USER kong
# Thu, 06 Oct 2022 22:24:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Oct 2022 22:24:50 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 06 Oct 2022 22:24:51 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Oct 2022 22:24:52 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 06 Oct 2022 22:24:53 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03acfdfb6c5719f8020cde65d66675e3fc1210d23237e732a442a3c89165d91`  
		Last Modified: Thu, 06 Oct 2022 22:28:13 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41df54f1460a81c6b2736b97ccf8c96640356c984b6dc10ce369bd5aea5939ab`  
		Last Modified: Thu, 06 Oct 2022 22:28:21 GMT  
		Size: 45.8 MB (45825354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c745ab820eb4933473001b324f80b2301d308393d979c897fde19248ac9e08`  
		Last Modified: Thu, 06 Oct 2022 22:28:13 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.8-ubuntu`

```console
$ docker pull kong@sha256:35bf8c7bbacaa4f390833471d329c7be06fee5ddd5bfd9d6d776495adfee756f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.8-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:cedff6e436f88215dadcd6bf2d25062b9b5d3170ff6c9947b02c1319876e5fdb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121292578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:142c60b0bbecd85bac643266c0995c1b42083af9b5c4da4d1ba31592bb7c7f8f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 18:04:26 GMT
ARG ASSET=ce
# Wed, 05 Oct 2022 18:04:26 GMT
ENV ASSET=ce
# Wed, 05 Oct 2022 18:04:26 GMT
ARG EE_PORTS
# Wed, 05 Oct 2022 18:04:26 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 05 Oct 2022 18:04:27 GMT
ARG KONG_VERSION=2.8.1
# Wed, 05 Oct 2022 18:04:27 GMT
ENV KONG_VERSION=2.8.1
# Wed, 05 Oct 2022 18:04:27 GMT
ARG KONG_AMD64_SHA=10d12d23e5890414d666663094d51a42de41f8a9806fbc0baaf9ac4d37794361
# Wed, 05 Oct 2022 18:04:27 GMT
ARG KONG_ARM64_SHA=61c13219ef64dac9aeae5ae775411e8cfcd406f068cf3e75d463f916ae6513cb
# Wed, 05 Oct 2022 18:04:48 GMT
# ARGS: KONG_AMD64_SHA=10d12d23e5890414d666663094d51a42de41f8a9806fbc0baaf9ac4d37794361 KONG_ARM64_SHA=61c13219ef64dac9aeae5ae775411e8cfcd406f068cf3e75d463f916ae6513cb
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 05 Oct 2022 18:04:49 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 05 Oct 2022 18:04:49 GMT
USER kong
# Wed, 05 Oct 2022 18:04:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 18:04:50 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 05 Oct 2022 18:04:50 GMT
STOPSIGNAL SIGQUIT
# Wed, 05 Oct 2022 18:04:50 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 05 Oct 2022 18:04:50 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af493d1a174862c166e0d67b32f1bb9d93e2304a59209a55e08cd858d032d8b`  
		Last Modified: Wed, 05 Oct 2022 18:07:23 GMT  
		Size: 25.1 MB (25081963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbcc176a053adb32647c56614ff026d0deba20cb6efd6372197e024bf7c5693e`  
		Last Modified: Wed, 05 Oct 2022 18:07:33 GMT  
		Size: 67.6 MB (67635284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69d17ca86369a39c8f6a302ebfa154002b3b253738effeb247bfa53ec0330cb`  
		Last Modified: Wed, 05 Oct 2022 18:07:21 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.8-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:4ace2178b0cbab1f0bfff08ccb4027a2b2c55f3d7a2f799c84b5a3e88b6f02df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121785614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bf83f8cd6bb6857178d8573b0a890e9a1ce3f3b92611defef27eb0f010b29f0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:00:20 GMT
ARG ASSET=ce
# Wed, 05 Oct 2022 16:00:20 GMT
ENV ASSET=ce
# Wed, 05 Oct 2022 16:00:21 GMT
ARG EE_PORTS
# Wed, 05 Oct 2022 16:00:23 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 05 Oct 2022 16:00:23 GMT
ARG KONG_VERSION=2.8.1
# Wed, 05 Oct 2022 16:00:24 GMT
ENV KONG_VERSION=2.8.1
# Wed, 05 Oct 2022 16:00:25 GMT
ARG KONG_AMD64_SHA=10d12d23e5890414d666663094d51a42de41f8a9806fbc0baaf9ac4d37794361
# Wed, 05 Oct 2022 16:00:26 GMT
ARG KONG_ARM64_SHA=61c13219ef64dac9aeae5ae775411e8cfcd406f068cf3e75d463f916ae6513cb
# Wed, 05 Oct 2022 16:00:54 GMT
# ARGS: KONG_AMD64_SHA=10d12d23e5890414d666663094d51a42de41f8a9806fbc0baaf9ac4d37794361 KONG_ARM64_SHA=61c13219ef64dac9aeae5ae775411e8cfcd406f068cf3e75d463f916ae6513cb
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 05 Oct 2022 16:00:56 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 05 Oct 2022 16:00:56 GMT
USER kong
# Wed, 05 Oct 2022 16:00:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 16:00:58 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 05 Oct 2022 16:00:59 GMT
STOPSIGNAL SIGQUIT
# Wed, 05 Oct 2022 16:01:00 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 05 Oct 2022 16:01:01 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f20e2ab08e0103d6be14c1b3d377ca9e5f15a0a1256d9621c287546c1b9f4de`  
		Last Modified: Wed, 05 Oct 2022 16:05:25 GMT  
		Size: 25.1 MB (25081964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b815f040535344818d17e5bc9921438e91fbdb7337887300b631c65b9ca2a71`  
		Last Modified: Wed, 05 Oct 2022 16:05:34 GMT  
		Size: 69.5 MB (69511147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9441e13ebe80993a48c4c1856e99266741e08b1aa47010addabad717a2202046`  
		Last Modified: Wed, 05 Oct 2022 16:05:23 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.8.1`

```console
$ docker pull kong@sha256:421e3813782a6773eb5642e60ed68135e40556b7abeac2fd9cf95b131abd59ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.8.1` - linux; amd64

```console
$ docker pull kong@sha256:e21b0b793879ab96720ed4188f9441260273f4bf775bcbff8d435e019ffb759a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49335657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cefb958bcd694597b65adc00053a762b1f9a6df3c6031af528d052d75a64e1a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 23:01:09 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 06 Oct 2022 23:01:10 GMT
ARG ASSET=ce
# Thu, 06 Oct 2022 23:01:10 GMT
ENV ASSET=ce
# Thu, 06 Oct 2022 23:01:10 GMT
ARG EE_PORTS
# Thu, 06 Oct 2022 23:01:10 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 06 Oct 2022 23:01:10 GMT
ARG KONG_VERSION=2.8.1
# Thu, 06 Oct 2022 23:01:10 GMT
ENV KONG_VERSION=2.8.1
# Thu, 06 Oct 2022 23:01:10 GMT
ARG KONG_AMD64_SHA=ccda33bf02803b6b8dd46b22990f92265fe61d900ba94e3e0fa26db0433098c0
# Thu, 06 Oct 2022 23:01:10 GMT
ARG KONG_ARM64_SHA=d21690332a89adf9900f7266e083f41f565eb009f2771ef112f3564878eeff53
# Thu, 06 Oct 2022 23:01:17 GMT
# ARGS: KONG_AMD64_SHA=ccda33bf02803b6b8dd46b22990f92265fe61d900ba94e3e0fa26db0433098c0 KONG_ARM64_SHA=d21690332a89adf9900f7266e083f41f565eb009f2771ef112f3564878eeff53
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 06 Oct 2022 23:01:18 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 06 Oct 2022 23:01:18 GMT
USER kong
# Thu, 06 Oct 2022 23:01:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Oct 2022 23:01:18 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 06 Oct 2022 23:01:18 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Oct 2022 23:01:18 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 06 Oct 2022 23:01:18 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70653f7a2d526d9024e271d864947f47000d34d971f36a44665b51e8c3b739c`  
		Last Modified: Thu, 06 Oct 2022 23:02:55 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531e3bd93090d08ef911bb2c8320f2fef2428ef96597535a55111fda18efde52`  
		Last Modified: Thu, 06 Oct 2022 23:03:02 GMT  
		Size: 46.5 MB (46528590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814dd06d26c72ec884803b7dd47e90f8855d4df9267025e9eb33d22aaa061e88`  
		Last Modified: Thu, 06 Oct 2022 23:02:55 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.8.1` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:ec9f01d724d09f67df585a96cc37203ab49bc15272f366eeec8f955324126202
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.5 MB (48534031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb476397266ce1811aad8dfb066804f5a235252247151be53548358254714a5d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 22:24:19 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 06 Oct 2022 22:24:20 GMT
ARG ASSET=ce
# Thu, 06 Oct 2022 22:24:21 GMT
ENV ASSET=ce
# Thu, 06 Oct 2022 22:24:22 GMT
ARG EE_PORTS
# Thu, 06 Oct 2022 22:24:24 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 06 Oct 2022 22:24:24 GMT
ARG KONG_VERSION=2.8.1
# Thu, 06 Oct 2022 22:24:25 GMT
ENV KONG_VERSION=2.8.1
# Thu, 06 Oct 2022 22:24:26 GMT
ARG KONG_AMD64_SHA=ccda33bf02803b6b8dd46b22990f92265fe61d900ba94e3e0fa26db0433098c0
# Thu, 06 Oct 2022 22:24:27 GMT
ARG KONG_ARM64_SHA=d21690332a89adf9900f7266e083f41f565eb009f2771ef112f3564878eeff53
# Thu, 06 Oct 2022 22:24:47 GMT
# ARGS: KONG_AMD64_SHA=ccda33bf02803b6b8dd46b22990f92265fe61d900ba94e3e0fa26db0433098c0 KONG_ARM64_SHA=d21690332a89adf9900f7266e083f41f565eb009f2771ef112f3564878eeff53
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 06 Oct 2022 22:24:48 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 06 Oct 2022 22:24:48 GMT
USER kong
# Thu, 06 Oct 2022 22:24:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Oct 2022 22:24:50 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 06 Oct 2022 22:24:51 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Oct 2022 22:24:52 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 06 Oct 2022 22:24:53 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03acfdfb6c5719f8020cde65d66675e3fc1210d23237e732a442a3c89165d91`  
		Last Modified: Thu, 06 Oct 2022 22:28:13 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41df54f1460a81c6b2736b97ccf8c96640356c984b6dc10ce369bd5aea5939ab`  
		Last Modified: Thu, 06 Oct 2022 22:28:21 GMT  
		Size: 45.8 MB (45825354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c745ab820eb4933473001b324f80b2301d308393d979c897fde19248ac9e08`  
		Last Modified: Thu, 06 Oct 2022 22:28:13 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.8.1-alpine`

```console
$ docker pull kong@sha256:421e3813782a6773eb5642e60ed68135e40556b7abeac2fd9cf95b131abd59ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.8.1-alpine` - linux; amd64

```console
$ docker pull kong@sha256:e21b0b793879ab96720ed4188f9441260273f4bf775bcbff8d435e019ffb759a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49335657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cefb958bcd694597b65adc00053a762b1f9a6df3c6031af528d052d75a64e1a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 23:01:09 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 06 Oct 2022 23:01:10 GMT
ARG ASSET=ce
# Thu, 06 Oct 2022 23:01:10 GMT
ENV ASSET=ce
# Thu, 06 Oct 2022 23:01:10 GMT
ARG EE_PORTS
# Thu, 06 Oct 2022 23:01:10 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 06 Oct 2022 23:01:10 GMT
ARG KONG_VERSION=2.8.1
# Thu, 06 Oct 2022 23:01:10 GMT
ENV KONG_VERSION=2.8.1
# Thu, 06 Oct 2022 23:01:10 GMT
ARG KONG_AMD64_SHA=ccda33bf02803b6b8dd46b22990f92265fe61d900ba94e3e0fa26db0433098c0
# Thu, 06 Oct 2022 23:01:10 GMT
ARG KONG_ARM64_SHA=d21690332a89adf9900f7266e083f41f565eb009f2771ef112f3564878eeff53
# Thu, 06 Oct 2022 23:01:17 GMT
# ARGS: KONG_AMD64_SHA=ccda33bf02803b6b8dd46b22990f92265fe61d900ba94e3e0fa26db0433098c0 KONG_ARM64_SHA=d21690332a89adf9900f7266e083f41f565eb009f2771ef112f3564878eeff53
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 06 Oct 2022 23:01:18 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 06 Oct 2022 23:01:18 GMT
USER kong
# Thu, 06 Oct 2022 23:01:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Oct 2022 23:01:18 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 06 Oct 2022 23:01:18 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Oct 2022 23:01:18 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 06 Oct 2022 23:01:18 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70653f7a2d526d9024e271d864947f47000d34d971f36a44665b51e8c3b739c`  
		Last Modified: Thu, 06 Oct 2022 23:02:55 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531e3bd93090d08ef911bb2c8320f2fef2428ef96597535a55111fda18efde52`  
		Last Modified: Thu, 06 Oct 2022 23:03:02 GMT  
		Size: 46.5 MB (46528590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814dd06d26c72ec884803b7dd47e90f8855d4df9267025e9eb33d22aaa061e88`  
		Last Modified: Thu, 06 Oct 2022 23:02:55 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.8.1-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:ec9f01d724d09f67df585a96cc37203ab49bc15272f366eeec8f955324126202
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.5 MB (48534031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb476397266ce1811aad8dfb066804f5a235252247151be53548358254714a5d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 22:24:19 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 06 Oct 2022 22:24:20 GMT
ARG ASSET=ce
# Thu, 06 Oct 2022 22:24:21 GMT
ENV ASSET=ce
# Thu, 06 Oct 2022 22:24:22 GMT
ARG EE_PORTS
# Thu, 06 Oct 2022 22:24:24 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 06 Oct 2022 22:24:24 GMT
ARG KONG_VERSION=2.8.1
# Thu, 06 Oct 2022 22:24:25 GMT
ENV KONG_VERSION=2.8.1
# Thu, 06 Oct 2022 22:24:26 GMT
ARG KONG_AMD64_SHA=ccda33bf02803b6b8dd46b22990f92265fe61d900ba94e3e0fa26db0433098c0
# Thu, 06 Oct 2022 22:24:27 GMT
ARG KONG_ARM64_SHA=d21690332a89adf9900f7266e083f41f565eb009f2771ef112f3564878eeff53
# Thu, 06 Oct 2022 22:24:47 GMT
# ARGS: KONG_AMD64_SHA=ccda33bf02803b6b8dd46b22990f92265fe61d900ba94e3e0fa26db0433098c0 KONG_ARM64_SHA=d21690332a89adf9900f7266e083f41f565eb009f2771ef112f3564878eeff53
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 06 Oct 2022 22:24:48 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 06 Oct 2022 22:24:48 GMT
USER kong
# Thu, 06 Oct 2022 22:24:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Oct 2022 22:24:50 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 06 Oct 2022 22:24:51 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Oct 2022 22:24:52 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 06 Oct 2022 22:24:53 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f03acfdfb6c5719f8020cde65d66675e3fc1210d23237e732a442a3c89165d91`  
		Last Modified: Thu, 06 Oct 2022 22:28:13 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41df54f1460a81c6b2736b97ccf8c96640356c984b6dc10ce369bd5aea5939ab`  
		Last Modified: Thu, 06 Oct 2022 22:28:21 GMT  
		Size: 45.8 MB (45825354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89c745ab820eb4933473001b324f80b2301d308393d979c897fde19248ac9e08`  
		Last Modified: Thu, 06 Oct 2022 22:28:13 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.8.1-ubuntu`

```console
$ docker pull kong@sha256:35bf8c7bbacaa4f390833471d329c7be06fee5ddd5bfd9d6d776495adfee756f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.8.1-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:cedff6e436f88215dadcd6bf2d25062b9b5d3170ff6c9947b02c1319876e5fdb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121292578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:142c60b0bbecd85bac643266c0995c1b42083af9b5c4da4d1ba31592bb7c7f8f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 18:04:26 GMT
ARG ASSET=ce
# Wed, 05 Oct 2022 18:04:26 GMT
ENV ASSET=ce
# Wed, 05 Oct 2022 18:04:26 GMT
ARG EE_PORTS
# Wed, 05 Oct 2022 18:04:26 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 05 Oct 2022 18:04:27 GMT
ARG KONG_VERSION=2.8.1
# Wed, 05 Oct 2022 18:04:27 GMT
ENV KONG_VERSION=2.8.1
# Wed, 05 Oct 2022 18:04:27 GMT
ARG KONG_AMD64_SHA=10d12d23e5890414d666663094d51a42de41f8a9806fbc0baaf9ac4d37794361
# Wed, 05 Oct 2022 18:04:27 GMT
ARG KONG_ARM64_SHA=61c13219ef64dac9aeae5ae775411e8cfcd406f068cf3e75d463f916ae6513cb
# Wed, 05 Oct 2022 18:04:48 GMT
# ARGS: KONG_AMD64_SHA=10d12d23e5890414d666663094d51a42de41f8a9806fbc0baaf9ac4d37794361 KONG_ARM64_SHA=61c13219ef64dac9aeae5ae775411e8cfcd406f068cf3e75d463f916ae6513cb
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 05 Oct 2022 18:04:49 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 05 Oct 2022 18:04:49 GMT
USER kong
# Wed, 05 Oct 2022 18:04:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 18:04:50 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 05 Oct 2022 18:04:50 GMT
STOPSIGNAL SIGQUIT
# Wed, 05 Oct 2022 18:04:50 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 05 Oct 2022 18:04:50 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af493d1a174862c166e0d67b32f1bb9d93e2304a59209a55e08cd858d032d8b`  
		Last Modified: Wed, 05 Oct 2022 18:07:23 GMT  
		Size: 25.1 MB (25081963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbcc176a053adb32647c56614ff026d0deba20cb6efd6372197e024bf7c5693e`  
		Last Modified: Wed, 05 Oct 2022 18:07:33 GMT  
		Size: 67.6 MB (67635284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69d17ca86369a39c8f6a302ebfa154002b3b253738effeb247bfa53ec0330cb`  
		Last Modified: Wed, 05 Oct 2022 18:07:21 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.8.1-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:4ace2178b0cbab1f0bfff08ccb4027a2b2c55f3d7a2f799c84b5a3e88b6f02df
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121785614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bf83f8cd6bb6857178d8573b0a890e9a1ce3f3b92611defef27eb0f010b29f0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:00:20 GMT
ARG ASSET=ce
# Wed, 05 Oct 2022 16:00:20 GMT
ENV ASSET=ce
# Wed, 05 Oct 2022 16:00:21 GMT
ARG EE_PORTS
# Wed, 05 Oct 2022 16:00:23 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 05 Oct 2022 16:00:23 GMT
ARG KONG_VERSION=2.8.1
# Wed, 05 Oct 2022 16:00:24 GMT
ENV KONG_VERSION=2.8.1
# Wed, 05 Oct 2022 16:00:25 GMT
ARG KONG_AMD64_SHA=10d12d23e5890414d666663094d51a42de41f8a9806fbc0baaf9ac4d37794361
# Wed, 05 Oct 2022 16:00:26 GMT
ARG KONG_ARM64_SHA=61c13219ef64dac9aeae5ae775411e8cfcd406f068cf3e75d463f916ae6513cb
# Wed, 05 Oct 2022 16:00:54 GMT
# ARGS: KONG_AMD64_SHA=10d12d23e5890414d666663094d51a42de41f8a9806fbc0baaf9ac4d37794361 KONG_ARM64_SHA=61c13219ef64dac9aeae5ae775411e8cfcd406f068cf3e75d463f916ae6513cb
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 05 Oct 2022 16:00:56 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 05 Oct 2022 16:00:56 GMT
USER kong
# Wed, 05 Oct 2022 16:00:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 16:00:58 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 05 Oct 2022 16:00:59 GMT
STOPSIGNAL SIGQUIT
# Wed, 05 Oct 2022 16:01:00 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 05 Oct 2022 16:01:01 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f20e2ab08e0103d6be14c1b3d377ca9e5f15a0a1256d9621c287546c1b9f4de`  
		Last Modified: Wed, 05 Oct 2022 16:05:25 GMT  
		Size: 25.1 MB (25081964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b815f040535344818d17e5bc9921438e91fbdb7337887300b631c65b9ca2a71`  
		Last Modified: Wed, 05 Oct 2022 16:05:34 GMT  
		Size: 69.5 MB (69511147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9441e13ebe80993a48c4c1856e99266741e08b1aa47010addabad717a2202046`  
		Last Modified: Wed, 05 Oct 2022 16:05:23 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.0`

```console
$ docker pull kong@sha256:b2e287f0ce26074043dd9785c109a98e47c4cfaea6a81f5750a0ce2cd80b773f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.0` - linux; amd64

```console
$ docker pull kong@sha256:7b259d28f8108b961de8001887d3bf1297f812a1456db19bca24e6eeb2c9b9cd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51522512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2712ffde79f4ab54edaaeb5188a3086e60f6bf4729459b724c58a651dae40ee9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 23:00:54 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 06 Oct 2022 23:00:54 GMT
ARG ASSET=ce
# Thu, 06 Oct 2022 23:00:54 GMT
ENV ASSET=ce
# Thu, 06 Oct 2022 23:00:54 GMT
ARG EE_PORTS
# Thu, 06 Oct 2022 23:00:54 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 06 Oct 2022 23:00:54 GMT
ARG KONG_VERSION=3.0.0
# Thu, 06 Oct 2022 23:00:54 GMT
ENV KONG_VERSION=3.0.0
# Thu, 06 Oct 2022 23:00:54 GMT
ARG KONG_AMD64_SHA=b8e21beb32f803fae0959694ce7b6cec796a4159757e61b9cc0d30bed9682d10
# Thu, 06 Oct 2022 23:00:55 GMT
ARG KONG_ARM64_SHA=4c5407c5ef2f0f29468e15ea4dc6a3f27011dbde3ce18170e4a4fd7e2bb2c03b
# Thu, 06 Oct 2022 23:01:03 GMT
# ARGS: KONG_AMD64_SHA=b8e21beb32f803fae0959694ce7b6cec796a4159757e61b9cc0d30bed9682d10 KONG_ARM64_SHA=4c5407c5ef2f0f29468e15ea4dc6a3f27011dbde3ce18170e4a4fd7e2bb2c03b
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 06 Oct 2022 23:01:04 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 06 Oct 2022 23:01:04 GMT
USER kong
# Thu, 06 Oct 2022 23:01:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Oct 2022 23:01:04 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 06 Oct 2022 23:01:04 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Oct 2022 23:01:04 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 06 Oct 2022 23:01:04 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd92c70efef838622de7ec873d6e99abea86fe7547f5686b49707d02b5a7436b`  
		Last Modified: Thu, 06 Oct 2022 23:02:30 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e46e65db14b2721c441faf7349324031c1da43116748d795b2537d1c5c02d46`  
		Last Modified: Thu, 06 Oct 2022 23:02:38 GMT  
		Size: 48.7 MB (48715447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef0a423f8e78c38f414b2543801e0a6fc4c7a42b3b227d2a9266006b3bfa9399`  
		Last Modified: Thu, 06 Oct 2022 23:02:30 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.0` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:07cc96e98c5a93b0a24b12453097a5056bbe6652ea947e31be1b45f83a6858f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50657214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dae9cfcb1fc2c5335f4793fd2dc08b8777e45ce78220aaee6efa2041bbaf4b4e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 22:23:32 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 06 Oct 2022 22:23:33 GMT
ARG ASSET=ce
# Thu, 06 Oct 2022 22:23:34 GMT
ENV ASSET=ce
# Thu, 06 Oct 2022 22:23:35 GMT
ARG EE_PORTS
# Thu, 06 Oct 2022 22:23:37 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 06 Oct 2022 22:23:37 GMT
ARG KONG_VERSION=3.0.0
# Thu, 06 Oct 2022 22:23:38 GMT
ENV KONG_VERSION=3.0.0
# Thu, 06 Oct 2022 22:23:39 GMT
ARG KONG_AMD64_SHA=b8e21beb32f803fae0959694ce7b6cec796a4159757e61b9cc0d30bed9682d10
# Thu, 06 Oct 2022 22:23:40 GMT
ARG KONG_ARM64_SHA=4c5407c5ef2f0f29468e15ea4dc6a3f27011dbde3ce18170e4a4fd7e2bb2c03b
# Thu, 06 Oct 2022 22:23:59 GMT
# ARGS: KONG_AMD64_SHA=b8e21beb32f803fae0959694ce7b6cec796a4159757e61b9cc0d30bed9682d10 KONG_ARM64_SHA=4c5407c5ef2f0f29468e15ea4dc6a3f27011dbde3ce18170e4a4fd7e2bb2c03b
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 06 Oct 2022 22:24:00 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 06 Oct 2022 22:24:00 GMT
USER kong
# Thu, 06 Oct 2022 22:24:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Oct 2022 22:24:02 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 06 Oct 2022 22:24:03 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Oct 2022 22:24:04 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 06 Oct 2022 22:24:05 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d339143be54324c526b7bb7573d46feecff9caac3bafd45fc2a0f66ca7d3c9fa`  
		Last Modified: Thu, 06 Oct 2022 22:27:42 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4477d8fd13d01bede4dbb9366bc6bb19d666262e0d375fd84802b05c0f3da7c6`  
		Last Modified: Thu, 06 Oct 2022 22:27:51 GMT  
		Size: 47.9 MB (47948537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:864124fbd6c9124ff43edf1b4578f47d7bb6c249f859b305824882885a4f9b90`  
		Last Modified: Thu, 06 Oct 2022 22:27:42 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.0-ubuntu`

```console
$ docker pull kong@sha256:8a6061f898745d8d1ae6b9b2cc702d422e354844eefbfcd529353297e65ff47d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.0-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:b94b30d589c2d304b5c32ab10ce3c5b16f58b77c2aa363583da387c335c0fb48
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.8 MB (126751347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a998d5233b41e636a9afe797738f040dfb82731ce74c88c9208bceae5ff1c5a9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 18:03:44 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 05 Oct 2022 18:03:44 GMT
ARG ASSET=ce
# Wed, 05 Oct 2022 18:03:44 GMT
ENV ASSET=ce
# Wed, 05 Oct 2022 18:03:44 GMT
ARG EE_PORTS
# Wed, 05 Oct 2022 18:03:44 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 05 Oct 2022 18:03:45 GMT
ARG KONG_VERSION=3.0.0
# Wed, 05 Oct 2022 18:03:45 GMT
ENV KONG_VERSION=3.0.0
# Wed, 05 Oct 2022 18:03:45 GMT
ARG KONG_AMD64_SHA=3a38f6c4ba1cfc8897e655e46b957c7b0f2dd930111bf3d02411fedd1de53d6d
# Wed, 05 Oct 2022 18:03:45 GMT
ARG KONG_ARM64_SHA=190f82dd47df19339c025f37701e62191aa3063e77e15c5e57d5b77869058f69
# Wed, 05 Oct 2022 18:04:17 GMT
# ARGS: KONG_AMD64_SHA=3a38f6c4ba1cfc8897e655e46b957c7b0f2dd930111bf3d02411fedd1de53d6d KONG_ARM64_SHA=190f82dd47df19339c025f37701e62191aa3063e77e15c5e57d5b77869058f69
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 05 Oct 2022 18:04:18 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 05 Oct 2022 18:04:18 GMT
USER kong
# Wed, 05 Oct 2022 18:04:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 18:04:18 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 05 Oct 2022 18:04:18 GMT
STOPSIGNAL SIGQUIT
# Wed, 05 Oct 2022 18:04:18 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 05 Oct 2022 18:04:18 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a405c4afb98d18d76913bfe72f63dbd4a4d8c04256b6a7dfcbf44e6afba6f4`  
		Last Modified: Wed, 05 Oct 2022 18:06:58 GMT  
		Size: 25.1 MB (25081967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4c61366193417348ac92ea7a0b85d3a941dd84e99ddce0ccf874f9e2dd064a6`  
		Last Modified: Wed, 05 Oct 2022 18:07:08 GMT  
		Size: 73.1 MB (73094048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff353d4dd575bdf6ca92775c17a2634b394fc8f507c04bbaedcdeee8e3eb48e`  
		Last Modified: Wed, 05 Oct 2022 18:06:56 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.0-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:fdb693a2f651e8ea7fb72a3fbf27e948512f177e59bf67df495ace7bea594054
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.0 MB (123985385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5108a12659480aceff1ac2460acb6b4634ddee97df269cb93243ad915c17149e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 15:59:24 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 05 Oct 2022 15:59:25 GMT
ARG ASSET=ce
# Wed, 05 Oct 2022 15:59:26 GMT
ENV ASSET=ce
# Wed, 05 Oct 2022 15:59:27 GMT
ARG EE_PORTS
# Wed, 05 Oct 2022 15:59:29 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 05 Oct 2022 15:59:29 GMT
ARG KONG_VERSION=3.0.0
# Wed, 05 Oct 2022 15:59:30 GMT
ENV KONG_VERSION=3.0.0
# Wed, 05 Oct 2022 15:59:31 GMT
ARG KONG_AMD64_SHA=3a38f6c4ba1cfc8897e655e46b957c7b0f2dd930111bf3d02411fedd1de53d6d
# Wed, 05 Oct 2022 15:59:32 GMT
ARG KONG_ARM64_SHA=190f82dd47df19339c025f37701e62191aa3063e77e15c5e57d5b77869058f69
# Wed, 05 Oct 2022 16:00:03 GMT
# ARGS: KONG_AMD64_SHA=3a38f6c4ba1cfc8897e655e46b957c7b0f2dd930111bf3d02411fedd1de53d6d KONG_ARM64_SHA=190f82dd47df19339c025f37701e62191aa3063e77e15c5e57d5b77869058f69
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 05 Oct 2022 16:00:04 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 05 Oct 2022 16:00:04 GMT
USER kong
# Wed, 05 Oct 2022 16:00:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 16:00:06 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 05 Oct 2022 16:00:07 GMT
STOPSIGNAL SIGQUIT
# Wed, 05 Oct 2022 16:00:08 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 05 Oct 2022 16:00:09 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b27ee648e3be2639065d71cfba87c6c9d9d97d20920837e201328261d5786d66`  
		Last Modified: Wed, 05 Oct 2022 16:04:57 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee063d7cb8f1088bc6868dfa03aa1ff3523850ba73fdfb7da30a73defb968a0b`  
		Last Modified: Wed, 05 Oct 2022 16:05:07 GMT  
		Size: 71.7 MB (71710928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd23356d620515a3c2a3d982ed3c2ae1f2950af4cb40f5f356f64f5e0ba84e0`  
		Last Modified: Wed, 05 Oct 2022 16:04:55 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.0.0`

```console
$ docker pull kong@sha256:b2e287f0ce26074043dd9785c109a98e47c4cfaea6a81f5750a0ce2cd80b773f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.0.0` - linux; amd64

```console
$ docker pull kong@sha256:7b259d28f8108b961de8001887d3bf1297f812a1456db19bca24e6eeb2c9b9cd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51522512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2712ffde79f4ab54edaaeb5188a3086e60f6bf4729459b724c58a651dae40ee9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 23:00:54 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 06 Oct 2022 23:00:54 GMT
ARG ASSET=ce
# Thu, 06 Oct 2022 23:00:54 GMT
ENV ASSET=ce
# Thu, 06 Oct 2022 23:00:54 GMT
ARG EE_PORTS
# Thu, 06 Oct 2022 23:00:54 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 06 Oct 2022 23:00:54 GMT
ARG KONG_VERSION=3.0.0
# Thu, 06 Oct 2022 23:00:54 GMT
ENV KONG_VERSION=3.0.0
# Thu, 06 Oct 2022 23:00:54 GMT
ARG KONG_AMD64_SHA=b8e21beb32f803fae0959694ce7b6cec796a4159757e61b9cc0d30bed9682d10
# Thu, 06 Oct 2022 23:00:55 GMT
ARG KONG_ARM64_SHA=4c5407c5ef2f0f29468e15ea4dc6a3f27011dbde3ce18170e4a4fd7e2bb2c03b
# Thu, 06 Oct 2022 23:01:03 GMT
# ARGS: KONG_AMD64_SHA=b8e21beb32f803fae0959694ce7b6cec796a4159757e61b9cc0d30bed9682d10 KONG_ARM64_SHA=4c5407c5ef2f0f29468e15ea4dc6a3f27011dbde3ce18170e4a4fd7e2bb2c03b
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 06 Oct 2022 23:01:04 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 06 Oct 2022 23:01:04 GMT
USER kong
# Thu, 06 Oct 2022 23:01:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Oct 2022 23:01:04 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 06 Oct 2022 23:01:04 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Oct 2022 23:01:04 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 06 Oct 2022 23:01:04 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd92c70efef838622de7ec873d6e99abea86fe7547f5686b49707d02b5a7436b`  
		Last Modified: Thu, 06 Oct 2022 23:02:30 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e46e65db14b2721c441faf7349324031c1da43116748d795b2537d1c5c02d46`  
		Last Modified: Thu, 06 Oct 2022 23:02:38 GMT  
		Size: 48.7 MB (48715447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef0a423f8e78c38f414b2543801e0a6fc4c7a42b3b227d2a9266006b3bfa9399`  
		Last Modified: Thu, 06 Oct 2022 23:02:30 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.0.0` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:07cc96e98c5a93b0a24b12453097a5056bbe6652ea947e31be1b45f83a6858f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50657214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dae9cfcb1fc2c5335f4793fd2dc08b8777e45ce78220aaee6efa2041bbaf4b4e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 22:23:32 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 06 Oct 2022 22:23:33 GMT
ARG ASSET=ce
# Thu, 06 Oct 2022 22:23:34 GMT
ENV ASSET=ce
# Thu, 06 Oct 2022 22:23:35 GMT
ARG EE_PORTS
# Thu, 06 Oct 2022 22:23:37 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 06 Oct 2022 22:23:37 GMT
ARG KONG_VERSION=3.0.0
# Thu, 06 Oct 2022 22:23:38 GMT
ENV KONG_VERSION=3.0.0
# Thu, 06 Oct 2022 22:23:39 GMT
ARG KONG_AMD64_SHA=b8e21beb32f803fae0959694ce7b6cec796a4159757e61b9cc0d30bed9682d10
# Thu, 06 Oct 2022 22:23:40 GMT
ARG KONG_ARM64_SHA=4c5407c5ef2f0f29468e15ea4dc6a3f27011dbde3ce18170e4a4fd7e2bb2c03b
# Thu, 06 Oct 2022 22:23:59 GMT
# ARGS: KONG_AMD64_SHA=b8e21beb32f803fae0959694ce7b6cec796a4159757e61b9cc0d30bed9682d10 KONG_ARM64_SHA=4c5407c5ef2f0f29468e15ea4dc6a3f27011dbde3ce18170e4a4fd7e2bb2c03b
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 06 Oct 2022 22:24:00 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 06 Oct 2022 22:24:00 GMT
USER kong
# Thu, 06 Oct 2022 22:24:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Oct 2022 22:24:02 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 06 Oct 2022 22:24:03 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Oct 2022 22:24:04 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 06 Oct 2022 22:24:05 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d339143be54324c526b7bb7573d46feecff9caac3bafd45fc2a0f66ca7d3c9fa`  
		Last Modified: Thu, 06 Oct 2022 22:27:42 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4477d8fd13d01bede4dbb9366bc6bb19d666262e0d375fd84802b05c0f3da7c6`  
		Last Modified: Thu, 06 Oct 2022 22:27:51 GMT  
		Size: 47.9 MB (47948537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:864124fbd6c9124ff43edf1b4578f47d7bb6c249f859b305824882885a4f9b90`  
		Last Modified: Thu, 06 Oct 2022 22:27:42 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.0.0-alpine`

```console
$ docker pull kong@sha256:b2e287f0ce26074043dd9785c109a98e47c4cfaea6a81f5750a0ce2cd80b773f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.0.0-alpine` - linux; amd64

```console
$ docker pull kong@sha256:7b259d28f8108b961de8001887d3bf1297f812a1456db19bca24e6eeb2c9b9cd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51522512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2712ffde79f4ab54edaaeb5188a3086e60f6bf4729459b724c58a651dae40ee9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 23:00:54 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 06 Oct 2022 23:00:54 GMT
ARG ASSET=ce
# Thu, 06 Oct 2022 23:00:54 GMT
ENV ASSET=ce
# Thu, 06 Oct 2022 23:00:54 GMT
ARG EE_PORTS
# Thu, 06 Oct 2022 23:00:54 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 06 Oct 2022 23:00:54 GMT
ARG KONG_VERSION=3.0.0
# Thu, 06 Oct 2022 23:00:54 GMT
ENV KONG_VERSION=3.0.0
# Thu, 06 Oct 2022 23:00:54 GMT
ARG KONG_AMD64_SHA=b8e21beb32f803fae0959694ce7b6cec796a4159757e61b9cc0d30bed9682d10
# Thu, 06 Oct 2022 23:00:55 GMT
ARG KONG_ARM64_SHA=4c5407c5ef2f0f29468e15ea4dc6a3f27011dbde3ce18170e4a4fd7e2bb2c03b
# Thu, 06 Oct 2022 23:01:03 GMT
# ARGS: KONG_AMD64_SHA=b8e21beb32f803fae0959694ce7b6cec796a4159757e61b9cc0d30bed9682d10 KONG_ARM64_SHA=4c5407c5ef2f0f29468e15ea4dc6a3f27011dbde3ce18170e4a4fd7e2bb2c03b
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 06 Oct 2022 23:01:04 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 06 Oct 2022 23:01:04 GMT
USER kong
# Thu, 06 Oct 2022 23:01:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Oct 2022 23:01:04 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 06 Oct 2022 23:01:04 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Oct 2022 23:01:04 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 06 Oct 2022 23:01:04 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd92c70efef838622de7ec873d6e99abea86fe7547f5686b49707d02b5a7436b`  
		Last Modified: Thu, 06 Oct 2022 23:02:30 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e46e65db14b2721c441faf7349324031c1da43116748d795b2537d1c5c02d46`  
		Last Modified: Thu, 06 Oct 2022 23:02:38 GMT  
		Size: 48.7 MB (48715447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef0a423f8e78c38f414b2543801e0a6fc4c7a42b3b227d2a9266006b3bfa9399`  
		Last Modified: Thu, 06 Oct 2022 23:02:30 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.0.0-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:07cc96e98c5a93b0a24b12453097a5056bbe6652ea947e31be1b45f83a6858f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50657214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dae9cfcb1fc2c5335f4793fd2dc08b8777e45ce78220aaee6efa2041bbaf4b4e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 22:23:32 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 06 Oct 2022 22:23:33 GMT
ARG ASSET=ce
# Thu, 06 Oct 2022 22:23:34 GMT
ENV ASSET=ce
# Thu, 06 Oct 2022 22:23:35 GMT
ARG EE_PORTS
# Thu, 06 Oct 2022 22:23:37 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 06 Oct 2022 22:23:37 GMT
ARG KONG_VERSION=3.0.0
# Thu, 06 Oct 2022 22:23:38 GMT
ENV KONG_VERSION=3.0.0
# Thu, 06 Oct 2022 22:23:39 GMT
ARG KONG_AMD64_SHA=b8e21beb32f803fae0959694ce7b6cec796a4159757e61b9cc0d30bed9682d10
# Thu, 06 Oct 2022 22:23:40 GMT
ARG KONG_ARM64_SHA=4c5407c5ef2f0f29468e15ea4dc6a3f27011dbde3ce18170e4a4fd7e2bb2c03b
# Thu, 06 Oct 2022 22:23:59 GMT
# ARGS: KONG_AMD64_SHA=b8e21beb32f803fae0959694ce7b6cec796a4159757e61b9cc0d30bed9682d10 KONG_ARM64_SHA=4c5407c5ef2f0f29468e15ea4dc6a3f27011dbde3ce18170e4a4fd7e2bb2c03b
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 06 Oct 2022 22:24:00 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 06 Oct 2022 22:24:00 GMT
USER kong
# Thu, 06 Oct 2022 22:24:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Oct 2022 22:24:02 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 06 Oct 2022 22:24:03 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Oct 2022 22:24:04 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 06 Oct 2022 22:24:05 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d339143be54324c526b7bb7573d46feecff9caac3bafd45fc2a0f66ca7d3c9fa`  
		Last Modified: Thu, 06 Oct 2022 22:27:42 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4477d8fd13d01bede4dbb9366bc6bb19d666262e0d375fd84802b05c0f3da7c6`  
		Last Modified: Thu, 06 Oct 2022 22:27:51 GMT  
		Size: 47.9 MB (47948537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:864124fbd6c9124ff43edf1b4578f47d7bb6c249f859b305824882885a4f9b90`  
		Last Modified: Thu, 06 Oct 2022 22:27:42 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.0.0-ubuntu`

```console
$ docker pull kong@sha256:8a6061f898745d8d1ae6b9b2cc702d422e354844eefbfcd529353297e65ff47d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.0.0-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:b94b30d589c2d304b5c32ab10ce3c5b16f58b77c2aa363583da387c335c0fb48
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.8 MB (126751347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a998d5233b41e636a9afe797738f040dfb82731ce74c88c9208bceae5ff1c5a9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 18:03:44 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 05 Oct 2022 18:03:44 GMT
ARG ASSET=ce
# Wed, 05 Oct 2022 18:03:44 GMT
ENV ASSET=ce
# Wed, 05 Oct 2022 18:03:44 GMT
ARG EE_PORTS
# Wed, 05 Oct 2022 18:03:44 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 05 Oct 2022 18:03:45 GMT
ARG KONG_VERSION=3.0.0
# Wed, 05 Oct 2022 18:03:45 GMT
ENV KONG_VERSION=3.0.0
# Wed, 05 Oct 2022 18:03:45 GMT
ARG KONG_AMD64_SHA=3a38f6c4ba1cfc8897e655e46b957c7b0f2dd930111bf3d02411fedd1de53d6d
# Wed, 05 Oct 2022 18:03:45 GMT
ARG KONG_ARM64_SHA=190f82dd47df19339c025f37701e62191aa3063e77e15c5e57d5b77869058f69
# Wed, 05 Oct 2022 18:04:17 GMT
# ARGS: KONG_AMD64_SHA=3a38f6c4ba1cfc8897e655e46b957c7b0f2dd930111bf3d02411fedd1de53d6d KONG_ARM64_SHA=190f82dd47df19339c025f37701e62191aa3063e77e15c5e57d5b77869058f69
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 05 Oct 2022 18:04:18 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 05 Oct 2022 18:04:18 GMT
USER kong
# Wed, 05 Oct 2022 18:04:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 18:04:18 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 05 Oct 2022 18:04:18 GMT
STOPSIGNAL SIGQUIT
# Wed, 05 Oct 2022 18:04:18 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 05 Oct 2022 18:04:18 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a405c4afb98d18d76913bfe72f63dbd4a4d8c04256b6a7dfcbf44e6afba6f4`  
		Last Modified: Wed, 05 Oct 2022 18:06:58 GMT  
		Size: 25.1 MB (25081967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4c61366193417348ac92ea7a0b85d3a941dd84e99ddce0ccf874f9e2dd064a6`  
		Last Modified: Wed, 05 Oct 2022 18:07:08 GMT  
		Size: 73.1 MB (73094048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff353d4dd575bdf6ca92775c17a2634b394fc8f507c04bbaedcdeee8e3eb48e`  
		Last Modified: Wed, 05 Oct 2022 18:06:56 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.0.0-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:fdb693a2f651e8ea7fb72a3fbf27e948512f177e59bf67df495ace7bea594054
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.0 MB (123985385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5108a12659480aceff1ac2460acb6b4634ddee97df269cb93243ad915c17149e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 15:59:24 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 05 Oct 2022 15:59:25 GMT
ARG ASSET=ce
# Wed, 05 Oct 2022 15:59:26 GMT
ENV ASSET=ce
# Wed, 05 Oct 2022 15:59:27 GMT
ARG EE_PORTS
# Wed, 05 Oct 2022 15:59:29 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 05 Oct 2022 15:59:29 GMT
ARG KONG_VERSION=3.0.0
# Wed, 05 Oct 2022 15:59:30 GMT
ENV KONG_VERSION=3.0.0
# Wed, 05 Oct 2022 15:59:31 GMT
ARG KONG_AMD64_SHA=3a38f6c4ba1cfc8897e655e46b957c7b0f2dd930111bf3d02411fedd1de53d6d
# Wed, 05 Oct 2022 15:59:32 GMT
ARG KONG_ARM64_SHA=190f82dd47df19339c025f37701e62191aa3063e77e15c5e57d5b77869058f69
# Wed, 05 Oct 2022 16:00:03 GMT
# ARGS: KONG_AMD64_SHA=3a38f6c4ba1cfc8897e655e46b957c7b0f2dd930111bf3d02411fedd1de53d6d KONG_ARM64_SHA=190f82dd47df19339c025f37701e62191aa3063e77e15c5e57d5b77869058f69
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 05 Oct 2022 16:00:04 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 05 Oct 2022 16:00:04 GMT
USER kong
# Wed, 05 Oct 2022 16:00:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 16:00:06 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 05 Oct 2022 16:00:07 GMT
STOPSIGNAL SIGQUIT
# Wed, 05 Oct 2022 16:00:08 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 05 Oct 2022 16:00:09 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b27ee648e3be2639065d71cfba87c6c9d9d97d20920837e201328261d5786d66`  
		Last Modified: Wed, 05 Oct 2022 16:04:57 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee063d7cb8f1088bc6868dfa03aa1ff3523850ba73fdfb7da30a73defb968a0b`  
		Last Modified: Wed, 05 Oct 2022 16:05:07 GMT  
		Size: 71.7 MB (71710928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd23356d620515a3c2a3d982ed3c2ae1f2950af4cb40f5f356f64f5e0ba84e0`  
		Last Modified: Wed, 05 Oct 2022 16:04:55 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:alpine`

```console
$ docker pull kong@sha256:b2e287f0ce26074043dd9785c109a98e47c4cfaea6a81f5750a0ce2cd80b773f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:alpine` - linux; amd64

```console
$ docker pull kong@sha256:7b259d28f8108b961de8001887d3bf1297f812a1456db19bca24e6eeb2c9b9cd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51522512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2712ffde79f4ab54edaaeb5188a3086e60f6bf4729459b724c58a651dae40ee9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 23:00:54 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 06 Oct 2022 23:00:54 GMT
ARG ASSET=ce
# Thu, 06 Oct 2022 23:00:54 GMT
ENV ASSET=ce
# Thu, 06 Oct 2022 23:00:54 GMT
ARG EE_PORTS
# Thu, 06 Oct 2022 23:00:54 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 06 Oct 2022 23:00:54 GMT
ARG KONG_VERSION=3.0.0
# Thu, 06 Oct 2022 23:00:54 GMT
ENV KONG_VERSION=3.0.0
# Thu, 06 Oct 2022 23:00:54 GMT
ARG KONG_AMD64_SHA=b8e21beb32f803fae0959694ce7b6cec796a4159757e61b9cc0d30bed9682d10
# Thu, 06 Oct 2022 23:00:55 GMT
ARG KONG_ARM64_SHA=4c5407c5ef2f0f29468e15ea4dc6a3f27011dbde3ce18170e4a4fd7e2bb2c03b
# Thu, 06 Oct 2022 23:01:03 GMT
# ARGS: KONG_AMD64_SHA=b8e21beb32f803fae0959694ce7b6cec796a4159757e61b9cc0d30bed9682d10 KONG_ARM64_SHA=4c5407c5ef2f0f29468e15ea4dc6a3f27011dbde3ce18170e4a4fd7e2bb2c03b
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 06 Oct 2022 23:01:04 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 06 Oct 2022 23:01:04 GMT
USER kong
# Thu, 06 Oct 2022 23:01:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Oct 2022 23:01:04 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 06 Oct 2022 23:01:04 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Oct 2022 23:01:04 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 06 Oct 2022 23:01:04 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd92c70efef838622de7ec873d6e99abea86fe7547f5686b49707d02b5a7436b`  
		Last Modified: Thu, 06 Oct 2022 23:02:30 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e46e65db14b2721c441faf7349324031c1da43116748d795b2537d1c5c02d46`  
		Last Modified: Thu, 06 Oct 2022 23:02:38 GMT  
		Size: 48.7 MB (48715447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef0a423f8e78c38f414b2543801e0a6fc4c7a42b3b227d2a9266006b3bfa9399`  
		Last Modified: Thu, 06 Oct 2022 23:02:30 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:07cc96e98c5a93b0a24b12453097a5056bbe6652ea947e31be1b45f83a6858f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50657214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dae9cfcb1fc2c5335f4793fd2dc08b8777e45ce78220aaee6efa2041bbaf4b4e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 22:23:32 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 06 Oct 2022 22:23:33 GMT
ARG ASSET=ce
# Thu, 06 Oct 2022 22:23:34 GMT
ENV ASSET=ce
# Thu, 06 Oct 2022 22:23:35 GMT
ARG EE_PORTS
# Thu, 06 Oct 2022 22:23:37 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 06 Oct 2022 22:23:37 GMT
ARG KONG_VERSION=3.0.0
# Thu, 06 Oct 2022 22:23:38 GMT
ENV KONG_VERSION=3.0.0
# Thu, 06 Oct 2022 22:23:39 GMT
ARG KONG_AMD64_SHA=b8e21beb32f803fae0959694ce7b6cec796a4159757e61b9cc0d30bed9682d10
# Thu, 06 Oct 2022 22:23:40 GMT
ARG KONG_ARM64_SHA=4c5407c5ef2f0f29468e15ea4dc6a3f27011dbde3ce18170e4a4fd7e2bb2c03b
# Thu, 06 Oct 2022 22:23:59 GMT
# ARGS: KONG_AMD64_SHA=b8e21beb32f803fae0959694ce7b6cec796a4159757e61b9cc0d30bed9682d10 KONG_ARM64_SHA=4c5407c5ef2f0f29468e15ea4dc6a3f27011dbde3ce18170e4a4fd7e2bb2c03b
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 06 Oct 2022 22:24:00 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 06 Oct 2022 22:24:00 GMT
USER kong
# Thu, 06 Oct 2022 22:24:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Oct 2022 22:24:02 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 06 Oct 2022 22:24:03 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Oct 2022 22:24:04 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 06 Oct 2022 22:24:05 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d339143be54324c526b7bb7573d46feecff9caac3bafd45fc2a0f66ca7d3c9fa`  
		Last Modified: Thu, 06 Oct 2022 22:27:42 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4477d8fd13d01bede4dbb9366bc6bb19d666262e0d375fd84802b05c0f3da7c6`  
		Last Modified: Thu, 06 Oct 2022 22:27:51 GMT  
		Size: 47.9 MB (47948537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:864124fbd6c9124ff43edf1b4578f47d7bb6c249f859b305824882885a4f9b90`  
		Last Modified: Thu, 06 Oct 2022 22:27:42 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:latest`

```console
$ docker pull kong@sha256:b2e287f0ce26074043dd9785c109a98e47c4cfaea6a81f5750a0ce2cd80b773f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:latest` - linux; amd64

```console
$ docker pull kong@sha256:7b259d28f8108b961de8001887d3bf1297f812a1456db19bca24e6eeb2c9b9cd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51522512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2712ffde79f4ab54edaaeb5188a3086e60f6bf4729459b724c58a651dae40ee9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 23:00:54 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 06 Oct 2022 23:00:54 GMT
ARG ASSET=ce
# Thu, 06 Oct 2022 23:00:54 GMT
ENV ASSET=ce
# Thu, 06 Oct 2022 23:00:54 GMT
ARG EE_PORTS
# Thu, 06 Oct 2022 23:00:54 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 06 Oct 2022 23:00:54 GMT
ARG KONG_VERSION=3.0.0
# Thu, 06 Oct 2022 23:00:54 GMT
ENV KONG_VERSION=3.0.0
# Thu, 06 Oct 2022 23:00:54 GMT
ARG KONG_AMD64_SHA=b8e21beb32f803fae0959694ce7b6cec796a4159757e61b9cc0d30bed9682d10
# Thu, 06 Oct 2022 23:00:55 GMT
ARG KONG_ARM64_SHA=4c5407c5ef2f0f29468e15ea4dc6a3f27011dbde3ce18170e4a4fd7e2bb2c03b
# Thu, 06 Oct 2022 23:01:03 GMT
# ARGS: KONG_AMD64_SHA=b8e21beb32f803fae0959694ce7b6cec796a4159757e61b9cc0d30bed9682d10 KONG_ARM64_SHA=4c5407c5ef2f0f29468e15ea4dc6a3f27011dbde3ce18170e4a4fd7e2bb2c03b
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 06 Oct 2022 23:01:04 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 06 Oct 2022 23:01:04 GMT
USER kong
# Thu, 06 Oct 2022 23:01:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Oct 2022 23:01:04 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 06 Oct 2022 23:01:04 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Oct 2022 23:01:04 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 06 Oct 2022 23:01:04 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd92c70efef838622de7ec873d6e99abea86fe7547f5686b49707d02b5a7436b`  
		Last Modified: Thu, 06 Oct 2022 23:02:30 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e46e65db14b2721c441faf7349324031c1da43116748d795b2537d1c5c02d46`  
		Last Modified: Thu, 06 Oct 2022 23:02:38 GMT  
		Size: 48.7 MB (48715447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef0a423f8e78c38f414b2543801e0a6fc4c7a42b3b227d2a9266006b3bfa9399`  
		Last Modified: Thu, 06 Oct 2022 23:02:30 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:latest` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:07cc96e98c5a93b0a24b12453097a5056bbe6652ea947e31be1b45f83a6858f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50657214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dae9cfcb1fc2c5335f4793fd2dc08b8777e45ce78220aaee6efa2041bbaf4b4e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 22:23:32 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 06 Oct 2022 22:23:33 GMT
ARG ASSET=ce
# Thu, 06 Oct 2022 22:23:34 GMT
ENV ASSET=ce
# Thu, 06 Oct 2022 22:23:35 GMT
ARG EE_PORTS
# Thu, 06 Oct 2022 22:23:37 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 06 Oct 2022 22:23:37 GMT
ARG KONG_VERSION=3.0.0
# Thu, 06 Oct 2022 22:23:38 GMT
ENV KONG_VERSION=3.0.0
# Thu, 06 Oct 2022 22:23:39 GMT
ARG KONG_AMD64_SHA=b8e21beb32f803fae0959694ce7b6cec796a4159757e61b9cc0d30bed9682d10
# Thu, 06 Oct 2022 22:23:40 GMT
ARG KONG_ARM64_SHA=4c5407c5ef2f0f29468e15ea4dc6a3f27011dbde3ce18170e4a4fd7e2bb2c03b
# Thu, 06 Oct 2022 22:23:59 GMT
# ARGS: KONG_AMD64_SHA=b8e21beb32f803fae0959694ce7b6cec796a4159757e61b9cc0d30bed9682d10 KONG_ARM64_SHA=4c5407c5ef2f0f29468e15ea4dc6a3f27011dbde3ce18170e4a4fd7e2bb2c03b
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 06 Oct 2022 22:24:00 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 06 Oct 2022 22:24:00 GMT
USER kong
# Thu, 06 Oct 2022 22:24:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Oct 2022 22:24:02 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 06 Oct 2022 22:24:03 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Oct 2022 22:24:04 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 06 Oct 2022 22:24:05 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d339143be54324c526b7bb7573d46feecff9caac3bafd45fc2a0f66ca7d3c9fa`  
		Last Modified: Thu, 06 Oct 2022 22:27:42 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4477d8fd13d01bede4dbb9366bc6bb19d666262e0d375fd84802b05c0f3da7c6`  
		Last Modified: Thu, 06 Oct 2022 22:27:51 GMT  
		Size: 47.9 MB (47948537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:864124fbd6c9124ff43edf1b4578f47d7bb6c249f859b305824882885a4f9b90`  
		Last Modified: Thu, 06 Oct 2022 22:27:42 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:ubuntu`

```console
$ docker pull kong@sha256:8a6061f898745d8d1ae6b9b2cc702d422e354844eefbfcd529353297e65ff47d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:b94b30d589c2d304b5c32ab10ce3c5b16f58b77c2aa363583da387c335c0fb48
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.8 MB (126751347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a998d5233b41e636a9afe797738f040dfb82731ce74c88c9208bceae5ff1c5a9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 18:03:44 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 05 Oct 2022 18:03:44 GMT
ARG ASSET=ce
# Wed, 05 Oct 2022 18:03:44 GMT
ENV ASSET=ce
# Wed, 05 Oct 2022 18:03:44 GMT
ARG EE_PORTS
# Wed, 05 Oct 2022 18:03:44 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 05 Oct 2022 18:03:45 GMT
ARG KONG_VERSION=3.0.0
# Wed, 05 Oct 2022 18:03:45 GMT
ENV KONG_VERSION=3.0.0
# Wed, 05 Oct 2022 18:03:45 GMT
ARG KONG_AMD64_SHA=3a38f6c4ba1cfc8897e655e46b957c7b0f2dd930111bf3d02411fedd1de53d6d
# Wed, 05 Oct 2022 18:03:45 GMT
ARG KONG_ARM64_SHA=190f82dd47df19339c025f37701e62191aa3063e77e15c5e57d5b77869058f69
# Wed, 05 Oct 2022 18:04:17 GMT
# ARGS: KONG_AMD64_SHA=3a38f6c4ba1cfc8897e655e46b957c7b0f2dd930111bf3d02411fedd1de53d6d KONG_ARM64_SHA=190f82dd47df19339c025f37701e62191aa3063e77e15c5e57d5b77869058f69
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 05 Oct 2022 18:04:18 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 05 Oct 2022 18:04:18 GMT
USER kong
# Wed, 05 Oct 2022 18:04:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 18:04:18 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 05 Oct 2022 18:04:18 GMT
STOPSIGNAL SIGQUIT
# Wed, 05 Oct 2022 18:04:18 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 05 Oct 2022 18:04:18 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a405c4afb98d18d76913bfe72f63dbd4a4d8c04256b6a7dfcbf44e6afba6f4`  
		Last Modified: Wed, 05 Oct 2022 18:06:58 GMT  
		Size: 25.1 MB (25081967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4c61366193417348ac92ea7a0b85d3a941dd84e99ddce0ccf874f9e2dd064a6`  
		Last Modified: Wed, 05 Oct 2022 18:07:08 GMT  
		Size: 73.1 MB (73094048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff353d4dd575bdf6ca92775c17a2634b394fc8f507c04bbaedcdeee8e3eb48e`  
		Last Modified: Wed, 05 Oct 2022 18:06:56 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:fdb693a2f651e8ea7fb72a3fbf27e948512f177e59bf67df495ace7bea594054
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.0 MB (123985385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5108a12659480aceff1ac2460acb6b4634ddee97df269cb93243ad915c17149e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 15:59:24 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 05 Oct 2022 15:59:25 GMT
ARG ASSET=ce
# Wed, 05 Oct 2022 15:59:26 GMT
ENV ASSET=ce
# Wed, 05 Oct 2022 15:59:27 GMT
ARG EE_PORTS
# Wed, 05 Oct 2022 15:59:29 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 05 Oct 2022 15:59:29 GMT
ARG KONG_VERSION=3.0.0
# Wed, 05 Oct 2022 15:59:30 GMT
ENV KONG_VERSION=3.0.0
# Wed, 05 Oct 2022 15:59:31 GMT
ARG KONG_AMD64_SHA=3a38f6c4ba1cfc8897e655e46b957c7b0f2dd930111bf3d02411fedd1de53d6d
# Wed, 05 Oct 2022 15:59:32 GMT
ARG KONG_ARM64_SHA=190f82dd47df19339c025f37701e62191aa3063e77e15c5e57d5b77869058f69
# Wed, 05 Oct 2022 16:00:03 GMT
# ARGS: KONG_AMD64_SHA=3a38f6c4ba1cfc8897e655e46b957c7b0f2dd930111bf3d02411fedd1de53d6d KONG_ARM64_SHA=190f82dd47df19339c025f37701e62191aa3063e77e15c5e57d5b77869058f69
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 05 Oct 2022 16:00:04 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 05 Oct 2022 16:00:04 GMT
USER kong
# Wed, 05 Oct 2022 16:00:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 05 Oct 2022 16:00:06 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 05 Oct 2022 16:00:07 GMT
STOPSIGNAL SIGQUIT
# Wed, 05 Oct 2022 16:00:08 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 05 Oct 2022 16:00:09 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b27ee648e3be2639065d71cfba87c6c9d9d97d20920837e201328261d5786d66`  
		Last Modified: Wed, 05 Oct 2022 16:04:57 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee063d7cb8f1088bc6868dfa03aa1ff3523850ba73fdfb7da30a73defb968a0b`  
		Last Modified: Wed, 05 Oct 2022 16:05:07 GMT  
		Size: 71.7 MB (71710928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd23356d620515a3c2a3d982ed3c2ae1f2950af4cb40f5f356f64f5e0ba84e0`  
		Last Modified: Wed, 05 Oct 2022 16:04:55 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
