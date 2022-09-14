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
$ docker pull kong@sha256:df40856b3bb7775b655016e432f4ab0eb0119dd7e194fda94cf268c159b45d11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.5` - linux; amd64

```console
$ docker pull kong@sha256:3d935fb8d979d10395b5712b3643c489d6085e85b04196f087b0bc4a57655ef1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49219622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:746e0ab1c399ba04ad448f99cba09ef46362b814962136724bbd16a0ff896cc7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:50:59 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 09 Aug 2022 20:50:59 GMT
ARG ASSET=ce
# Tue, 09 Aug 2022 20:50:59 GMT
ENV ASSET=ce
# Tue, 09 Aug 2022 20:51:00 GMT
ARG EE_PORTS
# Tue, 09 Aug 2022 20:51:00 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 09 Aug 2022 20:51:26 GMT
ARG KONG_VERSION=2.5.2
# Tue, 09 Aug 2022 20:51:26 GMT
ENV KONG_VERSION=2.5.2
# Tue, 09 Aug 2022 20:51:26 GMT
ARG KONG_AMD64_SHA=d4bc93bcb14cce8c37ced136632a290b441050c540db779e742bcd88e5cfd70d
# Tue, 09 Aug 2022 20:51:26 GMT
ARG KONG_ARM64_SHA=691e1dc29e96d6a95b60674513932c4f7547773014685ce0130549f980c1c46e
# Tue, 09 Aug 2022 20:51:33 GMT
# ARGS: KONG_AMD64_SHA=d4bc93bcb14cce8c37ced136632a290b441050c540db779e742bcd88e5cfd70d KONG_ARM64_SHA=691e1dc29e96d6a95b60674513932c4f7547773014685ce0130549f980c1c46e
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Tue, 09 Aug 2022 20:51:34 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 09 Aug 2022 20:51:34 GMT
USER kong
# Tue, 09 Aug 2022 20:51:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:51:34 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 09 Aug 2022 20:51:34 GMT
STOPSIGNAL SIGQUIT
# Tue, 09 Aug 2022 20:51:34 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 09 Aug 2022 20:51:34 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb31d71e8b572b72e18738ce5a5ce873f6bdbd4dfe392710abfaa0b239f5e9e`  
		Last Modified: Tue, 09 Aug 2022 20:52:29 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fe5a5d273313cadd6692e26c961154c8b932e85b748175c31cf56d87115e6f8`  
		Last Modified: Tue, 09 Aug 2022 20:53:19 GMT  
		Size: 46.4 MB (46395098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7318b6ebdf194ef2f4893426d03f77cfe5f9c10b99e54bdfc17aabd811165963`  
		Last Modified: Tue, 09 Aug 2022 20:53:11 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.5` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:def066852f719d3e64920b7701673370a967d25714d5d84625b4817b1efc5287
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.4 MB (48424283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12d9df74b229506dd2ac6abf64b84819420d931766015b2cf9b0cd31b0107ad2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:43:11 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 09 Aug 2022 20:43:12 GMT
ARG ASSET=ce
# Tue, 09 Aug 2022 20:43:13 GMT
ENV ASSET=ce
# Tue, 09 Aug 2022 20:43:14 GMT
ARG EE_PORTS
# Tue, 09 Aug 2022 20:43:16 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 09 Aug 2022 20:44:33 GMT
ARG KONG_VERSION=2.5.2
# Tue, 09 Aug 2022 20:44:34 GMT
ENV KONG_VERSION=2.5.2
# Tue, 09 Aug 2022 20:44:35 GMT
ARG KONG_AMD64_SHA=d4bc93bcb14cce8c37ced136632a290b441050c540db779e742bcd88e5cfd70d
# Tue, 09 Aug 2022 20:44:36 GMT
ARG KONG_ARM64_SHA=691e1dc29e96d6a95b60674513932c4f7547773014685ce0130549f980c1c46e
# Tue, 09 Aug 2022 20:44:55 GMT
# ARGS: KONG_AMD64_SHA=d4bc93bcb14cce8c37ced136632a290b441050c540db779e742bcd88e5cfd70d KONG_ARM64_SHA=691e1dc29e96d6a95b60674513932c4f7547773014685ce0130549f980c1c46e
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Tue, 09 Aug 2022 20:44:56 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 09 Aug 2022 20:44:56 GMT
USER kong
# Tue, 09 Aug 2022 20:44:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:44:58 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 09 Aug 2022 20:44:59 GMT
STOPSIGNAL SIGQUIT
# Tue, 09 Aug 2022 20:45:00 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 09 Aug 2022 20:45:01 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf24c8e5476c8b7b4206bb7d73b6e374dd6f847c367e880a7e72e96aa1dfd355`  
		Last Modified: Tue, 09 Aug 2022 20:46:28 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b772d249cbb4432f47594d8c8ae02be54a589b7a07a632fee725bd5519bd1db`  
		Last Modified: Tue, 09 Aug 2022 20:47:28 GMT  
		Size: 45.7 MB (45704832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45bc7a05e46049b909f0b4306fe1ca5056b6545e7f9d7a5649eb5474a5b21c59`  
		Last Modified: Tue, 09 Aug 2022 20:47:20 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.5-ubuntu`

```console
$ docker pull kong@sha256:a4ea19a76be144eb0bfbd913b2e3f028cb60255242433986f344d25be8b6f13a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.5-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:f0165f85b877d4f0c1c82a32c95e36aeac645915cdc65ab88c81d2f0bdb7b4c4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121288727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9932681193075606c9cd3d0d0b908d2e5533eec69af309828ccec1e0cedef490`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:37:42 GMT
ARG ASSET=ce
# Fri, 02 Sep 2022 03:37:42 GMT
ENV ASSET=ce
# Fri, 02 Sep 2022 03:37:42 GMT
ARG EE_PORTS
# Fri, 02 Sep 2022 03:37:42 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Fri, 02 Sep 2022 03:39:13 GMT
ARG KONG_VERSION=2.5.2
# Fri, 02 Sep 2022 03:39:13 GMT
ENV KONG_VERSION=2.5.2
# Fri, 02 Sep 2022 03:39:13 GMT
ARG KONG_AMD64_SHA=ae65ac9eb35f682768abfb080c61581440347db8dafd0a495639ff666a406a96
# Fri, 02 Sep 2022 03:39:13 GMT
ARG KONG_ARM64_SHA=b4720e3d0831d13364cc749200c77df356a2145478f6a55fd48618a9aa1967d9
# Fri, 02 Sep 2022 03:39:33 GMT
# ARGS: KONG_AMD64_SHA=ae65ac9eb35f682768abfb080c61581440347db8dafd0a495639ff666a406a96 KONG_ARM64_SHA=b4720e3d0831d13364cc749200c77df356a2145478f6a55fd48618a9aa1967d9
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 02 Sep 2022 03:39:34 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 02 Sep 2022 03:39:34 GMT
USER kong
# Fri, 02 Sep 2022 03:39:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 03:39:34 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 02 Sep 2022 03:39:34 GMT
STOPSIGNAL SIGQUIT
# Fri, 02 Sep 2022 03:39:34 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 02 Sep 2022 03:39:34 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c91420ce43ec4f22f2debc82905e36cd7e0b308aad6701592278451f47d0e47`  
		Last Modified: Fri, 02 Sep 2022 03:40:04 GMT  
		Size: 25.1 MB (25081963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6f47622da991aefd5e0e19719bb23e917727a07f242654701df0d2d4337782`  
		Last Modified: Fri, 02 Sep 2022 03:41:25 GMT  
		Size: 67.6 MB (67633199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922c8e445febcf021509f69323fdab8e112d68e5b72e4fbe341d7a28343f7094`  
		Last Modified: Fri, 02 Sep 2022 03:41:13 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.5-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:fef02faa1294e9764b5459eea0f2d94f8e76af0f2d02213644ed5f080faffcaa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.3 MB (118326325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d25c1b495c9dc2b4366416298e0c1734c8c0a4258aed983937dec6c81020c05a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:45:21 GMT
ARG ASSET=ce
# Fri, 02 Sep 2022 06:45:21 GMT
ENV ASSET=ce
# Fri, 02 Sep 2022 06:45:22 GMT
ARG EE_PORTS
# Fri, 02 Sep 2022 06:45:24 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Fri, 02 Sep 2022 06:48:38 GMT
ARG KONG_VERSION=2.5.2
# Fri, 02 Sep 2022 06:48:39 GMT
ENV KONG_VERSION=2.5.2
# Fri, 02 Sep 2022 06:48:40 GMT
ARG KONG_AMD64_SHA=ae65ac9eb35f682768abfb080c61581440347db8dafd0a495639ff666a406a96
# Fri, 02 Sep 2022 06:48:41 GMT
ARG KONG_ARM64_SHA=b4720e3d0831d13364cc749200c77df356a2145478f6a55fd48618a9aa1967d9
# Fri, 02 Sep 2022 06:49:14 GMT
# ARGS: KONG_AMD64_SHA=ae65ac9eb35f682768abfb080c61581440347db8dafd0a495639ff666a406a96 KONG_ARM64_SHA=b4720e3d0831d13364cc749200c77df356a2145478f6a55fd48618a9aa1967d9
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 02 Sep 2022 06:49:15 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 02 Sep 2022 06:49:15 GMT
USER kong
# Fri, 02 Sep 2022 06:49:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 06:49:17 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 02 Sep 2022 06:49:18 GMT
STOPSIGNAL SIGQUIT
# Fri, 02 Sep 2022 06:49:19 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 02 Sep 2022 06:49:20 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37921fee9fdc77f083b1d7e6150fcc91eaf74164601930750627e75ec46159c9`  
		Last Modified: Fri, 02 Sep 2022 06:50:16 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0b2a443cdfd26582508b29c8451357d237a3969ee840de1419762fe6dcca86`  
		Last Modified: Fri, 02 Sep 2022 06:51:43 GMT  
		Size: 66.1 MB (66051673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81425dde556f0f3633aa401e78b6bf41e2ce268f10261968c31bd7373e4419c8`  
		Last Modified: Fri, 02 Sep 2022 06:51:30 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.5.2`

```console
$ docker pull kong@sha256:df40856b3bb7775b655016e432f4ab0eb0119dd7e194fda94cf268c159b45d11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.5.2` - linux; amd64

```console
$ docker pull kong@sha256:3d935fb8d979d10395b5712b3643c489d6085e85b04196f087b0bc4a57655ef1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49219622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:746e0ab1c399ba04ad448f99cba09ef46362b814962136724bbd16a0ff896cc7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:50:59 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 09 Aug 2022 20:50:59 GMT
ARG ASSET=ce
# Tue, 09 Aug 2022 20:50:59 GMT
ENV ASSET=ce
# Tue, 09 Aug 2022 20:51:00 GMT
ARG EE_PORTS
# Tue, 09 Aug 2022 20:51:00 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 09 Aug 2022 20:51:26 GMT
ARG KONG_VERSION=2.5.2
# Tue, 09 Aug 2022 20:51:26 GMT
ENV KONG_VERSION=2.5.2
# Tue, 09 Aug 2022 20:51:26 GMT
ARG KONG_AMD64_SHA=d4bc93bcb14cce8c37ced136632a290b441050c540db779e742bcd88e5cfd70d
# Tue, 09 Aug 2022 20:51:26 GMT
ARG KONG_ARM64_SHA=691e1dc29e96d6a95b60674513932c4f7547773014685ce0130549f980c1c46e
# Tue, 09 Aug 2022 20:51:33 GMT
# ARGS: KONG_AMD64_SHA=d4bc93bcb14cce8c37ced136632a290b441050c540db779e742bcd88e5cfd70d KONG_ARM64_SHA=691e1dc29e96d6a95b60674513932c4f7547773014685ce0130549f980c1c46e
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Tue, 09 Aug 2022 20:51:34 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 09 Aug 2022 20:51:34 GMT
USER kong
# Tue, 09 Aug 2022 20:51:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:51:34 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 09 Aug 2022 20:51:34 GMT
STOPSIGNAL SIGQUIT
# Tue, 09 Aug 2022 20:51:34 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 09 Aug 2022 20:51:34 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb31d71e8b572b72e18738ce5a5ce873f6bdbd4dfe392710abfaa0b239f5e9e`  
		Last Modified: Tue, 09 Aug 2022 20:52:29 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fe5a5d273313cadd6692e26c961154c8b932e85b748175c31cf56d87115e6f8`  
		Last Modified: Tue, 09 Aug 2022 20:53:19 GMT  
		Size: 46.4 MB (46395098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7318b6ebdf194ef2f4893426d03f77cfe5f9c10b99e54bdfc17aabd811165963`  
		Last Modified: Tue, 09 Aug 2022 20:53:11 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.5.2` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:def066852f719d3e64920b7701673370a967d25714d5d84625b4817b1efc5287
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.4 MB (48424283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12d9df74b229506dd2ac6abf64b84819420d931766015b2cf9b0cd31b0107ad2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:43:11 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 09 Aug 2022 20:43:12 GMT
ARG ASSET=ce
# Tue, 09 Aug 2022 20:43:13 GMT
ENV ASSET=ce
# Tue, 09 Aug 2022 20:43:14 GMT
ARG EE_PORTS
# Tue, 09 Aug 2022 20:43:16 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 09 Aug 2022 20:44:33 GMT
ARG KONG_VERSION=2.5.2
# Tue, 09 Aug 2022 20:44:34 GMT
ENV KONG_VERSION=2.5.2
# Tue, 09 Aug 2022 20:44:35 GMT
ARG KONG_AMD64_SHA=d4bc93bcb14cce8c37ced136632a290b441050c540db779e742bcd88e5cfd70d
# Tue, 09 Aug 2022 20:44:36 GMT
ARG KONG_ARM64_SHA=691e1dc29e96d6a95b60674513932c4f7547773014685ce0130549f980c1c46e
# Tue, 09 Aug 2022 20:44:55 GMT
# ARGS: KONG_AMD64_SHA=d4bc93bcb14cce8c37ced136632a290b441050c540db779e742bcd88e5cfd70d KONG_ARM64_SHA=691e1dc29e96d6a95b60674513932c4f7547773014685ce0130549f980c1c46e
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Tue, 09 Aug 2022 20:44:56 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 09 Aug 2022 20:44:56 GMT
USER kong
# Tue, 09 Aug 2022 20:44:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:44:58 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 09 Aug 2022 20:44:59 GMT
STOPSIGNAL SIGQUIT
# Tue, 09 Aug 2022 20:45:00 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 09 Aug 2022 20:45:01 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf24c8e5476c8b7b4206bb7d73b6e374dd6f847c367e880a7e72e96aa1dfd355`  
		Last Modified: Tue, 09 Aug 2022 20:46:28 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b772d249cbb4432f47594d8c8ae02be54a589b7a07a632fee725bd5519bd1db`  
		Last Modified: Tue, 09 Aug 2022 20:47:28 GMT  
		Size: 45.7 MB (45704832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45bc7a05e46049b909f0b4306fe1ca5056b6545e7f9d7a5649eb5474a5b21c59`  
		Last Modified: Tue, 09 Aug 2022 20:47:20 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.5.2-alpine`

```console
$ docker pull kong@sha256:df40856b3bb7775b655016e432f4ab0eb0119dd7e194fda94cf268c159b45d11
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.5.2-alpine` - linux; amd64

```console
$ docker pull kong@sha256:3d935fb8d979d10395b5712b3643c489d6085e85b04196f087b0bc4a57655ef1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49219622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:746e0ab1c399ba04ad448f99cba09ef46362b814962136724bbd16a0ff896cc7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:50:59 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 09 Aug 2022 20:50:59 GMT
ARG ASSET=ce
# Tue, 09 Aug 2022 20:50:59 GMT
ENV ASSET=ce
# Tue, 09 Aug 2022 20:51:00 GMT
ARG EE_PORTS
# Tue, 09 Aug 2022 20:51:00 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 09 Aug 2022 20:51:26 GMT
ARG KONG_VERSION=2.5.2
# Tue, 09 Aug 2022 20:51:26 GMT
ENV KONG_VERSION=2.5.2
# Tue, 09 Aug 2022 20:51:26 GMT
ARG KONG_AMD64_SHA=d4bc93bcb14cce8c37ced136632a290b441050c540db779e742bcd88e5cfd70d
# Tue, 09 Aug 2022 20:51:26 GMT
ARG KONG_ARM64_SHA=691e1dc29e96d6a95b60674513932c4f7547773014685ce0130549f980c1c46e
# Tue, 09 Aug 2022 20:51:33 GMT
# ARGS: KONG_AMD64_SHA=d4bc93bcb14cce8c37ced136632a290b441050c540db779e742bcd88e5cfd70d KONG_ARM64_SHA=691e1dc29e96d6a95b60674513932c4f7547773014685ce0130549f980c1c46e
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Tue, 09 Aug 2022 20:51:34 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 09 Aug 2022 20:51:34 GMT
USER kong
# Tue, 09 Aug 2022 20:51:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:51:34 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 09 Aug 2022 20:51:34 GMT
STOPSIGNAL SIGQUIT
# Tue, 09 Aug 2022 20:51:34 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 09 Aug 2022 20:51:34 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb31d71e8b572b72e18738ce5a5ce873f6bdbd4dfe392710abfaa0b239f5e9e`  
		Last Modified: Tue, 09 Aug 2022 20:52:29 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fe5a5d273313cadd6692e26c961154c8b932e85b748175c31cf56d87115e6f8`  
		Last Modified: Tue, 09 Aug 2022 20:53:19 GMT  
		Size: 46.4 MB (46395098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7318b6ebdf194ef2f4893426d03f77cfe5f9c10b99e54bdfc17aabd811165963`  
		Last Modified: Tue, 09 Aug 2022 20:53:11 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.5.2-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:def066852f719d3e64920b7701673370a967d25714d5d84625b4817b1efc5287
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.4 MB (48424283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12d9df74b229506dd2ac6abf64b84819420d931766015b2cf9b0cd31b0107ad2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:43:11 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 09 Aug 2022 20:43:12 GMT
ARG ASSET=ce
# Tue, 09 Aug 2022 20:43:13 GMT
ENV ASSET=ce
# Tue, 09 Aug 2022 20:43:14 GMT
ARG EE_PORTS
# Tue, 09 Aug 2022 20:43:16 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 09 Aug 2022 20:44:33 GMT
ARG KONG_VERSION=2.5.2
# Tue, 09 Aug 2022 20:44:34 GMT
ENV KONG_VERSION=2.5.2
# Tue, 09 Aug 2022 20:44:35 GMT
ARG KONG_AMD64_SHA=d4bc93bcb14cce8c37ced136632a290b441050c540db779e742bcd88e5cfd70d
# Tue, 09 Aug 2022 20:44:36 GMT
ARG KONG_ARM64_SHA=691e1dc29e96d6a95b60674513932c4f7547773014685ce0130549f980c1c46e
# Tue, 09 Aug 2022 20:44:55 GMT
# ARGS: KONG_AMD64_SHA=d4bc93bcb14cce8c37ced136632a290b441050c540db779e742bcd88e5cfd70d KONG_ARM64_SHA=691e1dc29e96d6a95b60674513932c4f7547773014685ce0130549f980c1c46e
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Tue, 09 Aug 2022 20:44:56 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 09 Aug 2022 20:44:56 GMT
USER kong
# Tue, 09 Aug 2022 20:44:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:44:58 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 09 Aug 2022 20:44:59 GMT
STOPSIGNAL SIGQUIT
# Tue, 09 Aug 2022 20:45:00 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 09 Aug 2022 20:45:01 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf24c8e5476c8b7b4206bb7d73b6e374dd6f847c367e880a7e72e96aa1dfd355`  
		Last Modified: Tue, 09 Aug 2022 20:46:28 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b772d249cbb4432f47594d8c8ae02be54a589b7a07a632fee725bd5519bd1db`  
		Last Modified: Tue, 09 Aug 2022 20:47:28 GMT  
		Size: 45.7 MB (45704832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45bc7a05e46049b909f0b4306fe1ca5056b6545e7f9d7a5649eb5474a5b21c59`  
		Last Modified: Tue, 09 Aug 2022 20:47:20 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.5.2-ubuntu`

```console
$ docker pull kong@sha256:a4ea19a76be144eb0bfbd913b2e3f028cb60255242433986f344d25be8b6f13a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.5.2-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:f0165f85b877d4f0c1c82a32c95e36aeac645915cdc65ab88c81d2f0bdb7b4c4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121288727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9932681193075606c9cd3d0d0b908d2e5533eec69af309828ccec1e0cedef490`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:37:42 GMT
ARG ASSET=ce
# Fri, 02 Sep 2022 03:37:42 GMT
ENV ASSET=ce
# Fri, 02 Sep 2022 03:37:42 GMT
ARG EE_PORTS
# Fri, 02 Sep 2022 03:37:42 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Fri, 02 Sep 2022 03:39:13 GMT
ARG KONG_VERSION=2.5.2
# Fri, 02 Sep 2022 03:39:13 GMT
ENV KONG_VERSION=2.5.2
# Fri, 02 Sep 2022 03:39:13 GMT
ARG KONG_AMD64_SHA=ae65ac9eb35f682768abfb080c61581440347db8dafd0a495639ff666a406a96
# Fri, 02 Sep 2022 03:39:13 GMT
ARG KONG_ARM64_SHA=b4720e3d0831d13364cc749200c77df356a2145478f6a55fd48618a9aa1967d9
# Fri, 02 Sep 2022 03:39:33 GMT
# ARGS: KONG_AMD64_SHA=ae65ac9eb35f682768abfb080c61581440347db8dafd0a495639ff666a406a96 KONG_ARM64_SHA=b4720e3d0831d13364cc749200c77df356a2145478f6a55fd48618a9aa1967d9
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 02 Sep 2022 03:39:34 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 02 Sep 2022 03:39:34 GMT
USER kong
# Fri, 02 Sep 2022 03:39:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 03:39:34 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 02 Sep 2022 03:39:34 GMT
STOPSIGNAL SIGQUIT
# Fri, 02 Sep 2022 03:39:34 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 02 Sep 2022 03:39:34 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c91420ce43ec4f22f2debc82905e36cd7e0b308aad6701592278451f47d0e47`  
		Last Modified: Fri, 02 Sep 2022 03:40:04 GMT  
		Size: 25.1 MB (25081963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6f47622da991aefd5e0e19719bb23e917727a07f242654701df0d2d4337782`  
		Last Modified: Fri, 02 Sep 2022 03:41:25 GMT  
		Size: 67.6 MB (67633199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922c8e445febcf021509f69323fdab8e112d68e5b72e4fbe341d7a28343f7094`  
		Last Modified: Fri, 02 Sep 2022 03:41:13 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.5.2-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:fef02faa1294e9764b5459eea0f2d94f8e76af0f2d02213644ed5f080faffcaa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.3 MB (118326325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d25c1b495c9dc2b4366416298e0c1734c8c0a4258aed983937dec6c81020c05a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:45:21 GMT
ARG ASSET=ce
# Fri, 02 Sep 2022 06:45:21 GMT
ENV ASSET=ce
# Fri, 02 Sep 2022 06:45:22 GMT
ARG EE_PORTS
# Fri, 02 Sep 2022 06:45:24 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Fri, 02 Sep 2022 06:48:38 GMT
ARG KONG_VERSION=2.5.2
# Fri, 02 Sep 2022 06:48:39 GMT
ENV KONG_VERSION=2.5.2
# Fri, 02 Sep 2022 06:48:40 GMT
ARG KONG_AMD64_SHA=ae65ac9eb35f682768abfb080c61581440347db8dafd0a495639ff666a406a96
# Fri, 02 Sep 2022 06:48:41 GMT
ARG KONG_ARM64_SHA=b4720e3d0831d13364cc749200c77df356a2145478f6a55fd48618a9aa1967d9
# Fri, 02 Sep 2022 06:49:14 GMT
# ARGS: KONG_AMD64_SHA=ae65ac9eb35f682768abfb080c61581440347db8dafd0a495639ff666a406a96 KONG_ARM64_SHA=b4720e3d0831d13364cc749200c77df356a2145478f6a55fd48618a9aa1967d9
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 02 Sep 2022 06:49:15 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 02 Sep 2022 06:49:15 GMT
USER kong
# Fri, 02 Sep 2022 06:49:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 06:49:17 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 02 Sep 2022 06:49:18 GMT
STOPSIGNAL SIGQUIT
# Fri, 02 Sep 2022 06:49:19 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 02 Sep 2022 06:49:20 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37921fee9fdc77f083b1d7e6150fcc91eaf74164601930750627e75ec46159c9`  
		Last Modified: Fri, 02 Sep 2022 06:50:16 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0b2a443cdfd26582508b29c8451357d237a3969ee840de1419762fe6dcca86`  
		Last Modified: Fri, 02 Sep 2022 06:51:43 GMT  
		Size: 66.1 MB (66051673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81425dde556f0f3633aa401e78b6bf41e2ce268f10261968c31bd7373e4419c8`  
		Last Modified: Fri, 02 Sep 2022 06:51:30 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.6`

```console
$ docker pull kong@sha256:46225823d1a96d0a3a99d1342b8b2f7b09b8c86357d0d4ba78b6359994f7a11b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.6` - linux; amd64

```console
$ docker pull kong@sha256:65fc054f1e133a27e059f36e46ab834ca9d8cc96dc9411ee2a6baea87edd4878
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50240678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:829954c99f0b57a55aa6e7fb54f705d4825b9c86bc923a36a6b8f042112addfd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:50:59 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 09 Aug 2022 20:50:59 GMT
ARG ASSET=ce
# Tue, 09 Aug 2022 20:50:59 GMT
ENV ASSET=ce
# Tue, 09 Aug 2022 20:51:00 GMT
ARG EE_PORTS
# Tue, 09 Aug 2022 20:51:00 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 09 Aug 2022 20:51:13 GMT
ARG KONG_VERSION=2.6.1
# Tue, 09 Aug 2022 20:51:13 GMT
ENV KONG_VERSION=2.6.1
# Tue, 09 Aug 2022 20:51:13 GMT
ARG KONG_AMD64_SHA=9e7618ad06c148ed216be8bbf65a9c7cb95301e5349ef61b996fbb55ec4cfa87
# Tue, 09 Aug 2022 20:51:13 GMT
ARG KONG_ARM64_SHA=0fbf008685c6eac510d221595172e9e7bd51a846d410972d6950d9207cf400de
# Tue, 09 Aug 2022 20:51:20 GMT
# ARGS: KONG_AMD64_SHA=9e7618ad06c148ed216be8bbf65a9c7cb95301e5349ef61b996fbb55ec4cfa87 KONG_ARM64_SHA=0fbf008685c6eac510d221595172e9e7bd51a846d410972d6950d9207cf400de
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Tue, 09 Aug 2022 20:51:20 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 09 Aug 2022 20:51:21 GMT
USER kong
# Tue, 09 Aug 2022 20:51:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:51:21 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 09 Aug 2022 20:51:21 GMT
STOPSIGNAL SIGQUIT
# Tue, 09 Aug 2022 20:51:21 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 09 Aug 2022 20:51:21 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb31d71e8b572b72e18738ce5a5ce873f6bdbd4dfe392710abfaa0b239f5e9e`  
		Last Modified: Tue, 09 Aug 2022 20:52:29 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1143996ec4f5e396697ffc70d6e2d841941f1cb444050571fc9256fea564403d`  
		Last Modified: Tue, 09 Aug 2022 20:52:59 GMT  
		Size: 47.4 MB (47416156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb252670b28cd4ac88ae7c652f83f084aec63230dcf3decf1991f3db8a5ce5f`  
		Last Modified: Tue, 09 Aug 2022 20:52:51 GMT  
		Size: 878.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.6` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:3145b8288dcb870adcd915c96f9b4c96dd9583e4069f6f65026a7fcf62a28502
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.7 MB (49654939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3347c8c9f5cc1b42f01a55c503944a1ae2e9b94e715a74856a92c66ad524f30a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:43:11 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 09 Aug 2022 20:43:12 GMT
ARG ASSET=ce
# Tue, 09 Aug 2022 20:43:13 GMT
ENV ASSET=ce
# Tue, 09 Aug 2022 20:43:14 GMT
ARG EE_PORTS
# Tue, 09 Aug 2022 20:43:16 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 09 Aug 2022 20:43:53 GMT
ARG KONG_VERSION=2.6.1
# Tue, 09 Aug 2022 20:43:54 GMT
ENV KONG_VERSION=2.6.1
# Tue, 09 Aug 2022 20:43:55 GMT
ARG KONG_AMD64_SHA=9e7618ad06c148ed216be8bbf65a9c7cb95301e5349ef61b996fbb55ec4cfa87
# Tue, 09 Aug 2022 20:43:56 GMT
ARG KONG_ARM64_SHA=0fbf008685c6eac510d221595172e9e7bd51a846d410972d6950d9207cf400de
# Tue, 09 Aug 2022 20:44:16 GMT
# ARGS: KONG_AMD64_SHA=9e7618ad06c148ed216be8bbf65a9c7cb95301e5349ef61b996fbb55ec4cfa87 KONG_ARM64_SHA=0fbf008685c6eac510d221595172e9e7bd51a846d410972d6950d9207cf400de
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Tue, 09 Aug 2022 20:44:17 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 09 Aug 2022 20:44:17 GMT
USER kong
# Tue, 09 Aug 2022 20:44:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:44:19 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 09 Aug 2022 20:44:20 GMT
STOPSIGNAL SIGQUIT
# Tue, 09 Aug 2022 20:44:21 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 09 Aug 2022 20:44:22 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf24c8e5476c8b7b4206bb7d73b6e374dd6f847c367e880a7e72e96aa1dfd355`  
		Last Modified: Tue, 09 Aug 2022 20:46:28 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f92c8c87de2bd53ee08911b493553b45eecc09b0940d3958141d2feb9ca3aca`  
		Last Modified: Tue, 09 Aug 2022 20:47:05 GMT  
		Size: 46.9 MB (46935488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab85baf7f0279b614b72664a07828f1e5782e57b6510472232213c12692b2f09`  
		Last Modified: Tue, 09 Aug 2022 20:46:57 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.6-ubuntu`

```console
$ docker pull kong@sha256:f1f0a3d93110a5cf58417282f591adc1601eb48a48188ea9a78b6eae5b04952d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.6-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:9542c3534c12de388a017bd983f456e8b56fe6a700ab87ae43b30de08a7ea617
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128173896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7141d3ecfe4da2a0aee2ccb6ce774482a13d3f961fe489d745d83bb1162796be`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:37:42 GMT
ARG ASSET=ce
# Fri, 02 Sep 2022 03:37:42 GMT
ENV ASSET=ce
# Fri, 02 Sep 2022 03:37:42 GMT
ARG EE_PORTS
# Fri, 02 Sep 2022 03:37:42 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Fri, 02 Sep 2022 03:38:43 GMT
ARG KONG_VERSION=2.6.1
# Fri, 02 Sep 2022 03:38:43 GMT
ENV KONG_VERSION=2.6.1
# Fri, 02 Sep 2022 03:38:43 GMT
ARG KONG_AMD64_SHA=f70757f9317a1d40316f0187ae6e91c0c94b5b4346e564f7ae8430775bf7ad7e
# Fri, 02 Sep 2022 03:38:43 GMT
ARG KONG_ARM64_SHA=5cba6e7e28685fb7d80b77b70586cfb92c1de4b5198a6218bb1ca0c7f2502c89
# Fri, 02 Sep 2022 03:39:04 GMT
# ARGS: KONG_AMD64_SHA=f70757f9317a1d40316f0187ae6e91c0c94b5b4346e564f7ae8430775bf7ad7e KONG_ARM64_SHA=5cba6e7e28685fb7d80b77b70586cfb92c1de4b5198a6218bb1ca0c7f2502c89
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 02 Sep 2022 03:39:04 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 02 Sep 2022 03:39:04 GMT
USER kong
# Fri, 02 Sep 2022 03:39:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 03:39:05 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 02 Sep 2022 03:39:05 GMT
STOPSIGNAL SIGQUIT
# Fri, 02 Sep 2022 03:39:05 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 02 Sep 2022 03:39:05 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c91420ce43ec4f22f2debc82905e36cd7e0b308aad6701592278451f47d0e47`  
		Last Modified: Fri, 02 Sep 2022 03:40:04 GMT  
		Size: 25.1 MB (25081963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc70d4ea1dfaab2507ec7af1d45cf68d7bf3f288f69f4d72bc49aa4bca1b0b9`  
		Last Modified: Fri, 02 Sep 2022 03:41:01 GMT  
		Size: 74.5 MB (74518367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996eb19874f3e7d9bd5d389c9fdb2408eac42034c5cdc4ef5ce7ff1e58394e6f`  
		Last Modified: Fri, 02 Sep 2022 03:40:49 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.6-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:2893d9e2097a13a8fa441a6feee2e8f841ee40f1154db0b29b8bd15442f8806c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125228638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c65cde00a4855e6b742ae0ef16aa109f46eb8e0bd672d422867350bd827ef19d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:45:21 GMT
ARG ASSET=ce
# Fri, 02 Sep 2022 06:45:21 GMT
ENV ASSET=ce
# Fri, 02 Sep 2022 06:45:22 GMT
ARG EE_PORTS
# Fri, 02 Sep 2022 06:45:24 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Fri, 02 Sep 2022 06:47:22 GMT
ARG KONG_VERSION=2.6.1
# Fri, 02 Sep 2022 06:47:22 GMT
ENV KONG_VERSION=2.6.1
# Fri, 02 Sep 2022 06:47:23 GMT
ARG KONG_AMD64_SHA=f70757f9317a1d40316f0187ae6e91c0c94b5b4346e564f7ae8430775bf7ad7e
# Fri, 02 Sep 2022 06:47:24 GMT
ARG KONG_ARM64_SHA=5cba6e7e28685fb7d80b77b70586cfb92c1de4b5198a6218bb1ca0c7f2502c89
# Fri, 02 Sep 2022 06:48:16 GMT
# ARGS: KONG_AMD64_SHA=f70757f9317a1d40316f0187ae6e91c0c94b5b4346e564f7ae8430775bf7ad7e KONG_ARM64_SHA=5cba6e7e28685fb7d80b77b70586cfb92c1de4b5198a6218bb1ca0c7f2502c89
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 02 Sep 2022 06:48:17 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 02 Sep 2022 06:48:17 GMT
USER kong
# Fri, 02 Sep 2022 06:48:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 06:48:19 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 02 Sep 2022 06:48:20 GMT
STOPSIGNAL SIGQUIT
# Fri, 02 Sep 2022 06:48:21 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 02 Sep 2022 06:48:22 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37921fee9fdc77f083b1d7e6150fcc91eaf74164601930750627e75ec46159c9`  
		Last Modified: Fri, 02 Sep 2022 06:50:16 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5420de1b8ed7685ab84c5348ce89a133d3d14841dac3b64f067a0cc3549d059`  
		Last Modified: Fri, 02 Sep 2022 06:51:18 GMT  
		Size: 73.0 MB (72953986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90397f614ccf5812e5f0e0639025b0d1a36aabff4a61243a0ec8237bab890f84`  
		Last Modified: Fri, 02 Sep 2022 06:51:06 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.6.1`

```console
$ docker pull kong@sha256:46225823d1a96d0a3a99d1342b8b2f7b09b8c86357d0d4ba78b6359994f7a11b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.6.1` - linux; amd64

```console
$ docker pull kong@sha256:65fc054f1e133a27e059f36e46ab834ca9d8cc96dc9411ee2a6baea87edd4878
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50240678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:829954c99f0b57a55aa6e7fb54f705d4825b9c86bc923a36a6b8f042112addfd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:50:59 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 09 Aug 2022 20:50:59 GMT
ARG ASSET=ce
# Tue, 09 Aug 2022 20:50:59 GMT
ENV ASSET=ce
# Tue, 09 Aug 2022 20:51:00 GMT
ARG EE_PORTS
# Tue, 09 Aug 2022 20:51:00 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 09 Aug 2022 20:51:13 GMT
ARG KONG_VERSION=2.6.1
# Tue, 09 Aug 2022 20:51:13 GMT
ENV KONG_VERSION=2.6.1
# Tue, 09 Aug 2022 20:51:13 GMT
ARG KONG_AMD64_SHA=9e7618ad06c148ed216be8bbf65a9c7cb95301e5349ef61b996fbb55ec4cfa87
# Tue, 09 Aug 2022 20:51:13 GMT
ARG KONG_ARM64_SHA=0fbf008685c6eac510d221595172e9e7bd51a846d410972d6950d9207cf400de
# Tue, 09 Aug 2022 20:51:20 GMT
# ARGS: KONG_AMD64_SHA=9e7618ad06c148ed216be8bbf65a9c7cb95301e5349ef61b996fbb55ec4cfa87 KONG_ARM64_SHA=0fbf008685c6eac510d221595172e9e7bd51a846d410972d6950d9207cf400de
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Tue, 09 Aug 2022 20:51:20 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 09 Aug 2022 20:51:21 GMT
USER kong
# Tue, 09 Aug 2022 20:51:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:51:21 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 09 Aug 2022 20:51:21 GMT
STOPSIGNAL SIGQUIT
# Tue, 09 Aug 2022 20:51:21 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 09 Aug 2022 20:51:21 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb31d71e8b572b72e18738ce5a5ce873f6bdbd4dfe392710abfaa0b239f5e9e`  
		Last Modified: Tue, 09 Aug 2022 20:52:29 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1143996ec4f5e396697ffc70d6e2d841941f1cb444050571fc9256fea564403d`  
		Last Modified: Tue, 09 Aug 2022 20:52:59 GMT  
		Size: 47.4 MB (47416156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb252670b28cd4ac88ae7c652f83f084aec63230dcf3decf1991f3db8a5ce5f`  
		Last Modified: Tue, 09 Aug 2022 20:52:51 GMT  
		Size: 878.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.6.1` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:3145b8288dcb870adcd915c96f9b4c96dd9583e4069f6f65026a7fcf62a28502
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.7 MB (49654939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3347c8c9f5cc1b42f01a55c503944a1ae2e9b94e715a74856a92c66ad524f30a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:43:11 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 09 Aug 2022 20:43:12 GMT
ARG ASSET=ce
# Tue, 09 Aug 2022 20:43:13 GMT
ENV ASSET=ce
# Tue, 09 Aug 2022 20:43:14 GMT
ARG EE_PORTS
# Tue, 09 Aug 2022 20:43:16 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 09 Aug 2022 20:43:53 GMT
ARG KONG_VERSION=2.6.1
# Tue, 09 Aug 2022 20:43:54 GMT
ENV KONG_VERSION=2.6.1
# Tue, 09 Aug 2022 20:43:55 GMT
ARG KONG_AMD64_SHA=9e7618ad06c148ed216be8bbf65a9c7cb95301e5349ef61b996fbb55ec4cfa87
# Tue, 09 Aug 2022 20:43:56 GMT
ARG KONG_ARM64_SHA=0fbf008685c6eac510d221595172e9e7bd51a846d410972d6950d9207cf400de
# Tue, 09 Aug 2022 20:44:16 GMT
# ARGS: KONG_AMD64_SHA=9e7618ad06c148ed216be8bbf65a9c7cb95301e5349ef61b996fbb55ec4cfa87 KONG_ARM64_SHA=0fbf008685c6eac510d221595172e9e7bd51a846d410972d6950d9207cf400de
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Tue, 09 Aug 2022 20:44:17 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 09 Aug 2022 20:44:17 GMT
USER kong
# Tue, 09 Aug 2022 20:44:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:44:19 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 09 Aug 2022 20:44:20 GMT
STOPSIGNAL SIGQUIT
# Tue, 09 Aug 2022 20:44:21 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 09 Aug 2022 20:44:22 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf24c8e5476c8b7b4206bb7d73b6e374dd6f847c367e880a7e72e96aa1dfd355`  
		Last Modified: Tue, 09 Aug 2022 20:46:28 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f92c8c87de2bd53ee08911b493553b45eecc09b0940d3958141d2feb9ca3aca`  
		Last Modified: Tue, 09 Aug 2022 20:47:05 GMT  
		Size: 46.9 MB (46935488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab85baf7f0279b614b72664a07828f1e5782e57b6510472232213c12692b2f09`  
		Last Modified: Tue, 09 Aug 2022 20:46:57 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.6.1-alpine`

```console
$ docker pull kong@sha256:46225823d1a96d0a3a99d1342b8b2f7b09b8c86357d0d4ba78b6359994f7a11b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.6.1-alpine` - linux; amd64

```console
$ docker pull kong@sha256:65fc054f1e133a27e059f36e46ab834ca9d8cc96dc9411ee2a6baea87edd4878
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50240678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:829954c99f0b57a55aa6e7fb54f705d4825b9c86bc923a36a6b8f042112addfd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:50:59 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 09 Aug 2022 20:50:59 GMT
ARG ASSET=ce
# Tue, 09 Aug 2022 20:50:59 GMT
ENV ASSET=ce
# Tue, 09 Aug 2022 20:51:00 GMT
ARG EE_PORTS
# Tue, 09 Aug 2022 20:51:00 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 09 Aug 2022 20:51:13 GMT
ARG KONG_VERSION=2.6.1
# Tue, 09 Aug 2022 20:51:13 GMT
ENV KONG_VERSION=2.6.1
# Tue, 09 Aug 2022 20:51:13 GMT
ARG KONG_AMD64_SHA=9e7618ad06c148ed216be8bbf65a9c7cb95301e5349ef61b996fbb55ec4cfa87
# Tue, 09 Aug 2022 20:51:13 GMT
ARG KONG_ARM64_SHA=0fbf008685c6eac510d221595172e9e7bd51a846d410972d6950d9207cf400de
# Tue, 09 Aug 2022 20:51:20 GMT
# ARGS: KONG_AMD64_SHA=9e7618ad06c148ed216be8bbf65a9c7cb95301e5349ef61b996fbb55ec4cfa87 KONG_ARM64_SHA=0fbf008685c6eac510d221595172e9e7bd51a846d410972d6950d9207cf400de
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Tue, 09 Aug 2022 20:51:20 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 09 Aug 2022 20:51:21 GMT
USER kong
# Tue, 09 Aug 2022 20:51:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:51:21 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 09 Aug 2022 20:51:21 GMT
STOPSIGNAL SIGQUIT
# Tue, 09 Aug 2022 20:51:21 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 09 Aug 2022 20:51:21 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb31d71e8b572b72e18738ce5a5ce873f6bdbd4dfe392710abfaa0b239f5e9e`  
		Last Modified: Tue, 09 Aug 2022 20:52:29 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1143996ec4f5e396697ffc70d6e2d841941f1cb444050571fc9256fea564403d`  
		Last Modified: Tue, 09 Aug 2022 20:52:59 GMT  
		Size: 47.4 MB (47416156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb252670b28cd4ac88ae7c652f83f084aec63230dcf3decf1991f3db8a5ce5f`  
		Last Modified: Tue, 09 Aug 2022 20:52:51 GMT  
		Size: 878.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.6.1-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:3145b8288dcb870adcd915c96f9b4c96dd9583e4069f6f65026a7fcf62a28502
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.7 MB (49654939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3347c8c9f5cc1b42f01a55c503944a1ae2e9b94e715a74856a92c66ad524f30a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:43:11 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 09 Aug 2022 20:43:12 GMT
ARG ASSET=ce
# Tue, 09 Aug 2022 20:43:13 GMT
ENV ASSET=ce
# Tue, 09 Aug 2022 20:43:14 GMT
ARG EE_PORTS
# Tue, 09 Aug 2022 20:43:16 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 09 Aug 2022 20:43:53 GMT
ARG KONG_VERSION=2.6.1
# Tue, 09 Aug 2022 20:43:54 GMT
ENV KONG_VERSION=2.6.1
# Tue, 09 Aug 2022 20:43:55 GMT
ARG KONG_AMD64_SHA=9e7618ad06c148ed216be8bbf65a9c7cb95301e5349ef61b996fbb55ec4cfa87
# Tue, 09 Aug 2022 20:43:56 GMT
ARG KONG_ARM64_SHA=0fbf008685c6eac510d221595172e9e7bd51a846d410972d6950d9207cf400de
# Tue, 09 Aug 2022 20:44:16 GMT
# ARGS: KONG_AMD64_SHA=9e7618ad06c148ed216be8bbf65a9c7cb95301e5349ef61b996fbb55ec4cfa87 KONG_ARM64_SHA=0fbf008685c6eac510d221595172e9e7bd51a846d410972d6950d9207cf400de
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Tue, 09 Aug 2022 20:44:17 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 09 Aug 2022 20:44:17 GMT
USER kong
# Tue, 09 Aug 2022 20:44:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:44:19 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 09 Aug 2022 20:44:20 GMT
STOPSIGNAL SIGQUIT
# Tue, 09 Aug 2022 20:44:21 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 09 Aug 2022 20:44:22 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf24c8e5476c8b7b4206bb7d73b6e374dd6f847c367e880a7e72e96aa1dfd355`  
		Last Modified: Tue, 09 Aug 2022 20:46:28 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f92c8c87de2bd53ee08911b493553b45eecc09b0940d3958141d2feb9ca3aca`  
		Last Modified: Tue, 09 Aug 2022 20:47:05 GMT  
		Size: 46.9 MB (46935488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab85baf7f0279b614b72664a07828f1e5782e57b6510472232213c12692b2f09`  
		Last Modified: Tue, 09 Aug 2022 20:46:57 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.6.1-ubuntu`

```console
$ docker pull kong@sha256:f1f0a3d93110a5cf58417282f591adc1601eb48a48188ea9a78b6eae5b04952d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.6.1-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:9542c3534c12de388a017bd983f456e8b56fe6a700ab87ae43b30de08a7ea617
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128173896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7141d3ecfe4da2a0aee2ccb6ce774482a13d3f961fe489d745d83bb1162796be`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:37:42 GMT
ARG ASSET=ce
# Fri, 02 Sep 2022 03:37:42 GMT
ENV ASSET=ce
# Fri, 02 Sep 2022 03:37:42 GMT
ARG EE_PORTS
# Fri, 02 Sep 2022 03:37:42 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Fri, 02 Sep 2022 03:38:43 GMT
ARG KONG_VERSION=2.6.1
# Fri, 02 Sep 2022 03:38:43 GMT
ENV KONG_VERSION=2.6.1
# Fri, 02 Sep 2022 03:38:43 GMT
ARG KONG_AMD64_SHA=f70757f9317a1d40316f0187ae6e91c0c94b5b4346e564f7ae8430775bf7ad7e
# Fri, 02 Sep 2022 03:38:43 GMT
ARG KONG_ARM64_SHA=5cba6e7e28685fb7d80b77b70586cfb92c1de4b5198a6218bb1ca0c7f2502c89
# Fri, 02 Sep 2022 03:39:04 GMT
# ARGS: KONG_AMD64_SHA=f70757f9317a1d40316f0187ae6e91c0c94b5b4346e564f7ae8430775bf7ad7e KONG_ARM64_SHA=5cba6e7e28685fb7d80b77b70586cfb92c1de4b5198a6218bb1ca0c7f2502c89
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 02 Sep 2022 03:39:04 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 02 Sep 2022 03:39:04 GMT
USER kong
# Fri, 02 Sep 2022 03:39:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 03:39:05 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 02 Sep 2022 03:39:05 GMT
STOPSIGNAL SIGQUIT
# Fri, 02 Sep 2022 03:39:05 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 02 Sep 2022 03:39:05 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c91420ce43ec4f22f2debc82905e36cd7e0b308aad6701592278451f47d0e47`  
		Last Modified: Fri, 02 Sep 2022 03:40:04 GMT  
		Size: 25.1 MB (25081963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc70d4ea1dfaab2507ec7af1d45cf68d7bf3f288f69f4d72bc49aa4bca1b0b9`  
		Last Modified: Fri, 02 Sep 2022 03:41:01 GMT  
		Size: 74.5 MB (74518367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996eb19874f3e7d9bd5d389c9fdb2408eac42034c5cdc4ef5ce7ff1e58394e6f`  
		Last Modified: Fri, 02 Sep 2022 03:40:49 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.6.1-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:2893d9e2097a13a8fa441a6feee2e8f841ee40f1154db0b29b8bd15442f8806c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125228638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c65cde00a4855e6b742ae0ef16aa109f46eb8e0bd672d422867350bd827ef19d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:45:21 GMT
ARG ASSET=ce
# Fri, 02 Sep 2022 06:45:21 GMT
ENV ASSET=ce
# Fri, 02 Sep 2022 06:45:22 GMT
ARG EE_PORTS
# Fri, 02 Sep 2022 06:45:24 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Fri, 02 Sep 2022 06:47:22 GMT
ARG KONG_VERSION=2.6.1
# Fri, 02 Sep 2022 06:47:22 GMT
ENV KONG_VERSION=2.6.1
# Fri, 02 Sep 2022 06:47:23 GMT
ARG KONG_AMD64_SHA=f70757f9317a1d40316f0187ae6e91c0c94b5b4346e564f7ae8430775bf7ad7e
# Fri, 02 Sep 2022 06:47:24 GMT
ARG KONG_ARM64_SHA=5cba6e7e28685fb7d80b77b70586cfb92c1de4b5198a6218bb1ca0c7f2502c89
# Fri, 02 Sep 2022 06:48:16 GMT
# ARGS: KONG_AMD64_SHA=f70757f9317a1d40316f0187ae6e91c0c94b5b4346e564f7ae8430775bf7ad7e KONG_ARM64_SHA=5cba6e7e28685fb7d80b77b70586cfb92c1de4b5198a6218bb1ca0c7f2502c89
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 02 Sep 2022 06:48:17 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 02 Sep 2022 06:48:17 GMT
USER kong
# Fri, 02 Sep 2022 06:48:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 06:48:19 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 02 Sep 2022 06:48:20 GMT
STOPSIGNAL SIGQUIT
# Fri, 02 Sep 2022 06:48:21 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 02 Sep 2022 06:48:22 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37921fee9fdc77f083b1d7e6150fcc91eaf74164601930750627e75ec46159c9`  
		Last Modified: Fri, 02 Sep 2022 06:50:16 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5420de1b8ed7685ab84c5348ce89a133d3d14841dac3b64f067a0cc3549d059`  
		Last Modified: Fri, 02 Sep 2022 06:51:18 GMT  
		Size: 73.0 MB (72953986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90397f614ccf5812e5f0e0639025b0d1a36aabff4a61243a0ec8237bab890f84`  
		Last Modified: Fri, 02 Sep 2022 06:51:06 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.7`

```console
$ docker pull kong@sha256:c60af2f8633d4719bd6c8989de3a9e7c88cc500a17f1e371ec1f0dc51b6182bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.7` - linux; amd64

```console
$ docker pull kong@sha256:9c21d4bc5aae773be7872c2edd2e0d0fa365352984311e234d39e4a9708fb74c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50148848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dade8e963fd6f83ecc1ae7b3e50718539c7b263ff1fea242893d39800014e0d2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:50:59 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 09 Aug 2022 20:50:59 GMT
ARG ASSET=ce
# Tue, 09 Aug 2022 20:50:59 GMT
ENV ASSET=ce
# Tue, 09 Aug 2022 20:51:00 GMT
ARG EE_PORTS
# Tue, 09 Aug 2022 20:51:00 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 09 Aug 2022 20:51:00 GMT
ARG KONG_VERSION=2.7.2
# Tue, 09 Aug 2022 20:51:00 GMT
ENV KONG_VERSION=2.7.2
# Tue, 09 Aug 2022 20:51:00 GMT
ARG KONG_AMD64_SHA=16990765aee26fc194992f0f90fc81e78a46d77cd0fc1e6670f3b2f797c1fe6b
# Tue, 09 Aug 2022 20:51:00 GMT
ARG KONG_ARM64_SHA=3e5dde2479d53299e81dd903a04e30302108b0864c996a3662fda24ca7aee9f6
# Tue, 09 Aug 2022 20:51:07 GMT
# ARGS: KONG_AMD64_SHA=16990765aee26fc194992f0f90fc81e78a46d77cd0fc1e6670f3b2f797c1fe6b KONG_ARM64_SHA=3e5dde2479d53299e81dd903a04e30302108b0864c996a3662fda24ca7aee9f6
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Tue, 09 Aug 2022 20:51:08 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 09 Aug 2022 20:51:08 GMT
USER kong
# Tue, 09 Aug 2022 20:51:08 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:51:08 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 09 Aug 2022 20:51:08 GMT
STOPSIGNAL SIGQUIT
# Tue, 09 Aug 2022 20:51:08 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 09 Aug 2022 20:51:08 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb31d71e8b572b72e18738ce5a5ce873f6bdbd4dfe392710abfaa0b239f5e9e`  
		Last Modified: Tue, 09 Aug 2022 20:52:29 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bcaa0cf883df54fdb29ac9dbf919864e35c4557da6490c9fc6d6a0e58172aa8`  
		Last Modified: Tue, 09 Aug 2022 20:52:37 GMT  
		Size: 47.3 MB (47324324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb36999ccc7dbbae9dc7ae7adff69f22b48a3d2b6a56cab3458f90a1c2ef9f89`  
		Last Modified: Tue, 09 Aug 2022 20:52:29 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.7` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:39ba2815ffe5f5c822fb1a66c61abea4cc4ecc83eb3086cc04cbc9c82d23b040
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49578744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8860d91130909d7b20b4ca98a3d0402047cf8f45b60ffdd15418f8c258718f5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:43:11 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 09 Aug 2022 20:43:12 GMT
ARG ASSET=ce
# Tue, 09 Aug 2022 20:43:13 GMT
ENV ASSET=ce
# Tue, 09 Aug 2022 20:43:14 GMT
ARG EE_PORTS
# Tue, 09 Aug 2022 20:43:16 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 09 Aug 2022 20:43:16 GMT
ARG KONG_VERSION=2.7.2
# Tue, 09 Aug 2022 20:43:17 GMT
ENV KONG_VERSION=2.7.2
# Tue, 09 Aug 2022 20:43:18 GMT
ARG KONG_AMD64_SHA=16990765aee26fc194992f0f90fc81e78a46d77cd0fc1e6670f3b2f797c1fe6b
# Tue, 09 Aug 2022 20:43:19 GMT
ARG KONG_ARM64_SHA=3e5dde2479d53299e81dd903a04e30302108b0864c996a3662fda24ca7aee9f6
# Tue, 09 Aug 2022 20:43:37 GMT
# ARGS: KONG_AMD64_SHA=16990765aee26fc194992f0f90fc81e78a46d77cd0fc1e6670f3b2f797c1fe6b KONG_ARM64_SHA=3e5dde2479d53299e81dd903a04e30302108b0864c996a3662fda24ca7aee9f6
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Tue, 09 Aug 2022 20:43:38 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 09 Aug 2022 20:43:38 GMT
USER kong
# Tue, 09 Aug 2022 20:43:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:43:40 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 09 Aug 2022 20:43:41 GMT
STOPSIGNAL SIGQUIT
# Tue, 09 Aug 2022 20:43:42 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 09 Aug 2022 20:43:43 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf24c8e5476c8b7b4206bb7d73b6e374dd6f847c367e880a7e72e96aa1dfd355`  
		Last Modified: Tue, 09 Aug 2022 20:46:28 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c33ef81acec69a7618df2a3ff9095806decd55b4e1fe788bd6bd678ee4d8bb`  
		Last Modified: Tue, 09 Aug 2022 20:46:42 GMT  
		Size: 46.9 MB (46859292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f72441bb69318c800b3f9710d8aee21166344bb91a8a3274d9f3ab1b08db01f`  
		Last Modified: Tue, 09 Aug 2022 20:46:28 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.7-ubuntu`

```console
$ docker pull kong@sha256:5d98d90b3037ce816979b9d5397d1395a6f41d2e7b6875aa2b4e60113941ff65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.7-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:b7761ac4593efe882d1a45d1a56e965957c874c72f4f464bb54be0b917afa3cd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.1 MB (128088407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:652ae2e6d172008f0b7ee7a6e4da0d57749a376d8101b0b73cf9719e0793d955`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:37:42 GMT
ARG ASSET=ce
# Fri, 02 Sep 2022 03:37:42 GMT
ENV ASSET=ce
# Fri, 02 Sep 2022 03:37:42 GMT
ARG EE_PORTS
# Fri, 02 Sep 2022 03:37:42 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Fri, 02 Sep 2022 03:38:12 GMT
ARG KONG_VERSION=2.7.2
# Fri, 02 Sep 2022 03:38:13 GMT
ENV KONG_VERSION=2.7.2
# Fri, 02 Sep 2022 03:38:13 GMT
ARG KONG_AMD64_SHA=8124ddbfe80a1627b19a54e14b20ff0e176549699491cf5c61a4f0355470f8fc
# Fri, 02 Sep 2022 03:38:13 GMT
ARG KONG_ARM64_SHA=f40e616539ab64cb4fd333d19895ec9768b742bc25e5f2dbcb7f162bf90421d8
# Fri, 02 Sep 2022 03:38:33 GMT
# ARGS: KONG_AMD64_SHA=8124ddbfe80a1627b19a54e14b20ff0e176549699491cf5c61a4f0355470f8fc KONG_ARM64_SHA=f40e616539ab64cb4fd333d19895ec9768b742bc25e5f2dbcb7f162bf90421d8
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 02 Sep 2022 03:38:34 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 02 Sep 2022 03:38:34 GMT
USER kong
# Fri, 02 Sep 2022 03:38:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 03:38:34 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 02 Sep 2022 03:38:34 GMT
STOPSIGNAL SIGQUIT
# Fri, 02 Sep 2022 03:38:34 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 02 Sep 2022 03:38:34 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c91420ce43ec4f22f2debc82905e36cd7e0b308aad6701592278451f47d0e47`  
		Last Modified: Fri, 02 Sep 2022 03:40:04 GMT  
		Size: 25.1 MB (25081963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a9c69d1c8646312e7aad5c278ebfc2735949c11c3d95f2882e4e375339bb2`  
		Last Modified: Fri, 02 Sep 2022 03:40:38 GMT  
		Size: 74.4 MB (74432878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244eabcc9d362a5616a52dc4dfbf0b6de8598cb0ddd7e2eca6f3f47ad2d6b374`  
		Last Modified: Fri, 02 Sep 2022 03:40:26 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.7-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:bec46695261737d5fa1cc18d747b1113fbc97ecc7b67fc5bf1977df405eebe4c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.1 MB (125139673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ddc4984898199e1d8ea33ec26db00909306fd3050b2753dcb895688c620645b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:45:21 GMT
ARG ASSET=ce
# Fri, 02 Sep 2022 06:45:21 GMT
ENV ASSET=ce
# Fri, 02 Sep 2022 06:45:22 GMT
ARG EE_PORTS
# Fri, 02 Sep 2022 06:45:24 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Fri, 02 Sep 2022 06:46:16 GMT
ARG KONG_VERSION=2.7.2
# Fri, 02 Sep 2022 06:46:17 GMT
ENV KONG_VERSION=2.7.2
# Fri, 02 Sep 2022 06:46:18 GMT
ARG KONG_AMD64_SHA=8124ddbfe80a1627b19a54e14b20ff0e176549699491cf5c61a4f0355470f8fc
# Fri, 02 Sep 2022 06:46:19 GMT
ARG KONG_ARM64_SHA=f40e616539ab64cb4fd333d19895ec9768b742bc25e5f2dbcb7f162bf90421d8
# Fri, 02 Sep 2022 06:46:59 GMT
# ARGS: KONG_AMD64_SHA=8124ddbfe80a1627b19a54e14b20ff0e176549699491cf5c61a4f0355470f8fc KONG_ARM64_SHA=f40e616539ab64cb4fd333d19895ec9768b742bc25e5f2dbcb7f162bf90421d8
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 02 Sep 2022 06:47:00 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 02 Sep 2022 06:47:00 GMT
USER kong
# Fri, 02 Sep 2022 06:47:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 06:47:02 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 02 Sep 2022 06:47:03 GMT
STOPSIGNAL SIGQUIT
# Fri, 02 Sep 2022 06:47:04 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 02 Sep 2022 06:47:05 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37921fee9fdc77f083b1d7e6150fcc91eaf74164601930750627e75ec46159c9`  
		Last Modified: Fri, 02 Sep 2022 06:50:16 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e533f40a36a4076913850a50f0c4b06bedeaf27953e9ff68eb0409147ff9b8b8`  
		Last Modified: Fri, 02 Sep 2022 06:50:53 GMT  
		Size: 72.9 MB (72865021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8895e832ae3976fab3fdf671159d4f380325a31968556cad1ff49144e418909`  
		Last Modified: Fri, 02 Sep 2022 06:50:41 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.7.2`

```console
$ docker pull kong@sha256:c60af2f8633d4719bd6c8989de3a9e7c88cc500a17f1e371ec1f0dc51b6182bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.7.2` - linux; amd64

```console
$ docker pull kong@sha256:9c21d4bc5aae773be7872c2edd2e0d0fa365352984311e234d39e4a9708fb74c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50148848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dade8e963fd6f83ecc1ae7b3e50718539c7b263ff1fea242893d39800014e0d2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:50:59 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 09 Aug 2022 20:50:59 GMT
ARG ASSET=ce
# Tue, 09 Aug 2022 20:50:59 GMT
ENV ASSET=ce
# Tue, 09 Aug 2022 20:51:00 GMT
ARG EE_PORTS
# Tue, 09 Aug 2022 20:51:00 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 09 Aug 2022 20:51:00 GMT
ARG KONG_VERSION=2.7.2
# Tue, 09 Aug 2022 20:51:00 GMT
ENV KONG_VERSION=2.7.2
# Tue, 09 Aug 2022 20:51:00 GMT
ARG KONG_AMD64_SHA=16990765aee26fc194992f0f90fc81e78a46d77cd0fc1e6670f3b2f797c1fe6b
# Tue, 09 Aug 2022 20:51:00 GMT
ARG KONG_ARM64_SHA=3e5dde2479d53299e81dd903a04e30302108b0864c996a3662fda24ca7aee9f6
# Tue, 09 Aug 2022 20:51:07 GMT
# ARGS: KONG_AMD64_SHA=16990765aee26fc194992f0f90fc81e78a46d77cd0fc1e6670f3b2f797c1fe6b KONG_ARM64_SHA=3e5dde2479d53299e81dd903a04e30302108b0864c996a3662fda24ca7aee9f6
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Tue, 09 Aug 2022 20:51:08 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 09 Aug 2022 20:51:08 GMT
USER kong
# Tue, 09 Aug 2022 20:51:08 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:51:08 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 09 Aug 2022 20:51:08 GMT
STOPSIGNAL SIGQUIT
# Tue, 09 Aug 2022 20:51:08 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 09 Aug 2022 20:51:08 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb31d71e8b572b72e18738ce5a5ce873f6bdbd4dfe392710abfaa0b239f5e9e`  
		Last Modified: Tue, 09 Aug 2022 20:52:29 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bcaa0cf883df54fdb29ac9dbf919864e35c4557da6490c9fc6d6a0e58172aa8`  
		Last Modified: Tue, 09 Aug 2022 20:52:37 GMT  
		Size: 47.3 MB (47324324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb36999ccc7dbbae9dc7ae7adff69f22b48a3d2b6a56cab3458f90a1c2ef9f89`  
		Last Modified: Tue, 09 Aug 2022 20:52:29 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.7.2` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:39ba2815ffe5f5c822fb1a66c61abea4cc4ecc83eb3086cc04cbc9c82d23b040
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49578744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8860d91130909d7b20b4ca98a3d0402047cf8f45b60ffdd15418f8c258718f5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:43:11 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 09 Aug 2022 20:43:12 GMT
ARG ASSET=ce
# Tue, 09 Aug 2022 20:43:13 GMT
ENV ASSET=ce
# Tue, 09 Aug 2022 20:43:14 GMT
ARG EE_PORTS
# Tue, 09 Aug 2022 20:43:16 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 09 Aug 2022 20:43:16 GMT
ARG KONG_VERSION=2.7.2
# Tue, 09 Aug 2022 20:43:17 GMT
ENV KONG_VERSION=2.7.2
# Tue, 09 Aug 2022 20:43:18 GMT
ARG KONG_AMD64_SHA=16990765aee26fc194992f0f90fc81e78a46d77cd0fc1e6670f3b2f797c1fe6b
# Tue, 09 Aug 2022 20:43:19 GMT
ARG KONG_ARM64_SHA=3e5dde2479d53299e81dd903a04e30302108b0864c996a3662fda24ca7aee9f6
# Tue, 09 Aug 2022 20:43:37 GMT
# ARGS: KONG_AMD64_SHA=16990765aee26fc194992f0f90fc81e78a46d77cd0fc1e6670f3b2f797c1fe6b KONG_ARM64_SHA=3e5dde2479d53299e81dd903a04e30302108b0864c996a3662fda24ca7aee9f6
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Tue, 09 Aug 2022 20:43:38 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 09 Aug 2022 20:43:38 GMT
USER kong
# Tue, 09 Aug 2022 20:43:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:43:40 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 09 Aug 2022 20:43:41 GMT
STOPSIGNAL SIGQUIT
# Tue, 09 Aug 2022 20:43:42 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 09 Aug 2022 20:43:43 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf24c8e5476c8b7b4206bb7d73b6e374dd6f847c367e880a7e72e96aa1dfd355`  
		Last Modified: Tue, 09 Aug 2022 20:46:28 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c33ef81acec69a7618df2a3ff9095806decd55b4e1fe788bd6bd678ee4d8bb`  
		Last Modified: Tue, 09 Aug 2022 20:46:42 GMT  
		Size: 46.9 MB (46859292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f72441bb69318c800b3f9710d8aee21166344bb91a8a3274d9f3ab1b08db01f`  
		Last Modified: Tue, 09 Aug 2022 20:46:28 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.7.2-alpine`

```console
$ docker pull kong@sha256:c60af2f8633d4719bd6c8989de3a9e7c88cc500a17f1e371ec1f0dc51b6182bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.7.2-alpine` - linux; amd64

```console
$ docker pull kong@sha256:9c21d4bc5aae773be7872c2edd2e0d0fa365352984311e234d39e4a9708fb74c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50148848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dade8e963fd6f83ecc1ae7b3e50718539c7b263ff1fea242893d39800014e0d2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:50:59 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 09 Aug 2022 20:50:59 GMT
ARG ASSET=ce
# Tue, 09 Aug 2022 20:50:59 GMT
ENV ASSET=ce
# Tue, 09 Aug 2022 20:51:00 GMT
ARG EE_PORTS
# Tue, 09 Aug 2022 20:51:00 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 09 Aug 2022 20:51:00 GMT
ARG KONG_VERSION=2.7.2
# Tue, 09 Aug 2022 20:51:00 GMT
ENV KONG_VERSION=2.7.2
# Tue, 09 Aug 2022 20:51:00 GMT
ARG KONG_AMD64_SHA=16990765aee26fc194992f0f90fc81e78a46d77cd0fc1e6670f3b2f797c1fe6b
# Tue, 09 Aug 2022 20:51:00 GMT
ARG KONG_ARM64_SHA=3e5dde2479d53299e81dd903a04e30302108b0864c996a3662fda24ca7aee9f6
# Tue, 09 Aug 2022 20:51:07 GMT
# ARGS: KONG_AMD64_SHA=16990765aee26fc194992f0f90fc81e78a46d77cd0fc1e6670f3b2f797c1fe6b KONG_ARM64_SHA=3e5dde2479d53299e81dd903a04e30302108b0864c996a3662fda24ca7aee9f6
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Tue, 09 Aug 2022 20:51:08 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 09 Aug 2022 20:51:08 GMT
USER kong
# Tue, 09 Aug 2022 20:51:08 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:51:08 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 09 Aug 2022 20:51:08 GMT
STOPSIGNAL SIGQUIT
# Tue, 09 Aug 2022 20:51:08 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 09 Aug 2022 20:51:08 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb31d71e8b572b72e18738ce5a5ce873f6bdbd4dfe392710abfaa0b239f5e9e`  
		Last Modified: Tue, 09 Aug 2022 20:52:29 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bcaa0cf883df54fdb29ac9dbf919864e35c4557da6490c9fc6d6a0e58172aa8`  
		Last Modified: Tue, 09 Aug 2022 20:52:37 GMT  
		Size: 47.3 MB (47324324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb36999ccc7dbbae9dc7ae7adff69f22b48a3d2b6a56cab3458f90a1c2ef9f89`  
		Last Modified: Tue, 09 Aug 2022 20:52:29 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.7.2-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:39ba2815ffe5f5c822fb1a66c61abea4cc4ecc83eb3086cc04cbc9c82d23b040
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49578744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8860d91130909d7b20b4ca98a3d0402047cf8f45b60ffdd15418f8c258718f5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:43:11 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 09 Aug 2022 20:43:12 GMT
ARG ASSET=ce
# Tue, 09 Aug 2022 20:43:13 GMT
ENV ASSET=ce
# Tue, 09 Aug 2022 20:43:14 GMT
ARG EE_PORTS
# Tue, 09 Aug 2022 20:43:16 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 09 Aug 2022 20:43:16 GMT
ARG KONG_VERSION=2.7.2
# Tue, 09 Aug 2022 20:43:17 GMT
ENV KONG_VERSION=2.7.2
# Tue, 09 Aug 2022 20:43:18 GMT
ARG KONG_AMD64_SHA=16990765aee26fc194992f0f90fc81e78a46d77cd0fc1e6670f3b2f797c1fe6b
# Tue, 09 Aug 2022 20:43:19 GMT
ARG KONG_ARM64_SHA=3e5dde2479d53299e81dd903a04e30302108b0864c996a3662fda24ca7aee9f6
# Tue, 09 Aug 2022 20:43:37 GMT
# ARGS: KONG_AMD64_SHA=16990765aee26fc194992f0f90fc81e78a46d77cd0fc1e6670f3b2f797c1fe6b KONG_ARM64_SHA=3e5dde2479d53299e81dd903a04e30302108b0864c996a3662fda24ca7aee9f6
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Tue, 09 Aug 2022 20:43:38 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 09 Aug 2022 20:43:38 GMT
USER kong
# Tue, 09 Aug 2022 20:43:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:43:40 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 09 Aug 2022 20:43:41 GMT
STOPSIGNAL SIGQUIT
# Tue, 09 Aug 2022 20:43:42 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 09 Aug 2022 20:43:43 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf24c8e5476c8b7b4206bb7d73b6e374dd6f847c367e880a7e72e96aa1dfd355`  
		Last Modified: Tue, 09 Aug 2022 20:46:28 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c33ef81acec69a7618df2a3ff9095806decd55b4e1fe788bd6bd678ee4d8bb`  
		Last Modified: Tue, 09 Aug 2022 20:46:42 GMT  
		Size: 46.9 MB (46859292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f72441bb69318c800b3f9710d8aee21166344bb91a8a3274d9f3ab1b08db01f`  
		Last Modified: Tue, 09 Aug 2022 20:46:28 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.7.2-ubuntu`

```console
$ docker pull kong@sha256:5d98d90b3037ce816979b9d5397d1395a6f41d2e7b6875aa2b4e60113941ff65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.7.2-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:b7761ac4593efe882d1a45d1a56e965957c874c72f4f464bb54be0b917afa3cd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.1 MB (128088407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:652ae2e6d172008f0b7ee7a6e4da0d57749a376d8101b0b73cf9719e0793d955`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:37:42 GMT
ARG ASSET=ce
# Fri, 02 Sep 2022 03:37:42 GMT
ENV ASSET=ce
# Fri, 02 Sep 2022 03:37:42 GMT
ARG EE_PORTS
# Fri, 02 Sep 2022 03:37:42 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Fri, 02 Sep 2022 03:38:12 GMT
ARG KONG_VERSION=2.7.2
# Fri, 02 Sep 2022 03:38:13 GMT
ENV KONG_VERSION=2.7.2
# Fri, 02 Sep 2022 03:38:13 GMT
ARG KONG_AMD64_SHA=8124ddbfe80a1627b19a54e14b20ff0e176549699491cf5c61a4f0355470f8fc
# Fri, 02 Sep 2022 03:38:13 GMT
ARG KONG_ARM64_SHA=f40e616539ab64cb4fd333d19895ec9768b742bc25e5f2dbcb7f162bf90421d8
# Fri, 02 Sep 2022 03:38:33 GMT
# ARGS: KONG_AMD64_SHA=8124ddbfe80a1627b19a54e14b20ff0e176549699491cf5c61a4f0355470f8fc KONG_ARM64_SHA=f40e616539ab64cb4fd333d19895ec9768b742bc25e5f2dbcb7f162bf90421d8
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 02 Sep 2022 03:38:34 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 02 Sep 2022 03:38:34 GMT
USER kong
# Fri, 02 Sep 2022 03:38:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 03:38:34 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 02 Sep 2022 03:38:34 GMT
STOPSIGNAL SIGQUIT
# Fri, 02 Sep 2022 03:38:34 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 02 Sep 2022 03:38:34 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c91420ce43ec4f22f2debc82905e36cd7e0b308aad6701592278451f47d0e47`  
		Last Modified: Fri, 02 Sep 2022 03:40:04 GMT  
		Size: 25.1 MB (25081963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715a9c69d1c8646312e7aad5c278ebfc2735949c11c3d95f2882e4e375339bb2`  
		Last Modified: Fri, 02 Sep 2022 03:40:38 GMT  
		Size: 74.4 MB (74432878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244eabcc9d362a5616a52dc4dfbf0b6de8598cb0ddd7e2eca6f3f47ad2d6b374`  
		Last Modified: Fri, 02 Sep 2022 03:40:26 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.7.2-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:bec46695261737d5fa1cc18d747b1113fbc97ecc7b67fc5bf1977df405eebe4c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.1 MB (125139673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ddc4984898199e1d8ea33ec26db00909306fd3050b2753dcb895688c620645b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:45:21 GMT
ARG ASSET=ce
# Fri, 02 Sep 2022 06:45:21 GMT
ENV ASSET=ce
# Fri, 02 Sep 2022 06:45:22 GMT
ARG EE_PORTS
# Fri, 02 Sep 2022 06:45:24 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Fri, 02 Sep 2022 06:46:16 GMT
ARG KONG_VERSION=2.7.2
# Fri, 02 Sep 2022 06:46:17 GMT
ENV KONG_VERSION=2.7.2
# Fri, 02 Sep 2022 06:46:18 GMT
ARG KONG_AMD64_SHA=8124ddbfe80a1627b19a54e14b20ff0e176549699491cf5c61a4f0355470f8fc
# Fri, 02 Sep 2022 06:46:19 GMT
ARG KONG_ARM64_SHA=f40e616539ab64cb4fd333d19895ec9768b742bc25e5f2dbcb7f162bf90421d8
# Fri, 02 Sep 2022 06:46:59 GMT
# ARGS: KONG_AMD64_SHA=8124ddbfe80a1627b19a54e14b20ff0e176549699491cf5c61a4f0355470f8fc KONG_ARM64_SHA=f40e616539ab64cb4fd333d19895ec9768b742bc25e5f2dbcb7f162bf90421d8
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 02 Sep 2022 06:47:00 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 02 Sep 2022 06:47:00 GMT
USER kong
# Fri, 02 Sep 2022 06:47:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 06:47:02 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 02 Sep 2022 06:47:03 GMT
STOPSIGNAL SIGQUIT
# Fri, 02 Sep 2022 06:47:04 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 02 Sep 2022 06:47:05 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37921fee9fdc77f083b1d7e6150fcc91eaf74164601930750627e75ec46159c9`  
		Last Modified: Fri, 02 Sep 2022 06:50:16 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e533f40a36a4076913850a50f0c4b06bedeaf27953e9ff68eb0409147ff9b8b8`  
		Last Modified: Fri, 02 Sep 2022 06:50:53 GMT  
		Size: 72.9 MB (72865021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8895e832ae3976fab3fdf671159d4f380325a31968556cad1ff49144e418909`  
		Last Modified: Fri, 02 Sep 2022 06:50:41 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.8`

```console
$ docker pull kong@sha256:4dc4da99f8da9e4d7ab01da7feb3062ba12be1324fa8359f2396bbb7ac07bb3e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.8` - linux; amd64

```console
$ docker pull kong@sha256:7853bcf8b77f2d47fbda34b9ccba8d108c8145622905f5f66c2bc124435d4c88
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49349895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf394ffed022e33afd4c01e0f69d77671361bb35c0e0d391a7bf102860dafbfd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:50:46 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 09 Aug 2022 20:50:46 GMT
ARG ASSET=ce
# Tue, 09 Aug 2022 20:50:46 GMT
ENV ASSET=ce
# Tue, 09 Aug 2022 20:50:46 GMT
ARG EE_PORTS
# Tue, 09 Aug 2022 20:50:46 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 09 Aug 2022 20:50:46 GMT
ARG KONG_VERSION=2.8.1
# Tue, 09 Aug 2022 20:50:46 GMT
ENV KONG_VERSION=2.8.1
# Tue, 09 Aug 2022 20:50:46 GMT
ARG KONG_AMD64_SHA=ccda33bf02803b6b8dd46b22990f92265fe61d900ba94e3e0fa26db0433098c0
# Tue, 09 Aug 2022 20:50:46 GMT
ARG KONG_ARM64_SHA=d21690332a89adf9900f7266e083f41f565eb009f2771ef112f3564878eeff53
# Tue, 09 Aug 2022 20:50:53 GMT
# ARGS: KONG_AMD64_SHA=ccda33bf02803b6b8dd46b22990f92265fe61d900ba94e3e0fa26db0433098c0 KONG_ARM64_SHA=d21690332a89adf9900f7266e083f41f565eb009f2771ef112f3564878eeff53
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Tue, 09 Aug 2022 20:50:54 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 09 Aug 2022 20:50:54 GMT
USER kong
# Tue, 09 Aug 2022 20:50:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:50:54 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 09 Aug 2022 20:50:54 GMT
STOPSIGNAL SIGQUIT
# Tue, 09 Aug 2022 20:50:54 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 09 Aug 2022 20:50:55 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df79bc1e6d9219ba18210a0d465d9d48e3dd749d1fea9c0a50f0e8bb7c57453b`  
		Last Modified: Tue, 09 Aug 2022 20:52:03 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17afdc22f8ede5802cf3c22afe83fdce0451a7282f0d466737dd68f897abb103`  
		Last Modified: Tue, 09 Aug 2022 20:52:11 GMT  
		Size: 46.5 MB (46542829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4782db41dff7a89a4b61290bdcdef60323b2f97dac63b587f51b5f8990443ed8`  
		Last Modified: Tue, 09 Aug 2022 20:52:04 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.8` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:2e4a51fba3b574ee35f990aef3bfd1120ad2e2704f3bc618697382a9f13eaa5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.5 MB (48542736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef17c5908a084b9879dac56870037eccf0c01f792d09fde4b1509019edcc6834`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:42:36 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 09 Aug 2022 20:42:37 GMT
ARG ASSET=ce
# Tue, 09 Aug 2022 20:42:38 GMT
ENV ASSET=ce
# Tue, 09 Aug 2022 20:42:39 GMT
ARG EE_PORTS
# Tue, 09 Aug 2022 20:42:41 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 09 Aug 2022 20:42:41 GMT
ARG KONG_VERSION=2.8.1
# Tue, 09 Aug 2022 20:42:42 GMT
ENV KONG_VERSION=2.8.1
# Tue, 09 Aug 2022 20:42:43 GMT
ARG KONG_AMD64_SHA=ccda33bf02803b6b8dd46b22990f92265fe61d900ba94e3e0fa26db0433098c0
# Tue, 09 Aug 2022 20:42:44 GMT
ARG KONG_ARM64_SHA=d21690332a89adf9900f7266e083f41f565eb009f2771ef112f3564878eeff53
# Tue, 09 Aug 2022 20:42:53 GMT
# ARGS: KONG_AMD64_SHA=ccda33bf02803b6b8dd46b22990f92265fe61d900ba94e3e0fa26db0433098c0 KONG_ARM64_SHA=d21690332a89adf9900f7266e083f41f565eb009f2771ef112f3564878eeff53
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Tue, 09 Aug 2022 20:42:54 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 09 Aug 2022 20:42:54 GMT
USER kong
# Tue, 09 Aug 2022 20:42:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:42:56 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 09 Aug 2022 20:42:57 GMT
STOPSIGNAL SIGQUIT
# Tue, 09 Aug 2022 20:42:58 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 09 Aug 2022 20:42:59 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70974eef12350195e179ac6f7e3f7ece7a292a31c6a4f5e19006b7df7f02df11`  
		Last Modified: Tue, 09 Aug 2022 20:45:58 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8314b864c236792b78293d546cc56ce12740413e395c5cc628457e893f46c905`  
		Last Modified: Tue, 09 Aug 2022 20:46:06 GMT  
		Size: 45.8 MB (45834060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:422419cd811d0936d352e9b792f92bcf50bdc9af873da1eb9c5f91f48f0570ca`  
		Last Modified: Tue, 09 Aug 2022 20:45:58 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.8-ubuntu`

```console
$ docker pull kong@sha256:bf2dd2e92884a6714ffba920fd29ecaa8e4d2c353875282f5eb76df8c6215718
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.8-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:28eac960750f841fe427a5c4b71db772c479fbf663a6f05b430b1a45f0126dec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.2 MB (121210597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9455e296e925930165de8f07fd363f81f0301727329c2fc27818690384028f02`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:37:42 GMT
ARG ASSET=ce
# Fri, 02 Sep 2022 03:37:42 GMT
ENV ASSET=ce
# Fri, 02 Sep 2022 03:37:42 GMT
ARG EE_PORTS
# Fri, 02 Sep 2022 03:37:42 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Fri, 02 Sep 2022 03:37:42 GMT
ARG KONG_VERSION=2.8.1
# Fri, 02 Sep 2022 03:37:43 GMT
ENV KONG_VERSION=2.8.1
# Fri, 02 Sep 2022 03:37:43 GMT
ARG KONG_AMD64_SHA=10d12d23e5890414d666663094d51a42de41f8a9806fbc0baaf9ac4d37794361
# Fri, 02 Sep 2022 03:37:43 GMT
ARG KONG_ARM64_SHA=61c13219ef64dac9aeae5ae775411e8cfcd406f068cf3e75d463f916ae6513cb
# Fri, 02 Sep 2022 03:38:07 GMT
# ARGS: KONG_AMD64_SHA=10d12d23e5890414d666663094d51a42de41f8a9806fbc0baaf9ac4d37794361 KONG_ARM64_SHA=61c13219ef64dac9aeae5ae775411e8cfcd406f068cf3e75d463f916ae6513cb
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 02 Sep 2022 03:38:07 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 02 Sep 2022 03:38:07 GMT
USER kong
# Fri, 02 Sep 2022 03:38:08 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 03:38:08 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 02 Sep 2022 03:38:08 GMT
STOPSIGNAL SIGQUIT
# Fri, 02 Sep 2022 03:38:08 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 02 Sep 2022 03:38:08 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c91420ce43ec4f22f2debc82905e36cd7e0b308aad6701592278451f47d0e47`  
		Last Modified: Fri, 02 Sep 2022 03:40:04 GMT  
		Size: 25.1 MB (25081963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e512fe8bc0f00439f0b2a0d3f20a21012a2cabfa60e944c25928a3915e41b6`  
		Last Modified: Fri, 02 Sep 2022 03:40:13 GMT  
		Size: 67.6 MB (67555068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24068604cb591cd030a713d77045f6895fd1d4ff69bcac94cf115cf6d36a32ab`  
		Last Modified: Fri, 02 Sep 2022 03:40:02 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.8-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:7b2bf1303f661c575da457a9046b9620590b17bed4890b88bac7e818277a17a2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.7 MB (121715925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8824d66ce1a3f044fb009a0dd979f97b8dbf80491e6fa2a55c138baab821271e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:45:21 GMT
ARG ASSET=ce
# Fri, 02 Sep 2022 06:45:21 GMT
ENV ASSET=ce
# Fri, 02 Sep 2022 06:45:22 GMT
ARG EE_PORTS
# Fri, 02 Sep 2022 06:45:24 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Fri, 02 Sep 2022 06:45:24 GMT
ARG KONG_VERSION=2.8.1
# Fri, 02 Sep 2022 06:45:25 GMT
ENV KONG_VERSION=2.8.1
# Fri, 02 Sep 2022 06:45:26 GMT
ARG KONG_AMD64_SHA=10d12d23e5890414d666663094d51a42de41f8a9806fbc0baaf9ac4d37794361
# Fri, 02 Sep 2022 06:45:27 GMT
ARG KONG_ARM64_SHA=61c13219ef64dac9aeae5ae775411e8cfcd406f068cf3e75d463f916ae6513cb
# Fri, 02 Sep 2022 06:45:56 GMT
# ARGS: KONG_AMD64_SHA=10d12d23e5890414d666663094d51a42de41f8a9806fbc0baaf9ac4d37794361 KONG_ARM64_SHA=61c13219ef64dac9aeae5ae775411e8cfcd406f068cf3e75d463f916ae6513cb
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 02 Sep 2022 06:45:57 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 02 Sep 2022 06:45:57 GMT
USER kong
# Fri, 02 Sep 2022 06:45:58 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 06:45:59 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 02 Sep 2022 06:46:00 GMT
STOPSIGNAL SIGQUIT
# Fri, 02 Sep 2022 06:46:01 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 02 Sep 2022 06:46:02 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37921fee9fdc77f083b1d7e6150fcc91eaf74164601930750627e75ec46159c9`  
		Last Modified: Fri, 02 Sep 2022 06:50:16 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b2eb7f3cec9c8ba77ac0b9ea6c162a9999e3a4375f390e6e44c94e701bca00a`  
		Last Modified: Fri, 02 Sep 2022 06:50:26 GMT  
		Size: 69.4 MB (69441275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd6508437ef72723b0df33a3e5356b79b4143a273c6e2b63819b32a60b10904`  
		Last Modified: Fri, 02 Sep 2022 06:50:14 GMT  
		Size: 879.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.8.1`

```console
$ docker pull kong@sha256:4dc4da99f8da9e4d7ab01da7feb3062ba12be1324fa8359f2396bbb7ac07bb3e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.8.1` - linux; amd64

```console
$ docker pull kong@sha256:7853bcf8b77f2d47fbda34b9ccba8d108c8145622905f5f66c2bc124435d4c88
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49349895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf394ffed022e33afd4c01e0f69d77671361bb35c0e0d391a7bf102860dafbfd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:50:46 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 09 Aug 2022 20:50:46 GMT
ARG ASSET=ce
# Tue, 09 Aug 2022 20:50:46 GMT
ENV ASSET=ce
# Tue, 09 Aug 2022 20:50:46 GMT
ARG EE_PORTS
# Tue, 09 Aug 2022 20:50:46 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 09 Aug 2022 20:50:46 GMT
ARG KONG_VERSION=2.8.1
# Tue, 09 Aug 2022 20:50:46 GMT
ENV KONG_VERSION=2.8.1
# Tue, 09 Aug 2022 20:50:46 GMT
ARG KONG_AMD64_SHA=ccda33bf02803b6b8dd46b22990f92265fe61d900ba94e3e0fa26db0433098c0
# Tue, 09 Aug 2022 20:50:46 GMT
ARG KONG_ARM64_SHA=d21690332a89adf9900f7266e083f41f565eb009f2771ef112f3564878eeff53
# Tue, 09 Aug 2022 20:50:53 GMT
# ARGS: KONG_AMD64_SHA=ccda33bf02803b6b8dd46b22990f92265fe61d900ba94e3e0fa26db0433098c0 KONG_ARM64_SHA=d21690332a89adf9900f7266e083f41f565eb009f2771ef112f3564878eeff53
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Tue, 09 Aug 2022 20:50:54 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 09 Aug 2022 20:50:54 GMT
USER kong
# Tue, 09 Aug 2022 20:50:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:50:54 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 09 Aug 2022 20:50:54 GMT
STOPSIGNAL SIGQUIT
# Tue, 09 Aug 2022 20:50:54 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 09 Aug 2022 20:50:55 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df79bc1e6d9219ba18210a0d465d9d48e3dd749d1fea9c0a50f0e8bb7c57453b`  
		Last Modified: Tue, 09 Aug 2022 20:52:03 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17afdc22f8ede5802cf3c22afe83fdce0451a7282f0d466737dd68f897abb103`  
		Last Modified: Tue, 09 Aug 2022 20:52:11 GMT  
		Size: 46.5 MB (46542829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4782db41dff7a89a4b61290bdcdef60323b2f97dac63b587f51b5f8990443ed8`  
		Last Modified: Tue, 09 Aug 2022 20:52:04 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.8.1` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:2e4a51fba3b574ee35f990aef3bfd1120ad2e2704f3bc618697382a9f13eaa5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.5 MB (48542736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef17c5908a084b9879dac56870037eccf0c01f792d09fde4b1509019edcc6834`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:42:36 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 09 Aug 2022 20:42:37 GMT
ARG ASSET=ce
# Tue, 09 Aug 2022 20:42:38 GMT
ENV ASSET=ce
# Tue, 09 Aug 2022 20:42:39 GMT
ARG EE_PORTS
# Tue, 09 Aug 2022 20:42:41 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 09 Aug 2022 20:42:41 GMT
ARG KONG_VERSION=2.8.1
# Tue, 09 Aug 2022 20:42:42 GMT
ENV KONG_VERSION=2.8.1
# Tue, 09 Aug 2022 20:42:43 GMT
ARG KONG_AMD64_SHA=ccda33bf02803b6b8dd46b22990f92265fe61d900ba94e3e0fa26db0433098c0
# Tue, 09 Aug 2022 20:42:44 GMT
ARG KONG_ARM64_SHA=d21690332a89adf9900f7266e083f41f565eb009f2771ef112f3564878eeff53
# Tue, 09 Aug 2022 20:42:53 GMT
# ARGS: KONG_AMD64_SHA=ccda33bf02803b6b8dd46b22990f92265fe61d900ba94e3e0fa26db0433098c0 KONG_ARM64_SHA=d21690332a89adf9900f7266e083f41f565eb009f2771ef112f3564878eeff53
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Tue, 09 Aug 2022 20:42:54 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 09 Aug 2022 20:42:54 GMT
USER kong
# Tue, 09 Aug 2022 20:42:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:42:56 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 09 Aug 2022 20:42:57 GMT
STOPSIGNAL SIGQUIT
# Tue, 09 Aug 2022 20:42:58 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 09 Aug 2022 20:42:59 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70974eef12350195e179ac6f7e3f7ece7a292a31c6a4f5e19006b7df7f02df11`  
		Last Modified: Tue, 09 Aug 2022 20:45:58 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8314b864c236792b78293d546cc56ce12740413e395c5cc628457e893f46c905`  
		Last Modified: Tue, 09 Aug 2022 20:46:06 GMT  
		Size: 45.8 MB (45834060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:422419cd811d0936d352e9b792f92bcf50bdc9af873da1eb9c5f91f48f0570ca`  
		Last Modified: Tue, 09 Aug 2022 20:45:58 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.8.1-alpine`

```console
$ docker pull kong@sha256:4dc4da99f8da9e4d7ab01da7feb3062ba12be1324fa8359f2396bbb7ac07bb3e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.8.1-alpine` - linux; amd64

```console
$ docker pull kong@sha256:7853bcf8b77f2d47fbda34b9ccba8d108c8145622905f5f66c2bc124435d4c88
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49349895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf394ffed022e33afd4c01e0f69d77671361bb35c0e0d391a7bf102860dafbfd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:50:46 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 09 Aug 2022 20:50:46 GMT
ARG ASSET=ce
# Tue, 09 Aug 2022 20:50:46 GMT
ENV ASSET=ce
# Tue, 09 Aug 2022 20:50:46 GMT
ARG EE_PORTS
# Tue, 09 Aug 2022 20:50:46 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 09 Aug 2022 20:50:46 GMT
ARG KONG_VERSION=2.8.1
# Tue, 09 Aug 2022 20:50:46 GMT
ENV KONG_VERSION=2.8.1
# Tue, 09 Aug 2022 20:50:46 GMT
ARG KONG_AMD64_SHA=ccda33bf02803b6b8dd46b22990f92265fe61d900ba94e3e0fa26db0433098c0
# Tue, 09 Aug 2022 20:50:46 GMT
ARG KONG_ARM64_SHA=d21690332a89adf9900f7266e083f41f565eb009f2771ef112f3564878eeff53
# Tue, 09 Aug 2022 20:50:53 GMT
# ARGS: KONG_AMD64_SHA=ccda33bf02803b6b8dd46b22990f92265fe61d900ba94e3e0fa26db0433098c0 KONG_ARM64_SHA=d21690332a89adf9900f7266e083f41f565eb009f2771ef112f3564878eeff53
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Tue, 09 Aug 2022 20:50:54 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 09 Aug 2022 20:50:54 GMT
USER kong
# Tue, 09 Aug 2022 20:50:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:50:54 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 09 Aug 2022 20:50:54 GMT
STOPSIGNAL SIGQUIT
# Tue, 09 Aug 2022 20:50:54 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 09 Aug 2022 20:50:55 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df79bc1e6d9219ba18210a0d465d9d48e3dd749d1fea9c0a50f0e8bb7c57453b`  
		Last Modified: Tue, 09 Aug 2022 20:52:03 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17afdc22f8ede5802cf3c22afe83fdce0451a7282f0d466737dd68f897abb103`  
		Last Modified: Tue, 09 Aug 2022 20:52:11 GMT  
		Size: 46.5 MB (46542829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4782db41dff7a89a4b61290bdcdef60323b2f97dac63b587f51b5f8990443ed8`  
		Last Modified: Tue, 09 Aug 2022 20:52:04 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.8.1-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:2e4a51fba3b574ee35f990aef3bfd1120ad2e2704f3bc618697382a9f13eaa5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.5 MB (48542736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef17c5908a084b9879dac56870037eccf0c01f792d09fde4b1509019edcc6834`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:42:36 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 09 Aug 2022 20:42:37 GMT
ARG ASSET=ce
# Tue, 09 Aug 2022 20:42:38 GMT
ENV ASSET=ce
# Tue, 09 Aug 2022 20:42:39 GMT
ARG EE_PORTS
# Tue, 09 Aug 2022 20:42:41 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 09 Aug 2022 20:42:41 GMT
ARG KONG_VERSION=2.8.1
# Tue, 09 Aug 2022 20:42:42 GMT
ENV KONG_VERSION=2.8.1
# Tue, 09 Aug 2022 20:42:43 GMT
ARG KONG_AMD64_SHA=ccda33bf02803b6b8dd46b22990f92265fe61d900ba94e3e0fa26db0433098c0
# Tue, 09 Aug 2022 20:42:44 GMT
ARG KONG_ARM64_SHA=d21690332a89adf9900f7266e083f41f565eb009f2771ef112f3564878eeff53
# Tue, 09 Aug 2022 20:42:53 GMT
# ARGS: KONG_AMD64_SHA=ccda33bf02803b6b8dd46b22990f92265fe61d900ba94e3e0fa26db0433098c0 KONG_ARM64_SHA=d21690332a89adf9900f7266e083f41f565eb009f2771ef112f3564878eeff53
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Tue, 09 Aug 2022 20:42:54 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 09 Aug 2022 20:42:54 GMT
USER kong
# Tue, 09 Aug 2022 20:42:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:42:56 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 09 Aug 2022 20:42:57 GMT
STOPSIGNAL SIGQUIT
# Tue, 09 Aug 2022 20:42:58 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 09 Aug 2022 20:42:59 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70974eef12350195e179ac6f7e3f7ece7a292a31c6a4f5e19006b7df7f02df11`  
		Last Modified: Tue, 09 Aug 2022 20:45:58 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8314b864c236792b78293d546cc56ce12740413e395c5cc628457e893f46c905`  
		Last Modified: Tue, 09 Aug 2022 20:46:06 GMT  
		Size: 45.8 MB (45834060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:422419cd811d0936d352e9b792f92bcf50bdc9af873da1eb9c5f91f48f0570ca`  
		Last Modified: Tue, 09 Aug 2022 20:45:58 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.8.1-ubuntu`

```console
$ docker pull kong@sha256:bf2dd2e92884a6714ffba920fd29ecaa8e4d2c353875282f5eb76df8c6215718
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.8.1-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:28eac960750f841fe427a5c4b71db772c479fbf663a6f05b430b1a45f0126dec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.2 MB (121210597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9455e296e925930165de8f07fd363f81f0301727329c2fc27818690384028f02`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:37:42 GMT
ARG ASSET=ce
# Fri, 02 Sep 2022 03:37:42 GMT
ENV ASSET=ce
# Fri, 02 Sep 2022 03:37:42 GMT
ARG EE_PORTS
# Fri, 02 Sep 2022 03:37:42 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Fri, 02 Sep 2022 03:37:42 GMT
ARG KONG_VERSION=2.8.1
# Fri, 02 Sep 2022 03:37:43 GMT
ENV KONG_VERSION=2.8.1
# Fri, 02 Sep 2022 03:37:43 GMT
ARG KONG_AMD64_SHA=10d12d23e5890414d666663094d51a42de41f8a9806fbc0baaf9ac4d37794361
# Fri, 02 Sep 2022 03:37:43 GMT
ARG KONG_ARM64_SHA=61c13219ef64dac9aeae5ae775411e8cfcd406f068cf3e75d463f916ae6513cb
# Fri, 02 Sep 2022 03:38:07 GMT
# ARGS: KONG_AMD64_SHA=10d12d23e5890414d666663094d51a42de41f8a9806fbc0baaf9ac4d37794361 KONG_ARM64_SHA=61c13219ef64dac9aeae5ae775411e8cfcd406f068cf3e75d463f916ae6513cb
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 02 Sep 2022 03:38:07 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 02 Sep 2022 03:38:07 GMT
USER kong
# Fri, 02 Sep 2022 03:38:08 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 03:38:08 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 02 Sep 2022 03:38:08 GMT
STOPSIGNAL SIGQUIT
# Fri, 02 Sep 2022 03:38:08 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 02 Sep 2022 03:38:08 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c91420ce43ec4f22f2debc82905e36cd7e0b308aad6701592278451f47d0e47`  
		Last Modified: Fri, 02 Sep 2022 03:40:04 GMT  
		Size: 25.1 MB (25081963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e512fe8bc0f00439f0b2a0d3f20a21012a2cabfa60e944c25928a3915e41b6`  
		Last Modified: Fri, 02 Sep 2022 03:40:13 GMT  
		Size: 67.6 MB (67555068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24068604cb591cd030a713d77045f6895fd1d4ff69bcac94cf115cf6d36a32ab`  
		Last Modified: Fri, 02 Sep 2022 03:40:02 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.8.1-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:7b2bf1303f661c575da457a9046b9620590b17bed4890b88bac7e818277a17a2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.7 MB (121715925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8824d66ce1a3f044fb009a0dd979f97b8dbf80491e6fa2a55c138baab821271e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:45:21 GMT
ARG ASSET=ce
# Fri, 02 Sep 2022 06:45:21 GMT
ENV ASSET=ce
# Fri, 02 Sep 2022 06:45:22 GMT
ARG EE_PORTS
# Fri, 02 Sep 2022 06:45:24 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Fri, 02 Sep 2022 06:45:24 GMT
ARG KONG_VERSION=2.8.1
# Fri, 02 Sep 2022 06:45:25 GMT
ENV KONG_VERSION=2.8.1
# Fri, 02 Sep 2022 06:45:26 GMT
ARG KONG_AMD64_SHA=10d12d23e5890414d666663094d51a42de41f8a9806fbc0baaf9ac4d37794361
# Fri, 02 Sep 2022 06:45:27 GMT
ARG KONG_ARM64_SHA=61c13219ef64dac9aeae5ae775411e8cfcd406f068cf3e75d463f916ae6513cb
# Fri, 02 Sep 2022 06:45:56 GMT
# ARGS: KONG_AMD64_SHA=10d12d23e5890414d666663094d51a42de41f8a9806fbc0baaf9ac4d37794361 KONG_ARM64_SHA=61c13219ef64dac9aeae5ae775411e8cfcd406f068cf3e75d463f916ae6513cb
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 02 Sep 2022 06:45:57 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 02 Sep 2022 06:45:57 GMT
USER kong
# Fri, 02 Sep 2022 06:45:58 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 06:45:59 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 02 Sep 2022 06:46:00 GMT
STOPSIGNAL SIGQUIT
# Fri, 02 Sep 2022 06:46:01 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 02 Sep 2022 06:46:02 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37921fee9fdc77f083b1d7e6150fcc91eaf74164601930750627e75ec46159c9`  
		Last Modified: Fri, 02 Sep 2022 06:50:16 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b2eb7f3cec9c8ba77ac0b9ea6c162a9999e3a4375f390e6e44c94e701bca00a`  
		Last Modified: Fri, 02 Sep 2022 06:50:26 GMT  
		Size: 69.4 MB (69441275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd6508437ef72723b0df33a3e5356b79b4143a273c6e2b63819b32a60b10904`  
		Last Modified: Fri, 02 Sep 2022 06:50:14 GMT  
		Size: 879.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.0`

```console
$ docker pull kong@sha256:f051f4c130659d8dadefd047cf0e6d263fef9afb6c2ab65b282b10a00bbf7d68
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:3.0` - linux; amd64

```console
$ docker pull kong@sha256:8a54bbf5026200150c46a182e0d56d74ba7572d6cfe98e863fb20cdafce1d95e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51522357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5bce760c29ce855d5935d777f2ec45b3a9ca895a09334825360cebd26a222e6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 14 Sep 2022 00:07:19 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 14 Sep 2022 00:07:19 GMT
ARG ASSET=ce
# Wed, 14 Sep 2022 00:07:19 GMT
ENV ASSET=ce
# Wed, 14 Sep 2022 00:07:19 GMT
ARG EE_PORTS
# Wed, 14 Sep 2022 00:07:19 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 14 Sep 2022 00:07:19 GMT
ARG KONG_VERSION=3.0.0
# Wed, 14 Sep 2022 00:07:19 GMT
ENV KONG_VERSION=3.0.0
# Wed, 14 Sep 2022 00:07:20 GMT
ARG KONG_AMD64_SHA=b8e21beb32f803fae0959694ce7b6cec796a4159757e61b9cc0d30bed9682d10
# Wed, 14 Sep 2022 00:07:20 GMT
ARG KONG_ARM64_SHA=4c5407c5ef2f0f29468e15ea4dc6a3f27011dbde3ce18170e4a4fd7e2bb2c03b
# Wed, 14 Sep 2022 00:07:28 GMT
# ARGS: KONG_AMD64_SHA=b8e21beb32f803fae0959694ce7b6cec796a4159757e61b9cc0d30bed9682d10 KONG_ARM64_SHA=4c5407c5ef2f0f29468e15ea4dc6a3f27011dbde3ce18170e4a4fd7e2bb2c03b
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Wed, 14 Sep 2022 00:07:28 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 14 Sep 2022 00:07:28 GMT
USER kong
# Wed, 14 Sep 2022 00:07:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Sep 2022 00:07:29 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 14 Sep 2022 00:07:29 GMT
STOPSIGNAL SIGQUIT
# Wed, 14 Sep 2022 00:07:29 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 14 Sep 2022 00:07:29 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df4f8c583856d7a692eae94f47792d4cc4a214e2b9d36d1b6dd5eaded569804f`  
		Last Modified: Wed, 14 Sep 2022 00:09:25 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd3d1d803c378e5eb206c29367530e2f8a92578534afdf16cd4ff0da3e687f5`  
		Last Modified: Wed, 14 Sep 2022 00:09:33 GMT  
		Size: 48.7 MB (48715295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7a99de7f80d542680872b47fc5405bf068af5fa56916f994a15149ce05e441`  
		Last Modified: Wed, 14 Sep 2022 00:09:25 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.0-ubuntu`

```console
$ docker pull kong@sha256:03e3927b04eb875e37c3eb1632bbfd4ebbff1b34087cdab4583a1a3e35a16b36
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:3.0-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:e1b7a02b9e7a135b191170fde9406935383d015b7219c3a198a068430a68a29d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.7 MB (126666532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba3d56c232a3c9280f7ca9ed88c42b20112ba4997ef20356f1dc00c442f7d012`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Wed, 14 Sep 2022 00:07:33 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 14 Sep 2022 00:07:33 GMT
ARG ASSET=ce
# Wed, 14 Sep 2022 00:07:33 GMT
ENV ASSET=ce
# Wed, 14 Sep 2022 00:07:33 GMT
ARG EE_PORTS
# Wed, 14 Sep 2022 00:07:33 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 14 Sep 2022 00:07:34 GMT
ARG KONG_VERSION=3.0.0
# Wed, 14 Sep 2022 00:07:34 GMT
ENV KONG_VERSION=3.0.0
# Wed, 14 Sep 2022 00:07:34 GMT
ARG KONG_AMD64_SHA=3a38f6c4ba1cfc8897e655e46b957c7b0f2dd930111bf3d02411fedd1de53d6d
# Wed, 14 Sep 2022 00:07:34 GMT
ARG KONG_ARM64_SHA=190f82dd47df19339c025f37701e62191aa3063e77e15c5e57d5b77869058f69
# Wed, 14 Sep 2022 00:08:34 GMT
# ARGS: KONG_AMD64_SHA=3a38f6c4ba1cfc8897e655e46b957c7b0f2dd930111bf3d02411fedd1de53d6d KONG_ARM64_SHA=190f82dd47df19339c025f37701e62191aa3063e77e15c5e57d5b77869058f69
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 14 Sep 2022 00:08:35 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 14 Sep 2022 00:08:35 GMT
USER kong
# Wed, 14 Sep 2022 00:08:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Sep 2022 00:08:35 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 14 Sep 2022 00:08:35 GMT
STOPSIGNAL SIGQUIT
# Wed, 14 Sep 2022 00:08:35 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 14 Sep 2022 00:08:36 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f8ea18d6c5f278fa5820835cb24eea6a767e0f2db8069fa45a0a1a2e56c4b68`  
		Last Modified: Wed, 14 Sep 2022 00:09:51 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1fcce01ccb3758b7e74adaa6b4b0cb227b2ce8c0dde5c431af462be4e1fe93`  
		Last Modified: Wed, 14 Sep 2022 00:10:02 GMT  
		Size: 73.0 MB (73011012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a8c5f807f396934e8a026572c5fdc4c0ef99588049369adfdaac08e05f1d34`  
		Last Modified: Wed, 14 Sep 2022 00:09:50 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.0.0`

```console
$ docker pull kong@sha256:f051f4c130659d8dadefd047cf0e6d263fef9afb6c2ab65b282b10a00bbf7d68
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:3.0.0` - linux; amd64

```console
$ docker pull kong@sha256:8a54bbf5026200150c46a182e0d56d74ba7572d6cfe98e863fb20cdafce1d95e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51522357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5bce760c29ce855d5935d777f2ec45b3a9ca895a09334825360cebd26a222e6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 14 Sep 2022 00:07:19 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 14 Sep 2022 00:07:19 GMT
ARG ASSET=ce
# Wed, 14 Sep 2022 00:07:19 GMT
ENV ASSET=ce
# Wed, 14 Sep 2022 00:07:19 GMT
ARG EE_PORTS
# Wed, 14 Sep 2022 00:07:19 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 14 Sep 2022 00:07:19 GMT
ARG KONG_VERSION=3.0.0
# Wed, 14 Sep 2022 00:07:19 GMT
ENV KONG_VERSION=3.0.0
# Wed, 14 Sep 2022 00:07:20 GMT
ARG KONG_AMD64_SHA=b8e21beb32f803fae0959694ce7b6cec796a4159757e61b9cc0d30bed9682d10
# Wed, 14 Sep 2022 00:07:20 GMT
ARG KONG_ARM64_SHA=4c5407c5ef2f0f29468e15ea4dc6a3f27011dbde3ce18170e4a4fd7e2bb2c03b
# Wed, 14 Sep 2022 00:07:28 GMT
# ARGS: KONG_AMD64_SHA=b8e21beb32f803fae0959694ce7b6cec796a4159757e61b9cc0d30bed9682d10 KONG_ARM64_SHA=4c5407c5ef2f0f29468e15ea4dc6a3f27011dbde3ce18170e4a4fd7e2bb2c03b
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Wed, 14 Sep 2022 00:07:28 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 14 Sep 2022 00:07:28 GMT
USER kong
# Wed, 14 Sep 2022 00:07:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Sep 2022 00:07:29 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 14 Sep 2022 00:07:29 GMT
STOPSIGNAL SIGQUIT
# Wed, 14 Sep 2022 00:07:29 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 14 Sep 2022 00:07:29 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df4f8c583856d7a692eae94f47792d4cc4a214e2b9d36d1b6dd5eaded569804f`  
		Last Modified: Wed, 14 Sep 2022 00:09:25 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd3d1d803c378e5eb206c29367530e2f8a92578534afdf16cd4ff0da3e687f5`  
		Last Modified: Wed, 14 Sep 2022 00:09:33 GMT  
		Size: 48.7 MB (48715295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7a99de7f80d542680872b47fc5405bf068af5fa56916f994a15149ce05e441`  
		Last Modified: Wed, 14 Sep 2022 00:09:25 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.0.0-alpine`

```console
$ docker pull kong@sha256:f051f4c130659d8dadefd047cf0e6d263fef9afb6c2ab65b282b10a00bbf7d68
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:3.0.0-alpine` - linux; amd64

```console
$ docker pull kong@sha256:8a54bbf5026200150c46a182e0d56d74ba7572d6cfe98e863fb20cdafce1d95e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51522357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5bce760c29ce855d5935d777f2ec45b3a9ca895a09334825360cebd26a222e6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 14 Sep 2022 00:07:19 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 14 Sep 2022 00:07:19 GMT
ARG ASSET=ce
# Wed, 14 Sep 2022 00:07:19 GMT
ENV ASSET=ce
# Wed, 14 Sep 2022 00:07:19 GMT
ARG EE_PORTS
# Wed, 14 Sep 2022 00:07:19 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 14 Sep 2022 00:07:19 GMT
ARG KONG_VERSION=3.0.0
# Wed, 14 Sep 2022 00:07:19 GMT
ENV KONG_VERSION=3.0.0
# Wed, 14 Sep 2022 00:07:20 GMT
ARG KONG_AMD64_SHA=b8e21beb32f803fae0959694ce7b6cec796a4159757e61b9cc0d30bed9682d10
# Wed, 14 Sep 2022 00:07:20 GMT
ARG KONG_ARM64_SHA=4c5407c5ef2f0f29468e15ea4dc6a3f27011dbde3ce18170e4a4fd7e2bb2c03b
# Wed, 14 Sep 2022 00:07:28 GMT
# ARGS: KONG_AMD64_SHA=b8e21beb32f803fae0959694ce7b6cec796a4159757e61b9cc0d30bed9682d10 KONG_ARM64_SHA=4c5407c5ef2f0f29468e15ea4dc6a3f27011dbde3ce18170e4a4fd7e2bb2c03b
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Wed, 14 Sep 2022 00:07:28 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 14 Sep 2022 00:07:28 GMT
USER kong
# Wed, 14 Sep 2022 00:07:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Sep 2022 00:07:29 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 14 Sep 2022 00:07:29 GMT
STOPSIGNAL SIGQUIT
# Wed, 14 Sep 2022 00:07:29 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 14 Sep 2022 00:07:29 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df4f8c583856d7a692eae94f47792d4cc4a214e2b9d36d1b6dd5eaded569804f`  
		Last Modified: Wed, 14 Sep 2022 00:09:25 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd3d1d803c378e5eb206c29367530e2f8a92578534afdf16cd4ff0da3e687f5`  
		Last Modified: Wed, 14 Sep 2022 00:09:33 GMT  
		Size: 48.7 MB (48715295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7a99de7f80d542680872b47fc5405bf068af5fa56916f994a15149ce05e441`  
		Last Modified: Wed, 14 Sep 2022 00:09:25 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.0.0-ubuntu`

```console
$ docker pull kong@sha256:03e3927b04eb875e37c3eb1632bbfd4ebbff1b34087cdab4583a1a3e35a16b36
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:3.0.0-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:e1b7a02b9e7a135b191170fde9406935383d015b7219c3a198a068430a68a29d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.7 MB (126666532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba3d56c232a3c9280f7ca9ed88c42b20112ba4997ef20356f1dc00c442f7d012`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Wed, 14 Sep 2022 00:07:33 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 14 Sep 2022 00:07:33 GMT
ARG ASSET=ce
# Wed, 14 Sep 2022 00:07:33 GMT
ENV ASSET=ce
# Wed, 14 Sep 2022 00:07:33 GMT
ARG EE_PORTS
# Wed, 14 Sep 2022 00:07:33 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 14 Sep 2022 00:07:34 GMT
ARG KONG_VERSION=3.0.0
# Wed, 14 Sep 2022 00:07:34 GMT
ENV KONG_VERSION=3.0.0
# Wed, 14 Sep 2022 00:07:34 GMT
ARG KONG_AMD64_SHA=3a38f6c4ba1cfc8897e655e46b957c7b0f2dd930111bf3d02411fedd1de53d6d
# Wed, 14 Sep 2022 00:07:34 GMT
ARG KONG_ARM64_SHA=190f82dd47df19339c025f37701e62191aa3063e77e15c5e57d5b77869058f69
# Wed, 14 Sep 2022 00:08:34 GMT
# ARGS: KONG_AMD64_SHA=3a38f6c4ba1cfc8897e655e46b957c7b0f2dd930111bf3d02411fedd1de53d6d KONG_ARM64_SHA=190f82dd47df19339c025f37701e62191aa3063e77e15c5e57d5b77869058f69
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 14 Sep 2022 00:08:35 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 14 Sep 2022 00:08:35 GMT
USER kong
# Wed, 14 Sep 2022 00:08:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Sep 2022 00:08:35 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 14 Sep 2022 00:08:35 GMT
STOPSIGNAL SIGQUIT
# Wed, 14 Sep 2022 00:08:35 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 14 Sep 2022 00:08:36 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f8ea18d6c5f278fa5820835cb24eea6a767e0f2db8069fa45a0a1a2e56c4b68`  
		Last Modified: Wed, 14 Sep 2022 00:09:51 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1fcce01ccb3758b7e74adaa6b4b0cb227b2ce8c0dde5c431af462be4e1fe93`  
		Last Modified: Wed, 14 Sep 2022 00:10:02 GMT  
		Size: 73.0 MB (73011012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a8c5f807f396934e8a026572c5fdc4c0ef99588049369adfdaac08e05f1d34`  
		Last Modified: Wed, 14 Sep 2022 00:09:50 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:alpine`

```console
$ docker pull kong@sha256:fac529e0bca71571548f0dc65f240e8f94b780c115ca5deab654fe0687dacc5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:alpine` - linux; amd64

```console
$ docker pull kong@sha256:8a54bbf5026200150c46a182e0d56d74ba7572d6cfe98e863fb20cdafce1d95e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51522357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5bce760c29ce855d5935d777f2ec45b3a9ca895a09334825360cebd26a222e6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 14 Sep 2022 00:07:19 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 14 Sep 2022 00:07:19 GMT
ARG ASSET=ce
# Wed, 14 Sep 2022 00:07:19 GMT
ENV ASSET=ce
# Wed, 14 Sep 2022 00:07:19 GMT
ARG EE_PORTS
# Wed, 14 Sep 2022 00:07:19 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 14 Sep 2022 00:07:19 GMT
ARG KONG_VERSION=3.0.0
# Wed, 14 Sep 2022 00:07:19 GMT
ENV KONG_VERSION=3.0.0
# Wed, 14 Sep 2022 00:07:20 GMT
ARG KONG_AMD64_SHA=b8e21beb32f803fae0959694ce7b6cec796a4159757e61b9cc0d30bed9682d10
# Wed, 14 Sep 2022 00:07:20 GMT
ARG KONG_ARM64_SHA=4c5407c5ef2f0f29468e15ea4dc6a3f27011dbde3ce18170e4a4fd7e2bb2c03b
# Wed, 14 Sep 2022 00:07:28 GMT
# ARGS: KONG_AMD64_SHA=b8e21beb32f803fae0959694ce7b6cec796a4159757e61b9cc0d30bed9682d10 KONG_ARM64_SHA=4c5407c5ef2f0f29468e15ea4dc6a3f27011dbde3ce18170e4a4fd7e2bb2c03b
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Wed, 14 Sep 2022 00:07:28 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 14 Sep 2022 00:07:28 GMT
USER kong
# Wed, 14 Sep 2022 00:07:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Sep 2022 00:07:29 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 14 Sep 2022 00:07:29 GMT
STOPSIGNAL SIGQUIT
# Wed, 14 Sep 2022 00:07:29 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 14 Sep 2022 00:07:29 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df4f8c583856d7a692eae94f47792d4cc4a214e2b9d36d1b6dd5eaded569804f`  
		Last Modified: Wed, 14 Sep 2022 00:09:25 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd3d1d803c378e5eb206c29367530e2f8a92578534afdf16cd4ff0da3e687f5`  
		Last Modified: Wed, 14 Sep 2022 00:09:33 GMT  
		Size: 48.7 MB (48715295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7a99de7f80d542680872b47fc5405bf068af5fa56916f994a15149ce05e441`  
		Last Modified: Wed, 14 Sep 2022 00:09:25 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:2e4a51fba3b574ee35f990aef3bfd1120ad2e2704f3bc618697382a9f13eaa5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.5 MB (48542736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef17c5908a084b9879dac56870037eccf0c01f792d09fde4b1509019edcc6834`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:42:36 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 09 Aug 2022 20:42:37 GMT
ARG ASSET=ce
# Tue, 09 Aug 2022 20:42:38 GMT
ENV ASSET=ce
# Tue, 09 Aug 2022 20:42:39 GMT
ARG EE_PORTS
# Tue, 09 Aug 2022 20:42:41 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 09 Aug 2022 20:42:41 GMT
ARG KONG_VERSION=2.8.1
# Tue, 09 Aug 2022 20:42:42 GMT
ENV KONG_VERSION=2.8.1
# Tue, 09 Aug 2022 20:42:43 GMT
ARG KONG_AMD64_SHA=ccda33bf02803b6b8dd46b22990f92265fe61d900ba94e3e0fa26db0433098c0
# Tue, 09 Aug 2022 20:42:44 GMT
ARG KONG_ARM64_SHA=d21690332a89adf9900f7266e083f41f565eb009f2771ef112f3564878eeff53
# Tue, 09 Aug 2022 20:42:53 GMT
# ARGS: KONG_AMD64_SHA=ccda33bf02803b6b8dd46b22990f92265fe61d900ba94e3e0fa26db0433098c0 KONG_ARM64_SHA=d21690332a89adf9900f7266e083f41f565eb009f2771ef112f3564878eeff53
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Tue, 09 Aug 2022 20:42:54 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 09 Aug 2022 20:42:54 GMT
USER kong
# Tue, 09 Aug 2022 20:42:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:42:56 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 09 Aug 2022 20:42:57 GMT
STOPSIGNAL SIGQUIT
# Tue, 09 Aug 2022 20:42:58 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 09 Aug 2022 20:42:59 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70974eef12350195e179ac6f7e3f7ece7a292a31c6a4f5e19006b7df7f02df11`  
		Last Modified: Tue, 09 Aug 2022 20:45:58 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8314b864c236792b78293d546cc56ce12740413e395c5cc628457e893f46c905`  
		Last Modified: Tue, 09 Aug 2022 20:46:06 GMT  
		Size: 45.8 MB (45834060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:422419cd811d0936d352e9b792f92bcf50bdc9af873da1eb9c5f91f48f0570ca`  
		Last Modified: Tue, 09 Aug 2022 20:45:58 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:latest`

```console
$ docker pull kong@sha256:fac529e0bca71571548f0dc65f240e8f94b780c115ca5deab654fe0687dacc5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:latest` - linux; amd64

```console
$ docker pull kong@sha256:8a54bbf5026200150c46a182e0d56d74ba7572d6cfe98e863fb20cdafce1d95e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51522357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5bce760c29ce855d5935d777f2ec45b3a9ca895a09334825360cebd26a222e6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 14 Sep 2022 00:07:19 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 14 Sep 2022 00:07:19 GMT
ARG ASSET=ce
# Wed, 14 Sep 2022 00:07:19 GMT
ENV ASSET=ce
# Wed, 14 Sep 2022 00:07:19 GMT
ARG EE_PORTS
# Wed, 14 Sep 2022 00:07:19 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 14 Sep 2022 00:07:19 GMT
ARG KONG_VERSION=3.0.0
# Wed, 14 Sep 2022 00:07:19 GMT
ENV KONG_VERSION=3.0.0
# Wed, 14 Sep 2022 00:07:20 GMT
ARG KONG_AMD64_SHA=b8e21beb32f803fae0959694ce7b6cec796a4159757e61b9cc0d30bed9682d10
# Wed, 14 Sep 2022 00:07:20 GMT
ARG KONG_ARM64_SHA=4c5407c5ef2f0f29468e15ea4dc6a3f27011dbde3ce18170e4a4fd7e2bb2c03b
# Wed, 14 Sep 2022 00:07:28 GMT
# ARGS: KONG_AMD64_SHA=b8e21beb32f803fae0959694ce7b6cec796a4159757e61b9cc0d30bed9682d10 KONG_ARM64_SHA=4c5407c5ef2f0f29468e15ea4dc6a3f27011dbde3ce18170e4a4fd7e2bb2c03b
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Wed, 14 Sep 2022 00:07:28 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 14 Sep 2022 00:07:28 GMT
USER kong
# Wed, 14 Sep 2022 00:07:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Sep 2022 00:07:29 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 14 Sep 2022 00:07:29 GMT
STOPSIGNAL SIGQUIT
# Wed, 14 Sep 2022 00:07:29 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 14 Sep 2022 00:07:29 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df4f8c583856d7a692eae94f47792d4cc4a214e2b9d36d1b6dd5eaded569804f`  
		Last Modified: Wed, 14 Sep 2022 00:09:25 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcd3d1d803c378e5eb206c29367530e2f8a92578534afdf16cd4ff0da3e687f5`  
		Last Modified: Wed, 14 Sep 2022 00:09:33 GMT  
		Size: 48.7 MB (48715295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7a99de7f80d542680872b47fc5405bf068af5fa56916f994a15149ce05e441`  
		Last Modified: Wed, 14 Sep 2022 00:09:25 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:latest` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:2e4a51fba3b574ee35f990aef3bfd1120ad2e2704f3bc618697382a9f13eaa5a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.5 MB (48542736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef17c5908a084b9879dac56870037eccf0c01f792d09fde4b1509019edcc6834`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:42:36 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 09 Aug 2022 20:42:37 GMT
ARG ASSET=ce
# Tue, 09 Aug 2022 20:42:38 GMT
ENV ASSET=ce
# Tue, 09 Aug 2022 20:42:39 GMT
ARG EE_PORTS
# Tue, 09 Aug 2022 20:42:41 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 09 Aug 2022 20:42:41 GMT
ARG KONG_VERSION=2.8.1
# Tue, 09 Aug 2022 20:42:42 GMT
ENV KONG_VERSION=2.8.1
# Tue, 09 Aug 2022 20:42:43 GMT
ARG KONG_AMD64_SHA=ccda33bf02803b6b8dd46b22990f92265fe61d900ba94e3e0fa26db0433098c0
# Tue, 09 Aug 2022 20:42:44 GMT
ARG KONG_ARM64_SHA=d21690332a89adf9900f7266e083f41f565eb009f2771ef112f3564878eeff53
# Tue, 09 Aug 2022 20:42:53 GMT
# ARGS: KONG_AMD64_SHA=ccda33bf02803b6b8dd46b22990f92265fe61d900ba94e3e0fa26db0433098c0 KONG_ARM64_SHA=d21690332a89adf9900f7266e083f41f565eb009f2771ef112f3564878eeff53
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Tue, 09 Aug 2022 20:42:54 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 09 Aug 2022 20:42:54 GMT
USER kong
# Tue, 09 Aug 2022 20:42:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 09 Aug 2022 20:42:56 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 09 Aug 2022 20:42:57 GMT
STOPSIGNAL SIGQUIT
# Tue, 09 Aug 2022 20:42:58 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 09 Aug 2022 20:42:59 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70974eef12350195e179ac6f7e3f7ece7a292a31c6a4f5e19006b7df7f02df11`  
		Last Modified: Tue, 09 Aug 2022 20:45:58 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8314b864c236792b78293d546cc56ce12740413e395c5cc628457e893f46c905`  
		Last Modified: Tue, 09 Aug 2022 20:46:06 GMT  
		Size: 45.8 MB (45834060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:422419cd811d0936d352e9b792f92bcf50bdc9af873da1eb9c5f91f48f0570ca`  
		Last Modified: Tue, 09 Aug 2022 20:45:58 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:ubuntu`

```console
$ docker pull kong@sha256:8d61de4b25fcae2d7e0c3368f485486ef9132cec892b53657a79c2eaba544fe6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:e1b7a02b9e7a135b191170fde9406935383d015b7219c3a198a068430a68a29d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.7 MB (126666532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba3d56c232a3c9280f7ca9ed88c42b20112ba4997ef20356f1dc00c442f7d012`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:26 GMT
ADD file:ff6963f777661fb16cc12fb04a97c558bd94768a6e4ab5bd90e01f3086818853 in / 
# Thu, 01 Sep 2022 23:46:27 GMT
CMD ["bash"]
# Wed, 14 Sep 2022 00:07:33 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 14 Sep 2022 00:07:33 GMT
ARG ASSET=ce
# Wed, 14 Sep 2022 00:07:33 GMT
ENV ASSET=ce
# Wed, 14 Sep 2022 00:07:33 GMT
ARG EE_PORTS
# Wed, 14 Sep 2022 00:07:33 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 14 Sep 2022 00:07:34 GMT
ARG KONG_VERSION=3.0.0
# Wed, 14 Sep 2022 00:07:34 GMT
ENV KONG_VERSION=3.0.0
# Wed, 14 Sep 2022 00:07:34 GMT
ARG KONG_AMD64_SHA=3a38f6c4ba1cfc8897e655e46b957c7b0f2dd930111bf3d02411fedd1de53d6d
# Wed, 14 Sep 2022 00:07:34 GMT
ARG KONG_ARM64_SHA=190f82dd47df19339c025f37701e62191aa3063e77e15c5e57d5b77869058f69
# Wed, 14 Sep 2022 00:08:34 GMT
# ARGS: KONG_AMD64_SHA=3a38f6c4ba1cfc8897e655e46b957c7b0f2dd930111bf3d02411fedd1de53d6d KONG_ARM64_SHA=190f82dd47df19339c025f37701e62191aa3063e77e15c5e57d5b77869058f69
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 14 Sep 2022 00:08:35 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 14 Sep 2022 00:08:35 GMT
USER kong
# Wed, 14 Sep 2022 00:08:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Sep 2022 00:08:35 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 14 Sep 2022 00:08:35 GMT
STOPSIGNAL SIGQUIT
# Wed, 14 Sep 2022 00:08:35 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 14 Sep 2022 00:08:36 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:675920708c8bf10fbd02693dc8f43ee7dbe0a99cdfd55e06e6f1a8b43fd08e3f`  
		Last Modified: Thu, 01 Sep 2022 03:03:40 GMT  
		Size: 28.6 MB (28572685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f8ea18d6c5f278fa5820835cb24eea6a767e0f2db8069fa45a0a1a2e56c4b68`  
		Last Modified: Wed, 14 Sep 2022 00:09:51 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1fcce01ccb3758b7e74adaa6b4b0cb227b2ce8c0dde5c431af462be4e1fe93`  
		Last Modified: Wed, 14 Sep 2022 00:10:02 GMT  
		Size: 73.0 MB (73011012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a8c5f807f396934e8a026572c5fdc4c0ef99588049369adfdaac08e05f1d34`  
		Last Modified: Wed, 14 Sep 2022 00:09:50 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:7b2bf1303f661c575da457a9046b9620590b17bed4890b88bac7e818277a17a2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.7 MB (121715925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8824d66ce1a3f044fb009a0dd979f97b8dbf80491e6fa2a55c138baab821271e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 02 Sep 2022 00:57:42 GMT
ADD file:78c56cf572dbf860290780b955a94dc4de09bd3b8d64b6a83aee51afb349129a in / 
# Fri, 02 Sep 2022 00:57:43 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 06:45:21 GMT
ARG ASSET=ce
# Fri, 02 Sep 2022 06:45:21 GMT
ENV ASSET=ce
# Fri, 02 Sep 2022 06:45:22 GMT
ARG EE_PORTS
# Fri, 02 Sep 2022 06:45:24 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Fri, 02 Sep 2022 06:45:24 GMT
ARG KONG_VERSION=2.8.1
# Fri, 02 Sep 2022 06:45:25 GMT
ENV KONG_VERSION=2.8.1
# Fri, 02 Sep 2022 06:45:26 GMT
ARG KONG_AMD64_SHA=10d12d23e5890414d666663094d51a42de41f8a9806fbc0baaf9ac4d37794361
# Fri, 02 Sep 2022 06:45:27 GMT
ARG KONG_ARM64_SHA=61c13219ef64dac9aeae5ae775411e8cfcd406f068cf3e75d463f916ae6513cb
# Fri, 02 Sep 2022 06:45:56 GMT
# ARGS: KONG_AMD64_SHA=10d12d23e5890414d666663094d51a42de41f8a9806fbc0baaf9ac4d37794361 KONG_ARM64_SHA=61c13219ef64dac9aeae5ae775411e8cfcd406f068cf3e75d463f916ae6513cb
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 02 Sep 2022 06:45:57 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 02 Sep 2022 06:45:57 GMT
USER kong
# Fri, 02 Sep 2022 06:45:58 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 02 Sep 2022 06:45:59 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 02 Sep 2022 06:46:00 GMT
STOPSIGNAL SIGQUIT
# Fri, 02 Sep 2022 06:46:01 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 02 Sep 2022 06:46:02 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:7a9f619ee5e9c87f19eed59abef41d53eb0694f492da010ee069ff26e7b4ff3f`  
		Last Modified: Fri, 02 Sep 2022 00:59:23 GMT  
		Size: 27.2 MB (27191817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37921fee9fdc77f083b1d7e6150fcc91eaf74164601930750627e75ec46159c9`  
		Last Modified: Fri, 02 Sep 2022 06:50:16 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b2eb7f3cec9c8ba77ac0b9ea6c162a9999e3a4375f390e6e44c94e701bca00a`  
		Last Modified: Fri, 02 Sep 2022 06:50:26 GMT  
		Size: 69.4 MB (69441275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd6508437ef72723b0df33a3e5356b79b4143a273c6e2b63819b32a60b10904`  
		Last Modified: Fri, 02 Sep 2022 06:50:14 GMT  
		Size: 879.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
