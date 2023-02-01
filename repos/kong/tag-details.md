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
-	[`kong:2.8.3`](#kong283)
-	[`kong:2.8.3-alpine`](#kong283-alpine)
-	[`kong:2.8.3-ubuntu`](#kong283-ubuntu)
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
-	[`kong:alpine`](#kongalpine)
-	[`kong:latest`](#konglatest)
-	[`kong:ubuntu`](#kongubuntu)

## `kong:2.5`

```console
$ docker pull kong@sha256:4d459bf9f353e69df80d660a7544d29583e77d5292f827137f6add87f74d2364
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
$ docker pull kong@sha256:934f0f609894a62d5ab41685863f02b29e7aa7d454b8e00482ed493fa32aaed1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.4 MB (48391762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ddbd7a976f9e47f0c736179c4fe225a32899cb86cebf1dd093bf993018a77e6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 22:40:04 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 10 Nov 2022 22:40:04 GMT
ARG ASSET=ce
# Thu, 10 Nov 2022 22:40:04 GMT
ENV ASSET=ce
# Thu, 10 Nov 2022 22:40:04 GMT
ARG EE_PORTS
# Thu, 10 Nov 2022 22:40:04 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 10 Nov 2022 22:40:29 GMT
ARG KONG_VERSION=2.5.2
# Thu, 10 Nov 2022 22:40:29 GMT
ENV KONG_VERSION=2.5.2
# Thu, 10 Nov 2022 22:40:29 GMT
ARG KONG_AMD64_SHA=d4bc93bcb14cce8c37ced136632a290b441050c540db779e742bcd88e5cfd70d
# Thu, 10 Nov 2022 22:40:29 GMT
ARG KONG_ARM64_SHA=691e1dc29e96d6a95b60674513932c4f7547773014685ce0130549f980c1c46e
# Thu, 10 Nov 2022 22:40:35 GMT
# ARGS: KONG_AMD64_SHA=d4bc93bcb14cce8c37ced136632a290b441050c540db779e742bcd88e5cfd70d KONG_ARM64_SHA=691e1dc29e96d6a95b60674513932c4f7547773014685ce0130549f980c1c46e
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 10 Nov 2022 22:40:35 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 10 Nov 2022 22:40:35 GMT
USER kong
# Thu, 10 Nov 2022 22:40:36 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 10 Nov 2022 22:40:36 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 10 Nov 2022 22:40:36 GMT
STOPSIGNAL SIGQUIT
# Thu, 10 Nov 2022 22:40:36 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 10 Nov 2022 22:40:36 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9f5eba777c2192f562d24cd3da16152dec7d8942677370e1524b03a6e36a2b`  
		Last Modified: Thu, 10 Nov 2022 22:41:58 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578c76f657afd39a075841d957e371975dda66e218c2055e95e692d64aa969ee`  
		Last Modified: Thu, 10 Nov 2022 22:42:47 GMT  
		Size: 45.7 MB (45672316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ad9797993253de6ac3a029a742d251a5445f0acc9ac38af3e937ae07078d3f`  
		Last Modified: Thu, 10 Nov 2022 22:42:40 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.5-ubuntu`

```console
$ docker pull kong@sha256:35fbe9f437ff098d994ae4043430815d9b6ea401ff03e205c028190390f03ec3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.5-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:7a6f68a9807b9aa1b5f78f232705e3c25f08b3b8e1450b7ca1d54e6a61ded9c7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121322032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:034c59249c73bc265b7db741b3b1274cebc2c2d3f8821439961846042079643e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 01 Feb 2023 11:42:37 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:42:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:42:39 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Wed, 01 Feb 2023 11:42:39 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 19:15:07 GMT
ARG ASSET=ce
# Wed, 01 Feb 2023 19:15:07 GMT
ENV ASSET=ce
# Wed, 01 Feb 2023 19:15:07 GMT
ARG EE_PORTS
# Wed, 01 Feb 2023 19:15:07 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 01 Feb 2023 19:16:07 GMT
ARG KONG_VERSION=2.5.2
# Wed, 01 Feb 2023 19:16:07 GMT
ENV KONG_VERSION=2.5.2
# Wed, 01 Feb 2023 19:16:07 GMT
ARG KONG_AMD64_SHA=ae65ac9eb35f682768abfb080c61581440347db8dafd0a495639ff666a406a96
# Wed, 01 Feb 2023 19:16:07 GMT
ARG KONG_ARM64_SHA=b4720e3d0831d13364cc749200c77df356a2145478f6a55fd48618a9aa1967d9
# Wed, 01 Feb 2023 19:16:31 GMT
# ARGS: KONG_AMD64_SHA=ae65ac9eb35f682768abfb080c61581440347db8dafd0a495639ff666a406a96 KONG_ARM64_SHA=b4720e3d0831d13364cc749200c77df356a2145478f6a55fd48618a9aa1967d9
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 01 Feb 2023 19:16:31 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 01 Feb 2023 19:16:32 GMT
USER kong
# Wed, 01 Feb 2023 19:16:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Feb 2023 19:16:32 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 01 Feb 2023 19:16:32 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Feb 2023 19:16:32 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 01 Feb 2023 19:16:32 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072b4eaa2b5682c7004efd6ccb6e88c462f0ea7270baf54965422fbd56e3d58b`  
		Last Modified: Wed, 01 Feb 2023 19:18:00 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2ccd67fa8db19ca641bafe4b2f46436e78c4a341db2835bf2e948c5a9b7e4a`  
		Last Modified: Wed, 01 Feb 2023 19:18:53 GMT  
		Size: 67.7 MB (67661313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90664d7068f7ab06678f38c2b7d553c07cb3de9d11ae6cabe3ad791eacecd541`  
		Last Modified: Wed, 01 Feb 2023 19:18:41 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.5-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:c403fe46663533549a50ef8c43d88e3cc996b7f8cb3ba32ebf2ce67e55116bb5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118361330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b376280a31b1da6c29f4d21df3ae39e2be2c9bec07db8f078291f41cec94a27`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:44:46 GMT
ARG ASSET=ce
# Wed, 01 Feb 2023 18:44:46 GMT
ENV ASSET=ce
# Wed, 01 Feb 2023 18:44:46 GMT
ARG EE_PORTS
# Wed, 01 Feb 2023 18:44:46 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 01 Feb 2023 18:45:36 GMT
ARG KONG_VERSION=2.5.2
# Wed, 01 Feb 2023 18:45:36 GMT
ENV KONG_VERSION=2.5.2
# Wed, 01 Feb 2023 18:45:36 GMT
ARG KONG_AMD64_SHA=ae65ac9eb35f682768abfb080c61581440347db8dafd0a495639ff666a406a96
# Wed, 01 Feb 2023 18:45:36 GMT
ARG KONG_ARM64_SHA=b4720e3d0831d13364cc749200c77df356a2145478f6a55fd48618a9aa1967d9
# Wed, 01 Feb 2023 18:45:52 GMT
# ARGS: KONG_AMD64_SHA=ae65ac9eb35f682768abfb080c61581440347db8dafd0a495639ff666a406a96 KONG_ARM64_SHA=b4720e3d0831d13364cc749200c77df356a2145478f6a55fd48618a9aa1967d9
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 01 Feb 2023 18:45:53 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 01 Feb 2023 18:45:53 GMT
USER kong
# Wed, 01 Feb 2023 18:45:53 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Feb 2023 18:45:53 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 01 Feb 2023 18:45:53 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Feb 2023 18:45:53 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 01 Feb 2023 18:45:54 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932a6b0f471e3c11d4540f1a320c68c9a8fc4fd47d236ea7d3ce0cf1970089a3`  
		Last Modified: Wed, 01 Feb 2023 18:47:15 GMT  
		Size: 25.1 MB (25081963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed898b509b7b648925b652fbc183d740e449827da9b564517c201a941c60d98`  
		Last Modified: Wed, 01 Feb 2023 18:48:02 GMT  
		Size: 66.1 MB (66084750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1165bc13dac0c2cae5fd709a05d702a4c42104e5df24e99acccc40fc36ea473`  
		Last Modified: Wed, 01 Feb 2023 18:47:52 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.5.2`

```console
$ docker pull kong@sha256:4d459bf9f353e69df80d660a7544d29583e77d5292f827137f6add87f74d2364
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
$ docker pull kong@sha256:934f0f609894a62d5ab41685863f02b29e7aa7d454b8e00482ed493fa32aaed1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.4 MB (48391762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ddbd7a976f9e47f0c736179c4fe225a32899cb86cebf1dd093bf993018a77e6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 22:40:04 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 10 Nov 2022 22:40:04 GMT
ARG ASSET=ce
# Thu, 10 Nov 2022 22:40:04 GMT
ENV ASSET=ce
# Thu, 10 Nov 2022 22:40:04 GMT
ARG EE_PORTS
# Thu, 10 Nov 2022 22:40:04 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 10 Nov 2022 22:40:29 GMT
ARG KONG_VERSION=2.5.2
# Thu, 10 Nov 2022 22:40:29 GMT
ENV KONG_VERSION=2.5.2
# Thu, 10 Nov 2022 22:40:29 GMT
ARG KONG_AMD64_SHA=d4bc93bcb14cce8c37ced136632a290b441050c540db779e742bcd88e5cfd70d
# Thu, 10 Nov 2022 22:40:29 GMT
ARG KONG_ARM64_SHA=691e1dc29e96d6a95b60674513932c4f7547773014685ce0130549f980c1c46e
# Thu, 10 Nov 2022 22:40:35 GMT
# ARGS: KONG_AMD64_SHA=d4bc93bcb14cce8c37ced136632a290b441050c540db779e742bcd88e5cfd70d KONG_ARM64_SHA=691e1dc29e96d6a95b60674513932c4f7547773014685ce0130549f980c1c46e
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 10 Nov 2022 22:40:35 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 10 Nov 2022 22:40:35 GMT
USER kong
# Thu, 10 Nov 2022 22:40:36 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 10 Nov 2022 22:40:36 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 10 Nov 2022 22:40:36 GMT
STOPSIGNAL SIGQUIT
# Thu, 10 Nov 2022 22:40:36 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 10 Nov 2022 22:40:36 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9f5eba777c2192f562d24cd3da16152dec7d8942677370e1524b03a6e36a2b`  
		Last Modified: Thu, 10 Nov 2022 22:41:58 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578c76f657afd39a075841d957e371975dda66e218c2055e95e692d64aa969ee`  
		Last Modified: Thu, 10 Nov 2022 22:42:47 GMT  
		Size: 45.7 MB (45672316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ad9797993253de6ac3a029a742d251a5445f0acc9ac38af3e937ae07078d3f`  
		Last Modified: Thu, 10 Nov 2022 22:42:40 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.5.2-alpine`

```console
$ docker pull kong@sha256:4d459bf9f353e69df80d660a7544d29583e77d5292f827137f6add87f74d2364
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
$ docker pull kong@sha256:934f0f609894a62d5ab41685863f02b29e7aa7d454b8e00482ed493fa32aaed1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.4 MB (48391762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ddbd7a976f9e47f0c736179c4fe225a32899cb86cebf1dd093bf993018a77e6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 22:40:04 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 10 Nov 2022 22:40:04 GMT
ARG ASSET=ce
# Thu, 10 Nov 2022 22:40:04 GMT
ENV ASSET=ce
# Thu, 10 Nov 2022 22:40:04 GMT
ARG EE_PORTS
# Thu, 10 Nov 2022 22:40:04 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 10 Nov 2022 22:40:29 GMT
ARG KONG_VERSION=2.5.2
# Thu, 10 Nov 2022 22:40:29 GMT
ENV KONG_VERSION=2.5.2
# Thu, 10 Nov 2022 22:40:29 GMT
ARG KONG_AMD64_SHA=d4bc93bcb14cce8c37ced136632a290b441050c540db779e742bcd88e5cfd70d
# Thu, 10 Nov 2022 22:40:29 GMT
ARG KONG_ARM64_SHA=691e1dc29e96d6a95b60674513932c4f7547773014685ce0130549f980c1c46e
# Thu, 10 Nov 2022 22:40:35 GMT
# ARGS: KONG_AMD64_SHA=d4bc93bcb14cce8c37ced136632a290b441050c540db779e742bcd88e5cfd70d KONG_ARM64_SHA=691e1dc29e96d6a95b60674513932c4f7547773014685ce0130549f980c1c46e
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 10 Nov 2022 22:40:35 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 10 Nov 2022 22:40:35 GMT
USER kong
# Thu, 10 Nov 2022 22:40:36 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 10 Nov 2022 22:40:36 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 10 Nov 2022 22:40:36 GMT
STOPSIGNAL SIGQUIT
# Thu, 10 Nov 2022 22:40:36 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 10 Nov 2022 22:40:36 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9f5eba777c2192f562d24cd3da16152dec7d8942677370e1524b03a6e36a2b`  
		Last Modified: Thu, 10 Nov 2022 22:41:58 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578c76f657afd39a075841d957e371975dda66e218c2055e95e692d64aa969ee`  
		Last Modified: Thu, 10 Nov 2022 22:42:47 GMT  
		Size: 45.7 MB (45672316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ad9797993253de6ac3a029a742d251a5445f0acc9ac38af3e937ae07078d3f`  
		Last Modified: Thu, 10 Nov 2022 22:42:40 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.5.2-ubuntu`

```console
$ docker pull kong@sha256:35fbe9f437ff098d994ae4043430815d9b6ea401ff03e205c028190390f03ec3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.5.2-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:7a6f68a9807b9aa1b5f78f232705e3c25f08b3b8e1450b7ca1d54e6a61ded9c7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121322032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:034c59249c73bc265b7db741b3b1274cebc2c2d3f8821439961846042079643e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 01 Feb 2023 11:42:37 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:42:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:42:39 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Wed, 01 Feb 2023 11:42:39 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 19:15:07 GMT
ARG ASSET=ce
# Wed, 01 Feb 2023 19:15:07 GMT
ENV ASSET=ce
# Wed, 01 Feb 2023 19:15:07 GMT
ARG EE_PORTS
# Wed, 01 Feb 2023 19:15:07 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 01 Feb 2023 19:16:07 GMT
ARG KONG_VERSION=2.5.2
# Wed, 01 Feb 2023 19:16:07 GMT
ENV KONG_VERSION=2.5.2
# Wed, 01 Feb 2023 19:16:07 GMT
ARG KONG_AMD64_SHA=ae65ac9eb35f682768abfb080c61581440347db8dafd0a495639ff666a406a96
# Wed, 01 Feb 2023 19:16:07 GMT
ARG KONG_ARM64_SHA=b4720e3d0831d13364cc749200c77df356a2145478f6a55fd48618a9aa1967d9
# Wed, 01 Feb 2023 19:16:31 GMT
# ARGS: KONG_AMD64_SHA=ae65ac9eb35f682768abfb080c61581440347db8dafd0a495639ff666a406a96 KONG_ARM64_SHA=b4720e3d0831d13364cc749200c77df356a2145478f6a55fd48618a9aa1967d9
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 01 Feb 2023 19:16:31 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 01 Feb 2023 19:16:32 GMT
USER kong
# Wed, 01 Feb 2023 19:16:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Feb 2023 19:16:32 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 01 Feb 2023 19:16:32 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Feb 2023 19:16:32 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 01 Feb 2023 19:16:32 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072b4eaa2b5682c7004efd6ccb6e88c462f0ea7270baf54965422fbd56e3d58b`  
		Last Modified: Wed, 01 Feb 2023 19:18:00 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2ccd67fa8db19ca641bafe4b2f46436e78c4a341db2835bf2e948c5a9b7e4a`  
		Last Modified: Wed, 01 Feb 2023 19:18:53 GMT  
		Size: 67.7 MB (67661313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90664d7068f7ab06678f38c2b7d553c07cb3de9d11ae6cabe3ad791eacecd541`  
		Last Modified: Wed, 01 Feb 2023 19:18:41 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.5.2-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:c403fe46663533549a50ef8c43d88e3cc996b7f8cb3ba32ebf2ce67e55116bb5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118361330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b376280a31b1da6c29f4d21df3ae39e2be2c9bec07db8f078291f41cec94a27`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:44:46 GMT
ARG ASSET=ce
# Wed, 01 Feb 2023 18:44:46 GMT
ENV ASSET=ce
# Wed, 01 Feb 2023 18:44:46 GMT
ARG EE_PORTS
# Wed, 01 Feb 2023 18:44:46 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 01 Feb 2023 18:45:36 GMT
ARG KONG_VERSION=2.5.2
# Wed, 01 Feb 2023 18:45:36 GMT
ENV KONG_VERSION=2.5.2
# Wed, 01 Feb 2023 18:45:36 GMT
ARG KONG_AMD64_SHA=ae65ac9eb35f682768abfb080c61581440347db8dafd0a495639ff666a406a96
# Wed, 01 Feb 2023 18:45:36 GMT
ARG KONG_ARM64_SHA=b4720e3d0831d13364cc749200c77df356a2145478f6a55fd48618a9aa1967d9
# Wed, 01 Feb 2023 18:45:52 GMT
# ARGS: KONG_AMD64_SHA=ae65ac9eb35f682768abfb080c61581440347db8dafd0a495639ff666a406a96 KONG_ARM64_SHA=b4720e3d0831d13364cc749200c77df356a2145478f6a55fd48618a9aa1967d9
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 01 Feb 2023 18:45:53 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 01 Feb 2023 18:45:53 GMT
USER kong
# Wed, 01 Feb 2023 18:45:53 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Feb 2023 18:45:53 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 01 Feb 2023 18:45:53 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Feb 2023 18:45:53 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 01 Feb 2023 18:45:54 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932a6b0f471e3c11d4540f1a320c68c9a8fc4fd47d236ea7d3ce0cf1970089a3`  
		Last Modified: Wed, 01 Feb 2023 18:47:15 GMT  
		Size: 25.1 MB (25081963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed898b509b7b648925b652fbc183d740e449827da9b564517c201a941c60d98`  
		Last Modified: Wed, 01 Feb 2023 18:48:02 GMT  
		Size: 66.1 MB (66084750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1165bc13dac0c2cae5fd709a05d702a4c42104e5df24e99acccc40fc36ea473`  
		Last Modified: Wed, 01 Feb 2023 18:47:52 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.6`

```console
$ docker pull kong@sha256:62eb6d17133b007cbf5831b39197c669b8700c55283270395b876d1ecfd69a70
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
$ docker pull kong@sha256:607d9bdc48adf88bcee03b5dfa77a2d7d8293c803e12c97c897a129b27e6a669
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49626411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:119c7b9aedaeb47ed122d6ec970ab5c7214b29169221bfdb9cfe7a7602e49454`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 22:40:04 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 10 Nov 2022 22:40:04 GMT
ARG ASSET=ce
# Thu, 10 Nov 2022 22:40:04 GMT
ENV ASSET=ce
# Thu, 10 Nov 2022 22:40:04 GMT
ARG EE_PORTS
# Thu, 10 Nov 2022 22:40:04 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 10 Nov 2022 22:40:17 GMT
ARG KONG_VERSION=2.6.1
# Thu, 10 Nov 2022 22:40:17 GMT
ENV KONG_VERSION=2.6.1
# Thu, 10 Nov 2022 22:40:18 GMT
ARG KONG_AMD64_SHA=9e7618ad06c148ed216be8bbf65a9c7cb95301e5349ef61b996fbb55ec4cfa87
# Thu, 10 Nov 2022 22:40:18 GMT
ARG KONG_ARM64_SHA=0fbf008685c6eac510d221595172e9e7bd51a846d410972d6950d9207cf400de
# Thu, 10 Nov 2022 22:40:23 GMT
# ARGS: KONG_AMD64_SHA=9e7618ad06c148ed216be8bbf65a9c7cb95301e5349ef61b996fbb55ec4cfa87 KONG_ARM64_SHA=0fbf008685c6eac510d221595172e9e7bd51a846d410972d6950d9207cf400de
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 10 Nov 2022 22:40:24 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 10 Nov 2022 22:40:24 GMT
USER kong
# Thu, 10 Nov 2022 22:40:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 10 Nov 2022 22:40:24 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 10 Nov 2022 22:40:24 GMT
STOPSIGNAL SIGQUIT
# Thu, 10 Nov 2022 22:40:25 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 10 Nov 2022 22:40:25 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9f5eba777c2192f562d24cd3da16152dec7d8942677370e1524b03a6e36a2b`  
		Last Modified: Thu, 10 Nov 2022 22:41:58 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9dc6c1f293dd1473f1dd7e3176777c7089b6bdcebd2c879cbc2a0040daf2bf2`  
		Last Modified: Thu, 10 Nov 2022 22:42:28 GMT  
		Size: 46.9 MB (46906964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7605604f20571f531c42364dbfc0858fe97409b5faa3f8407a409e04c2946b7`  
		Last Modified: Thu, 10 Nov 2022 22:42:21 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.6-ubuntu`

```console
$ docker pull kong@sha256:681d9648fe1d11bb70fb41d9f4a1b0d86f4ee2aa1e837d8ae8c522d8f8b45065
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.6-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:6baab70d45d0ff8c50cd2d7678e06186f1529aa2966d0de643cb99605aa31fb9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128209529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d003d033a257b9b41eca91d900869068fb8949e9b5e3cffe7645b31172f64306`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 01 Feb 2023 11:42:37 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:42:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:42:39 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Wed, 01 Feb 2023 11:42:39 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 19:15:07 GMT
ARG ASSET=ce
# Wed, 01 Feb 2023 19:15:07 GMT
ENV ASSET=ce
# Wed, 01 Feb 2023 19:15:07 GMT
ARG EE_PORTS
# Wed, 01 Feb 2023 19:15:07 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 01 Feb 2023 19:15:37 GMT
ARG KONG_VERSION=2.6.1
# Wed, 01 Feb 2023 19:15:37 GMT
ENV KONG_VERSION=2.6.1
# Wed, 01 Feb 2023 19:15:37 GMT
ARG KONG_AMD64_SHA=f70757f9317a1d40316f0187ae6e91c0c94b5b4346e564f7ae8430775bf7ad7e
# Wed, 01 Feb 2023 19:15:37 GMT
ARG KONG_ARM64_SHA=5cba6e7e28685fb7d80b77b70586cfb92c1de4b5198a6218bb1ca0c7f2502c89
# Wed, 01 Feb 2023 19:15:58 GMT
# ARGS: KONG_AMD64_SHA=f70757f9317a1d40316f0187ae6e91c0c94b5b4346e564f7ae8430775bf7ad7e KONG_ARM64_SHA=5cba6e7e28685fb7d80b77b70586cfb92c1de4b5198a6218bb1ca0c7f2502c89
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 01 Feb 2023 19:15:59 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 01 Feb 2023 19:15:59 GMT
USER kong
# Wed, 01 Feb 2023 19:15:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Feb 2023 19:15:59 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 01 Feb 2023 19:15:59 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Feb 2023 19:15:59 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 01 Feb 2023 19:15:59 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072b4eaa2b5682c7004efd6ccb6e88c462f0ea7270baf54965422fbd56e3d58b`  
		Last Modified: Wed, 01 Feb 2023 19:18:00 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5f2da2983c2d98a171c6e46c44ba0620a37d4fc18747ef402601b17cfee336`  
		Last Modified: Wed, 01 Feb 2023 19:18:32 GMT  
		Size: 74.5 MB (74548810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab354b652070024db6e53b31e87b253b391d6cac90e6bb85d0a97f6e65c9138`  
		Last Modified: Wed, 01 Feb 2023 19:18:20 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.6-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:daa785b57c1679ece84578e217d870eba958fafeb14e64aaaa4ad8e1947f3b26
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125250376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e8f686caff9495cc0ca89c6c469f57b38e31c75d6c23b71ac1bddfd3aa13c36`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:44:46 GMT
ARG ASSET=ce
# Wed, 01 Feb 2023 18:44:46 GMT
ENV ASSET=ce
# Wed, 01 Feb 2023 18:44:46 GMT
ARG EE_PORTS
# Wed, 01 Feb 2023 18:44:46 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 01 Feb 2023 18:45:11 GMT
ARG KONG_VERSION=2.6.1
# Wed, 01 Feb 2023 18:45:11 GMT
ENV KONG_VERSION=2.6.1
# Wed, 01 Feb 2023 18:45:11 GMT
ARG KONG_AMD64_SHA=f70757f9317a1d40316f0187ae6e91c0c94b5b4346e564f7ae8430775bf7ad7e
# Wed, 01 Feb 2023 18:45:11 GMT
ARG KONG_ARM64_SHA=5cba6e7e28685fb7d80b77b70586cfb92c1de4b5198a6218bb1ca0c7f2502c89
# Wed, 01 Feb 2023 18:45:27 GMT
# ARGS: KONG_AMD64_SHA=f70757f9317a1d40316f0187ae6e91c0c94b5b4346e564f7ae8430775bf7ad7e KONG_ARM64_SHA=5cba6e7e28685fb7d80b77b70586cfb92c1de4b5198a6218bb1ca0c7f2502c89
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 01 Feb 2023 18:45:28 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 01 Feb 2023 18:45:29 GMT
USER kong
# Wed, 01 Feb 2023 18:45:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Feb 2023 18:45:29 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 01 Feb 2023 18:45:29 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Feb 2023 18:45:29 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 01 Feb 2023 18:45:29 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932a6b0f471e3c11d4540f1a320c68c9a8fc4fd47d236ea7d3ce0cf1970089a3`  
		Last Modified: Wed, 01 Feb 2023 18:47:15 GMT  
		Size: 25.1 MB (25081963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f4e46a3589846fd358faf31fdcdf0d7dc3271755a3ee6ec3699741757f3b8d`  
		Last Modified: Wed, 01 Feb 2023 18:47:42 GMT  
		Size: 73.0 MB (72973794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88024e9e7f16bad8deb4e994dd476b794a156be3e67c19c80b27d771c08a909e`  
		Last Modified: Wed, 01 Feb 2023 18:47:33 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.6.1`

```console
$ docker pull kong@sha256:62eb6d17133b007cbf5831b39197c669b8700c55283270395b876d1ecfd69a70
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
$ docker pull kong@sha256:607d9bdc48adf88bcee03b5dfa77a2d7d8293c803e12c97c897a129b27e6a669
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49626411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:119c7b9aedaeb47ed122d6ec970ab5c7214b29169221bfdb9cfe7a7602e49454`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 22:40:04 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 10 Nov 2022 22:40:04 GMT
ARG ASSET=ce
# Thu, 10 Nov 2022 22:40:04 GMT
ENV ASSET=ce
# Thu, 10 Nov 2022 22:40:04 GMT
ARG EE_PORTS
# Thu, 10 Nov 2022 22:40:04 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 10 Nov 2022 22:40:17 GMT
ARG KONG_VERSION=2.6.1
# Thu, 10 Nov 2022 22:40:17 GMT
ENV KONG_VERSION=2.6.1
# Thu, 10 Nov 2022 22:40:18 GMT
ARG KONG_AMD64_SHA=9e7618ad06c148ed216be8bbf65a9c7cb95301e5349ef61b996fbb55ec4cfa87
# Thu, 10 Nov 2022 22:40:18 GMT
ARG KONG_ARM64_SHA=0fbf008685c6eac510d221595172e9e7bd51a846d410972d6950d9207cf400de
# Thu, 10 Nov 2022 22:40:23 GMT
# ARGS: KONG_AMD64_SHA=9e7618ad06c148ed216be8bbf65a9c7cb95301e5349ef61b996fbb55ec4cfa87 KONG_ARM64_SHA=0fbf008685c6eac510d221595172e9e7bd51a846d410972d6950d9207cf400de
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 10 Nov 2022 22:40:24 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 10 Nov 2022 22:40:24 GMT
USER kong
# Thu, 10 Nov 2022 22:40:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 10 Nov 2022 22:40:24 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 10 Nov 2022 22:40:24 GMT
STOPSIGNAL SIGQUIT
# Thu, 10 Nov 2022 22:40:25 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 10 Nov 2022 22:40:25 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9f5eba777c2192f562d24cd3da16152dec7d8942677370e1524b03a6e36a2b`  
		Last Modified: Thu, 10 Nov 2022 22:41:58 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9dc6c1f293dd1473f1dd7e3176777c7089b6bdcebd2c879cbc2a0040daf2bf2`  
		Last Modified: Thu, 10 Nov 2022 22:42:28 GMT  
		Size: 46.9 MB (46906964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7605604f20571f531c42364dbfc0858fe97409b5faa3f8407a409e04c2946b7`  
		Last Modified: Thu, 10 Nov 2022 22:42:21 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.6.1-alpine`

```console
$ docker pull kong@sha256:62eb6d17133b007cbf5831b39197c669b8700c55283270395b876d1ecfd69a70
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
$ docker pull kong@sha256:607d9bdc48adf88bcee03b5dfa77a2d7d8293c803e12c97c897a129b27e6a669
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49626411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:119c7b9aedaeb47ed122d6ec970ab5c7214b29169221bfdb9cfe7a7602e49454`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 22:40:04 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 10 Nov 2022 22:40:04 GMT
ARG ASSET=ce
# Thu, 10 Nov 2022 22:40:04 GMT
ENV ASSET=ce
# Thu, 10 Nov 2022 22:40:04 GMT
ARG EE_PORTS
# Thu, 10 Nov 2022 22:40:04 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 10 Nov 2022 22:40:17 GMT
ARG KONG_VERSION=2.6.1
# Thu, 10 Nov 2022 22:40:17 GMT
ENV KONG_VERSION=2.6.1
# Thu, 10 Nov 2022 22:40:18 GMT
ARG KONG_AMD64_SHA=9e7618ad06c148ed216be8bbf65a9c7cb95301e5349ef61b996fbb55ec4cfa87
# Thu, 10 Nov 2022 22:40:18 GMT
ARG KONG_ARM64_SHA=0fbf008685c6eac510d221595172e9e7bd51a846d410972d6950d9207cf400de
# Thu, 10 Nov 2022 22:40:23 GMT
# ARGS: KONG_AMD64_SHA=9e7618ad06c148ed216be8bbf65a9c7cb95301e5349ef61b996fbb55ec4cfa87 KONG_ARM64_SHA=0fbf008685c6eac510d221595172e9e7bd51a846d410972d6950d9207cf400de
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 10 Nov 2022 22:40:24 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 10 Nov 2022 22:40:24 GMT
USER kong
# Thu, 10 Nov 2022 22:40:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 10 Nov 2022 22:40:24 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 10 Nov 2022 22:40:24 GMT
STOPSIGNAL SIGQUIT
# Thu, 10 Nov 2022 22:40:25 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 10 Nov 2022 22:40:25 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9f5eba777c2192f562d24cd3da16152dec7d8942677370e1524b03a6e36a2b`  
		Last Modified: Thu, 10 Nov 2022 22:41:58 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9dc6c1f293dd1473f1dd7e3176777c7089b6bdcebd2c879cbc2a0040daf2bf2`  
		Last Modified: Thu, 10 Nov 2022 22:42:28 GMT  
		Size: 46.9 MB (46906964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7605604f20571f531c42364dbfc0858fe97409b5faa3f8407a409e04c2946b7`  
		Last Modified: Thu, 10 Nov 2022 22:42:21 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.6.1-ubuntu`

```console
$ docker pull kong@sha256:681d9648fe1d11bb70fb41d9f4a1b0d86f4ee2aa1e837d8ae8c522d8f8b45065
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.6.1-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:6baab70d45d0ff8c50cd2d7678e06186f1529aa2966d0de643cb99605aa31fb9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128209529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d003d033a257b9b41eca91d900869068fb8949e9b5e3cffe7645b31172f64306`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 01 Feb 2023 11:42:37 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:42:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:42:39 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Wed, 01 Feb 2023 11:42:39 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 19:15:07 GMT
ARG ASSET=ce
# Wed, 01 Feb 2023 19:15:07 GMT
ENV ASSET=ce
# Wed, 01 Feb 2023 19:15:07 GMT
ARG EE_PORTS
# Wed, 01 Feb 2023 19:15:07 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 01 Feb 2023 19:15:37 GMT
ARG KONG_VERSION=2.6.1
# Wed, 01 Feb 2023 19:15:37 GMT
ENV KONG_VERSION=2.6.1
# Wed, 01 Feb 2023 19:15:37 GMT
ARG KONG_AMD64_SHA=f70757f9317a1d40316f0187ae6e91c0c94b5b4346e564f7ae8430775bf7ad7e
# Wed, 01 Feb 2023 19:15:37 GMT
ARG KONG_ARM64_SHA=5cba6e7e28685fb7d80b77b70586cfb92c1de4b5198a6218bb1ca0c7f2502c89
# Wed, 01 Feb 2023 19:15:58 GMT
# ARGS: KONG_AMD64_SHA=f70757f9317a1d40316f0187ae6e91c0c94b5b4346e564f7ae8430775bf7ad7e KONG_ARM64_SHA=5cba6e7e28685fb7d80b77b70586cfb92c1de4b5198a6218bb1ca0c7f2502c89
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 01 Feb 2023 19:15:59 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 01 Feb 2023 19:15:59 GMT
USER kong
# Wed, 01 Feb 2023 19:15:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Feb 2023 19:15:59 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 01 Feb 2023 19:15:59 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Feb 2023 19:15:59 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 01 Feb 2023 19:15:59 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072b4eaa2b5682c7004efd6ccb6e88c462f0ea7270baf54965422fbd56e3d58b`  
		Last Modified: Wed, 01 Feb 2023 19:18:00 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5f2da2983c2d98a171c6e46c44ba0620a37d4fc18747ef402601b17cfee336`  
		Last Modified: Wed, 01 Feb 2023 19:18:32 GMT  
		Size: 74.5 MB (74548810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab354b652070024db6e53b31e87b253b391d6cac90e6bb85d0a97f6e65c9138`  
		Last Modified: Wed, 01 Feb 2023 19:18:20 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.6.1-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:daa785b57c1679ece84578e217d870eba958fafeb14e64aaaa4ad8e1947f3b26
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125250376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e8f686caff9495cc0ca89c6c469f57b38e31c75d6c23b71ac1bddfd3aa13c36`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:44:46 GMT
ARG ASSET=ce
# Wed, 01 Feb 2023 18:44:46 GMT
ENV ASSET=ce
# Wed, 01 Feb 2023 18:44:46 GMT
ARG EE_PORTS
# Wed, 01 Feb 2023 18:44:46 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 01 Feb 2023 18:45:11 GMT
ARG KONG_VERSION=2.6.1
# Wed, 01 Feb 2023 18:45:11 GMT
ENV KONG_VERSION=2.6.1
# Wed, 01 Feb 2023 18:45:11 GMT
ARG KONG_AMD64_SHA=f70757f9317a1d40316f0187ae6e91c0c94b5b4346e564f7ae8430775bf7ad7e
# Wed, 01 Feb 2023 18:45:11 GMT
ARG KONG_ARM64_SHA=5cba6e7e28685fb7d80b77b70586cfb92c1de4b5198a6218bb1ca0c7f2502c89
# Wed, 01 Feb 2023 18:45:27 GMT
# ARGS: KONG_AMD64_SHA=f70757f9317a1d40316f0187ae6e91c0c94b5b4346e564f7ae8430775bf7ad7e KONG_ARM64_SHA=5cba6e7e28685fb7d80b77b70586cfb92c1de4b5198a6218bb1ca0c7f2502c89
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 01 Feb 2023 18:45:28 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 01 Feb 2023 18:45:29 GMT
USER kong
# Wed, 01 Feb 2023 18:45:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Feb 2023 18:45:29 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 01 Feb 2023 18:45:29 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Feb 2023 18:45:29 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 01 Feb 2023 18:45:29 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932a6b0f471e3c11d4540f1a320c68c9a8fc4fd47d236ea7d3ce0cf1970089a3`  
		Last Modified: Wed, 01 Feb 2023 18:47:15 GMT  
		Size: 25.1 MB (25081963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f4e46a3589846fd358faf31fdcdf0d7dc3271755a3ee6ec3699741757f3b8d`  
		Last Modified: Wed, 01 Feb 2023 18:47:42 GMT  
		Size: 73.0 MB (72973794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88024e9e7f16bad8deb4e994dd476b794a156be3e67c19c80b27d771c08a909e`  
		Last Modified: Wed, 01 Feb 2023 18:47:33 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.7`

```console
$ docker pull kong@sha256:95cbba86c8addbfee6726b5a7743ab9bb8158c4a801caa75aafe3fe03992f170
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
$ docker pull kong@sha256:7c35b5df861fc05fc12db8f1c7f98f5b07d1490f9bce31d0a58edea1098c466c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49544935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee3bd472c5d632ebf186555ef7b7d99ef7ba814308a256a1ec8a7367f9924db7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 22:40:04 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 10 Nov 2022 22:40:04 GMT
ARG ASSET=ce
# Thu, 10 Nov 2022 22:40:04 GMT
ENV ASSET=ce
# Thu, 10 Nov 2022 22:40:04 GMT
ARG EE_PORTS
# Thu, 10 Nov 2022 22:40:04 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 10 Nov 2022 22:40:05 GMT
ARG KONG_VERSION=2.7.2
# Thu, 10 Nov 2022 22:40:05 GMT
ENV KONG_VERSION=2.7.2
# Thu, 10 Nov 2022 22:40:05 GMT
ARG KONG_AMD64_SHA=16990765aee26fc194992f0f90fc81e78a46d77cd0fc1e6670f3b2f797c1fe6b
# Thu, 10 Nov 2022 22:40:05 GMT
ARG KONG_ARM64_SHA=3e5dde2479d53299e81dd903a04e30302108b0864c996a3662fda24ca7aee9f6
# Thu, 10 Nov 2022 22:40:11 GMT
# ARGS: KONG_AMD64_SHA=16990765aee26fc194992f0f90fc81e78a46d77cd0fc1e6670f3b2f797c1fe6b KONG_ARM64_SHA=3e5dde2479d53299e81dd903a04e30302108b0864c996a3662fda24ca7aee9f6
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 10 Nov 2022 22:40:12 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 10 Nov 2022 22:40:12 GMT
USER kong
# Thu, 10 Nov 2022 22:40:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 10 Nov 2022 22:40:12 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 10 Nov 2022 22:40:12 GMT
STOPSIGNAL SIGQUIT
# Thu, 10 Nov 2022 22:40:12 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 10 Nov 2022 22:40:12 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9f5eba777c2192f562d24cd3da16152dec7d8942677370e1524b03a6e36a2b`  
		Last Modified: Thu, 10 Nov 2022 22:41:58 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14140154bb3de6de0062d495454ecbf830c029091e8d80c241b3d684de9e2f6f`  
		Last Modified: Thu, 10 Nov 2022 22:42:05 GMT  
		Size: 46.8 MB (46825491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7424b484ab8703ef3d0f7813540b8ce7e9de2dc487b6d9ae31593abecc0b9f44`  
		Last Modified: Thu, 10 Nov 2022 22:41:58 GMT  
		Size: 878.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.7-ubuntu`

```console
$ docker pull kong@sha256:6cc0e033edffbc99f1cc4708d0d77694b0e51aa85ee47164cb97e006d93871b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.7-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:48d67b6a2b115752de1675da5d2e476f4a1dd0c330b76840713e59cdafa433bc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.1 MB (128114844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a303de445c182d63c0d0aa56b343bae28ee491cde033e3103388ff3de847573`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 01 Feb 2023 11:42:37 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:42:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:42:39 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Wed, 01 Feb 2023 11:42:39 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 19:15:07 GMT
ARG ASSET=ce
# Wed, 01 Feb 2023 19:15:07 GMT
ENV ASSET=ce
# Wed, 01 Feb 2023 19:15:07 GMT
ARG EE_PORTS
# Wed, 01 Feb 2023 19:15:07 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 01 Feb 2023 19:15:07 GMT
ARG KONG_VERSION=2.7.2
# Wed, 01 Feb 2023 19:15:07 GMT
ENV KONG_VERSION=2.7.2
# Wed, 01 Feb 2023 19:15:08 GMT
ARG KONG_AMD64_SHA=8124ddbfe80a1627b19a54e14b20ff0e176549699491cf5c61a4f0355470f8fc
# Wed, 01 Feb 2023 19:15:08 GMT
ARG KONG_ARM64_SHA=f40e616539ab64cb4fd333d19895ec9768b742bc25e5f2dbcb7f162bf90421d8
# Wed, 01 Feb 2023 19:15:28 GMT
# ARGS: KONG_AMD64_SHA=8124ddbfe80a1627b19a54e14b20ff0e176549699491cf5c61a4f0355470f8fc KONG_ARM64_SHA=f40e616539ab64cb4fd333d19895ec9768b742bc25e5f2dbcb7f162bf90421d8
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 01 Feb 2023 19:15:29 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 01 Feb 2023 19:15:29 GMT
USER kong
# Wed, 01 Feb 2023 19:15:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Feb 2023 19:15:30 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 01 Feb 2023 19:15:30 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Feb 2023 19:15:30 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 01 Feb 2023 19:15:30 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072b4eaa2b5682c7004efd6ccb6e88c462f0ea7270baf54965422fbd56e3d58b`  
		Last Modified: Wed, 01 Feb 2023 19:18:00 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672e097467ff2355b497b4fd0ba431bffe58789abcd0c77ae6ccef509f8af274`  
		Last Modified: Wed, 01 Feb 2023 19:18:10 GMT  
		Size: 74.5 MB (74454125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09980069b9e0e2dcb6a918acfc80f1f06490b7c88b415423ac261df0bb6ae0f`  
		Last Modified: Wed, 01 Feb 2023 19:17:58 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.7-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:36702ed887b6953cbcc46e4e8ee6be7c577a8196d865c42a1b26354ec4874404
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125159180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71a06a709e6d688eae904192fa8499a7c470b01d6f6d74ffbdbca05b6a992774`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:44:46 GMT
ARG ASSET=ce
# Wed, 01 Feb 2023 18:44:46 GMT
ENV ASSET=ce
# Wed, 01 Feb 2023 18:44:46 GMT
ARG EE_PORTS
# Wed, 01 Feb 2023 18:44:46 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 01 Feb 2023 18:44:46 GMT
ARG KONG_VERSION=2.7.2
# Wed, 01 Feb 2023 18:44:47 GMT
ENV KONG_VERSION=2.7.2
# Wed, 01 Feb 2023 18:44:47 GMT
ARG KONG_AMD64_SHA=8124ddbfe80a1627b19a54e14b20ff0e176549699491cf5c61a4f0355470f8fc
# Wed, 01 Feb 2023 18:44:47 GMT
ARG KONG_ARM64_SHA=f40e616539ab64cb4fd333d19895ec9768b742bc25e5f2dbcb7f162bf90421d8
# Wed, 01 Feb 2023 18:45:04 GMT
# ARGS: KONG_AMD64_SHA=8124ddbfe80a1627b19a54e14b20ff0e176549699491cf5c61a4f0355470f8fc KONG_ARM64_SHA=f40e616539ab64cb4fd333d19895ec9768b742bc25e5f2dbcb7f162bf90421d8
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 01 Feb 2023 18:45:05 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 01 Feb 2023 18:45:05 GMT
USER kong
# Wed, 01 Feb 2023 18:45:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Feb 2023 18:45:05 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 01 Feb 2023 18:45:05 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Feb 2023 18:45:05 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 01 Feb 2023 18:45:05 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932a6b0f471e3c11d4540f1a320c68c9a8fc4fd47d236ea7d3ce0cf1970089a3`  
		Last Modified: Wed, 01 Feb 2023 18:47:15 GMT  
		Size: 25.1 MB (25081963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48d9b56d4d5d1190059c41d0eae91ff6943ef1b831f4ee5d0530ecd8aa9c1c95`  
		Last Modified: Wed, 01 Feb 2023 18:47:23 GMT  
		Size: 72.9 MB (72882602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9393375ddd21b48773c2090577639a9182d7c396f9657db82768f6587eb2c7ab`  
		Last Modified: Wed, 01 Feb 2023 18:47:13 GMT  
		Size: 878.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.7.2`

```console
$ docker pull kong@sha256:95cbba86c8addbfee6726b5a7743ab9bb8158c4a801caa75aafe3fe03992f170
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
$ docker pull kong@sha256:7c35b5df861fc05fc12db8f1c7f98f5b07d1490f9bce31d0a58edea1098c466c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49544935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee3bd472c5d632ebf186555ef7b7d99ef7ba814308a256a1ec8a7367f9924db7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 22:40:04 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 10 Nov 2022 22:40:04 GMT
ARG ASSET=ce
# Thu, 10 Nov 2022 22:40:04 GMT
ENV ASSET=ce
# Thu, 10 Nov 2022 22:40:04 GMT
ARG EE_PORTS
# Thu, 10 Nov 2022 22:40:04 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 10 Nov 2022 22:40:05 GMT
ARG KONG_VERSION=2.7.2
# Thu, 10 Nov 2022 22:40:05 GMT
ENV KONG_VERSION=2.7.2
# Thu, 10 Nov 2022 22:40:05 GMT
ARG KONG_AMD64_SHA=16990765aee26fc194992f0f90fc81e78a46d77cd0fc1e6670f3b2f797c1fe6b
# Thu, 10 Nov 2022 22:40:05 GMT
ARG KONG_ARM64_SHA=3e5dde2479d53299e81dd903a04e30302108b0864c996a3662fda24ca7aee9f6
# Thu, 10 Nov 2022 22:40:11 GMT
# ARGS: KONG_AMD64_SHA=16990765aee26fc194992f0f90fc81e78a46d77cd0fc1e6670f3b2f797c1fe6b KONG_ARM64_SHA=3e5dde2479d53299e81dd903a04e30302108b0864c996a3662fda24ca7aee9f6
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 10 Nov 2022 22:40:12 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 10 Nov 2022 22:40:12 GMT
USER kong
# Thu, 10 Nov 2022 22:40:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 10 Nov 2022 22:40:12 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 10 Nov 2022 22:40:12 GMT
STOPSIGNAL SIGQUIT
# Thu, 10 Nov 2022 22:40:12 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 10 Nov 2022 22:40:12 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9f5eba777c2192f562d24cd3da16152dec7d8942677370e1524b03a6e36a2b`  
		Last Modified: Thu, 10 Nov 2022 22:41:58 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14140154bb3de6de0062d495454ecbf830c029091e8d80c241b3d684de9e2f6f`  
		Last Modified: Thu, 10 Nov 2022 22:42:05 GMT  
		Size: 46.8 MB (46825491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7424b484ab8703ef3d0f7813540b8ce7e9de2dc487b6d9ae31593abecc0b9f44`  
		Last Modified: Thu, 10 Nov 2022 22:41:58 GMT  
		Size: 878.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.7.2-alpine`

```console
$ docker pull kong@sha256:95cbba86c8addbfee6726b5a7743ab9bb8158c4a801caa75aafe3fe03992f170
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
$ docker pull kong@sha256:7c35b5df861fc05fc12db8f1c7f98f5b07d1490f9bce31d0a58edea1098c466c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49544935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee3bd472c5d632ebf186555ef7b7d99ef7ba814308a256a1ec8a7367f9924db7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 22:40:04 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 10 Nov 2022 22:40:04 GMT
ARG ASSET=ce
# Thu, 10 Nov 2022 22:40:04 GMT
ENV ASSET=ce
# Thu, 10 Nov 2022 22:40:04 GMT
ARG EE_PORTS
# Thu, 10 Nov 2022 22:40:04 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 10 Nov 2022 22:40:05 GMT
ARG KONG_VERSION=2.7.2
# Thu, 10 Nov 2022 22:40:05 GMT
ENV KONG_VERSION=2.7.2
# Thu, 10 Nov 2022 22:40:05 GMT
ARG KONG_AMD64_SHA=16990765aee26fc194992f0f90fc81e78a46d77cd0fc1e6670f3b2f797c1fe6b
# Thu, 10 Nov 2022 22:40:05 GMT
ARG KONG_ARM64_SHA=3e5dde2479d53299e81dd903a04e30302108b0864c996a3662fda24ca7aee9f6
# Thu, 10 Nov 2022 22:40:11 GMT
# ARGS: KONG_AMD64_SHA=16990765aee26fc194992f0f90fc81e78a46d77cd0fc1e6670f3b2f797c1fe6b KONG_ARM64_SHA=3e5dde2479d53299e81dd903a04e30302108b0864c996a3662fda24ca7aee9f6
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 10 Nov 2022 22:40:12 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 10 Nov 2022 22:40:12 GMT
USER kong
# Thu, 10 Nov 2022 22:40:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 10 Nov 2022 22:40:12 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 10 Nov 2022 22:40:12 GMT
STOPSIGNAL SIGQUIT
# Thu, 10 Nov 2022 22:40:12 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 10 Nov 2022 22:40:12 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9f5eba777c2192f562d24cd3da16152dec7d8942677370e1524b03a6e36a2b`  
		Last Modified: Thu, 10 Nov 2022 22:41:58 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14140154bb3de6de0062d495454ecbf830c029091e8d80c241b3d684de9e2f6f`  
		Last Modified: Thu, 10 Nov 2022 22:42:05 GMT  
		Size: 46.8 MB (46825491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7424b484ab8703ef3d0f7813540b8ce7e9de2dc487b6d9ae31593abecc0b9f44`  
		Last Modified: Thu, 10 Nov 2022 22:41:58 GMT  
		Size: 878.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.7.2-ubuntu`

```console
$ docker pull kong@sha256:6cc0e033edffbc99f1cc4708d0d77694b0e51aa85ee47164cb97e006d93871b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.7.2-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:48d67b6a2b115752de1675da5d2e476f4a1dd0c330b76840713e59cdafa433bc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.1 MB (128114844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a303de445c182d63c0d0aa56b343bae28ee491cde033e3103388ff3de847573`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 01 Feb 2023 11:42:37 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:42:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:42:39 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Wed, 01 Feb 2023 11:42:39 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 19:15:07 GMT
ARG ASSET=ce
# Wed, 01 Feb 2023 19:15:07 GMT
ENV ASSET=ce
# Wed, 01 Feb 2023 19:15:07 GMT
ARG EE_PORTS
# Wed, 01 Feb 2023 19:15:07 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 01 Feb 2023 19:15:07 GMT
ARG KONG_VERSION=2.7.2
# Wed, 01 Feb 2023 19:15:07 GMT
ENV KONG_VERSION=2.7.2
# Wed, 01 Feb 2023 19:15:08 GMT
ARG KONG_AMD64_SHA=8124ddbfe80a1627b19a54e14b20ff0e176549699491cf5c61a4f0355470f8fc
# Wed, 01 Feb 2023 19:15:08 GMT
ARG KONG_ARM64_SHA=f40e616539ab64cb4fd333d19895ec9768b742bc25e5f2dbcb7f162bf90421d8
# Wed, 01 Feb 2023 19:15:28 GMT
# ARGS: KONG_AMD64_SHA=8124ddbfe80a1627b19a54e14b20ff0e176549699491cf5c61a4f0355470f8fc KONG_ARM64_SHA=f40e616539ab64cb4fd333d19895ec9768b742bc25e5f2dbcb7f162bf90421d8
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 01 Feb 2023 19:15:29 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 01 Feb 2023 19:15:29 GMT
USER kong
# Wed, 01 Feb 2023 19:15:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Feb 2023 19:15:30 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 01 Feb 2023 19:15:30 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Feb 2023 19:15:30 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 01 Feb 2023 19:15:30 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072b4eaa2b5682c7004efd6ccb6e88c462f0ea7270baf54965422fbd56e3d58b`  
		Last Modified: Wed, 01 Feb 2023 19:18:00 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672e097467ff2355b497b4fd0ba431bffe58789abcd0c77ae6ccef509f8af274`  
		Last Modified: Wed, 01 Feb 2023 19:18:10 GMT  
		Size: 74.5 MB (74454125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09980069b9e0e2dcb6a918acfc80f1f06490b7c88b415423ac261df0bb6ae0f`  
		Last Modified: Wed, 01 Feb 2023 19:17:58 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.7.2-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:36702ed887b6953cbcc46e4e8ee6be7c577a8196d865c42a1b26354ec4874404
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125159180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71a06a709e6d688eae904192fa8499a7c470b01d6f6d74ffbdbca05b6a992774`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:44:46 GMT
ARG ASSET=ce
# Wed, 01 Feb 2023 18:44:46 GMT
ENV ASSET=ce
# Wed, 01 Feb 2023 18:44:46 GMT
ARG EE_PORTS
# Wed, 01 Feb 2023 18:44:46 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 01 Feb 2023 18:44:46 GMT
ARG KONG_VERSION=2.7.2
# Wed, 01 Feb 2023 18:44:47 GMT
ENV KONG_VERSION=2.7.2
# Wed, 01 Feb 2023 18:44:47 GMT
ARG KONG_AMD64_SHA=8124ddbfe80a1627b19a54e14b20ff0e176549699491cf5c61a4f0355470f8fc
# Wed, 01 Feb 2023 18:44:47 GMT
ARG KONG_ARM64_SHA=f40e616539ab64cb4fd333d19895ec9768b742bc25e5f2dbcb7f162bf90421d8
# Wed, 01 Feb 2023 18:45:04 GMT
# ARGS: KONG_AMD64_SHA=8124ddbfe80a1627b19a54e14b20ff0e176549699491cf5c61a4f0355470f8fc KONG_ARM64_SHA=f40e616539ab64cb4fd333d19895ec9768b742bc25e5f2dbcb7f162bf90421d8
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 01 Feb 2023 18:45:05 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 01 Feb 2023 18:45:05 GMT
USER kong
# Wed, 01 Feb 2023 18:45:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Feb 2023 18:45:05 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 01 Feb 2023 18:45:05 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Feb 2023 18:45:05 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 01 Feb 2023 18:45:05 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:932a6b0f471e3c11d4540f1a320c68c9a8fc4fd47d236ea7d3ce0cf1970089a3`  
		Last Modified: Wed, 01 Feb 2023 18:47:15 GMT  
		Size: 25.1 MB (25081963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48d9b56d4d5d1190059c41d0eae91ff6943ef1b831f4ee5d0530ecd8aa9c1c95`  
		Last Modified: Wed, 01 Feb 2023 18:47:23 GMT  
		Size: 72.9 MB (72882602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9393375ddd21b48773c2090577639a9182d7c396f9657db82768f6587eb2c7ab`  
		Last Modified: Wed, 01 Feb 2023 18:47:13 GMT  
		Size: 878.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.8`

```console
$ docker pull kong@sha256:c4b2838a87f28dda665fc52cd57b2e4956c3012cc6d60bef9ab15b8b474a3588
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.8` - linux; amd64

```console
$ docker pull kong@sha256:a8eb48a7e0b6a6231f4f44f8e0ec795dd322b44c7004dc00922862dad7d68199
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49335332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97a4481ac0d615c6a0ae74e00fa1e67ac5efbe29eb4429e696bd6020f6fb919e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:33:20 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 12 Nov 2022 08:33:20 GMT
ARG ASSET=ce
# Sat, 12 Nov 2022 08:33:20 GMT
ENV ASSET=ce
# Sat, 12 Nov 2022 08:33:20 GMT
ARG EE_PORTS
# Sat, 12 Nov 2022 08:33:20 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Sat, 12 Nov 2022 08:33:20 GMT
ARG KONG_VERSION=2.8.3
# Sat, 12 Nov 2022 08:33:20 GMT
ENV KONG_VERSION=2.8.3
# Sat, 12 Nov 2022 08:33:20 GMT
ARG KONG_AMD64_SHA=962ac92c9834cb59f1d6563412714f3d6eecfe6c6849a84cfcbe7a4b3facbf46
# Sat, 12 Nov 2022 08:33:20 GMT
ARG KONG_ARM64_SHA=7076e6ee6a03df86795a1a08cf86e0349a150095e61be266db462cb7de9fd745
# Sat, 12 Nov 2022 08:33:27 GMT
# ARGS: KONG_AMD64_SHA=962ac92c9834cb59f1d6563412714f3d6eecfe6c6849a84cfcbe7a4b3facbf46 KONG_ARM64_SHA=7076e6ee6a03df86795a1a08cf86e0349a150095e61be266db462cb7de9fd745
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Sat, 12 Nov 2022 08:33:28 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Sat, 12 Nov 2022 08:33:28 GMT
USER kong
# Sat, 12 Nov 2022 08:33:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 12 Nov 2022 08:33:28 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 12 Nov 2022 08:33:28 GMT
STOPSIGNAL SIGQUIT
# Sat, 12 Nov 2022 08:33:28 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Sat, 12 Nov 2022 08:33:28 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb280baa9a48dcb41479263bee3784fcbf4fd49e55fb1ce556437aac0a14f66e`  
		Last Modified: Sat, 12 Nov 2022 08:34:42 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a483e5d82932b46ee26095c1122af40655ec240003f002ade98f3ef69ab4bcf`  
		Last Modified: Sat, 12 Nov 2022 08:34:50 GMT  
		Size: 46.5 MB (46528047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0809b8d4226790980e9e9596b9ebf2858c446e3db58b4f87d07ffe23495c750e`  
		Last Modified: Sat, 12 Nov 2022 08:34:42 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.8` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:8a5a7357d6cbda1840574130d109fc37b8088750d32c87b50f3b7909b7975425
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.5 MB (48524280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5957d67fc55af3d11bdbd87de76f7480e3c4d8bcb715d6cfd01922780f46ea9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Wed, 26 Oct 2022 01:56:09 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 26 Oct 2022 01:56:09 GMT
ARG ASSET=ce
# Wed, 26 Oct 2022 01:56:09 GMT
ENV ASSET=ce
# Wed, 26 Oct 2022 01:56:10 GMT
ARG EE_PORTS
# Wed, 26 Oct 2022 01:56:10 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 26 Oct 2022 01:56:10 GMT
ARG KONG_VERSION=2.8.1
# Wed, 26 Oct 2022 01:56:10 GMT
ENV KONG_VERSION=2.8.1
# Wed, 26 Oct 2022 01:56:10 GMT
ARG KONG_AMD64_SHA=ccda33bf02803b6b8dd46b22990f92265fe61d900ba94e3e0fa26db0433098c0
# Wed, 26 Oct 2022 01:56:10 GMT
ARG KONG_ARM64_SHA=d21690332a89adf9900f7266e083f41f565eb009f2771ef112f3564878eeff53
# Wed, 26 Oct 2022 01:56:16 GMT
# ARGS: KONG_AMD64_SHA=ccda33bf02803b6b8dd46b22990f92265fe61d900ba94e3e0fa26db0433098c0 KONG_ARM64_SHA=d21690332a89adf9900f7266e083f41f565eb009f2771ef112f3564878eeff53
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Wed, 26 Oct 2022 01:56:17 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 26 Oct 2022 01:56:17 GMT
USER kong
# Wed, 26 Oct 2022 01:56:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 26 Oct 2022 01:56:17 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 26 Oct 2022 01:56:17 GMT
STOPSIGNAL SIGQUIT
# Wed, 26 Oct 2022 01:56:17 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 26 Oct 2022 01:56:17 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd91e9229603b76d74826c966b221aacc86c840445a63234a9e2850a10a0062`  
		Last Modified: Wed, 26 Oct 2022 01:59:28 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:450997ae687cb58c194a458badbbb0c90dc4aed7eab5e3b1db610305ef840dd0`  
		Last Modified: Wed, 26 Oct 2022 01:59:35 GMT  
		Size: 45.8 MB (45815605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8380bfcbd9b9294f70da613229b53465eef3ac9234edb9cbfb19006dbb36293`  
		Last Modified: Wed, 26 Oct 2022 01:59:28 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.8-ubuntu`

```console
$ docker pull kong@sha256:6a10a398412f83bf45061f593eeacaeb6e69916e113c3d66a30acff87954dbd1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.8-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:47ba3e7316b9ee85b981e4c52b2f31dea602e8d311f0ddd3257d632dc51570de
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.2 MB (119165413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f4637d1f3adbd9c010e4a589b07f04959be7b91ec1c90302fb3c966bfa232b0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 26 Jan 2023 10:03:03 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:03:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:03:04 GMT
ADD file:365c129e10f7ef1594e8086543b45f524313e36dd6a25b68f4da542a09491f04 in / 
# Thu, 26 Jan 2023 10:03:05 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 20:40:52 GMT
ARG ASSET=ce
# Tue, 31 Jan 2023 20:40:52 GMT
ENV ASSET=ce
# Tue, 31 Jan 2023 20:40:52 GMT
ARG EE_PORTS
# Tue, 31 Jan 2023 20:40:52 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Tue, 31 Jan 2023 20:40:52 GMT
ARG KONG_VERSION=2.8.3
# Tue, 31 Jan 2023 20:40:52 GMT
ENV KONG_VERSION=2.8.3
# Tue, 31 Jan 2023 20:40:52 GMT
ARG KONG_AMD64_SHA=897e159da8e1432e474794d1e25d81fe6548adfa7b68beb186365d732e031d63
# Tue, 31 Jan 2023 20:40:53 GMT
ARG KONG_ARM64_SHA=5f806a19dcb3f4f41108fd6472a2480c7f6032519ecb506de5c9da8a0faf8172
# Tue, 31 Jan 2023 20:41:30 GMT
# ARGS: KONG_AMD64_SHA=897e159da8e1432e474794d1e25d81fe6548adfa7b68beb186365d732e031d63 KONG_ARM64_SHA=5f806a19dcb3f4f41108fd6472a2480c7f6032519ecb506de5c9da8a0faf8172
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 31 Jan 2023 20:41:31 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 31 Jan 2023 20:41:31 GMT
USER kong
# Tue, 31 Jan 2023 20:41:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 31 Jan 2023 20:41:32 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 31 Jan 2023 20:41:32 GMT
STOPSIGNAL SIGQUIT
# Tue, 31 Jan 2023 20:41:32 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 31 Jan 2023 20:41:32 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:456d651ccb276bafe702e453add4a4f15b511fd3234cb7db898c22540ad3c8c1`  
		Last Modified: Tue, 31 Jan 2023 17:46:32 GMT  
		Size: 26.7 MB (26711594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ac58f523609354efd23ed45020b8da1d0c9e9bca3efbdbfd65732bbd82b1c2`  
		Last Modified: Tue, 31 Jan 2023 20:44:30 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab6e44b0bed2cd2caaf016aba9d3475ef3a38e4645ec05d28faae8ff90c3ea7d`  
		Last Modified: Tue, 31 Jan 2023 20:44:40 GMT  
		Size: 67.4 MB (67370984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c572d0e6bf4e7d2a2cbfe9366caab0a0484e071873acc78b282d2530a64a843f`  
		Last Modified: Tue, 31 Jan 2023 20:44:28 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.8-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:b3821340749f078fca49fdcf6c59874924c3bc99affad7eb4870a4c105283bd8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.7 MB (121736114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25cd5e3353682a08855cc43120d77ffacbaba519aaf68736d4bed76ab5609ea4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 01:56:21 GMT
ARG ASSET=ce
# Wed, 26 Oct 2022 01:56:21 GMT
ENV ASSET=ce
# Wed, 26 Oct 2022 01:56:21 GMT
ARG EE_PORTS
# Wed, 26 Oct 2022 01:56:21 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 26 Oct 2022 01:56:21 GMT
ARG KONG_VERSION=2.8.1
# Wed, 26 Oct 2022 01:56:21 GMT
ENV KONG_VERSION=2.8.1
# Wed, 26 Oct 2022 01:56:21 GMT
ARG KONG_AMD64_SHA=10d12d23e5890414d666663094d51a42de41f8a9806fbc0baaf9ac4d37794361
# Wed, 26 Oct 2022 01:56:21 GMT
ARG KONG_ARM64_SHA=61c13219ef64dac9aeae5ae775411e8cfcd406f068cf3e75d463f916ae6513cb
# Wed, 26 Oct 2022 01:56:36 GMT
# ARGS: KONG_AMD64_SHA=10d12d23e5890414d666663094d51a42de41f8a9806fbc0baaf9ac4d37794361 KONG_ARM64_SHA=61c13219ef64dac9aeae5ae775411e8cfcd406f068cf3e75d463f916ae6513cb
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 26 Oct 2022 01:56:37 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 26 Oct 2022 01:56:38 GMT
USER kong
# Wed, 26 Oct 2022 01:56:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 26 Oct 2022 01:56:38 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 26 Oct 2022 01:56:38 GMT
STOPSIGNAL SIGQUIT
# Wed, 26 Oct 2022 01:56:38 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 26 Oct 2022 01:56:38 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f13f9d5d996e141886cffb3feec65b77fb24a51d5f42dc401d608fdec73f4c5`  
		Last Modified: Wed, 26 Oct 2022 01:59:48 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:955e7d3f453f82dabe911edc9a1755176cbb03bb5422778efe0345f2afb442a2`  
		Last Modified: Wed, 26 Oct 2022 01:59:56 GMT  
		Size: 69.5 MB (69457280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae91fafd7b2bd72f523a509de3e8ae8fe69535d0bab2a8bdbd09fb0ab63dd97a`  
		Last Modified: Wed, 26 Oct 2022 01:59:47 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.8.3`

```console
$ docker pull kong@sha256:52ba05e86adcc19d7409c82840fee3773d84f3ff9f768832459af78914aeafb7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:2.8.3` - linux; amd64

```console
$ docker pull kong@sha256:a8eb48a7e0b6a6231f4f44f8e0ec795dd322b44c7004dc00922862dad7d68199
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49335332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97a4481ac0d615c6a0ae74e00fa1e67ac5efbe29eb4429e696bd6020f6fb919e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:33:20 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 12 Nov 2022 08:33:20 GMT
ARG ASSET=ce
# Sat, 12 Nov 2022 08:33:20 GMT
ENV ASSET=ce
# Sat, 12 Nov 2022 08:33:20 GMT
ARG EE_PORTS
# Sat, 12 Nov 2022 08:33:20 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Sat, 12 Nov 2022 08:33:20 GMT
ARG KONG_VERSION=2.8.3
# Sat, 12 Nov 2022 08:33:20 GMT
ENV KONG_VERSION=2.8.3
# Sat, 12 Nov 2022 08:33:20 GMT
ARG KONG_AMD64_SHA=962ac92c9834cb59f1d6563412714f3d6eecfe6c6849a84cfcbe7a4b3facbf46
# Sat, 12 Nov 2022 08:33:20 GMT
ARG KONG_ARM64_SHA=7076e6ee6a03df86795a1a08cf86e0349a150095e61be266db462cb7de9fd745
# Sat, 12 Nov 2022 08:33:27 GMT
# ARGS: KONG_AMD64_SHA=962ac92c9834cb59f1d6563412714f3d6eecfe6c6849a84cfcbe7a4b3facbf46 KONG_ARM64_SHA=7076e6ee6a03df86795a1a08cf86e0349a150095e61be266db462cb7de9fd745
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Sat, 12 Nov 2022 08:33:28 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Sat, 12 Nov 2022 08:33:28 GMT
USER kong
# Sat, 12 Nov 2022 08:33:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 12 Nov 2022 08:33:28 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 12 Nov 2022 08:33:28 GMT
STOPSIGNAL SIGQUIT
# Sat, 12 Nov 2022 08:33:28 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Sat, 12 Nov 2022 08:33:28 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb280baa9a48dcb41479263bee3784fcbf4fd49e55fb1ce556437aac0a14f66e`  
		Last Modified: Sat, 12 Nov 2022 08:34:42 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a483e5d82932b46ee26095c1122af40655ec240003f002ade98f3ef69ab4bcf`  
		Last Modified: Sat, 12 Nov 2022 08:34:50 GMT  
		Size: 46.5 MB (46528047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0809b8d4226790980e9e9596b9ebf2858c446e3db58b4f87d07ffe23495c750e`  
		Last Modified: Sat, 12 Nov 2022 08:34:42 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.8.3-alpine`

```console
$ docker pull kong@sha256:52ba05e86adcc19d7409c82840fee3773d84f3ff9f768832459af78914aeafb7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:2.8.3-alpine` - linux; amd64

```console
$ docker pull kong@sha256:a8eb48a7e0b6a6231f4f44f8e0ec795dd322b44c7004dc00922862dad7d68199
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49335332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97a4481ac0d615c6a0ae74e00fa1e67ac5efbe29eb4429e696bd6020f6fb919e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:33:20 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 12 Nov 2022 08:33:20 GMT
ARG ASSET=ce
# Sat, 12 Nov 2022 08:33:20 GMT
ENV ASSET=ce
# Sat, 12 Nov 2022 08:33:20 GMT
ARG EE_PORTS
# Sat, 12 Nov 2022 08:33:20 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Sat, 12 Nov 2022 08:33:20 GMT
ARG KONG_VERSION=2.8.3
# Sat, 12 Nov 2022 08:33:20 GMT
ENV KONG_VERSION=2.8.3
# Sat, 12 Nov 2022 08:33:20 GMT
ARG KONG_AMD64_SHA=962ac92c9834cb59f1d6563412714f3d6eecfe6c6849a84cfcbe7a4b3facbf46
# Sat, 12 Nov 2022 08:33:20 GMT
ARG KONG_ARM64_SHA=7076e6ee6a03df86795a1a08cf86e0349a150095e61be266db462cb7de9fd745
# Sat, 12 Nov 2022 08:33:27 GMT
# ARGS: KONG_AMD64_SHA=962ac92c9834cb59f1d6563412714f3d6eecfe6c6849a84cfcbe7a4b3facbf46 KONG_ARM64_SHA=7076e6ee6a03df86795a1a08cf86e0349a150095e61be266db462cb7de9fd745
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Sat, 12 Nov 2022 08:33:28 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Sat, 12 Nov 2022 08:33:28 GMT
USER kong
# Sat, 12 Nov 2022 08:33:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 12 Nov 2022 08:33:28 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 12 Nov 2022 08:33:28 GMT
STOPSIGNAL SIGQUIT
# Sat, 12 Nov 2022 08:33:28 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Sat, 12 Nov 2022 08:33:28 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb280baa9a48dcb41479263bee3784fcbf4fd49e55fb1ce556437aac0a14f66e`  
		Last Modified: Sat, 12 Nov 2022 08:34:42 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a483e5d82932b46ee26095c1122af40655ec240003f002ade98f3ef69ab4bcf`  
		Last Modified: Sat, 12 Nov 2022 08:34:50 GMT  
		Size: 46.5 MB (46528047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0809b8d4226790980e9e9596b9ebf2858c446e3db58b4f87d07ffe23495c750e`  
		Last Modified: Sat, 12 Nov 2022 08:34:42 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.8.3-ubuntu`

```console
$ docker pull kong@sha256:ea9023045972dfcdd5293c40475c303c0615044a56d9349f78adc4fbeae25029
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:2.8.3-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:47ba3e7316b9ee85b981e4c52b2f31dea602e8d311f0ddd3257d632dc51570de
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.2 MB (119165413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f4637d1f3adbd9c010e4a589b07f04959be7b91ec1c90302fb3c966bfa232b0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 26 Jan 2023 10:03:03 GMT
ARG RELEASE
# Thu, 26 Jan 2023 10:03:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 26 Jan 2023 10:03:03 GMT
LABEL org.opencontainers.image.version=18.04
# Thu, 26 Jan 2023 10:03:04 GMT
ADD file:365c129e10f7ef1594e8086543b45f524313e36dd6a25b68f4da542a09491f04 in / 
# Thu, 26 Jan 2023 10:03:05 GMT
CMD ["/bin/bash"]
# Tue, 31 Jan 2023 20:40:52 GMT
ARG ASSET=ce
# Tue, 31 Jan 2023 20:40:52 GMT
ENV ASSET=ce
# Tue, 31 Jan 2023 20:40:52 GMT
ARG EE_PORTS
# Tue, 31 Jan 2023 20:40:52 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Tue, 31 Jan 2023 20:40:52 GMT
ARG KONG_VERSION=2.8.3
# Tue, 31 Jan 2023 20:40:52 GMT
ENV KONG_VERSION=2.8.3
# Tue, 31 Jan 2023 20:40:52 GMT
ARG KONG_AMD64_SHA=897e159da8e1432e474794d1e25d81fe6548adfa7b68beb186365d732e031d63
# Tue, 31 Jan 2023 20:40:53 GMT
ARG KONG_ARM64_SHA=5f806a19dcb3f4f41108fd6472a2480c7f6032519ecb506de5c9da8a0faf8172
# Tue, 31 Jan 2023 20:41:30 GMT
# ARGS: KONG_AMD64_SHA=897e159da8e1432e474794d1e25d81fe6548adfa7b68beb186365d732e031d63 KONG_ARM64_SHA=5f806a19dcb3f4f41108fd6472a2480c7f6032519ecb506de5c9da8a0faf8172
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 31 Jan 2023 20:41:31 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 31 Jan 2023 20:41:31 GMT
USER kong
# Tue, 31 Jan 2023 20:41:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 31 Jan 2023 20:41:32 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 31 Jan 2023 20:41:32 GMT
STOPSIGNAL SIGQUIT
# Tue, 31 Jan 2023 20:41:32 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 31 Jan 2023 20:41:32 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:456d651ccb276bafe702e453add4a4f15b511fd3234cb7db898c22540ad3c8c1`  
		Last Modified: Tue, 31 Jan 2023 17:46:32 GMT  
		Size: 26.7 MB (26711594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ac58f523609354efd23ed45020b8da1d0c9e9bca3efbdbfd65732bbd82b1c2`  
		Last Modified: Tue, 31 Jan 2023 20:44:30 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab6e44b0bed2cd2caaf016aba9d3475ef3a38e4645ec05d28faae8ff90c3ea7d`  
		Last Modified: Tue, 31 Jan 2023 20:44:40 GMT  
		Size: 67.4 MB (67370984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c572d0e6bf4e7d2a2cbfe9366caab0a0484e071873acc78b282d2530a64a843f`  
		Last Modified: Tue, 31 Jan 2023 20:44:28 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3`

```console
$ docker pull kong@sha256:dcdba428472f86b8a9f347a7193dd53c9784f8b12b0202a7adea95705282da0d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3` - linux; amd64

```console
$ docker pull kong@sha256:6a0ef502333581e2f1b25ad2e532afff20b43ea91a276303fa96462f2364cff6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75686904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50300dadf96a12e349a3c96c8020f3e55705cabf25d7a1bca57b897153d01d98`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:33:04 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Mon, 12 Dec 2022 20:41:34 GMT
ARG KONG_VERSION=3.1.1
# Mon, 12 Dec 2022 20:41:35 GMT
ENV KONG_VERSION=3.1.1
# Mon, 12 Dec 2022 20:41:35 GMT
ARG KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c
# Mon, 12 Dec 2022 20:41:35 GMT
ARG KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
# Mon, 12 Dec 2022 20:41:35 GMT
ARG ASSET=remote
# Mon, 12 Dec 2022 20:41:35 GMT
ARG EE_PORTS
# Mon, 12 Dec 2022 20:41:35 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Mon, 12 Dec 2022 20:41:43 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Mon, 12 Dec 2022 20:41:43 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Mon, 12 Dec 2022 20:41:43 GMT
USER kong
# Mon, 12 Dec 2022 20:41:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 12 Dec 2022 20:41:44 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 12 Dec 2022 20:41:44 GMT
STOPSIGNAL SIGQUIT
# Mon, 12 Dec 2022 20:41:44 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Mon, 12 Dec 2022 20:41:44 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4245fbd880e03000929048a63dc35a8e73f2d3e2162ef59119c062ae74512ec1`  
		Last Modified: Mon, 12 Dec 2022 20:44:05 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d360b82d153352e631967e1f4f6f80c42ed7c39bf695f61a8564f66805849362`  
		Last Modified: Mon, 12 Dec 2022 20:44:13 GMT  
		Size: 72.9 MB (72879617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af39bd0e0446eebd2b69924662cdf612ccfd6af7ee8d2fc59767a630d38b94d5`  
		Last Modified: Mon, 12 Dec 2022 20:44:05 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:2b1b75324a3021ab839cad67fcd4e9fa3576df5376a3b2435cd2a61dc1f19238
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.7 MB (73703801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a913906fe4dd3d3643e9e9162a080a80aaa4b642f20d10bc757058df3edce2a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:27:43 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Mon, 12 Dec 2022 20:46:19 GMT
ARG KONG_VERSION=3.1.1
# Mon, 12 Dec 2022 20:46:19 GMT
ENV KONG_VERSION=3.1.1
# Mon, 12 Dec 2022 20:46:19 GMT
ARG KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c
# Mon, 12 Dec 2022 20:46:19 GMT
ARG KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
# Mon, 12 Dec 2022 20:46:19 GMT
ARG ASSET=remote
# Mon, 12 Dec 2022 20:46:19 GMT
ARG EE_PORTS
# Mon, 12 Dec 2022 20:46:20 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Mon, 12 Dec 2022 20:46:25 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Mon, 12 Dec 2022 20:46:26 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Mon, 12 Dec 2022 20:46:26 GMT
USER kong
# Mon, 12 Dec 2022 20:46:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 12 Dec 2022 20:46:26 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 12 Dec 2022 20:46:26 GMT
STOPSIGNAL SIGQUIT
# Mon, 12 Dec 2022 20:46:27 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Mon, 12 Dec 2022 20:46:27 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeff28f77ed1e045528bd0af2f7c16b98cb84035a76ab2e1986c9a39e2b05c69`  
		Last Modified: Mon, 12 Dec 2022 20:50:07 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec35e57c6aef4decd274441c8789b0036d9f06497f7c821653816583d576be4`  
		Last Modified: Mon, 12 Dec 2022 20:50:15 GMT  
		Size: 71.0 MB (70995033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61994d980a524616d1c005e5c26edde7a13297ac2984b86f20f39b7aefa8375`  
		Last Modified: Mon, 12 Dec 2022 20:50:07 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.0`

```console
$ docker pull kong@sha256:41aeb18710f9f013ab100c64fcbcbf135f4bc86a02a223ea430eba5126ac4236
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.0` - linux; amd64

```console
$ docker pull kong@sha256:e851935170b4941070b88bf069318f460a9dd71c6aeba24288f0b1c02fd7a00a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75641360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66375da6de1c9c2fad461f78c21cf54a3c92d52f9efdbdb53a476c581f9071c1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:33:04 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Mon, 12 Dec 2022 20:42:35 GMT
ARG KONG_VERSION=3.0.2
# Mon, 12 Dec 2022 20:42:35 GMT
ENV KONG_VERSION=3.0.2
# Mon, 12 Dec 2022 20:42:36 GMT
ARG KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e
# Mon, 12 Dec 2022 20:42:36 GMT
ARG KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
# Mon, 12 Dec 2022 20:42:36 GMT
ARG ASSET=remote
# Mon, 12 Dec 2022 20:42:36 GMT
ARG EE_PORTS
# Mon, 12 Dec 2022 20:42:36 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Mon, 12 Dec 2022 20:42:44 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Mon, 12 Dec 2022 20:42:44 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Mon, 12 Dec 2022 20:42:44 GMT
USER kong
# Mon, 12 Dec 2022 20:42:44 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 12 Dec 2022 20:42:45 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 12 Dec 2022 20:42:45 GMT
STOPSIGNAL SIGQUIT
# Mon, 12 Dec 2022 20:42:45 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Mon, 12 Dec 2022 20:42:45 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ce3bc3467fc6cbbb1b4db6112cb387fb374dce5e594c2111943e111eb83232`  
		Last Modified: Mon, 12 Dec 2022 20:44:52 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaf774428b1b8be21abebbf3b21d48ba289619eee4de360e45ce009a3fd6564`  
		Last Modified: Mon, 12 Dec 2022 20:45:00 GMT  
		Size: 72.8 MB (72834073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b5059df9a75157888e9047c65e85b9d7355cd35659cdb32b6698eda0ebfe84`  
		Last Modified: Mon, 12 Dec 2022 20:44:52 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.0` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:3f03ac5beba7ca91712d42515ba227d6856212e0c0f85051382363e5834197fe
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73630764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0691f183c15b7e3c985bf1e18778bc91a478585c6c1abb5c2368fc952e34647`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:27:43 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Mon, 12 Dec 2022 20:47:10 GMT
ARG KONG_VERSION=3.0.2
# Mon, 12 Dec 2022 20:47:10 GMT
ENV KONG_VERSION=3.0.2
# Mon, 12 Dec 2022 20:47:10 GMT
ARG KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e
# Mon, 12 Dec 2022 20:47:10 GMT
ARG KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
# Mon, 12 Dec 2022 20:47:10 GMT
ARG ASSET=remote
# Mon, 12 Dec 2022 20:47:10 GMT
ARG EE_PORTS
# Mon, 12 Dec 2022 20:47:10 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Mon, 12 Dec 2022 20:47:17 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Mon, 12 Dec 2022 20:47:18 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Mon, 12 Dec 2022 20:47:18 GMT
USER kong
# Mon, 12 Dec 2022 20:47:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 12 Dec 2022 20:47:18 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 12 Dec 2022 20:47:18 GMT
STOPSIGNAL SIGQUIT
# Mon, 12 Dec 2022 20:47:18 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Mon, 12 Dec 2022 20:47:18 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82accb5ba8bca390e42a33ef922d7b8d2ce4b36c10556c5cc2c22444691f375`  
		Last Modified: Mon, 12 Dec 2022 20:50:52 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07788a5b24972181c810b4530c8dc927e43be9d6dc90d7aec7ab5912966448b9`  
		Last Modified: Mon, 12 Dec 2022 20:50:59 GMT  
		Size: 70.9 MB (70921992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb4668e024363002d321f57f790c111fe2ce64400fac1f418be0089ae225115`  
		Last Modified: Mon, 12 Dec 2022 20:50:52 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.0-alpine`

```console
$ docker pull kong@sha256:41aeb18710f9f013ab100c64fcbcbf135f4bc86a02a223ea430eba5126ac4236
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.0-alpine` - linux; amd64

```console
$ docker pull kong@sha256:e851935170b4941070b88bf069318f460a9dd71c6aeba24288f0b1c02fd7a00a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75641360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66375da6de1c9c2fad461f78c21cf54a3c92d52f9efdbdb53a476c581f9071c1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:33:04 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Mon, 12 Dec 2022 20:42:35 GMT
ARG KONG_VERSION=3.0.2
# Mon, 12 Dec 2022 20:42:35 GMT
ENV KONG_VERSION=3.0.2
# Mon, 12 Dec 2022 20:42:36 GMT
ARG KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e
# Mon, 12 Dec 2022 20:42:36 GMT
ARG KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
# Mon, 12 Dec 2022 20:42:36 GMT
ARG ASSET=remote
# Mon, 12 Dec 2022 20:42:36 GMT
ARG EE_PORTS
# Mon, 12 Dec 2022 20:42:36 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Mon, 12 Dec 2022 20:42:44 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Mon, 12 Dec 2022 20:42:44 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Mon, 12 Dec 2022 20:42:44 GMT
USER kong
# Mon, 12 Dec 2022 20:42:44 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 12 Dec 2022 20:42:45 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 12 Dec 2022 20:42:45 GMT
STOPSIGNAL SIGQUIT
# Mon, 12 Dec 2022 20:42:45 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Mon, 12 Dec 2022 20:42:45 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ce3bc3467fc6cbbb1b4db6112cb387fb374dce5e594c2111943e111eb83232`  
		Last Modified: Mon, 12 Dec 2022 20:44:52 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaf774428b1b8be21abebbf3b21d48ba289619eee4de360e45ce009a3fd6564`  
		Last Modified: Mon, 12 Dec 2022 20:45:00 GMT  
		Size: 72.8 MB (72834073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b5059df9a75157888e9047c65e85b9d7355cd35659cdb32b6698eda0ebfe84`  
		Last Modified: Mon, 12 Dec 2022 20:44:52 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.0-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:3f03ac5beba7ca91712d42515ba227d6856212e0c0f85051382363e5834197fe
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73630764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0691f183c15b7e3c985bf1e18778bc91a478585c6c1abb5c2368fc952e34647`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:27:43 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Mon, 12 Dec 2022 20:47:10 GMT
ARG KONG_VERSION=3.0.2
# Mon, 12 Dec 2022 20:47:10 GMT
ENV KONG_VERSION=3.0.2
# Mon, 12 Dec 2022 20:47:10 GMT
ARG KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e
# Mon, 12 Dec 2022 20:47:10 GMT
ARG KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
# Mon, 12 Dec 2022 20:47:10 GMT
ARG ASSET=remote
# Mon, 12 Dec 2022 20:47:10 GMT
ARG EE_PORTS
# Mon, 12 Dec 2022 20:47:10 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Mon, 12 Dec 2022 20:47:17 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Mon, 12 Dec 2022 20:47:18 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Mon, 12 Dec 2022 20:47:18 GMT
USER kong
# Mon, 12 Dec 2022 20:47:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 12 Dec 2022 20:47:18 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 12 Dec 2022 20:47:18 GMT
STOPSIGNAL SIGQUIT
# Mon, 12 Dec 2022 20:47:18 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Mon, 12 Dec 2022 20:47:18 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82accb5ba8bca390e42a33ef922d7b8d2ce4b36c10556c5cc2c22444691f375`  
		Last Modified: Mon, 12 Dec 2022 20:50:52 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07788a5b24972181c810b4530c8dc927e43be9d6dc90d7aec7ab5912966448b9`  
		Last Modified: Mon, 12 Dec 2022 20:50:59 GMT  
		Size: 70.9 MB (70921992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb4668e024363002d321f57f790c111fe2ce64400fac1f418be0089ae225115`  
		Last Modified: Mon, 12 Dec 2022 20:50:52 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.0-ubuntu`

```console
$ docker pull kong@sha256:f975702307d493e9b6464c64b1565c8eb1d80a44a9b84de7acce309f82b27fa4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.0-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:3b7e53ceecfc24817da29e6eab7599e1f189742af534b9b4cd49e8e4fa6827d8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.7 MB (101687690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2ac92d5ed4ab29e9b17611f40b7daa8a60f7f86b12cef66d34751b32d1423c9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 01 Feb 2023 11:42:37 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:42:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:42:39 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Wed, 01 Feb 2023 11:42:39 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 19:13:51 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 01 Feb 2023 19:13:51 GMT
ARG ASSET=ce
# Wed, 01 Feb 2023 19:13:51 GMT
ENV ASSET=ce
# Wed, 01 Feb 2023 19:13:51 GMT
ARG EE_PORTS
# Wed, 01 Feb 2023 19:13:51 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Wed, 01 Feb 2023 19:14:33 GMT
ARG KONG_VERSION=3.0.2
# Wed, 01 Feb 2023 19:14:33 GMT
ENV KONG_VERSION=3.0.2
# Wed, 01 Feb 2023 19:14:33 GMT
ARG KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396
# Wed, 01 Feb 2023 19:14:34 GMT
ARG KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
# Wed, 01 Feb 2023 19:14:56 GMT
# ARGS: KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396 KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 01 Feb 2023 19:14:56 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 01 Feb 2023 19:14:56 GMT
USER kong
# Wed, 01 Feb 2023 19:14:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Feb 2023 19:14:57 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 01 Feb 2023 19:14:57 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Feb 2023 19:14:57 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 01 Feb 2023 19:14:57 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a22125083e90234102050bb19d1918bdb2c3c04bea9c73a62fe9ccd73c83f60e`  
		Last Modified: Wed, 01 Feb 2023 19:17:08 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bc6163aec9c5286fd48954140b124f805c85920f05c5fc8c123ae949abda04`  
		Last Modified: Wed, 01 Feb 2023 19:17:45 GMT  
		Size: 73.1 MB (73108800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c084ebfde52c6319e39771771fce6fd96cd2d0af16bee4bebf1ed3f2f290e6`  
		Last Modified: Wed, 01 Feb 2023 19:17:34 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.0-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:e1773ae08f5a088494abecc9c8b600d43dbe7e178974bd3198a0144af2a9c595
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.9 MB (98927676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d27fc3453f206813267d59b006ea588d03906ba945dbe0d950f89eec4f7935e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:41:14 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 01 Feb 2023 18:41:14 GMT
ARG ASSET=ce
# Wed, 01 Feb 2023 18:41:14 GMT
ENV ASSET=ce
# Wed, 01 Feb 2023 18:41:14 GMT
ARG EE_PORTS
# Wed, 01 Feb 2023 18:41:14 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Wed, 01 Feb 2023 18:41:43 GMT
ARG KONG_VERSION=3.0.2
# Wed, 01 Feb 2023 18:41:43 GMT
ENV KONG_VERSION=3.0.2
# Wed, 01 Feb 2023 18:41:43 GMT
ARG KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396
# Wed, 01 Feb 2023 18:41:43 GMT
ARG KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
# Wed, 01 Feb 2023 18:42:00 GMT
# ARGS: KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396 KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 01 Feb 2023 18:42:01 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 01 Feb 2023 18:42:02 GMT
USER kong
# Wed, 01 Feb 2023 18:42:02 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Feb 2023 18:42:02 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 01 Feb 2023 18:42:02 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Feb 2023 18:42:02 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 01 Feb 2023 18:42:02 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36cafd2db5bc28f83d39ad8aa707289dd7921854bd71e7466ef84e32030ac701`  
		Last Modified: Wed, 01 Feb 2023 18:46:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f82a479db349414a8512c852f22f42c42d61d3522dd558893c8d4720eae23297`  
		Last Modified: Wed, 01 Feb 2023 18:47:04 GMT  
		Size: 71.7 MB (71732929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8b71125ec6b28c0a0071999a38465d054a7f97f28ed8187bf7e80d2527f09d`  
		Last Modified: Wed, 01 Feb 2023 18:46:54 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.0.2`

```console
$ docker pull kong@sha256:41aeb18710f9f013ab100c64fcbcbf135f4bc86a02a223ea430eba5126ac4236
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.0.2` - linux; amd64

```console
$ docker pull kong@sha256:e851935170b4941070b88bf069318f460a9dd71c6aeba24288f0b1c02fd7a00a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75641360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66375da6de1c9c2fad461f78c21cf54a3c92d52f9efdbdb53a476c581f9071c1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:33:04 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Mon, 12 Dec 2022 20:42:35 GMT
ARG KONG_VERSION=3.0.2
# Mon, 12 Dec 2022 20:42:35 GMT
ENV KONG_VERSION=3.0.2
# Mon, 12 Dec 2022 20:42:36 GMT
ARG KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e
# Mon, 12 Dec 2022 20:42:36 GMT
ARG KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
# Mon, 12 Dec 2022 20:42:36 GMT
ARG ASSET=remote
# Mon, 12 Dec 2022 20:42:36 GMT
ARG EE_PORTS
# Mon, 12 Dec 2022 20:42:36 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Mon, 12 Dec 2022 20:42:44 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Mon, 12 Dec 2022 20:42:44 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Mon, 12 Dec 2022 20:42:44 GMT
USER kong
# Mon, 12 Dec 2022 20:42:44 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 12 Dec 2022 20:42:45 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 12 Dec 2022 20:42:45 GMT
STOPSIGNAL SIGQUIT
# Mon, 12 Dec 2022 20:42:45 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Mon, 12 Dec 2022 20:42:45 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ce3bc3467fc6cbbb1b4db6112cb387fb374dce5e594c2111943e111eb83232`  
		Last Modified: Mon, 12 Dec 2022 20:44:52 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaf774428b1b8be21abebbf3b21d48ba289619eee4de360e45ce009a3fd6564`  
		Last Modified: Mon, 12 Dec 2022 20:45:00 GMT  
		Size: 72.8 MB (72834073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b5059df9a75157888e9047c65e85b9d7355cd35659cdb32b6698eda0ebfe84`  
		Last Modified: Mon, 12 Dec 2022 20:44:52 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.0.2` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:3f03ac5beba7ca91712d42515ba227d6856212e0c0f85051382363e5834197fe
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73630764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0691f183c15b7e3c985bf1e18778bc91a478585c6c1abb5c2368fc952e34647`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:27:43 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Mon, 12 Dec 2022 20:47:10 GMT
ARG KONG_VERSION=3.0.2
# Mon, 12 Dec 2022 20:47:10 GMT
ENV KONG_VERSION=3.0.2
# Mon, 12 Dec 2022 20:47:10 GMT
ARG KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e
# Mon, 12 Dec 2022 20:47:10 GMT
ARG KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
# Mon, 12 Dec 2022 20:47:10 GMT
ARG ASSET=remote
# Mon, 12 Dec 2022 20:47:10 GMT
ARG EE_PORTS
# Mon, 12 Dec 2022 20:47:10 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Mon, 12 Dec 2022 20:47:17 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Mon, 12 Dec 2022 20:47:18 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Mon, 12 Dec 2022 20:47:18 GMT
USER kong
# Mon, 12 Dec 2022 20:47:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 12 Dec 2022 20:47:18 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 12 Dec 2022 20:47:18 GMT
STOPSIGNAL SIGQUIT
# Mon, 12 Dec 2022 20:47:18 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Mon, 12 Dec 2022 20:47:18 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82accb5ba8bca390e42a33ef922d7b8d2ce4b36c10556c5cc2c22444691f375`  
		Last Modified: Mon, 12 Dec 2022 20:50:52 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07788a5b24972181c810b4530c8dc927e43be9d6dc90d7aec7ab5912966448b9`  
		Last Modified: Mon, 12 Dec 2022 20:50:59 GMT  
		Size: 70.9 MB (70921992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb4668e024363002d321f57f790c111fe2ce64400fac1f418be0089ae225115`  
		Last Modified: Mon, 12 Dec 2022 20:50:52 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.0.2-alpine`

```console
$ docker pull kong@sha256:41aeb18710f9f013ab100c64fcbcbf135f4bc86a02a223ea430eba5126ac4236
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.0.2-alpine` - linux; amd64

```console
$ docker pull kong@sha256:e851935170b4941070b88bf069318f460a9dd71c6aeba24288f0b1c02fd7a00a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75641360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66375da6de1c9c2fad461f78c21cf54a3c92d52f9efdbdb53a476c581f9071c1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:33:04 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Mon, 12 Dec 2022 20:42:35 GMT
ARG KONG_VERSION=3.0.2
# Mon, 12 Dec 2022 20:42:35 GMT
ENV KONG_VERSION=3.0.2
# Mon, 12 Dec 2022 20:42:36 GMT
ARG KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e
# Mon, 12 Dec 2022 20:42:36 GMT
ARG KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
# Mon, 12 Dec 2022 20:42:36 GMT
ARG ASSET=remote
# Mon, 12 Dec 2022 20:42:36 GMT
ARG EE_PORTS
# Mon, 12 Dec 2022 20:42:36 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Mon, 12 Dec 2022 20:42:44 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Mon, 12 Dec 2022 20:42:44 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Mon, 12 Dec 2022 20:42:44 GMT
USER kong
# Mon, 12 Dec 2022 20:42:44 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 12 Dec 2022 20:42:45 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 12 Dec 2022 20:42:45 GMT
STOPSIGNAL SIGQUIT
# Mon, 12 Dec 2022 20:42:45 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Mon, 12 Dec 2022 20:42:45 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ce3bc3467fc6cbbb1b4db6112cb387fb374dce5e594c2111943e111eb83232`  
		Last Modified: Mon, 12 Dec 2022 20:44:52 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaf774428b1b8be21abebbf3b21d48ba289619eee4de360e45ce009a3fd6564`  
		Last Modified: Mon, 12 Dec 2022 20:45:00 GMT  
		Size: 72.8 MB (72834073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b5059df9a75157888e9047c65e85b9d7355cd35659cdb32b6698eda0ebfe84`  
		Last Modified: Mon, 12 Dec 2022 20:44:52 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.0.2-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:3f03ac5beba7ca91712d42515ba227d6856212e0c0f85051382363e5834197fe
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73630764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0691f183c15b7e3c985bf1e18778bc91a478585c6c1abb5c2368fc952e34647`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:27:43 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Mon, 12 Dec 2022 20:47:10 GMT
ARG KONG_VERSION=3.0.2
# Mon, 12 Dec 2022 20:47:10 GMT
ENV KONG_VERSION=3.0.2
# Mon, 12 Dec 2022 20:47:10 GMT
ARG KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e
# Mon, 12 Dec 2022 20:47:10 GMT
ARG KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
# Mon, 12 Dec 2022 20:47:10 GMT
ARG ASSET=remote
# Mon, 12 Dec 2022 20:47:10 GMT
ARG EE_PORTS
# Mon, 12 Dec 2022 20:47:10 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Mon, 12 Dec 2022 20:47:17 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Mon, 12 Dec 2022 20:47:18 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Mon, 12 Dec 2022 20:47:18 GMT
USER kong
# Mon, 12 Dec 2022 20:47:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 12 Dec 2022 20:47:18 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 12 Dec 2022 20:47:18 GMT
STOPSIGNAL SIGQUIT
# Mon, 12 Dec 2022 20:47:18 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Mon, 12 Dec 2022 20:47:18 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82accb5ba8bca390e42a33ef922d7b8d2ce4b36c10556c5cc2c22444691f375`  
		Last Modified: Mon, 12 Dec 2022 20:50:52 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07788a5b24972181c810b4530c8dc927e43be9d6dc90d7aec7ab5912966448b9`  
		Last Modified: Mon, 12 Dec 2022 20:50:59 GMT  
		Size: 70.9 MB (70921992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb4668e024363002d321f57f790c111fe2ce64400fac1f418be0089ae225115`  
		Last Modified: Mon, 12 Dec 2022 20:50:52 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.0.2-ubuntu`

```console
$ docker pull kong@sha256:f975702307d493e9b6464c64b1565c8eb1d80a44a9b84de7acce309f82b27fa4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.0.2-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:3b7e53ceecfc24817da29e6eab7599e1f189742af534b9b4cd49e8e4fa6827d8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.7 MB (101687690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2ac92d5ed4ab29e9b17611f40b7daa8a60f7f86b12cef66d34751b32d1423c9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 01 Feb 2023 11:42:37 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:42:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:42:39 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Wed, 01 Feb 2023 11:42:39 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 19:13:51 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 01 Feb 2023 19:13:51 GMT
ARG ASSET=ce
# Wed, 01 Feb 2023 19:13:51 GMT
ENV ASSET=ce
# Wed, 01 Feb 2023 19:13:51 GMT
ARG EE_PORTS
# Wed, 01 Feb 2023 19:13:51 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Wed, 01 Feb 2023 19:14:33 GMT
ARG KONG_VERSION=3.0.2
# Wed, 01 Feb 2023 19:14:33 GMT
ENV KONG_VERSION=3.0.2
# Wed, 01 Feb 2023 19:14:33 GMT
ARG KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396
# Wed, 01 Feb 2023 19:14:34 GMT
ARG KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
# Wed, 01 Feb 2023 19:14:56 GMT
# ARGS: KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396 KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 01 Feb 2023 19:14:56 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 01 Feb 2023 19:14:56 GMT
USER kong
# Wed, 01 Feb 2023 19:14:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Feb 2023 19:14:57 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 01 Feb 2023 19:14:57 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Feb 2023 19:14:57 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 01 Feb 2023 19:14:57 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a22125083e90234102050bb19d1918bdb2c3c04bea9c73a62fe9ccd73c83f60e`  
		Last Modified: Wed, 01 Feb 2023 19:17:08 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bc6163aec9c5286fd48954140b124f805c85920f05c5fc8c123ae949abda04`  
		Last Modified: Wed, 01 Feb 2023 19:17:45 GMT  
		Size: 73.1 MB (73108800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c084ebfde52c6319e39771771fce6fd96cd2d0af16bee4bebf1ed3f2f290e6`  
		Last Modified: Wed, 01 Feb 2023 19:17:34 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.0.2-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:e1773ae08f5a088494abecc9c8b600d43dbe7e178974bd3198a0144af2a9c595
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.9 MB (98927676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d27fc3453f206813267d59b006ea588d03906ba945dbe0d950f89eec4f7935e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:41:14 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 01 Feb 2023 18:41:14 GMT
ARG ASSET=ce
# Wed, 01 Feb 2023 18:41:14 GMT
ENV ASSET=ce
# Wed, 01 Feb 2023 18:41:14 GMT
ARG EE_PORTS
# Wed, 01 Feb 2023 18:41:14 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Wed, 01 Feb 2023 18:41:43 GMT
ARG KONG_VERSION=3.0.2
# Wed, 01 Feb 2023 18:41:43 GMT
ENV KONG_VERSION=3.0.2
# Wed, 01 Feb 2023 18:41:43 GMT
ARG KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396
# Wed, 01 Feb 2023 18:41:43 GMT
ARG KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
# Wed, 01 Feb 2023 18:42:00 GMT
# ARGS: KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396 KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 01 Feb 2023 18:42:01 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 01 Feb 2023 18:42:02 GMT
USER kong
# Wed, 01 Feb 2023 18:42:02 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Feb 2023 18:42:02 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 01 Feb 2023 18:42:02 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Feb 2023 18:42:02 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 01 Feb 2023 18:42:02 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36cafd2db5bc28f83d39ad8aa707289dd7921854bd71e7466ef84e32030ac701`  
		Last Modified: Wed, 01 Feb 2023 18:46:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f82a479db349414a8512c852f22f42c42d61d3522dd558893c8d4720eae23297`  
		Last Modified: Wed, 01 Feb 2023 18:47:04 GMT  
		Size: 71.7 MB (71732929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8b71125ec6b28c0a0071999a38465d054a7f97f28ed8187bf7e80d2527f09d`  
		Last Modified: Wed, 01 Feb 2023 18:46:54 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.1`

```console
$ docker pull kong@sha256:dcdba428472f86b8a9f347a7193dd53c9784f8b12b0202a7adea95705282da0d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.1` - linux; amd64

```console
$ docker pull kong@sha256:6a0ef502333581e2f1b25ad2e532afff20b43ea91a276303fa96462f2364cff6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75686904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50300dadf96a12e349a3c96c8020f3e55705cabf25d7a1bca57b897153d01d98`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:33:04 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Mon, 12 Dec 2022 20:41:34 GMT
ARG KONG_VERSION=3.1.1
# Mon, 12 Dec 2022 20:41:35 GMT
ENV KONG_VERSION=3.1.1
# Mon, 12 Dec 2022 20:41:35 GMT
ARG KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c
# Mon, 12 Dec 2022 20:41:35 GMT
ARG KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
# Mon, 12 Dec 2022 20:41:35 GMT
ARG ASSET=remote
# Mon, 12 Dec 2022 20:41:35 GMT
ARG EE_PORTS
# Mon, 12 Dec 2022 20:41:35 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Mon, 12 Dec 2022 20:41:43 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Mon, 12 Dec 2022 20:41:43 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Mon, 12 Dec 2022 20:41:43 GMT
USER kong
# Mon, 12 Dec 2022 20:41:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 12 Dec 2022 20:41:44 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 12 Dec 2022 20:41:44 GMT
STOPSIGNAL SIGQUIT
# Mon, 12 Dec 2022 20:41:44 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Mon, 12 Dec 2022 20:41:44 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4245fbd880e03000929048a63dc35a8e73f2d3e2162ef59119c062ae74512ec1`  
		Last Modified: Mon, 12 Dec 2022 20:44:05 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d360b82d153352e631967e1f4f6f80c42ed7c39bf695f61a8564f66805849362`  
		Last Modified: Mon, 12 Dec 2022 20:44:13 GMT  
		Size: 72.9 MB (72879617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af39bd0e0446eebd2b69924662cdf612ccfd6af7ee8d2fc59767a630d38b94d5`  
		Last Modified: Mon, 12 Dec 2022 20:44:05 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.1` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:2b1b75324a3021ab839cad67fcd4e9fa3576df5376a3b2435cd2a61dc1f19238
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.7 MB (73703801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a913906fe4dd3d3643e9e9162a080a80aaa4b642f20d10bc757058df3edce2a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:27:43 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Mon, 12 Dec 2022 20:46:19 GMT
ARG KONG_VERSION=3.1.1
# Mon, 12 Dec 2022 20:46:19 GMT
ENV KONG_VERSION=3.1.1
# Mon, 12 Dec 2022 20:46:19 GMT
ARG KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c
# Mon, 12 Dec 2022 20:46:19 GMT
ARG KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
# Mon, 12 Dec 2022 20:46:19 GMT
ARG ASSET=remote
# Mon, 12 Dec 2022 20:46:19 GMT
ARG EE_PORTS
# Mon, 12 Dec 2022 20:46:20 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Mon, 12 Dec 2022 20:46:25 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Mon, 12 Dec 2022 20:46:26 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Mon, 12 Dec 2022 20:46:26 GMT
USER kong
# Mon, 12 Dec 2022 20:46:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 12 Dec 2022 20:46:26 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 12 Dec 2022 20:46:26 GMT
STOPSIGNAL SIGQUIT
# Mon, 12 Dec 2022 20:46:27 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Mon, 12 Dec 2022 20:46:27 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeff28f77ed1e045528bd0af2f7c16b98cb84035a76ab2e1986c9a39e2b05c69`  
		Last Modified: Mon, 12 Dec 2022 20:50:07 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec35e57c6aef4decd274441c8789b0036d9f06497f7c821653816583d576be4`  
		Last Modified: Mon, 12 Dec 2022 20:50:15 GMT  
		Size: 71.0 MB (70995033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61994d980a524616d1c005e5c26edde7a13297ac2984b86f20f39b7aefa8375`  
		Last Modified: Mon, 12 Dec 2022 20:50:07 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.1-ubuntu`

```console
$ docker pull kong@sha256:df65a153ee9897f9909b1542797ed2ec3556482f64d8086f058c5e34ffc9a460
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.1-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:2e482739b5155d63e1cf76e3d6a81909f323552693a36f85cc3033cf4892718b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.7 MB (101724911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b65ea580c9b344f6392f645b956e1f7642e3e48bd0c110b6c0e11336ccce11d6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 01 Feb 2023 11:42:37 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:42:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:42:39 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Wed, 01 Feb 2023 11:42:39 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 19:13:51 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 01 Feb 2023 19:13:51 GMT
ARG ASSET=ce
# Wed, 01 Feb 2023 19:13:51 GMT
ENV ASSET=ce
# Wed, 01 Feb 2023 19:13:51 GMT
ARG EE_PORTS
# Wed, 01 Feb 2023 19:13:51 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Wed, 01 Feb 2023 19:13:51 GMT
ARG KONG_VERSION=3.1.1
# Wed, 01 Feb 2023 19:13:52 GMT
ENV KONG_VERSION=3.1.1
# Wed, 01 Feb 2023 19:13:52 GMT
ARG KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b
# Wed, 01 Feb 2023 19:13:52 GMT
ARG KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
# Wed, 01 Feb 2023 19:14:28 GMT
# ARGS: KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 01 Feb 2023 19:14:29 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 01 Feb 2023 19:14:29 GMT
USER kong
# Wed, 01 Feb 2023 19:14:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Feb 2023 19:14:29 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 01 Feb 2023 19:14:29 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Feb 2023 19:14:29 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 01 Feb 2023 19:14:29 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a22125083e90234102050bb19d1918bdb2c3c04bea9c73a62fe9ccd73c83f60e`  
		Last Modified: Wed, 01 Feb 2023 19:17:08 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e8dc9e1b22d6e7ad79f283f2ab4c4a807ed6e310a25f512783dfba9d33e0fbf`  
		Last Modified: Wed, 01 Feb 2023 19:17:21 GMT  
		Size: 73.1 MB (73146021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d523f9590e88b534d4ccca2f54947d36099583997a52ef86067e3a87de965ce`  
		Last Modified: Wed, 01 Feb 2023 19:17:09 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.1-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:2807a54ce70edbd17a4f85420c7ee484b553a19ecbc15df434c08c6a1ea7d178
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.9 MB (98948034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fc3e88b30ac604a1992c70f8d3eea4700df7916403c7f306170be51fce16baf`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:41:14 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 01 Feb 2023 18:41:14 GMT
ARG ASSET=ce
# Wed, 01 Feb 2023 18:41:14 GMT
ENV ASSET=ce
# Wed, 01 Feb 2023 18:41:14 GMT
ARG EE_PORTS
# Wed, 01 Feb 2023 18:41:14 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Wed, 01 Feb 2023 18:41:14 GMT
ARG KONG_VERSION=3.1.1
# Wed, 01 Feb 2023 18:41:14 GMT
ENV KONG_VERSION=3.1.1
# Wed, 01 Feb 2023 18:41:14 GMT
ARG KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b
# Wed, 01 Feb 2023 18:41:14 GMT
ARG KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
# Wed, 01 Feb 2023 18:41:35 GMT
# ARGS: KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 01 Feb 2023 18:41:36 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 01 Feb 2023 18:41:36 GMT
USER kong
# Wed, 01 Feb 2023 18:41:36 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Feb 2023 18:41:36 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 01 Feb 2023 18:41:37 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Feb 2023 18:41:37 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 01 Feb 2023 18:41:37 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36cafd2db5bc28f83d39ad8aa707289dd7921854bd71e7466ef84e32030ac701`  
		Last Modified: Wed, 01 Feb 2023 18:46:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28f235d14f58889c349b65eecb325ce55df27ab1e42d7683a55ec9046cefe97`  
		Last Modified: Wed, 01 Feb 2023 18:46:43 GMT  
		Size: 71.8 MB (71753287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4c2525fd3153551fc7a4a02eff76bfda933b637a850e4ad32f985a2b6a8e6c`  
		Last Modified: Wed, 01 Feb 2023 18:46:33 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.1.1`

```console
$ docker pull kong@sha256:dcdba428472f86b8a9f347a7193dd53c9784f8b12b0202a7adea95705282da0d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.1.1` - linux; amd64

```console
$ docker pull kong@sha256:6a0ef502333581e2f1b25ad2e532afff20b43ea91a276303fa96462f2364cff6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75686904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50300dadf96a12e349a3c96c8020f3e55705cabf25d7a1bca57b897153d01d98`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:33:04 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Mon, 12 Dec 2022 20:41:34 GMT
ARG KONG_VERSION=3.1.1
# Mon, 12 Dec 2022 20:41:35 GMT
ENV KONG_VERSION=3.1.1
# Mon, 12 Dec 2022 20:41:35 GMT
ARG KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c
# Mon, 12 Dec 2022 20:41:35 GMT
ARG KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
# Mon, 12 Dec 2022 20:41:35 GMT
ARG ASSET=remote
# Mon, 12 Dec 2022 20:41:35 GMT
ARG EE_PORTS
# Mon, 12 Dec 2022 20:41:35 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Mon, 12 Dec 2022 20:41:43 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Mon, 12 Dec 2022 20:41:43 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Mon, 12 Dec 2022 20:41:43 GMT
USER kong
# Mon, 12 Dec 2022 20:41:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 12 Dec 2022 20:41:44 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 12 Dec 2022 20:41:44 GMT
STOPSIGNAL SIGQUIT
# Mon, 12 Dec 2022 20:41:44 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Mon, 12 Dec 2022 20:41:44 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4245fbd880e03000929048a63dc35a8e73f2d3e2162ef59119c062ae74512ec1`  
		Last Modified: Mon, 12 Dec 2022 20:44:05 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d360b82d153352e631967e1f4f6f80c42ed7c39bf695f61a8564f66805849362`  
		Last Modified: Mon, 12 Dec 2022 20:44:13 GMT  
		Size: 72.9 MB (72879617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af39bd0e0446eebd2b69924662cdf612ccfd6af7ee8d2fc59767a630d38b94d5`  
		Last Modified: Mon, 12 Dec 2022 20:44:05 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.1.1` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:2b1b75324a3021ab839cad67fcd4e9fa3576df5376a3b2435cd2a61dc1f19238
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.7 MB (73703801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a913906fe4dd3d3643e9e9162a080a80aaa4b642f20d10bc757058df3edce2a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:27:43 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Mon, 12 Dec 2022 20:46:19 GMT
ARG KONG_VERSION=3.1.1
# Mon, 12 Dec 2022 20:46:19 GMT
ENV KONG_VERSION=3.1.1
# Mon, 12 Dec 2022 20:46:19 GMT
ARG KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c
# Mon, 12 Dec 2022 20:46:19 GMT
ARG KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
# Mon, 12 Dec 2022 20:46:19 GMT
ARG ASSET=remote
# Mon, 12 Dec 2022 20:46:19 GMT
ARG EE_PORTS
# Mon, 12 Dec 2022 20:46:20 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Mon, 12 Dec 2022 20:46:25 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Mon, 12 Dec 2022 20:46:26 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Mon, 12 Dec 2022 20:46:26 GMT
USER kong
# Mon, 12 Dec 2022 20:46:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 12 Dec 2022 20:46:26 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 12 Dec 2022 20:46:26 GMT
STOPSIGNAL SIGQUIT
# Mon, 12 Dec 2022 20:46:27 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Mon, 12 Dec 2022 20:46:27 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeff28f77ed1e045528bd0af2f7c16b98cb84035a76ab2e1986c9a39e2b05c69`  
		Last Modified: Mon, 12 Dec 2022 20:50:07 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec35e57c6aef4decd274441c8789b0036d9f06497f7c821653816583d576be4`  
		Last Modified: Mon, 12 Dec 2022 20:50:15 GMT  
		Size: 71.0 MB (70995033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61994d980a524616d1c005e5c26edde7a13297ac2984b86f20f39b7aefa8375`  
		Last Modified: Mon, 12 Dec 2022 20:50:07 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.1.1-alpine`

```console
$ docker pull kong@sha256:dcdba428472f86b8a9f347a7193dd53c9784f8b12b0202a7adea95705282da0d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.1.1-alpine` - linux; amd64

```console
$ docker pull kong@sha256:6a0ef502333581e2f1b25ad2e532afff20b43ea91a276303fa96462f2364cff6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75686904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50300dadf96a12e349a3c96c8020f3e55705cabf25d7a1bca57b897153d01d98`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:33:04 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Mon, 12 Dec 2022 20:41:34 GMT
ARG KONG_VERSION=3.1.1
# Mon, 12 Dec 2022 20:41:35 GMT
ENV KONG_VERSION=3.1.1
# Mon, 12 Dec 2022 20:41:35 GMT
ARG KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c
# Mon, 12 Dec 2022 20:41:35 GMT
ARG KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
# Mon, 12 Dec 2022 20:41:35 GMT
ARG ASSET=remote
# Mon, 12 Dec 2022 20:41:35 GMT
ARG EE_PORTS
# Mon, 12 Dec 2022 20:41:35 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Mon, 12 Dec 2022 20:41:43 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Mon, 12 Dec 2022 20:41:43 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Mon, 12 Dec 2022 20:41:43 GMT
USER kong
# Mon, 12 Dec 2022 20:41:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 12 Dec 2022 20:41:44 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 12 Dec 2022 20:41:44 GMT
STOPSIGNAL SIGQUIT
# Mon, 12 Dec 2022 20:41:44 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Mon, 12 Dec 2022 20:41:44 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4245fbd880e03000929048a63dc35a8e73f2d3e2162ef59119c062ae74512ec1`  
		Last Modified: Mon, 12 Dec 2022 20:44:05 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d360b82d153352e631967e1f4f6f80c42ed7c39bf695f61a8564f66805849362`  
		Last Modified: Mon, 12 Dec 2022 20:44:13 GMT  
		Size: 72.9 MB (72879617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af39bd0e0446eebd2b69924662cdf612ccfd6af7ee8d2fc59767a630d38b94d5`  
		Last Modified: Mon, 12 Dec 2022 20:44:05 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.1.1-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:2b1b75324a3021ab839cad67fcd4e9fa3576df5376a3b2435cd2a61dc1f19238
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.7 MB (73703801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a913906fe4dd3d3643e9e9162a080a80aaa4b642f20d10bc757058df3edce2a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:27:43 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Mon, 12 Dec 2022 20:46:19 GMT
ARG KONG_VERSION=3.1.1
# Mon, 12 Dec 2022 20:46:19 GMT
ENV KONG_VERSION=3.1.1
# Mon, 12 Dec 2022 20:46:19 GMT
ARG KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c
# Mon, 12 Dec 2022 20:46:19 GMT
ARG KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
# Mon, 12 Dec 2022 20:46:19 GMT
ARG ASSET=remote
# Mon, 12 Dec 2022 20:46:19 GMT
ARG EE_PORTS
# Mon, 12 Dec 2022 20:46:20 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Mon, 12 Dec 2022 20:46:25 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Mon, 12 Dec 2022 20:46:26 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Mon, 12 Dec 2022 20:46:26 GMT
USER kong
# Mon, 12 Dec 2022 20:46:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 12 Dec 2022 20:46:26 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 12 Dec 2022 20:46:26 GMT
STOPSIGNAL SIGQUIT
# Mon, 12 Dec 2022 20:46:27 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Mon, 12 Dec 2022 20:46:27 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeff28f77ed1e045528bd0af2f7c16b98cb84035a76ab2e1986c9a39e2b05c69`  
		Last Modified: Mon, 12 Dec 2022 20:50:07 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec35e57c6aef4decd274441c8789b0036d9f06497f7c821653816583d576be4`  
		Last Modified: Mon, 12 Dec 2022 20:50:15 GMT  
		Size: 71.0 MB (70995033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61994d980a524616d1c005e5c26edde7a13297ac2984b86f20f39b7aefa8375`  
		Last Modified: Mon, 12 Dec 2022 20:50:07 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.1.1-ubuntu`

```console
$ docker pull kong@sha256:df65a153ee9897f9909b1542797ed2ec3556482f64d8086f058c5e34ffc9a460
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.1.1-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:2e482739b5155d63e1cf76e3d6a81909f323552693a36f85cc3033cf4892718b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.7 MB (101724911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b65ea580c9b344f6392f645b956e1f7642e3e48bd0c110b6c0e11336ccce11d6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 01 Feb 2023 11:42:37 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:42:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:42:39 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Wed, 01 Feb 2023 11:42:39 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 19:13:51 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 01 Feb 2023 19:13:51 GMT
ARG ASSET=ce
# Wed, 01 Feb 2023 19:13:51 GMT
ENV ASSET=ce
# Wed, 01 Feb 2023 19:13:51 GMT
ARG EE_PORTS
# Wed, 01 Feb 2023 19:13:51 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Wed, 01 Feb 2023 19:13:51 GMT
ARG KONG_VERSION=3.1.1
# Wed, 01 Feb 2023 19:13:52 GMT
ENV KONG_VERSION=3.1.1
# Wed, 01 Feb 2023 19:13:52 GMT
ARG KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b
# Wed, 01 Feb 2023 19:13:52 GMT
ARG KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
# Wed, 01 Feb 2023 19:14:28 GMT
# ARGS: KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 01 Feb 2023 19:14:29 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 01 Feb 2023 19:14:29 GMT
USER kong
# Wed, 01 Feb 2023 19:14:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Feb 2023 19:14:29 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 01 Feb 2023 19:14:29 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Feb 2023 19:14:29 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 01 Feb 2023 19:14:29 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a22125083e90234102050bb19d1918bdb2c3c04bea9c73a62fe9ccd73c83f60e`  
		Last Modified: Wed, 01 Feb 2023 19:17:08 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e8dc9e1b22d6e7ad79f283f2ab4c4a807ed6e310a25f512783dfba9d33e0fbf`  
		Last Modified: Wed, 01 Feb 2023 19:17:21 GMT  
		Size: 73.1 MB (73146021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d523f9590e88b534d4ccca2f54947d36099583997a52ef86067e3a87de965ce`  
		Last Modified: Wed, 01 Feb 2023 19:17:09 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.1.1-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:2807a54ce70edbd17a4f85420c7ee484b553a19ecbc15df434c08c6a1ea7d178
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.9 MB (98948034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fc3e88b30ac604a1992c70f8d3eea4700df7916403c7f306170be51fce16baf`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:41:14 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 01 Feb 2023 18:41:14 GMT
ARG ASSET=ce
# Wed, 01 Feb 2023 18:41:14 GMT
ENV ASSET=ce
# Wed, 01 Feb 2023 18:41:14 GMT
ARG EE_PORTS
# Wed, 01 Feb 2023 18:41:14 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Wed, 01 Feb 2023 18:41:14 GMT
ARG KONG_VERSION=3.1.1
# Wed, 01 Feb 2023 18:41:14 GMT
ENV KONG_VERSION=3.1.1
# Wed, 01 Feb 2023 18:41:14 GMT
ARG KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b
# Wed, 01 Feb 2023 18:41:14 GMT
ARG KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
# Wed, 01 Feb 2023 18:41:35 GMT
# ARGS: KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 01 Feb 2023 18:41:36 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 01 Feb 2023 18:41:36 GMT
USER kong
# Wed, 01 Feb 2023 18:41:36 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Feb 2023 18:41:36 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 01 Feb 2023 18:41:37 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Feb 2023 18:41:37 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 01 Feb 2023 18:41:37 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36cafd2db5bc28f83d39ad8aa707289dd7921854bd71e7466ef84e32030ac701`  
		Last Modified: Wed, 01 Feb 2023 18:46:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28f235d14f58889c349b65eecb325ce55df27ab1e42d7683a55ec9046cefe97`  
		Last Modified: Wed, 01 Feb 2023 18:46:43 GMT  
		Size: 71.8 MB (71753287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4c2525fd3153551fc7a4a02eff76bfda933b637a850e4ad32f985a2b6a8e6c`  
		Last Modified: Wed, 01 Feb 2023 18:46:33 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:alpine`

```console
$ docker pull kong@sha256:dcdba428472f86b8a9f347a7193dd53c9784f8b12b0202a7adea95705282da0d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:alpine` - linux; amd64

```console
$ docker pull kong@sha256:6a0ef502333581e2f1b25ad2e532afff20b43ea91a276303fa96462f2364cff6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75686904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50300dadf96a12e349a3c96c8020f3e55705cabf25d7a1bca57b897153d01d98`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:33:04 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Mon, 12 Dec 2022 20:41:34 GMT
ARG KONG_VERSION=3.1.1
# Mon, 12 Dec 2022 20:41:35 GMT
ENV KONG_VERSION=3.1.1
# Mon, 12 Dec 2022 20:41:35 GMT
ARG KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c
# Mon, 12 Dec 2022 20:41:35 GMT
ARG KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
# Mon, 12 Dec 2022 20:41:35 GMT
ARG ASSET=remote
# Mon, 12 Dec 2022 20:41:35 GMT
ARG EE_PORTS
# Mon, 12 Dec 2022 20:41:35 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Mon, 12 Dec 2022 20:41:43 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Mon, 12 Dec 2022 20:41:43 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Mon, 12 Dec 2022 20:41:43 GMT
USER kong
# Mon, 12 Dec 2022 20:41:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 12 Dec 2022 20:41:44 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 12 Dec 2022 20:41:44 GMT
STOPSIGNAL SIGQUIT
# Mon, 12 Dec 2022 20:41:44 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Mon, 12 Dec 2022 20:41:44 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4245fbd880e03000929048a63dc35a8e73f2d3e2162ef59119c062ae74512ec1`  
		Last Modified: Mon, 12 Dec 2022 20:44:05 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d360b82d153352e631967e1f4f6f80c42ed7c39bf695f61a8564f66805849362`  
		Last Modified: Mon, 12 Dec 2022 20:44:13 GMT  
		Size: 72.9 MB (72879617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af39bd0e0446eebd2b69924662cdf612ccfd6af7ee8d2fc59767a630d38b94d5`  
		Last Modified: Mon, 12 Dec 2022 20:44:05 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:2b1b75324a3021ab839cad67fcd4e9fa3576df5376a3b2435cd2a61dc1f19238
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.7 MB (73703801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a913906fe4dd3d3643e9e9162a080a80aaa4b642f20d10bc757058df3edce2a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:27:43 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Mon, 12 Dec 2022 20:46:19 GMT
ARG KONG_VERSION=3.1.1
# Mon, 12 Dec 2022 20:46:19 GMT
ENV KONG_VERSION=3.1.1
# Mon, 12 Dec 2022 20:46:19 GMT
ARG KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c
# Mon, 12 Dec 2022 20:46:19 GMT
ARG KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
# Mon, 12 Dec 2022 20:46:19 GMT
ARG ASSET=remote
# Mon, 12 Dec 2022 20:46:19 GMT
ARG EE_PORTS
# Mon, 12 Dec 2022 20:46:20 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Mon, 12 Dec 2022 20:46:25 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Mon, 12 Dec 2022 20:46:26 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Mon, 12 Dec 2022 20:46:26 GMT
USER kong
# Mon, 12 Dec 2022 20:46:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 12 Dec 2022 20:46:26 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 12 Dec 2022 20:46:26 GMT
STOPSIGNAL SIGQUIT
# Mon, 12 Dec 2022 20:46:27 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Mon, 12 Dec 2022 20:46:27 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeff28f77ed1e045528bd0af2f7c16b98cb84035a76ab2e1986c9a39e2b05c69`  
		Last Modified: Mon, 12 Dec 2022 20:50:07 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec35e57c6aef4decd274441c8789b0036d9f06497f7c821653816583d576be4`  
		Last Modified: Mon, 12 Dec 2022 20:50:15 GMT  
		Size: 71.0 MB (70995033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61994d980a524616d1c005e5c26edde7a13297ac2984b86f20f39b7aefa8375`  
		Last Modified: Mon, 12 Dec 2022 20:50:07 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:latest`

```console
$ docker pull kong@sha256:dcdba428472f86b8a9f347a7193dd53c9784f8b12b0202a7adea95705282da0d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:latest` - linux; amd64

```console
$ docker pull kong@sha256:6a0ef502333581e2f1b25ad2e532afff20b43ea91a276303fa96462f2364cff6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75686904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50300dadf96a12e349a3c96c8020f3e55705cabf25d7a1bca57b897153d01d98`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:33:04 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Mon, 12 Dec 2022 20:41:34 GMT
ARG KONG_VERSION=3.1.1
# Mon, 12 Dec 2022 20:41:35 GMT
ENV KONG_VERSION=3.1.1
# Mon, 12 Dec 2022 20:41:35 GMT
ARG KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c
# Mon, 12 Dec 2022 20:41:35 GMT
ARG KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
# Mon, 12 Dec 2022 20:41:35 GMT
ARG ASSET=remote
# Mon, 12 Dec 2022 20:41:35 GMT
ARG EE_PORTS
# Mon, 12 Dec 2022 20:41:35 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Mon, 12 Dec 2022 20:41:43 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Mon, 12 Dec 2022 20:41:43 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Mon, 12 Dec 2022 20:41:43 GMT
USER kong
# Mon, 12 Dec 2022 20:41:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 12 Dec 2022 20:41:44 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 12 Dec 2022 20:41:44 GMT
STOPSIGNAL SIGQUIT
# Mon, 12 Dec 2022 20:41:44 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Mon, 12 Dec 2022 20:41:44 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4245fbd880e03000929048a63dc35a8e73f2d3e2162ef59119c062ae74512ec1`  
		Last Modified: Mon, 12 Dec 2022 20:44:05 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d360b82d153352e631967e1f4f6f80c42ed7c39bf695f61a8564f66805849362`  
		Last Modified: Mon, 12 Dec 2022 20:44:13 GMT  
		Size: 72.9 MB (72879617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af39bd0e0446eebd2b69924662cdf612ccfd6af7ee8d2fc59767a630d38b94d5`  
		Last Modified: Mon, 12 Dec 2022 20:44:05 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:latest` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:2b1b75324a3021ab839cad67fcd4e9fa3576df5376a3b2435cd2a61dc1f19238
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.7 MB (73703801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a913906fe4dd3d3643e9e9162a080a80aaa4b642f20d10bc757058df3edce2a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 04:27:43 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Mon, 12 Dec 2022 20:46:19 GMT
ARG KONG_VERSION=3.1.1
# Mon, 12 Dec 2022 20:46:19 GMT
ENV KONG_VERSION=3.1.1
# Mon, 12 Dec 2022 20:46:19 GMT
ARG KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c
# Mon, 12 Dec 2022 20:46:19 GMT
ARG KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
# Mon, 12 Dec 2022 20:46:19 GMT
ARG ASSET=remote
# Mon, 12 Dec 2022 20:46:19 GMT
ARG EE_PORTS
# Mon, 12 Dec 2022 20:46:20 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Mon, 12 Dec 2022 20:46:25 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Mon, 12 Dec 2022 20:46:26 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Mon, 12 Dec 2022 20:46:26 GMT
USER kong
# Mon, 12 Dec 2022 20:46:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 12 Dec 2022 20:46:26 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 12 Dec 2022 20:46:26 GMT
STOPSIGNAL SIGQUIT
# Mon, 12 Dec 2022 20:46:27 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Mon, 12 Dec 2022 20:46:27 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeff28f77ed1e045528bd0af2f7c16b98cb84035a76ab2e1986c9a39e2b05c69`  
		Last Modified: Mon, 12 Dec 2022 20:50:07 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec35e57c6aef4decd274441c8789b0036d9f06497f7c821653816583d576be4`  
		Last Modified: Mon, 12 Dec 2022 20:50:15 GMT  
		Size: 71.0 MB (70995033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61994d980a524616d1c005e5c26edde7a13297ac2984b86f20f39b7aefa8375`  
		Last Modified: Mon, 12 Dec 2022 20:50:07 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:ubuntu`

```console
$ docker pull kong@sha256:df65a153ee9897f9909b1542797ed2ec3556482f64d8086f058c5e34ffc9a460
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:2e482739b5155d63e1cf76e3d6a81909f323552693a36f85cc3033cf4892718b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.7 MB (101724911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b65ea580c9b344f6392f645b956e1f7642e3e48bd0c110b6c0e11336ccce11d6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 01 Feb 2023 11:42:37 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:42:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:42:39 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Wed, 01 Feb 2023 11:42:39 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 19:13:51 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 01 Feb 2023 19:13:51 GMT
ARG ASSET=ce
# Wed, 01 Feb 2023 19:13:51 GMT
ENV ASSET=ce
# Wed, 01 Feb 2023 19:13:51 GMT
ARG EE_PORTS
# Wed, 01 Feb 2023 19:13:51 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Wed, 01 Feb 2023 19:13:51 GMT
ARG KONG_VERSION=3.1.1
# Wed, 01 Feb 2023 19:13:52 GMT
ENV KONG_VERSION=3.1.1
# Wed, 01 Feb 2023 19:13:52 GMT
ARG KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b
# Wed, 01 Feb 2023 19:13:52 GMT
ARG KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
# Wed, 01 Feb 2023 19:14:28 GMT
# ARGS: KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 01 Feb 2023 19:14:29 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 01 Feb 2023 19:14:29 GMT
USER kong
# Wed, 01 Feb 2023 19:14:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Feb 2023 19:14:29 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 01 Feb 2023 19:14:29 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Feb 2023 19:14:29 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 01 Feb 2023 19:14:29 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a22125083e90234102050bb19d1918bdb2c3c04bea9c73a62fe9ccd73c83f60e`  
		Last Modified: Wed, 01 Feb 2023 19:17:08 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e8dc9e1b22d6e7ad79f283f2ab4c4a807ed6e310a25f512783dfba9d33e0fbf`  
		Last Modified: Wed, 01 Feb 2023 19:17:21 GMT  
		Size: 73.1 MB (73146021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d523f9590e88b534d4ccca2f54947d36099583997a52ef86067e3a87de965ce`  
		Last Modified: Wed, 01 Feb 2023 19:17:09 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:2807a54ce70edbd17a4f85420c7ee484b553a19ecbc15df434c08c6a1ea7d178
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.9 MB (98948034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fc3e88b30ac604a1992c70f8d3eea4700df7916403c7f306170be51fce16baf`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 01 Feb 2023 11:27:52 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:27:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:27:52 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:27:56 GMT
ADD file:72ca0af0100de6591b59c44bd8856655c8441eb0fcbf7c32e427f6be5108a4a4 in / 
# Wed, 01 Feb 2023 11:27:56 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:41:14 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 01 Feb 2023 18:41:14 GMT
ARG ASSET=ce
# Wed, 01 Feb 2023 18:41:14 GMT
ENV ASSET=ce
# Wed, 01 Feb 2023 18:41:14 GMT
ARG EE_PORTS
# Wed, 01 Feb 2023 18:41:14 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Wed, 01 Feb 2023 18:41:14 GMT
ARG KONG_VERSION=3.1.1
# Wed, 01 Feb 2023 18:41:14 GMT
ENV KONG_VERSION=3.1.1
# Wed, 01 Feb 2023 18:41:14 GMT
ARG KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b
# Wed, 01 Feb 2023 18:41:14 GMT
ARG KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
# Wed, 01 Feb 2023 18:41:35 GMT
# ARGS: KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 01 Feb 2023 18:41:36 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 01 Feb 2023 18:41:36 GMT
USER kong
# Wed, 01 Feb 2023 18:41:36 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Feb 2023 18:41:36 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 01 Feb 2023 18:41:37 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Feb 2023 18:41:37 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 01 Feb 2023 18:41:37 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:70cf24b162395e1500d40f2b012f253bfd5d15f029ef9d636620fa2365ae503c`  
		Last Modified: Sat, 28 Jan 2023 04:42:53 GMT  
		Size: 27.2 MB (27193737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36cafd2db5bc28f83d39ad8aa707289dd7921854bd71e7466ef84e32030ac701`  
		Last Modified: Wed, 01 Feb 2023 18:46:34 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28f235d14f58889c349b65eecb325ce55df27ab1e42d7683a55ec9046cefe97`  
		Last Modified: Wed, 01 Feb 2023 18:46:43 GMT  
		Size: 71.8 MB (71753287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4c2525fd3153551fc7a4a02eff76bfda933b637a850e4ad32f985a2b6a8e6c`  
		Last Modified: Wed, 01 Feb 2023 18:46:33 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
