<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kong`

-	[`kong:2.5`](#kong25)
-	[`kong:2.5-centos`](#kong25-centos)
-	[`kong:2.5-ubuntu`](#kong25-ubuntu)
-	[`kong:2.5.1`](#kong251)
-	[`kong:2.5.1-alpine`](#kong251-alpine)
-	[`kong:2.5.1-centos`](#kong251-centos)
-	[`kong:2.5.1-ubuntu`](#kong251-ubuntu)
-	[`kong:2.6`](#kong26)
-	[`kong:2.6-centos`](#kong26-centos)
-	[`kong:2.6-ubuntu`](#kong26-ubuntu)
-	[`kong:2.6.0`](#kong260)
-	[`kong:2.6.0-alpine`](#kong260-alpine)
-	[`kong:2.6.0-centos`](#kong260-centos)
-	[`kong:2.6.0-ubuntu`](#kong260-ubuntu)
-	[`kong:2.7`](#kong27)
-	[`kong:2.7-centos`](#kong27-centos)
-	[`kong:2.7-ubuntu`](#kong27-ubuntu)
-	[`kong:2.7.0`](#kong270)
-	[`kong:2.7.0-alpine`](#kong270-alpine)
-	[`kong:2.7.0-centos`](#kong270-centos)
-	[`kong:2.7.0-ubuntu`](#kong270-ubuntu)
-	[`kong:alpine`](#kongalpine)
-	[`kong:centos`](#kongcentos)
-	[`kong:latest`](#konglatest)
-	[`kong:ubuntu`](#kongubuntu)

## `kong:2.5`

```console
$ docker pull kong@sha256:37006fbba165f8f3051c2a810c972354f4ff38677cbba0191d6eb00eaaefaf25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.5` - linux; amd64

```console
$ docker pull kong@sha256:6896f87b90dcea49ee7009a9963a709e5644ebf0dff8491d2c010bf7fab6a974
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.8 MB (49826551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b114251eef2a2e43dbd58ea78009aa1eee554e03aad3399ccd64dac711f6437`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 05:49:01 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 13 Nov 2021 05:49:02 GMT
ARG ASSET=ce
# Sat, 13 Nov 2021 05:49:02 GMT
ENV ASSET=ce
# Sat, 13 Nov 2021 05:49:02 GMT
ARG EE_PORTS
# Sat, 13 Nov 2021 05:49:02 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Sat, 13 Nov 2021 05:49:25 GMT
ARG KONG_VERSION=2.5.1
# Sat, 13 Nov 2021 05:49:25 GMT
ENV KONG_VERSION=2.5.1
# Sat, 13 Nov 2021 05:49:25 GMT
ARG KONG_AMD64_SHA=f3fc429372e473e8616cf6afc56543a151bd08ba2bc235176d671515f691f20b
# Sat, 13 Nov 2021 05:49:25 GMT
ENV KONG_AMD64_SHA=f3fc429372e473e8616cf6afc56543a151bd08ba2bc235176d671515f691f20b
# Sat, 13 Nov 2021 05:49:26 GMT
ARG KONG_ARM64_SHA=e6d002b49aab10c1ae74cd533640eddc9e7f0ce30562cd7079d4b76d9eb70340
# Sat, 13 Nov 2021 05:49:26 GMT
ENV KONG_ARM64_SHA=e6d002b49aab10c1ae74cd533640eddc9e7f0ce30562cd7079d4b76d9eb70340
# Sat, 13 Nov 2021 05:49:35 GMT
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Sat, 13 Nov 2021 05:49:36 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Sat, 13 Nov 2021 05:49:36 GMT
USER kong
# Sat, 13 Nov 2021 05:49:37 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 13 Nov 2021 05:49:37 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 13 Nov 2021 05:49:37 GMT
STOPSIGNAL SIGQUIT
# Sat, 13 Nov 2021 05:49:37 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Sat, 13 Nov 2021 05:49:38 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e8b2c66462e7a485d21bf9baf11a6e252511cd3612b6fa68b0c1da6972f4cd`  
		Last Modified: Sat, 13 Nov 2021 05:50:42 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc7ab7edbafff55c804c295704914b38324636bc651035e4f405b24f4b86948`  
		Last Modified: Sat, 13 Nov 2021 05:51:23 GMT  
		Size: 47.0 MB (47002560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1a49a9faa0e6e6630ec2942c9320fa92d94e2e7f5be3ed6cb179adc2cdf39e`  
		Last Modified: Sat, 13 Nov 2021 05:51:14 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.5` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:44d38e7552f62fc3b5be6ff2bef42b19b300b1e913e79698c2a44a6c3c2f102f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49243531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6568234779ad7209323efea6272d617507673ec43ebc2623d13726b2170f51d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:11:28 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 13 Nov 2021 06:11:29 GMT
ARG ASSET=ce
# Sat, 13 Nov 2021 06:11:30 GMT
ENV ASSET=ce
# Sat, 13 Nov 2021 06:11:31 GMT
ARG EE_PORTS
# Sat, 13 Nov 2021 06:11:33 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Sat, 13 Nov 2021 06:13:43 GMT
ARG KONG_VERSION=2.5.1
# Sat, 13 Nov 2021 06:13:43 GMT
ENV KONG_VERSION=2.5.1
# Sat, 13 Nov 2021 06:13:44 GMT
ARG KONG_AMD64_SHA=f3fc429372e473e8616cf6afc56543a151bd08ba2bc235176d671515f691f20b
# Sat, 13 Nov 2021 06:13:45 GMT
ENV KONG_AMD64_SHA=f3fc429372e473e8616cf6afc56543a151bd08ba2bc235176d671515f691f20b
# Sat, 13 Nov 2021 06:13:46 GMT
ARG KONG_ARM64_SHA=e6d002b49aab10c1ae74cd533640eddc9e7f0ce30562cd7079d4b76d9eb70340
# Sat, 13 Nov 2021 06:13:47 GMT
ENV KONG_ARM64_SHA=e6d002b49aab10c1ae74cd533640eddc9e7f0ce30562cd7079d4b76d9eb70340
# Sat, 13 Nov 2021 06:14:01 GMT
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Sat, 13 Nov 2021 06:14:02 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Sat, 13 Nov 2021 06:14:02 GMT
USER kong
# Sat, 13 Nov 2021 06:14:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 13 Nov 2021 06:14:04 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 13 Nov 2021 06:14:05 GMT
STOPSIGNAL SIGQUIT
# Sat, 13 Nov 2021 06:14:06 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Sat, 13 Nov 2021 06:14:07 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53315a86544ab6e48bbf724baae0beec28097187f7ffcda4174c31e3cbb0224e`  
		Last Modified: Sat, 13 Nov 2021 06:16:59 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e017ba0adce02b70c202fa4e8327a67f0d9497050e133752e4416b5658ac0a8`  
		Last Modified: Sat, 13 Nov 2021 06:17:35 GMT  
		Size: 46.5 MB (46524818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75406dbc9d0f6741b0268d704cf6a2dbb08dd974edd43eb9582b19aaaf8e2f98`  
		Last Modified: Sat, 13 Nov 2021 06:17:27 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.5-centos`

```console
$ docker pull kong@sha256:29f839eedc97022967ae46e0ec2ba5dfe75b37525c409b475b7a61a7c0e0ee91
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:2.5-centos` - linux; amd64

```console
$ docker pull kong@sha256:033decce472824142c52050eeb2ad85a24f1f775d00888d421ad065b3113e223
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.9 MB (160921195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5212ef94876a94444a623c7c826d7ea5bd5d0fce1958eb2cd472a8a0f58befd1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:04 GMT
ADD file:805cb5e15fb6e0bb0326ca33fd2942e068863ce2a8491bb71522c652f31fb466 in / 
# Wed, 15 Sep 2021 18:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20210915
# Wed, 15 Sep 2021 18:20:05 GMT
CMD ["/bin/bash"]
# Wed, 15 Sep 2021 23:21:23 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 15 Sep 2021 23:21:23 GMT
ARG ASSET=ce
# Wed, 15 Sep 2021 23:21:23 GMT
ENV ASSET=ce
# Wed, 15 Sep 2021 23:21:24 GMT
ARG EE_PORTS
# Wed, 15 Sep 2021 23:21:24 GMT
COPY file:ff02c070e4c89f043b176279a7e41464b5fab8cb98cfcd6332fad2d2741fc41d in /tmp/kong.rpm 
# Wed, 15 Sep 2021 23:21:24 GMT
ARG KONG_VERSION=2.5.1
# Wed, 15 Sep 2021 23:21:24 GMT
ENV KONG_VERSION=2.5.1
# Wed, 15 Sep 2021 23:21:24 GMT
ARG KONG_SHA256=36c03c53a4e3a3f6f0968f68258fa93a584af5c33ed29fa5e05e089dfb97b730
# Wed, 15 Sep 2021 23:21:58 GMT
# ARGS: KONG_SHA256=36c03c53a4e3a3f6f0968f68258fa93a584af5c33ed29fa5e05e089dfb97b730
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then       curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-centos-7/Packages/k/kong-$KONG_VERSION.el7.amd64.rpm -o /tmp/kong.rpm       && echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -;     fi;     yum install -y -q unzip shadow-utils git     && yum clean all -q     && rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki     && yum install -y /tmp/kong.rpm     && yum clean all     && rm /tmp/kong.rpm     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 15 Sep 2021 23:21:59 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 15 Sep 2021 23:21:59 GMT
USER kong
# Wed, 15 Sep 2021 23:21:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 15 Sep 2021 23:22:00 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 15 Sep 2021 23:22:00 GMT
STOPSIGNAL SIGQUIT
# Wed, 15 Sep 2021 23:22:00 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 15 Sep 2021 23:22:00 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:a1d0c75327776413fa0db9ed3adcdbadedc95a662eb1d360dad82bb913f8a1d1`  
		Last Modified: Wed, 15 Sep 2021 18:21:25 GMT  
		Size: 83.5 MB (83518086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fb8a137fa2b84d66997b2207a6880267b365a0a2d08a22a00c4965ecbec7f93`  
		Last Modified: Wed, 15 Sep 2021 23:23:25 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5520f68e079f5dbe56c351330fdc8e5688d18f21e5b3059e73da20ea1f82e79c`  
		Last Modified: Wed, 15 Sep 2021 23:23:37 GMT  
		Size: 77.4 MB (77402098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af293b6ea93ad38f2ce79b696ebdcf75d1917845c0eaf599089bea1eec48e287`  
		Last Modified: Wed, 15 Sep 2021 23:23:25 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.5-ubuntu`

```console
$ docker pull kong@sha256:54a2d4bb7b7a60e2c29fdb26143041c8d499137ef40f7657d5d7c46f6c550936
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.5-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:984db305e82194630fa8b842fd82cd74634730da76621969c5240f3fd96b447f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (128046129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb8ce0a424cd4b135cf95e7461d26bd1de5a69d4ce6b763c9d1b1d9c03b02a5e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 07:37:26 GMT
ARG ASSET=ce
# Wed, 02 Feb 2022 07:37:27 GMT
ENV ASSET=ce
# Wed, 02 Feb 2022 07:37:27 GMT
ARG EE_PORTS
# Wed, 02 Feb 2022 07:37:27 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 02 Feb 2022 07:39:25 GMT
ARG KONG_VERSION=2.5.1
# Wed, 02 Feb 2022 07:39:25 GMT
ENV KONG_VERSION=2.5.1
# Wed, 02 Feb 2022 07:39:45 GMT
RUN set -ex     && apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)/pool/all/k/kong/kong_${KONG_VERSION}_$(dpkg --print-architecture).deb -o /tmp/kong.deb       && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 02 Feb 2022 07:39:46 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 02 Feb 2022 07:39:46 GMT
USER kong
# Wed, 02 Feb 2022 07:39:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Feb 2022 07:39:47 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 02 Feb 2022 07:39:47 GMT
STOPSIGNAL SIGQUIT
# Wed, 02 Feb 2022 07:39:47 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 02 Feb 2022 07:39:47 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d35932487d0dcc4bbc7da3fcbb5c567b891759923d10b1daed30b77b8c8c10`  
		Last Modified: Wed, 02 Feb 2022 07:40:24 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d9a12df81804755feee104739245e48405adf65b0c08167c3b19ae67f500995`  
		Last Modified: Wed, 02 Feb 2022 07:41:23 GMT  
		Size: 74.4 MB (74399196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd99c61c4596638fb15f1739da1eef2b22147e1056ce1697b49bfb687ff74da`  
		Last Modified: Wed, 02 Feb 2022 07:41:11 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.5-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:7fb163125ba0769471c7adccc2609abcd37c3e58afcfb159ab99aa30f5ba58f2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125879708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8100ea3c312d55c4a34fcf3706f2584737cc61f1662715a6dd709d77d3f79138`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 31 Aug 2021 01:41:19 GMT
ADD file:3c6dc937cb7b4c81b42126f377d23320ec1d0a8ca34d38e7c45871f1d08dac43 in / 
# Tue, 31 Aug 2021 01:41:20 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:41:20 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:41:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:41:21 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 03:13:00 GMT
ARG ASSET=ce
# Tue, 31 Aug 2021 03:13:00 GMT
ENV ASSET=ce
# Tue, 31 Aug 2021 03:13:00 GMT
ARG EE_PORTS
# Tue, 31 Aug 2021 03:13:00 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Tue, 31 Aug 2021 03:13:01 GMT
ARG KONG_VERSION=2.5.0
# Tue, 31 Aug 2021 03:13:01 GMT
ENV KONG_VERSION=2.5.0
# Tue, 31 Aug 2021 03:13:24 GMT
RUN set -ex     && apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)/pool/all/k/kong/kong_${KONG_VERSION}_$(dpkg --print-architecture).deb -o /tmp/kong.deb       && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 31 Aug 2021 03:13:25 GMT
COPY file:ae813ec19d3fef1de3793f6717c2aed3a9daa94e583e9e55448084541de3c5ff in /docker-entrypoint.sh 
# Tue, 31 Aug 2021 03:13:25 GMT
USER kong
# Tue, 31 Aug 2021 03:13:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 31 Aug 2021 03:13:25 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 31 Aug 2021 03:13:26 GMT
STOPSIGNAL SIGQUIT
# Tue, 31 Aug 2021 03:13:26 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 31 Aug 2021 03:13:26 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:828b35a09f0b2f3d1dead43aa2468ff5eba6c463423b3fff7ee6d150f6fd1b6b`  
		Last Modified: Thu, 05 Aug 2021 00:25:09 GMT  
		Size: 41.2 MB (41239253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85569e0c17003d9cf46a8b94076418863e0abfc5474bb830403acf246947fea7`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32ca509d28808ab7c61361835292ee8eddecd0c0949d658bde0ab1a77ecbf6e`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 469.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8168af71f81f1ffa234c301e9cc2ee87b560ad8b74ef4100f8ab4a6abf3a8ad3`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eee59a359925630cd377c9610b18f7d7797349cdbabeda7b8c8685852a5ff83`  
		Last Modified: Tue, 31 Aug 2021 03:14:48 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbbe71eb414d43ff3fbf75c0de9133ebafceaf672848c6e2c17e4ab47780e97b`  
		Last Modified: Tue, 31 Aug 2021 03:15:00 GMT  
		Size: 59.6 MB (59556314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a45ed64e5c35d56c7aafb050d22218142de8f6d3142eba9294d41638844747`  
		Last Modified: Tue, 31 Aug 2021 03:14:46 GMT  
		Size: 690.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.5.1`

```console
$ docker pull kong@sha256:37006fbba165f8f3051c2a810c972354f4ff38677cbba0191d6eb00eaaefaf25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.5.1` - linux; amd64

```console
$ docker pull kong@sha256:6896f87b90dcea49ee7009a9963a709e5644ebf0dff8491d2c010bf7fab6a974
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.8 MB (49826551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b114251eef2a2e43dbd58ea78009aa1eee554e03aad3399ccd64dac711f6437`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 05:49:01 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 13 Nov 2021 05:49:02 GMT
ARG ASSET=ce
# Sat, 13 Nov 2021 05:49:02 GMT
ENV ASSET=ce
# Sat, 13 Nov 2021 05:49:02 GMT
ARG EE_PORTS
# Sat, 13 Nov 2021 05:49:02 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Sat, 13 Nov 2021 05:49:25 GMT
ARG KONG_VERSION=2.5.1
# Sat, 13 Nov 2021 05:49:25 GMT
ENV KONG_VERSION=2.5.1
# Sat, 13 Nov 2021 05:49:25 GMT
ARG KONG_AMD64_SHA=f3fc429372e473e8616cf6afc56543a151bd08ba2bc235176d671515f691f20b
# Sat, 13 Nov 2021 05:49:25 GMT
ENV KONG_AMD64_SHA=f3fc429372e473e8616cf6afc56543a151bd08ba2bc235176d671515f691f20b
# Sat, 13 Nov 2021 05:49:26 GMT
ARG KONG_ARM64_SHA=e6d002b49aab10c1ae74cd533640eddc9e7f0ce30562cd7079d4b76d9eb70340
# Sat, 13 Nov 2021 05:49:26 GMT
ENV KONG_ARM64_SHA=e6d002b49aab10c1ae74cd533640eddc9e7f0ce30562cd7079d4b76d9eb70340
# Sat, 13 Nov 2021 05:49:35 GMT
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Sat, 13 Nov 2021 05:49:36 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Sat, 13 Nov 2021 05:49:36 GMT
USER kong
# Sat, 13 Nov 2021 05:49:37 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 13 Nov 2021 05:49:37 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 13 Nov 2021 05:49:37 GMT
STOPSIGNAL SIGQUIT
# Sat, 13 Nov 2021 05:49:37 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Sat, 13 Nov 2021 05:49:38 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e8b2c66462e7a485d21bf9baf11a6e252511cd3612b6fa68b0c1da6972f4cd`  
		Last Modified: Sat, 13 Nov 2021 05:50:42 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc7ab7edbafff55c804c295704914b38324636bc651035e4f405b24f4b86948`  
		Last Modified: Sat, 13 Nov 2021 05:51:23 GMT  
		Size: 47.0 MB (47002560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1a49a9faa0e6e6630ec2942c9320fa92d94e2e7f5be3ed6cb179adc2cdf39e`  
		Last Modified: Sat, 13 Nov 2021 05:51:14 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.5.1` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:44d38e7552f62fc3b5be6ff2bef42b19b300b1e913e79698c2a44a6c3c2f102f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49243531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6568234779ad7209323efea6272d617507673ec43ebc2623d13726b2170f51d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:11:28 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 13 Nov 2021 06:11:29 GMT
ARG ASSET=ce
# Sat, 13 Nov 2021 06:11:30 GMT
ENV ASSET=ce
# Sat, 13 Nov 2021 06:11:31 GMT
ARG EE_PORTS
# Sat, 13 Nov 2021 06:11:33 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Sat, 13 Nov 2021 06:13:43 GMT
ARG KONG_VERSION=2.5.1
# Sat, 13 Nov 2021 06:13:43 GMT
ENV KONG_VERSION=2.5.1
# Sat, 13 Nov 2021 06:13:44 GMT
ARG KONG_AMD64_SHA=f3fc429372e473e8616cf6afc56543a151bd08ba2bc235176d671515f691f20b
# Sat, 13 Nov 2021 06:13:45 GMT
ENV KONG_AMD64_SHA=f3fc429372e473e8616cf6afc56543a151bd08ba2bc235176d671515f691f20b
# Sat, 13 Nov 2021 06:13:46 GMT
ARG KONG_ARM64_SHA=e6d002b49aab10c1ae74cd533640eddc9e7f0ce30562cd7079d4b76d9eb70340
# Sat, 13 Nov 2021 06:13:47 GMT
ENV KONG_ARM64_SHA=e6d002b49aab10c1ae74cd533640eddc9e7f0ce30562cd7079d4b76d9eb70340
# Sat, 13 Nov 2021 06:14:01 GMT
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Sat, 13 Nov 2021 06:14:02 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Sat, 13 Nov 2021 06:14:02 GMT
USER kong
# Sat, 13 Nov 2021 06:14:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 13 Nov 2021 06:14:04 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 13 Nov 2021 06:14:05 GMT
STOPSIGNAL SIGQUIT
# Sat, 13 Nov 2021 06:14:06 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Sat, 13 Nov 2021 06:14:07 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53315a86544ab6e48bbf724baae0beec28097187f7ffcda4174c31e3cbb0224e`  
		Last Modified: Sat, 13 Nov 2021 06:16:59 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e017ba0adce02b70c202fa4e8327a67f0d9497050e133752e4416b5658ac0a8`  
		Last Modified: Sat, 13 Nov 2021 06:17:35 GMT  
		Size: 46.5 MB (46524818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75406dbc9d0f6741b0268d704cf6a2dbb08dd974edd43eb9582b19aaaf8e2f98`  
		Last Modified: Sat, 13 Nov 2021 06:17:27 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.5.1-alpine`

```console
$ docker pull kong@sha256:37006fbba165f8f3051c2a810c972354f4ff38677cbba0191d6eb00eaaefaf25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.5.1-alpine` - linux; amd64

```console
$ docker pull kong@sha256:6896f87b90dcea49ee7009a9963a709e5644ebf0dff8491d2c010bf7fab6a974
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.8 MB (49826551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b114251eef2a2e43dbd58ea78009aa1eee554e03aad3399ccd64dac711f6437`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 05:49:01 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 13 Nov 2021 05:49:02 GMT
ARG ASSET=ce
# Sat, 13 Nov 2021 05:49:02 GMT
ENV ASSET=ce
# Sat, 13 Nov 2021 05:49:02 GMT
ARG EE_PORTS
# Sat, 13 Nov 2021 05:49:02 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Sat, 13 Nov 2021 05:49:25 GMT
ARG KONG_VERSION=2.5.1
# Sat, 13 Nov 2021 05:49:25 GMT
ENV KONG_VERSION=2.5.1
# Sat, 13 Nov 2021 05:49:25 GMT
ARG KONG_AMD64_SHA=f3fc429372e473e8616cf6afc56543a151bd08ba2bc235176d671515f691f20b
# Sat, 13 Nov 2021 05:49:25 GMT
ENV KONG_AMD64_SHA=f3fc429372e473e8616cf6afc56543a151bd08ba2bc235176d671515f691f20b
# Sat, 13 Nov 2021 05:49:26 GMT
ARG KONG_ARM64_SHA=e6d002b49aab10c1ae74cd533640eddc9e7f0ce30562cd7079d4b76d9eb70340
# Sat, 13 Nov 2021 05:49:26 GMT
ENV KONG_ARM64_SHA=e6d002b49aab10c1ae74cd533640eddc9e7f0ce30562cd7079d4b76d9eb70340
# Sat, 13 Nov 2021 05:49:35 GMT
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Sat, 13 Nov 2021 05:49:36 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Sat, 13 Nov 2021 05:49:36 GMT
USER kong
# Sat, 13 Nov 2021 05:49:37 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 13 Nov 2021 05:49:37 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 13 Nov 2021 05:49:37 GMT
STOPSIGNAL SIGQUIT
# Sat, 13 Nov 2021 05:49:37 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Sat, 13 Nov 2021 05:49:38 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e8b2c66462e7a485d21bf9baf11a6e252511cd3612b6fa68b0c1da6972f4cd`  
		Last Modified: Sat, 13 Nov 2021 05:50:42 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc7ab7edbafff55c804c295704914b38324636bc651035e4f405b24f4b86948`  
		Last Modified: Sat, 13 Nov 2021 05:51:23 GMT  
		Size: 47.0 MB (47002560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1a49a9faa0e6e6630ec2942c9320fa92d94e2e7f5be3ed6cb179adc2cdf39e`  
		Last Modified: Sat, 13 Nov 2021 05:51:14 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.5.1-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:44d38e7552f62fc3b5be6ff2bef42b19b300b1e913e79698c2a44a6c3c2f102f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49243531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6568234779ad7209323efea6272d617507673ec43ebc2623d13726b2170f51d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:11:28 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 13 Nov 2021 06:11:29 GMT
ARG ASSET=ce
# Sat, 13 Nov 2021 06:11:30 GMT
ENV ASSET=ce
# Sat, 13 Nov 2021 06:11:31 GMT
ARG EE_PORTS
# Sat, 13 Nov 2021 06:11:33 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Sat, 13 Nov 2021 06:13:43 GMT
ARG KONG_VERSION=2.5.1
# Sat, 13 Nov 2021 06:13:43 GMT
ENV KONG_VERSION=2.5.1
# Sat, 13 Nov 2021 06:13:44 GMT
ARG KONG_AMD64_SHA=f3fc429372e473e8616cf6afc56543a151bd08ba2bc235176d671515f691f20b
# Sat, 13 Nov 2021 06:13:45 GMT
ENV KONG_AMD64_SHA=f3fc429372e473e8616cf6afc56543a151bd08ba2bc235176d671515f691f20b
# Sat, 13 Nov 2021 06:13:46 GMT
ARG KONG_ARM64_SHA=e6d002b49aab10c1ae74cd533640eddc9e7f0ce30562cd7079d4b76d9eb70340
# Sat, 13 Nov 2021 06:13:47 GMT
ENV KONG_ARM64_SHA=e6d002b49aab10c1ae74cd533640eddc9e7f0ce30562cd7079d4b76d9eb70340
# Sat, 13 Nov 2021 06:14:01 GMT
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Sat, 13 Nov 2021 06:14:02 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Sat, 13 Nov 2021 06:14:02 GMT
USER kong
# Sat, 13 Nov 2021 06:14:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 13 Nov 2021 06:14:04 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 13 Nov 2021 06:14:05 GMT
STOPSIGNAL SIGQUIT
# Sat, 13 Nov 2021 06:14:06 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Sat, 13 Nov 2021 06:14:07 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53315a86544ab6e48bbf724baae0beec28097187f7ffcda4174c31e3cbb0224e`  
		Last Modified: Sat, 13 Nov 2021 06:16:59 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e017ba0adce02b70c202fa4e8327a67f0d9497050e133752e4416b5658ac0a8`  
		Last Modified: Sat, 13 Nov 2021 06:17:35 GMT  
		Size: 46.5 MB (46524818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75406dbc9d0f6741b0268d704cf6a2dbb08dd974edd43eb9582b19aaaf8e2f98`  
		Last Modified: Sat, 13 Nov 2021 06:17:27 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.5.1-centos`

```console
$ docker pull kong@sha256:29f839eedc97022967ae46e0ec2ba5dfe75b37525c409b475b7a61a7c0e0ee91
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:2.5.1-centos` - linux; amd64

```console
$ docker pull kong@sha256:033decce472824142c52050eeb2ad85a24f1f775d00888d421ad065b3113e223
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.9 MB (160921195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5212ef94876a94444a623c7c826d7ea5bd5d0fce1958eb2cd472a8a0f58befd1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:04 GMT
ADD file:805cb5e15fb6e0bb0326ca33fd2942e068863ce2a8491bb71522c652f31fb466 in / 
# Wed, 15 Sep 2021 18:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20210915
# Wed, 15 Sep 2021 18:20:05 GMT
CMD ["/bin/bash"]
# Wed, 15 Sep 2021 23:21:23 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 15 Sep 2021 23:21:23 GMT
ARG ASSET=ce
# Wed, 15 Sep 2021 23:21:23 GMT
ENV ASSET=ce
# Wed, 15 Sep 2021 23:21:24 GMT
ARG EE_PORTS
# Wed, 15 Sep 2021 23:21:24 GMT
COPY file:ff02c070e4c89f043b176279a7e41464b5fab8cb98cfcd6332fad2d2741fc41d in /tmp/kong.rpm 
# Wed, 15 Sep 2021 23:21:24 GMT
ARG KONG_VERSION=2.5.1
# Wed, 15 Sep 2021 23:21:24 GMT
ENV KONG_VERSION=2.5.1
# Wed, 15 Sep 2021 23:21:24 GMT
ARG KONG_SHA256=36c03c53a4e3a3f6f0968f68258fa93a584af5c33ed29fa5e05e089dfb97b730
# Wed, 15 Sep 2021 23:21:58 GMT
# ARGS: KONG_SHA256=36c03c53a4e3a3f6f0968f68258fa93a584af5c33ed29fa5e05e089dfb97b730
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then       curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-centos-7/Packages/k/kong-$KONG_VERSION.el7.amd64.rpm -o /tmp/kong.rpm       && echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -;     fi;     yum install -y -q unzip shadow-utils git     && yum clean all -q     && rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki     && yum install -y /tmp/kong.rpm     && yum clean all     && rm /tmp/kong.rpm     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 15 Sep 2021 23:21:59 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 15 Sep 2021 23:21:59 GMT
USER kong
# Wed, 15 Sep 2021 23:21:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 15 Sep 2021 23:22:00 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 15 Sep 2021 23:22:00 GMT
STOPSIGNAL SIGQUIT
# Wed, 15 Sep 2021 23:22:00 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 15 Sep 2021 23:22:00 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:a1d0c75327776413fa0db9ed3adcdbadedc95a662eb1d360dad82bb913f8a1d1`  
		Last Modified: Wed, 15 Sep 2021 18:21:25 GMT  
		Size: 83.5 MB (83518086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fb8a137fa2b84d66997b2207a6880267b365a0a2d08a22a00c4965ecbec7f93`  
		Last Modified: Wed, 15 Sep 2021 23:23:25 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5520f68e079f5dbe56c351330fdc8e5688d18f21e5b3059e73da20ea1f82e79c`  
		Last Modified: Wed, 15 Sep 2021 23:23:37 GMT  
		Size: 77.4 MB (77402098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af293b6ea93ad38f2ce79b696ebdcf75d1917845c0eaf599089bea1eec48e287`  
		Last Modified: Wed, 15 Sep 2021 23:23:25 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.5.1-ubuntu`

```console
$ docker pull kong@sha256:8b4d5584a8d44b94c11443c269f4ed7402e947a4181fb3a1e4be1d539d2cef98
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:2.5.1-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:984db305e82194630fa8b842fd82cd74634730da76621969c5240f3fd96b447f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (128046129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb8ce0a424cd4b135cf95e7461d26bd1de5a69d4ce6b763c9d1b1d9c03b02a5e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 07:37:26 GMT
ARG ASSET=ce
# Wed, 02 Feb 2022 07:37:27 GMT
ENV ASSET=ce
# Wed, 02 Feb 2022 07:37:27 GMT
ARG EE_PORTS
# Wed, 02 Feb 2022 07:37:27 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 02 Feb 2022 07:39:25 GMT
ARG KONG_VERSION=2.5.1
# Wed, 02 Feb 2022 07:39:25 GMT
ENV KONG_VERSION=2.5.1
# Wed, 02 Feb 2022 07:39:45 GMT
RUN set -ex     && apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)/pool/all/k/kong/kong_${KONG_VERSION}_$(dpkg --print-architecture).deb -o /tmp/kong.deb       && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 02 Feb 2022 07:39:46 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 02 Feb 2022 07:39:46 GMT
USER kong
# Wed, 02 Feb 2022 07:39:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Feb 2022 07:39:47 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 02 Feb 2022 07:39:47 GMT
STOPSIGNAL SIGQUIT
# Wed, 02 Feb 2022 07:39:47 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 02 Feb 2022 07:39:47 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d35932487d0dcc4bbc7da3fcbb5c567b891759923d10b1daed30b77b8c8c10`  
		Last Modified: Wed, 02 Feb 2022 07:40:24 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d9a12df81804755feee104739245e48405adf65b0c08167c3b19ae67f500995`  
		Last Modified: Wed, 02 Feb 2022 07:41:23 GMT  
		Size: 74.4 MB (74399196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd99c61c4596638fb15f1739da1eef2b22147e1056ce1697b49bfb687ff74da`  
		Last Modified: Wed, 02 Feb 2022 07:41:11 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.6`

```console
$ docker pull kong@sha256:134f182c5a20389f4071a71a5946a427cb0d5de6ad382ca66a4156fef441636c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.6` - linux; amd64

```console
$ docker pull kong@sha256:95515d0f66dd958be1e30af772ada51bd4812d2a27bcb9124074fd1a2df4402e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 MB (49865802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d51b92ff33146bb0aa7d22bd05cf622124574febe4ee673d92dfed8299b140ce`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 05:49:01 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 13 Nov 2021 05:49:02 GMT
ARG ASSET=ce
# Sat, 13 Nov 2021 05:49:02 GMT
ENV ASSET=ce
# Sat, 13 Nov 2021 05:49:02 GMT
ARG EE_PORTS
# Sat, 13 Nov 2021 05:49:02 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Sat, 13 Nov 2021 05:49:03 GMT
ARG KONG_VERSION=2.6.0
# Sat, 13 Nov 2021 05:49:03 GMT
ENV KONG_VERSION=2.6.0
# Sat, 13 Nov 2021 05:49:03 GMT
ARG KONG_AMD64_SHA=43fb5f27185e274e22b4a36b93b1b7e27afe94b9fd2efbe4ec69b8ed8a9e5902
# Sat, 13 Nov 2021 05:49:03 GMT
ENV KONG_AMD64_SHA=43fb5f27185e274e22b4a36b93b1b7e27afe94b9fd2efbe4ec69b8ed8a9e5902
# Sat, 13 Nov 2021 05:49:03 GMT
ARG KONG_ARM64_SHA=a057eaa6d10ecf49443ec0cac6e1b70a62ee357a777e0e169c780e18fd5c5544
# Sat, 13 Nov 2021 05:49:04 GMT
ENV KONG_ARM64_SHA=a057eaa6d10ecf49443ec0cac6e1b70a62ee357a777e0e169c780e18fd5c5544
# Sat, 13 Nov 2021 05:49:12 GMT
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Sat, 13 Nov 2021 05:49:13 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Sat, 13 Nov 2021 05:49:13 GMT
USER kong
# Sat, 13 Nov 2021 05:49:13 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 13 Nov 2021 05:49:14 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 13 Nov 2021 05:49:14 GMT
STOPSIGNAL SIGQUIT
# Sat, 13 Nov 2021 05:49:14 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Sat, 13 Nov 2021 05:49:15 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e8b2c66462e7a485d21bf9baf11a6e252511cd3612b6fa68b0c1da6972f4cd`  
		Last Modified: Sat, 13 Nov 2021 05:50:42 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c7e18e0a769d4001d507fbe88c18e222f1ef8b290b08b684cbe031f308a212`  
		Last Modified: Sat, 13 Nov 2021 05:50:51 GMT  
		Size: 47.0 MB (47041810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72f9e277edccd9c623819e5913361a38ef18b0d49d8563a765c7cbda0260b9d4`  
		Last Modified: Sat, 13 Nov 2021 05:50:42 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.6` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:dd3e38ff91a3e3c07a6df2dc1779ff3b8ecf032549ff6dc28e21e4e06f706775
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49271665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28105dd1de87006bd942029226d1f8bdf5ab9948dfea537b0f76c4b27b184fda`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:11:28 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 13 Nov 2021 06:11:29 GMT
ARG ASSET=ce
# Sat, 13 Nov 2021 06:11:30 GMT
ENV ASSET=ce
# Sat, 13 Nov 2021 06:11:31 GMT
ARG EE_PORTS
# Sat, 13 Nov 2021 06:11:33 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Sat, 13 Nov 2021 06:11:33 GMT
ARG KONG_VERSION=2.6.0
# Sat, 13 Nov 2021 06:11:34 GMT
ENV KONG_VERSION=2.6.0
# Sat, 13 Nov 2021 06:11:35 GMT
ARG KONG_AMD64_SHA=43fb5f27185e274e22b4a36b93b1b7e27afe94b9fd2efbe4ec69b8ed8a9e5902
# Sat, 13 Nov 2021 06:11:36 GMT
ENV KONG_AMD64_SHA=43fb5f27185e274e22b4a36b93b1b7e27afe94b9fd2efbe4ec69b8ed8a9e5902
# Sat, 13 Nov 2021 06:11:37 GMT
ARG KONG_ARM64_SHA=a057eaa6d10ecf49443ec0cac6e1b70a62ee357a777e0e169c780e18fd5c5544
# Sat, 13 Nov 2021 06:11:38 GMT
ENV KONG_ARM64_SHA=a057eaa6d10ecf49443ec0cac6e1b70a62ee357a777e0e169c780e18fd5c5544
# Sat, 13 Nov 2021 06:11:56 GMT
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Sat, 13 Nov 2021 06:11:57 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Sat, 13 Nov 2021 06:11:57 GMT
USER kong
# Sat, 13 Nov 2021 06:11:58 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 13 Nov 2021 06:11:59 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 13 Nov 2021 06:12:00 GMT
STOPSIGNAL SIGQUIT
# Sat, 13 Nov 2021 06:12:01 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Sat, 13 Nov 2021 06:12:02 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53315a86544ab6e48bbf724baae0beec28097187f7ffcda4174c31e3cbb0224e`  
		Last Modified: Sat, 13 Nov 2021 06:16:59 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b212018ea5e6b01778c1aa4de7a912a6e2f2da7a8d9580291a89607a2e1aa4`  
		Last Modified: Sat, 13 Nov 2021 06:17:08 GMT  
		Size: 46.6 MB (46552952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c1c626e2a45c65a7f5d968620e36a052607a53c9ca3cdfc4b056a5dfdc0c3e`  
		Last Modified: Sat, 13 Nov 2021 06:16:59 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.6-centos`

```console
$ docker pull kong@sha256:03453c57b918faa98be9faf2ee7b91239c4a4030a5478b750712408b4104b6f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:2.6-centos` - linux; amd64

```console
$ docker pull kong@sha256:27efe9259a4da91b92a42030be7bec0d4d3e09b6483ac9473dd4996037c84d3c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.0 MB (160965349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee5d952d7b8eb428c80083082cfea96234e5a263dea8f0a1ef32882fbcec5920`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:04 GMT
ADD file:805cb5e15fb6e0bb0326ca33fd2942e068863ce2a8491bb71522c652f31fb466 in / 
# Wed, 15 Sep 2021 18:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20210915
# Wed, 15 Sep 2021 18:20:05 GMT
CMD ["/bin/bash"]
# Wed, 15 Sep 2021 23:21:23 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 15 Sep 2021 23:21:23 GMT
ARG ASSET=ce
# Wed, 15 Sep 2021 23:21:23 GMT
ENV ASSET=ce
# Wed, 15 Sep 2021 23:21:24 GMT
ARG EE_PORTS
# Wed, 15 Sep 2021 23:21:24 GMT
COPY file:ff02c070e4c89f043b176279a7e41464b5fab8cb98cfcd6332fad2d2741fc41d in /tmp/kong.rpm 
# Tue, 05 Oct 2021 17:43:00 GMT
ARG KONG_VERSION=2.6.0
# Tue, 05 Oct 2021 17:43:00 GMT
ENV KONG_VERSION=2.6.0
# Tue, 05 Oct 2021 17:43:01 GMT
ARG KONG_SHA256=f83a1030b01aa3deb4535394b550228f4804a6fd35a4ea4b11e12dcbcacdadc0
# Tue, 05 Oct 2021 17:43:40 GMT
# ARGS: KONG_SHA256=f83a1030b01aa3deb4535394b550228f4804a6fd35a4ea4b11e12dcbcacdadc0
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then       curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-centos-7/Packages/k/kong-$KONG_VERSION.el7.amd64.rpm -o /tmp/kong.rpm       && echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -;     fi;     yum install -y -q unzip shadow-utils git     && yum clean all -q     && rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki     && yum install -y /tmp/kong.rpm     && yum clean all     && rm /tmp/kong.rpm     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 05 Oct 2021 17:43:41 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 05 Oct 2021 17:43:41 GMT
USER kong
# Tue, 05 Oct 2021 17:43:41 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 Oct 2021 17:43:42 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 05 Oct 2021 17:43:42 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 Oct 2021 17:43:42 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 05 Oct 2021 17:43:42 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:a1d0c75327776413fa0db9ed3adcdbadedc95a662eb1d360dad82bb913f8a1d1`  
		Last Modified: Wed, 15 Sep 2021 18:21:25 GMT  
		Size: 83.5 MB (83518086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fb8a137fa2b84d66997b2207a6880267b365a0a2d08a22a00c4965ecbec7f93`  
		Last Modified: Wed, 15 Sep 2021 23:23:25 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3563bfe40d23f8dbed26358d7c01a711109642f9d164dacf921387cfe9d5ca`  
		Last Modified: Tue, 05 Oct 2021 17:45:39 GMT  
		Size: 77.4 MB (77446253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b3206af33126cd570c9aa494380def6d75f1e4cdde13c3ea55ccedd8641c93`  
		Last Modified: Tue, 05 Oct 2021 17:45:26 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.6-ubuntu`

```console
$ docker pull kong@sha256:a4bc8848afa4e33c231177411d8d3bd809bfaae6bea719a10d0101ecd65b6b63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:2.6-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:da92ee41d6137e994b1f7a064a764606979286ad86e05dc0c3fde3cfd1f34885
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.1 MB (128086633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2970bdd95b6c3fc00f7e232f61a7f1a28d1751918f0032be961404b2bbc9b572`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 07:37:26 GMT
ARG ASSET=ce
# Wed, 02 Feb 2022 07:37:27 GMT
ENV ASSET=ce
# Wed, 02 Feb 2022 07:37:27 GMT
ARG EE_PORTS
# Wed, 02 Feb 2022 07:37:27 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 02 Feb 2022 07:38:53 GMT
ARG KONG_VERSION=2.6.0
# Wed, 02 Feb 2022 07:38:53 GMT
ENV KONG_VERSION=2.6.0
# Wed, 02 Feb 2022 07:39:14 GMT
RUN set -ex     && apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)/pool/all/k/kong/kong_${KONG_VERSION}_$(dpkg --print-architecture).deb -o /tmp/kong.deb       && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 02 Feb 2022 07:39:15 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 02 Feb 2022 07:39:16 GMT
USER kong
# Wed, 02 Feb 2022 07:39:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Feb 2022 07:39:16 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 02 Feb 2022 07:39:16 GMT
STOPSIGNAL SIGQUIT
# Wed, 02 Feb 2022 07:39:16 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 02 Feb 2022 07:39:16 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d35932487d0dcc4bbc7da3fcbb5c567b891759923d10b1daed30b77b8c8c10`  
		Last Modified: Wed, 02 Feb 2022 07:40:24 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f81290c4ad9767b85067bdc76a90d270e0b5bb1bef57a1ad1e4853d9127190a4`  
		Last Modified: Wed, 02 Feb 2022 07:41:00 GMT  
		Size: 74.4 MB (74439700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a290ed6f06a60d17e1a2e44758a212e222780719512217ac8563759abcf73f7a`  
		Last Modified: Wed, 02 Feb 2022 07:40:48 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.6.0`

```console
$ docker pull kong@sha256:134f182c5a20389f4071a71a5946a427cb0d5de6ad382ca66a4156fef441636c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.6.0` - linux; amd64

```console
$ docker pull kong@sha256:95515d0f66dd958be1e30af772ada51bd4812d2a27bcb9124074fd1a2df4402e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 MB (49865802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d51b92ff33146bb0aa7d22bd05cf622124574febe4ee673d92dfed8299b140ce`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 05:49:01 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 13 Nov 2021 05:49:02 GMT
ARG ASSET=ce
# Sat, 13 Nov 2021 05:49:02 GMT
ENV ASSET=ce
# Sat, 13 Nov 2021 05:49:02 GMT
ARG EE_PORTS
# Sat, 13 Nov 2021 05:49:02 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Sat, 13 Nov 2021 05:49:03 GMT
ARG KONG_VERSION=2.6.0
# Sat, 13 Nov 2021 05:49:03 GMT
ENV KONG_VERSION=2.6.0
# Sat, 13 Nov 2021 05:49:03 GMT
ARG KONG_AMD64_SHA=43fb5f27185e274e22b4a36b93b1b7e27afe94b9fd2efbe4ec69b8ed8a9e5902
# Sat, 13 Nov 2021 05:49:03 GMT
ENV KONG_AMD64_SHA=43fb5f27185e274e22b4a36b93b1b7e27afe94b9fd2efbe4ec69b8ed8a9e5902
# Sat, 13 Nov 2021 05:49:03 GMT
ARG KONG_ARM64_SHA=a057eaa6d10ecf49443ec0cac6e1b70a62ee357a777e0e169c780e18fd5c5544
# Sat, 13 Nov 2021 05:49:04 GMT
ENV KONG_ARM64_SHA=a057eaa6d10ecf49443ec0cac6e1b70a62ee357a777e0e169c780e18fd5c5544
# Sat, 13 Nov 2021 05:49:12 GMT
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Sat, 13 Nov 2021 05:49:13 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Sat, 13 Nov 2021 05:49:13 GMT
USER kong
# Sat, 13 Nov 2021 05:49:13 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 13 Nov 2021 05:49:14 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 13 Nov 2021 05:49:14 GMT
STOPSIGNAL SIGQUIT
# Sat, 13 Nov 2021 05:49:14 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Sat, 13 Nov 2021 05:49:15 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e8b2c66462e7a485d21bf9baf11a6e252511cd3612b6fa68b0c1da6972f4cd`  
		Last Modified: Sat, 13 Nov 2021 05:50:42 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c7e18e0a769d4001d507fbe88c18e222f1ef8b290b08b684cbe031f308a212`  
		Last Modified: Sat, 13 Nov 2021 05:50:51 GMT  
		Size: 47.0 MB (47041810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72f9e277edccd9c623819e5913361a38ef18b0d49d8563a765c7cbda0260b9d4`  
		Last Modified: Sat, 13 Nov 2021 05:50:42 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.6.0` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:dd3e38ff91a3e3c07a6df2dc1779ff3b8ecf032549ff6dc28e21e4e06f706775
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49271665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28105dd1de87006bd942029226d1f8bdf5ab9948dfea537b0f76c4b27b184fda`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:11:28 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 13 Nov 2021 06:11:29 GMT
ARG ASSET=ce
# Sat, 13 Nov 2021 06:11:30 GMT
ENV ASSET=ce
# Sat, 13 Nov 2021 06:11:31 GMT
ARG EE_PORTS
# Sat, 13 Nov 2021 06:11:33 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Sat, 13 Nov 2021 06:11:33 GMT
ARG KONG_VERSION=2.6.0
# Sat, 13 Nov 2021 06:11:34 GMT
ENV KONG_VERSION=2.6.0
# Sat, 13 Nov 2021 06:11:35 GMT
ARG KONG_AMD64_SHA=43fb5f27185e274e22b4a36b93b1b7e27afe94b9fd2efbe4ec69b8ed8a9e5902
# Sat, 13 Nov 2021 06:11:36 GMT
ENV KONG_AMD64_SHA=43fb5f27185e274e22b4a36b93b1b7e27afe94b9fd2efbe4ec69b8ed8a9e5902
# Sat, 13 Nov 2021 06:11:37 GMT
ARG KONG_ARM64_SHA=a057eaa6d10ecf49443ec0cac6e1b70a62ee357a777e0e169c780e18fd5c5544
# Sat, 13 Nov 2021 06:11:38 GMT
ENV KONG_ARM64_SHA=a057eaa6d10ecf49443ec0cac6e1b70a62ee357a777e0e169c780e18fd5c5544
# Sat, 13 Nov 2021 06:11:56 GMT
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Sat, 13 Nov 2021 06:11:57 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Sat, 13 Nov 2021 06:11:57 GMT
USER kong
# Sat, 13 Nov 2021 06:11:58 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 13 Nov 2021 06:11:59 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 13 Nov 2021 06:12:00 GMT
STOPSIGNAL SIGQUIT
# Sat, 13 Nov 2021 06:12:01 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Sat, 13 Nov 2021 06:12:02 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53315a86544ab6e48bbf724baae0beec28097187f7ffcda4174c31e3cbb0224e`  
		Last Modified: Sat, 13 Nov 2021 06:16:59 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b212018ea5e6b01778c1aa4de7a912a6e2f2da7a8d9580291a89607a2e1aa4`  
		Last Modified: Sat, 13 Nov 2021 06:17:08 GMT  
		Size: 46.6 MB (46552952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c1c626e2a45c65a7f5d968620e36a052607a53c9ca3cdfc4b056a5dfdc0c3e`  
		Last Modified: Sat, 13 Nov 2021 06:16:59 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.6.0-alpine`

```console
$ docker pull kong@sha256:134f182c5a20389f4071a71a5946a427cb0d5de6ad382ca66a4156fef441636c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.6.0-alpine` - linux; amd64

```console
$ docker pull kong@sha256:95515d0f66dd958be1e30af772ada51bd4812d2a27bcb9124074fd1a2df4402e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 MB (49865802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d51b92ff33146bb0aa7d22bd05cf622124574febe4ee673d92dfed8299b140ce`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 05:49:01 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 13 Nov 2021 05:49:02 GMT
ARG ASSET=ce
# Sat, 13 Nov 2021 05:49:02 GMT
ENV ASSET=ce
# Sat, 13 Nov 2021 05:49:02 GMT
ARG EE_PORTS
# Sat, 13 Nov 2021 05:49:02 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Sat, 13 Nov 2021 05:49:03 GMT
ARG KONG_VERSION=2.6.0
# Sat, 13 Nov 2021 05:49:03 GMT
ENV KONG_VERSION=2.6.0
# Sat, 13 Nov 2021 05:49:03 GMT
ARG KONG_AMD64_SHA=43fb5f27185e274e22b4a36b93b1b7e27afe94b9fd2efbe4ec69b8ed8a9e5902
# Sat, 13 Nov 2021 05:49:03 GMT
ENV KONG_AMD64_SHA=43fb5f27185e274e22b4a36b93b1b7e27afe94b9fd2efbe4ec69b8ed8a9e5902
# Sat, 13 Nov 2021 05:49:03 GMT
ARG KONG_ARM64_SHA=a057eaa6d10ecf49443ec0cac6e1b70a62ee357a777e0e169c780e18fd5c5544
# Sat, 13 Nov 2021 05:49:04 GMT
ENV KONG_ARM64_SHA=a057eaa6d10ecf49443ec0cac6e1b70a62ee357a777e0e169c780e18fd5c5544
# Sat, 13 Nov 2021 05:49:12 GMT
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Sat, 13 Nov 2021 05:49:13 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Sat, 13 Nov 2021 05:49:13 GMT
USER kong
# Sat, 13 Nov 2021 05:49:13 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 13 Nov 2021 05:49:14 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 13 Nov 2021 05:49:14 GMT
STOPSIGNAL SIGQUIT
# Sat, 13 Nov 2021 05:49:14 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Sat, 13 Nov 2021 05:49:15 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e8b2c66462e7a485d21bf9baf11a6e252511cd3612b6fa68b0c1da6972f4cd`  
		Last Modified: Sat, 13 Nov 2021 05:50:42 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c7e18e0a769d4001d507fbe88c18e222f1ef8b290b08b684cbe031f308a212`  
		Last Modified: Sat, 13 Nov 2021 05:50:51 GMT  
		Size: 47.0 MB (47041810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72f9e277edccd9c623819e5913361a38ef18b0d49d8563a765c7cbda0260b9d4`  
		Last Modified: Sat, 13 Nov 2021 05:50:42 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.6.0-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:dd3e38ff91a3e3c07a6df2dc1779ff3b8ecf032549ff6dc28e21e4e06f706775
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49271665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28105dd1de87006bd942029226d1f8bdf5ab9948dfea537b0f76c4b27b184fda`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:11:28 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 13 Nov 2021 06:11:29 GMT
ARG ASSET=ce
# Sat, 13 Nov 2021 06:11:30 GMT
ENV ASSET=ce
# Sat, 13 Nov 2021 06:11:31 GMT
ARG EE_PORTS
# Sat, 13 Nov 2021 06:11:33 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Sat, 13 Nov 2021 06:11:33 GMT
ARG KONG_VERSION=2.6.0
# Sat, 13 Nov 2021 06:11:34 GMT
ENV KONG_VERSION=2.6.0
# Sat, 13 Nov 2021 06:11:35 GMT
ARG KONG_AMD64_SHA=43fb5f27185e274e22b4a36b93b1b7e27afe94b9fd2efbe4ec69b8ed8a9e5902
# Sat, 13 Nov 2021 06:11:36 GMT
ENV KONG_AMD64_SHA=43fb5f27185e274e22b4a36b93b1b7e27afe94b9fd2efbe4ec69b8ed8a9e5902
# Sat, 13 Nov 2021 06:11:37 GMT
ARG KONG_ARM64_SHA=a057eaa6d10ecf49443ec0cac6e1b70a62ee357a777e0e169c780e18fd5c5544
# Sat, 13 Nov 2021 06:11:38 GMT
ENV KONG_ARM64_SHA=a057eaa6d10ecf49443ec0cac6e1b70a62ee357a777e0e169c780e18fd5c5544
# Sat, 13 Nov 2021 06:11:56 GMT
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Sat, 13 Nov 2021 06:11:57 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Sat, 13 Nov 2021 06:11:57 GMT
USER kong
# Sat, 13 Nov 2021 06:11:58 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 13 Nov 2021 06:11:59 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 13 Nov 2021 06:12:00 GMT
STOPSIGNAL SIGQUIT
# Sat, 13 Nov 2021 06:12:01 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Sat, 13 Nov 2021 06:12:02 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53315a86544ab6e48bbf724baae0beec28097187f7ffcda4174c31e3cbb0224e`  
		Last Modified: Sat, 13 Nov 2021 06:16:59 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b212018ea5e6b01778c1aa4de7a912a6e2f2da7a8d9580291a89607a2e1aa4`  
		Last Modified: Sat, 13 Nov 2021 06:17:08 GMT  
		Size: 46.6 MB (46552952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c1c626e2a45c65a7f5d968620e36a052607a53c9ca3cdfc4b056a5dfdc0c3e`  
		Last Modified: Sat, 13 Nov 2021 06:16:59 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.6.0-centos`

```console
$ docker pull kong@sha256:03453c57b918faa98be9faf2ee7b91239c4a4030a5478b750712408b4104b6f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:2.6.0-centos` - linux; amd64

```console
$ docker pull kong@sha256:27efe9259a4da91b92a42030be7bec0d4d3e09b6483ac9473dd4996037c84d3c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.0 MB (160965349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee5d952d7b8eb428c80083082cfea96234e5a263dea8f0a1ef32882fbcec5920`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:04 GMT
ADD file:805cb5e15fb6e0bb0326ca33fd2942e068863ce2a8491bb71522c652f31fb466 in / 
# Wed, 15 Sep 2021 18:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20210915
# Wed, 15 Sep 2021 18:20:05 GMT
CMD ["/bin/bash"]
# Wed, 15 Sep 2021 23:21:23 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 15 Sep 2021 23:21:23 GMT
ARG ASSET=ce
# Wed, 15 Sep 2021 23:21:23 GMT
ENV ASSET=ce
# Wed, 15 Sep 2021 23:21:24 GMT
ARG EE_PORTS
# Wed, 15 Sep 2021 23:21:24 GMT
COPY file:ff02c070e4c89f043b176279a7e41464b5fab8cb98cfcd6332fad2d2741fc41d in /tmp/kong.rpm 
# Tue, 05 Oct 2021 17:43:00 GMT
ARG KONG_VERSION=2.6.0
# Tue, 05 Oct 2021 17:43:00 GMT
ENV KONG_VERSION=2.6.0
# Tue, 05 Oct 2021 17:43:01 GMT
ARG KONG_SHA256=f83a1030b01aa3deb4535394b550228f4804a6fd35a4ea4b11e12dcbcacdadc0
# Tue, 05 Oct 2021 17:43:40 GMT
# ARGS: KONG_SHA256=f83a1030b01aa3deb4535394b550228f4804a6fd35a4ea4b11e12dcbcacdadc0
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then       curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-centos-7/Packages/k/kong-$KONG_VERSION.el7.amd64.rpm -o /tmp/kong.rpm       && echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -;     fi;     yum install -y -q unzip shadow-utils git     && yum clean all -q     && rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki     && yum install -y /tmp/kong.rpm     && yum clean all     && rm /tmp/kong.rpm     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 05 Oct 2021 17:43:41 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 05 Oct 2021 17:43:41 GMT
USER kong
# Tue, 05 Oct 2021 17:43:41 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 Oct 2021 17:43:42 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 05 Oct 2021 17:43:42 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 Oct 2021 17:43:42 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 05 Oct 2021 17:43:42 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:a1d0c75327776413fa0db9ed3adcdbadedc95a662eb1d360dad82bb913f8a1d1`  
		Last Modified: Wed, 15 Sep 2021 18:21:25 GMT  
		Size: 83.5 MB (83518086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fb8a137fa2b84d66997b2207a6880267b365a0a2d08a22a00c4965ecbec7f93`  
		Last Modified: Wed, 15 Sep 2021 23:23:25 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3563bfe40d23f8dbed26358d7c01a711109642f9d164dacf921387cfe9d5ca`  
		Last Modified: Tue, 05 Oct 2021 17:45:39 GMT  
		Size: 77.4 MB (77446253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b3206af33126cd570c9aa494380def6d75f1e4cdde13c3ea55ccedd8641c93`  
		Last Modified: Tue, 05 Oct 2021 17:45:26 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.6.0-ubuntu`

```console
$ docker pull kong@sha256:a4bc8848afa4e33c231177411d8d3bd809bfaae6bea719a10d0101ecd65b6b63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:2.6.0-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:da92ee41d6137e994b1f7a064a764606979286ad86e05dc0c3fde3cfd1f34885
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.1 MB (128086633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2970bdd95b6c3fc00f7e232f61a7f1a28d1751918f0032be961404b2bbc9b572`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 07:37:26 GMT
ARG ASSET=ce
# Wed, 02 Feb 2022 07:37:27 GMT
ENV ASSET=ce
# Wed, 02 Feb 2022 07:37:27 GMT
ARG EE_PORTS
# Wed, 02 Feb 2022 07:37:27 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 02 Feb 2022 07:38:53 GMT
ARG KONG_VERSION=2.6.0
# Wed, 02 Feb 2022 07:38:53 GMT
ENV KONG_VERSION=2.6.0
# Wed, 02 Feb 2022 07:39:14 GMT
RUN set -ex     && apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)/pool/all/k/kong/kong_${KONG_VERSION}_$(dpkg --print-architecture).deb -o /tmp/kong.deb       && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 02 Feb 2022 07:39:15 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 02 Feb 2022 07:39:16 GMT
USER kong
# Wed, 02 Feb 2022 07:39:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Feb 2022 07:39:16 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 02 Feb 2022 07:39:16 GMT
STOPSIGNAL SIGQUIT
# Wed, 02 Feb 2022 07:39:16 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 02 Feb 2022 07:39:16 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d35932487d0dcc4bbc7da3fcbb5c567b891759923d10b1daed30b77b8c8c10`  
		Last Modified: Wed, 02 Feb 2022 07:40:24 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f81290c4ad9767b85067bdc76a90d270e0b5bb1bef57a1ad1e4853d9127190a4`  
		Last Modified: Wed, 02 Feb 2022 07:41:00 GMT  
		Size: 74.4 MB (74439700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a290ed6f06a60d17e1a2e44758a212e222780719512217ac8563759abcf73f7a`  
		Last Modified: Wed, 02 Feb 2022 07:40:48 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.7`

```console
$ docker pull kong@sha256:aa4ba1bcb806cfdd178cec95e1e4e232b0e83fc3bcb33bd1c820e482ace603b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.7` - linux; amd64

```console
$ docker pull kong@sha256:4d3e93207305ace881fe9e95ac27717b6fbdd9e0ec1873c34e94908a4f4c9335
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.8 MB (49804489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b5e76d7c686a63026bf97ed8875443f9dd65ea60b9718701d60f46f261c8d81`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 05:49:01 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 13 Nov 2021 05:49:02 GMT
ARG ASSET=ce
# Sat, 13 Nov 2021 05:49:02 GMT
ENV ASSET=ce
# Sat, 13 Nov 2021 05:49:02 GMT
ARG EE_PORTS
# Sat, 13 Nov 2021 05:49:02 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Fri, 17 Dec 2021 19:24:11 GMT
ARG KONG_VERSION=2.7.0
# Fri, 17 Dec 2021 19:24:11 GMT
ENV KONG_VERSION=2.7.0
# Fri, 17 Dec 2021 19:24:11 GMT
ARG KONG_AMD64_SHA=4caec31903319d1c09542e967e6e4d601bc469b5f28b13f83907a8115a9ff2e5
# Fri, 17 Dec 2021 19:24:12 GMT
ARG KONG_ARM64_SHA=923997ff72b52058f0c91ba09e400ea43c89f9d9e82ccb74f188a44e461a35b7
# Fri, 17 Dec 2021 19:24:20 GMT
# ARGS: KONG_AMD64_SHA=4caec31903319d1c09542e967e6e4d601bc469b5f28b13f83907a8115a9ff2e5 KONG_ARM64_SHA=923997ff72b52058f0c91ba09e400ea43c89f9d9e82ccb74f188a44e461a35b7
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Fri, 17 Dec 2021 19:24:21 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 17 Dec 2021 19:24:21 GMT
USER kong
# Fri, 17 Dec 2021 19:24:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 17 Dec 2021 19:24:21 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 17 Dec 2021 19:24:21 GMT
STOPSIGNAL SIGQUIT
# Fri, 17 Dec 2021 19:24:22 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 17 Dec 2021 19:24:22 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e8b2c66462e7a485d21bf9baf11a6e252511cd3612b6fa68b0c1da6972f4cd`  
		Last Modified: Sat, 13 Nov 2021 05:50:42 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cffbbfa9e3c838b26474ddc1351c354216e7de77da210b380683aef16de7b7c`  
		Last Modified: Fri, 17 Dec 2021 19:26:34 GMT  
		Size: 47.0 MB (46980496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90796a75eb7495312970b99de66ba7619a15ebd227f2bdb5153227f4aabc0999`  
		Last Modified: Fri, 17 Dec 2021 19:26:27 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.7` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:65530f037f12433ea809bae28fc24c1572737cda5126ef4745c6d32e349ac880
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49220211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4725fbe7d43e3205d4b59651b38492c470131a539294fbb5e69c6d91f44b89d0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:11:28 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 13 Nov 2021 06:11:29 GMT
ARG ASSET=ce
# Sat, 13 Nov 2021 06:11:30 GMT
ENV ASSET=ce
# Sat, 13 Nov 2021 06:11:31 GMT
ARG EE_PORTS
# Sat, 13 Nov 2021 06:11:33 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Fri, 17 Dec 2021 19:00:49 GMT
ARG KONG_VERSION=2.7.0
# Fri, 17 Dec 2021 19:00:50 GMT
ENV KONG_VERSION=2.7.0
# Fri, 17 Dec 2021 19:00:51 GMT
ARG KONG_AMD64_SHA=4caec31903319d1c09542e967e6e4d601bc469b5f28b13f83907a8115a9ff2e5
# Fri, 17 Dec 2021 19:00:52 GMT
ARG KONG_ARM64_SHA=923997ff72b52058f0c91ba09e400ea43c89f9d9e82ccb74f188a44e461a35b7
# Fri, 17 Dec 2021 19:01:19 GMT
# ARGS: KONG_AMD64_SHA=4caec31903319d1c09542e967e6e4d601bc469b5f28b13f83907a8115a9ff2e5 KONG_ARM64_SHA=923997ff72b52058f0c91ba09e400ea43c89f9d9e82ccb74f188a44e461a35b7
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Fri, 17 Dec 2021 19:01:20 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 17 Dec 2021 19:01:20 GMT
USER kong
# Fri, 17 Dec 2021 19:01:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 17 Dec 2021 19:01:22 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 17 Dec 2021 19:01:23 GMT
STOPSIGNAL SIGQUIT
# Fri, 17 Dec 2021 19:01:24 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 17 Dec 2021 19:01:25 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53315a86544ab6e48bbf724baae0beec28097187f7ffcda4174c31e3cbb0224e`  
		Last Modified: Sat, 13 Nov 2021 06:16:59 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73af152486c60eac70ed3dddb3b5f38dc02c78b8f47f4dd1b8b85a9c952099cc`  
		Last Modified: Fri, 17 Dec 2021 19:07:19 GMT  
		Size: 46.5 MB (46501501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539bcc814240d49734fbef7216ba4e444af56798b1de7719bde1aa66d7f9e38d`  
		Last Modified: Fri, 17 Dec 2021 19:07:10 GMT  
		Size: 879.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.7-centos`

```console
$ docker pull kong@sha256:2994d66df2c9c1be536b6ca2a5b7835fd1fbf532a4cbca34838d1660f8095375
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:2.7-centos` - linux; amd64

```console
$ docker pull kong@sha256:e64a8c7b55dad59f0428afdbc090e37f4a1b34412617f387e700928b1f24dd2b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.8 MB (167828026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af7f82237e6e981dabf88fb7e5f947940bac0edbca09cce784d467e789f2e5cc`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:04 GMT
ADD file:805cb5e15fb6e0bb0326ca33fd2942e068863ce2a8491bb71522c652f31fb466 in / 
# Wed, 15 Sep 2021 18:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20210915
# Wed, 15 Sep 2021 18:20:05 GMT
CMD ["/bin/bash"]
# Wed, 15 Sep 2021 23:21:23 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 15 Sep 2021 23:21:23 GMT
ARG ASSET=ce
# Wed, 15 Sep 2021 23:21:23 GMT
ENV ASSET=ce
# Wed, 15 Sep 2021 23:21:24 GMT
ARG EE_PORTS
# Wed, 15 Sep 2021 23:21:24 GMT
COPY file:ff02c070e4c89f043b176279a7e41464b5fab8cb98cfcd6332fad2d2741fc41d in /tmp/kong.rpm 
# Fri, 17 Dec 2021 19:25:13 GMT
ARG KONG_VERSION=2.7.0
# Fri, 17 Dec 2021 19:25:13 GMT
ENV KONG_VERSION=2.7.0
# Fri, 17 Dec 2021 19:25:13 GMT
ARG KONG_SHA256=d69aedffbecf697482f7ef3f9ea8087e6487702e1683732205aaed108adb0c3d
# Fri, 17 Dec 2021 19:25:47 GMT
# ARGS: KONG_SHA256=d69aedffbecf697482f7ef3f9ea8087e6487702e1683732205aaed108adb0c3d
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then       curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-centos-8/Packages/k/kong-$KONG_VERSION.el8.amd64.rpm -o /tmp/kong.rpm       && echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -;     else       yum update -y       && yum upgrade -y ;     fi;     yum install -y -q unzip shadow-utils git     && yum clean all -q     && rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki     && yum install -y /tmp/kong.rpm     && yum clean all     && rm /tmp/kong.rpm     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Fri, 17 Dec 2021 19:25:48 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 17 Dec 2021 19:25:49 GMT
USER kong
# Fri, 17 Dec 2021 19:25:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 17 Dec 2021 19:25:49 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 17 Dec 2021 19:25:49 GMT
STOPSIGNAL SIGQUIT
# Fri, 17 Dec 2021 19:25:49 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 17 Dec 2021 19:25:49 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:a1d0c75327776413fa0db9ed3adcdbadedc95a662eb1d360dad82bb913f8a1d1`  
		Last Modified: Wed, 15 Sep 2021 18:21:25 GMT  
		Size: 83.5 MB (83518086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fb8a137fa2b84d66997b2207a6880267b365a0a2d08a22a00c4965ecbec7f93`  
		Last Modified: Wed, 15 Sep 2021 23:23:25 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e996b8fb0de9267b17e982ed3ce78d349259cae8470c908bb640e92ddec100a1`  
		Last Modified: Fri, 17 Dec 2021 19:27:28 GMT  
		Size: 84.3 MB (84308930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51848fd42fef75bdf5043f5c7d5f2b813b128048cb57533a1762dc5ce48490d0`  
		Last Modified: Fri, 17 Dec 2021 19:27:16 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.7-ubuntu`

```console
$ docker pull kong@sha256:2beb92e999485c19ae37aab16ed92d9ff18ce3b59c8845c6863fe1856a057f7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:2.7-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:c0ae1dc6a1364b17f731e5ae460e9bbce6da4f728b32215aca1beaf466c17330
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (127995385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6405f15bf32e76cb7c66422c22ddc684deb2f7086d37d218542df4e99fa4f9da`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 07:37:26 GMT
ARG ASSET=ce
# Wed, 02 Feb 2022 07:37:27 GMT
ENV ASSET=ce
# Wed, 02 Feb 2022 07:37:27 GMT
ARG EE_PORTS
# Wed, 02 Feb 2022 07:37:27 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 02 Feb 2022 07:37:27 GMT
ARG KONG_VERSION=2.7.0
# Wed, 02 Feb 2022 07:37:28 GMT
ENV KONG_VERSION=2.7.0
# Wed, 02 Feb 2022 07:37:28 GMT
ARG KONG_SHA256=6c0d6091f40b2b870b75fd2429b5c1be025e6b0893b5d1f70a0698e77fe027c2
# Wed, 02 Feb 2022 07:38:39 GMT
# ARGS: KONG_SHA256=6c0d6091f40b2b870b75fd2429b5c1be025e6b0893b5d1f70a0698e77fe027c2
RUN set -ex     && apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)/pool/all/k/kong/kong_${KONG_VERSION}_amd64.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 02 Feb 2022 07:38:40 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 02 Feb 2022 07:38:40 GMT
USER kong
# Wed, 02 Feb 2022 07:38:40 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Feb 2022 07:38:41 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 02 Feb 2022 07:38:41 GMT
STOPSIGNAL SIGQUIT
# Wed, 02 Feb 2022 07:38:41 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 02 Feb 2022 07:38:41 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d35932487d0dcc4bbc7da3fcbb5c567b891759923d10b1daed30b77b8c8c10`  
		Last Modified: Wed, 02 Feb 2022 07:40:24 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145fb8793413e96ebe9b80fc283f1d27b04574f1db21bd5d78708baa43e6a5c7`  
		Last Modified: Wed, 02 Feb 2022 07:40:34 GMT  
		Size: 74.3 MB (74348451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a23060917a28e29ede5c56084d74197a1ac2cebcd3e29d82840fe9ead82f95`  
		Last Modified: Wed, 02 Feb 2022 07:40:22 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.7.0`

```console
$ docker pull kong@sha256:aa4ba1bcb806cfdd178cec95e1e4e232b0e83fc3bcb33bd1c820e482ace603b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.7.0` - linux; amd64

```console
$ docker pull kong@sha256:4d3e93207305ace881fe9e95ac27717b6fbdd9e0ec1873c34e94908a4f4c9335
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.8 MB (49804489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b5e76d7c686a63026bf97ed8875443f9dd65ea60b9718701d60f46f261c8d81`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 05:49:01 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 13 Nov 2021 05:49:02 GMT
ARG ASSET=ce
# Sat, 13 Nov 2021 05:49:02 GMT
ENV ASSET=ce
# Sat, 13 Nov 2021 05:49:02 GMT
ARG EE_PORTS
# Sat, 13 Nov 2021 05:49:02 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Fri, 17 Dec 2021 19:24:11 GMT
ARG KONG_VERSION=2.7.0
# Fri, 17 Dec 2021 19:24:11 GMT
ENV KONG_VERSION=2.7.0
# Fri, 17 Dec 2021 19:24:11 GMT
ARG KONG_AMD64_SHA=4caec31903319d1c09542e967e6e4d601bc469b5f28b13f83907a8115a9ff2e5
# Fri, 17 Dec 2021 19:24:12 GMT
ARG KONG_ARM64_SHA=923997ff72b52058f0c91ba09e400ea43c89f9d9e82ccb74f188a44e461a35b7
# Fri, 17 Dec 2021 19:24:20 GMT
# ARGS: KONG_AMD64_SHA=4caec31903319d1c09542e967e6e4d601bc469b5f28b13f83907a8115a9ff2e5 KONG_ARM64_SHA=923997ff72b52058f0c91ba09e400ea43c89f9d9e82ccb74f188a44e461a35b7
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Fri, 17 Dec 2021 19:24:21 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 17 Dec 2021 19:24:21 GMT
USER kong
# Fri, 17 Dec 2021 19:24:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 17 Dec 2021 19:24:21 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 17 Dec 2021 19:24:21 GMT
STOPSIGNAL SIGQUIT
# Fri, 17 Dec 2021 19:24:22 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 17 Dec 2021 19:24:22 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e8b2c66462e7a485d21bf9baf11a6e252511cd3612b6fa68b0c1da6972f4cd`  
		Last Modified: Sat, 13 Nov 2021 05:50:42 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cffbbfa9e3c838b26474ddc1351c354216e7de77da210b380683aef16de7b7c`  
		Last Modified: Fri, 17 Dec 2021 19:26:34 GMT  
		Size: 47.0 MB (46980496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90796a75eb7495312970b99de66ba7619a15ebd227f2bdb5153227f4aabc0999`  
		Last Modified: Fri, 17 Dec 2021 19:26:27 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.7.0` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:65530f037f12433ea809bae28fc24c1572737cda5126ef4745c6d32e349ac880
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49220211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4725fbe7d43e3205d4b59651b38492c470131a539294fbb5e69c6d91f44b89d0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:11:28 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 13 Nov 2021 06:11:29 GMT
ARG ASSET=ce
# Sat, 13 Nov 2021 06:11:30 GMT
ENV ASSET=ce
# Sat, 13 Nov 2021 06:11:31 GMT
ARG EE_PORTS
# Sat, 13 Nov 2021 06:11:33 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Fri, 17 Dec 2021 19:00:49 GMT
ARG KONG_VERSION=2.7.0
# Fri, 17 Dec 2021 19:00:50 GMT
ENV KONG_VERSION=2.7.0
# Fri, 17 Dec 2021 19:00:51 GMT
ARG KONG_AMD64_SHA=4caec31903319d1c09542e967e6e4d601bc469b5f28b13f83907a8115a9ff2e5
# Fri, 17 Dec 2021 19:00:52 GMT
ARG KONG_ARM64_SHA=923997ff72b52058f0c91ba09e400ea43c89f9d9e82ccb74f188a44e461a35b7
# Fri, 17 Dec 2021 19:01:19 GMT
# ARGS: KONG_AMD64_SHA=4caec31903319d1c09542e967e6e4d601bc469b5f28b13f83907a8115a9ff2e5 KONG_ARM64_SHA=923997ff72b52058f0c91ba09e400ea43c89f9d9e82ccb74f188a44e461a35b7
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Fri, 17 Dec 2021 19:01:20 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 17 Dec 2021 19:01:20 GMT
USER kong
# Fri, 17 Dec 2021 19:01:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 17 Dec 2021 19:01:22 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 17 Dec 2021 19:01:23 GMT
STOPSIGNAL SIGQUIT
# Fri, 17 Dec 2021 19:01:24 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 17 Dec 2021 19:01:25 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53315a86544ab6e48bbf724baae0beec28097187f7ffcda4174c31e3cbb0224e`  
		Last Modified: Sat, 13 Nov 2021 06:16:59 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73af152486c60eac70ed3dddb3b5f38dc02c78b8f47f4dd1b8b85a9c952099cc`  
		Last Modified: Fri, 17 Dec 2021 19:07:19 GMT  
		Size: 46.5 MB (46501501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539bcc814240d49734fbef7216ba4e444af56798b1de7719bde1aa66d7f9e38d`  
		Last Modified: Fri, 17 Dec 2021 19:07:10 GMT  
		Size: 879.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.7.0-alpine`

```console
$ docker pull kong@sha256:aa4ba1bcb806cfdd178cec95e1e4e232b0e83fc3bcb33bd1c820e482ace603b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.7.0-alpine` - linux; amd64

```console
$ docker pull kong@sha256:4d3e93207305ace881fe9e95ac27717b6fbdd9e0ec1873c34e94908a4f4c9335
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.8 MB (49804489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b5e76d7c686a63026bf97ed8875443f9dd65ea60b9718701d60f46f261c8d81`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 05:49:01 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 13 Nov 2021 05:49:02 GMT
ARG ASSET=ce
# Sat, 13 Nov 2021 05:49:02 GMT
ENV ASSET=ce
# Sat, 13 Nov 2021 05:49:02 GMT
ARG EE_PORTS
# Sat, 13 Nov 2021 05:49:02 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Fri, 17 Dec 2021 19:24:11 GMT
ARG KONG_VERSION=2.7.0
# Fri, 17 Dec 2021 19:24:11 GMT
ENV KONG_VERSION=2.7.0
# Fri, 17 Dec 2021 19:24:11 GMT
ARG KONG_AMD64_SHA=4caec31903319d1c09542e967e6e4d601bc469b5f28b13f83907a8115a9ff2e5
# Fri, 17 Dec 2021 19:24:12 GMT
ARG KONG_ARM64_SHA=923997ff72b52058f0c91ba09e400ea43c89f9d9e82ccb74f188a44e461a35b7
# Fri, 17 Dec 2021 19:24:20 GMT
# ARGS: KONG_AMD64_SHA=4caec31903319d1c09542e967e6e4d601bc469b5f28b13f83907a8115a9ff2e5 KONG_ARM64_SHA=923997ff72b52058f0c91ba09e400ea43c89f9d9e82ccb74f188a44e461a35b7
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Fri, 17 Dec 2021 19:24:21 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 17 Dec 2021 19:24:21 GMT
USER kong
# Fri, 17 Dec 2021 19:24:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 17 Dec 2021 19:24:21 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 17 Dec 2021 19:24:21 GMT
STOPSIGNAL SIGQUIT
# Fri, 17 Dec 2021 19:24:22 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 17 Dec 2021 19:24:22 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e8b2c66462e7a485d21bf9baf11a6e252511cd3612b6fa68b0c1da6972f4cd`  
		Last Modified: Sat, 13 Nov 2021 05:50:42 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cffbbfa9e3c838b26474ddc1351c354216e7de77da210b380683aef16de7b7c`  
		Last Modified: Fri, 17 Dec 2021 19:26:34 GMT  
		Size: 47.0 MB (46980496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90796a75eb7495312970b99de66ba7619a15ebd227f2bdb5153227f4aabc0999`  
		Last Modified: Fri, 17 Dec 2021 19:26:27 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.7.0-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:65530f037f12433ea809bae28fc24c1572737cda5126ef4745c6d32e349ac880
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49220211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4725fbe7d43e3205d4b59651b38492c470131a539294fbb5e69c6d91f44b89d0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:11:28 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 13 Nov 2021 06:11:29 GMT
ARG ASSET=ce
# Sat, 13 Nov 2021 06:11:30 GMT
ENV ASSET=ce
# Sat, 13 Nov 2021 06:11:31 GMT
ARG EE_PORTS
# Sat, 13 Nov 2021 06:11:33 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Fri, 17 Dec 2021 19:00:49 GMT
ARG KONG_VERSION=2.7.0
# Fri, 17 Dec 2021 19:00:50 GMT
ENV KONG_VERSION=2.7.0
# Fri, 17 Dec 2021 19:00:51 GMT
ARG KONG_AMD64_SHA=4caec31903319d1c09542e967e6e4d601bc469b5f28b13f83907a8115a9ff2e5
# Fri, 17 Dec 2021 19:00:52 GMT
ARG KONG_ARM64_SHA=923997ff72b52058f0c91ba09e400ea43c89f9d9e82ccb74f188a44e461a35b7
# Fri, 17 Dec 2021 19:01:19 GMT
# ARGS: KONG_AMD64_SHA=4caec31903319d1c09542e967e6e4d601bc469b5f28b13f83907a8115a9ff2e5 KONG_ARM64_SHA=923997ff72b52058f0c91ba09e400ea43c89f9d9e82ccb74f188a44e461a35b7
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Fri, 17 Dec 2021 19:01:20 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 17 Dec 2021 19:01:20 GMT
USER kong
# Fri, 17 Dec 2021 19:01:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 17 Dec 2021 19:01:22 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 17 Dec 2021 19:01:23 GMT
STOPSIGNAL SIGQUIT
# Fri, 17 Dec 2021 19:01:24 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 17 Dec 2021 19:01:25 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53315a86544ab6e48bbf724baae0beec28097187f7ffcda4174c31e3cbb0224e`  
		Last Modified: Sat, 13 Nov 2021 06:16:59 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73af152486c60eac70ed3dddb3b5f38dc02c78b8f47f4dd1b8b85a9c952099cc`  
		Last Modified: Fri, 17 Dec 2021 19:07:19 GMT  
		Size: 46.5 MB (46501501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539bcc814240d49734fbef7216ba4e444af56798b1de7719bde1aa66d7f9e38d`  
		Last Modified: Fri, 17 Dec 2021 19:07:10 GMT  
		Size: 879.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.7.0-centos`

```console
$ docker pull kong@sha256:2994d66df2c9c1be536b6ca2a5b7835fd1fbf532a4cbca34838d1660f8095375
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:2.7.0-centos` - linux; amd64

```console
$ docker pull kong@sha256:e64a8c7b55dad59f0428afdbc090e37f4a1b34412617f387e700928b1f24dd2b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.8 MB (167828026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af7f82237e6e981dabf88fb7e5f947940bac0edbca09cce784d467e789f2e5cc`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:04 GMT
ADD file:805cb5e15fb6e0bb0326ca33fd2942e068863ce2a8491bb71522c652f31fb466 in / 
# Wed, 15 Sep 2021 18:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20210915
# Wed, 15 Sep 2021 18:20:05 GMT
CMD ["/bin/bash"]
# Wed, 15 Sep 2021 23:21:23 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 15 Sep 2021 23:21:23 GMT
ARG ASSET=ce
# Wed, 15 Sep 2021 23:21:23 GMT
ENV ASSET=ce
# Wed, 15 Sep 2021 23:21:24 GMT
ARG EE_PORTS
# Wed, 15 Sep 2021 23:21:24 GMT
COPY file:ff02c070e4c89f043b176279a7e41464b5fab8cb98cfcd6332fad2d2741fc41d in /tmp/kong.rpm 
# Fri, 17 Dec 2021 19:25:13 GMT
ARG KONG_VERSION=2.7.0
# Fri, 17 Dec 2021 19:25:13 GMT
ENV KONG_VERSION=2.7.0
# Fri, 17 Dec 2021 19:25:13 GMT
ARG KONG_SHA256=d69aedffbecf697482f7ef3f9ea8087e6487702e1683732205aaed108adb0c3d
# Fri, 17 Dec 2021 19:25:47 GMT
# ARGS: KONG_SHA256=d69aedffbecf697482f7ef3f9ea8087e6487702e1683732205aaed108adb0c3d
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then       curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-centos-8/Packages/k/kong-$KONG_VERSION.el8.amd64.rpm -o /tmp/kong.rpm       && echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -;     else       yum update -y       && yum upgrade -y ;     fi;     yum install -y -q unzip shadow-utils git     && yum clean all -q     && rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki     && yum install -y /tmp/kong.rpm     && yum clean all     && rm /tmp/kong.rpm     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Fri, 17 Dec 2021 19:25:48 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 17 Dec 2021 19:25:49 GMT
USER kong
# Fri, 17 Dec 2021 19:25:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 17 Dec 2021 19:25:49 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 17 Dec 2021 19:25:49 GMT
STOPSIGNAL SIGQUIT
# Fri, 17 Dec 2021 19:25:49 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 17 Dec 2021 19:25:49 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:a1d0c75327776413fa0db9ed3adcdbadedc95a662eb1d360dad82bb913f8a1d1`  
		Last Modified: Wed, 15 Sep 2021 18:21:25 GMT  
		Size: 83.5 MB (83518086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fb8a137fa2b84d66997b2207a6880267b365a0a2d08a22a00c4965ecbec7f93`  
		Last Modified: Wed, 15 Sep 2021 23:23:25 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e996b8fb0de9267b17e982ed3ce78d349259cae8470c908bb640e92ddec100a1`  
		Last Modified: Fri, 17 Dec 2021 19:27:28 GMT  
		Size: 84.3 MB (84308930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51848fd42fef75bdf5043f5c7d5f2b813b128048cb57533a1762dc5ce48490d0`  
		Last Modified: Fri, 17 Dec 2021 19:27:16 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.7.0-ubuntu`

```console
$ docker pull kong@sha256:2beb92e999485c19ae37aab16ed92d9ff18ce3b59c8845c6863fe1856a057f7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:2.7.0-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:c0ae1dc6a1364b17f731e5ae460e9bbce6da4f728b32215aca1beaf466c17330
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (127995385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6405f15bf32e76cb7c66422c22ddc684deb2f7086d37d218542df4e99fa4f9da`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 07:37:26 GMT
ARG ASSET=ce
# Wed, 02 Feb 2022 07:37:27 GMT
ENV ASSET=ce
# Wed, 02 Feb 2022 07:37:27 GMT
ARG EE_PORTS
# Wed, 02 Feb 2022 07:37:27 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 02 Feb 2022 07:37:27 GMT
ARG KONG_VERSION=2.7.0
# Wed, 02 Feb 2022 07:37:28 GMT
ENV KONG_VERSION=2.7.0
# Wed, 02 Feb 2022 07:37:28 GMT
ARG KONG_SHA256=6c0d6091f40b2b870b75fd2429b5c1be025e6b0893b5d1f70a0698e77fe027c2
# Wed, 02 Feb 2022 07:38:39 GMT
# ARGS: KONG_SHA256=6c0d6091f40b2b870b75fd2429b5c1be025e6b0893b5d1f70a0698e77fe027c2
RUN set -ex     && apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)/pool/all/k/kong/kong_${KONG_VERSION}_amd64.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 02 Feb 2022 07:38:40 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 02 Feb 2022 07:38:40 GMT
USER kong
# Wed, 02 Feb 2022 07:38:40 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Feb 2022 07:38:41 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 02 Feb 2022 07:38:41 GMT
STOPSIGNAL SIGQUIT
# Wed, 02 Feb 2022 07:38:41 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 02 Feb 2022 07:38:41 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d35932487d0dcc4bbc7da3fcbb5c567b891759923d10b1daed30b77b8c8c10`  
		Last Modified: Wed, 02 Feb 2022 07:40:24 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145fb8793413e96ebe9b80fc283f1d27b04574f1db21bd5d78708baa43e6a5c7`  
		Last Modified: Wed, 02 Feb 2022 07:40:34 GMT  
		Size: 74.3 MB (74348451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a23060917a28e29ede5c56084d74197a1ac2cebcd3e29d82840fe9ead82f95`  
		Last Modified: Wed, 02 Feb 2022 07:40:22 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:alpine`

```console
$ docker pull kong@sha256:aa4ba1bcb806cfdd178cec95e1e4e232b0e83fc3bcb33bd1c820e482ace603b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:alpine` - linux; amd64

```console
$ docker pull kong@sha256:4d3e93207305ace881fe9e95ac27717b6fbdd9e0ec1873c34e94908a4f4c9335
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.8 MB (49804489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b5e76d7c686a63026bf97ed8875443f9dd65ea60b9718701d60f46f261c8d81`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 05:49:01 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 13 Nov 2021 05:49:02 GMT
ARG ASSET=ce
# Sat, 13 Nov 2021 05:49:02 GMT
ENV ASSET=ce
# Sat, 13 Nov 2021 05:49:02 GMT
ARG EE_PORTS
# Sat, 13 Nov 2021 05:49:02 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Fri, 17 Dec 2021 19:24:11 GMT
ARG KONG_VERSION=2.7.0
# Fri, 17 Dec 2021 19:24:11 GMT
ENV KONG_VERSION=2.7.0
# Fri, 17 Dec 2021 19:24:11 GMT
ARG KONG_AMD64_SHA=4caec31903319d1c09542e967e6e4d601bc469b5f28b13f83907a8115a9ff2e5
# Fri, 17 Dec 2021 19:24:12 GMT
ARG KONG_ARM64_SHA=923997ff72b52058f0c91ba09e400ea43c89f9d9e82ccb74f188a44e461a35b7
# Fri, 17 Dec 2021 19:24:20 GMT
# ARGS: KONG_AMD64_SHA=4caec31903319d1c09542e967e6e4d601bc469b5f28b13f83907a8115a9ff2e5 KONG_ARM64_SHA=923997ff72b52058f0c91ba09e400ea43c89f9d9e82ccb74f188a44e461a35b7
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Fri, 17 Dec 2021 19:24:21 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 17 Dec 2021 19:24:21 GMT
USER kong
# Fri, 17 Dec 2021 19:24:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 17 Dec 2021 19:24:21 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 17 Dec 2021 19:24:21 GMT
STOPSIGNAL SIGQUIT
# Fri, 17 Dec 2021 19:24:22 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 17 Dec 2021 19:24:22 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e8b2c66462e7a485d21bf9baf11a6e252511cd3612b6fa68b0c1da6972f4cd`  
		Last Modified: Sat, 13 Nov 2021 05:50:42 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cffbbfa9e3c838b26474ddc1351c354216e7de77da210b380683aef16de7b7c`  
		Last Modified: Fri, 17 Dec 2021 19:26:34 GMT  
		Size: 47.0 MB (46980496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90796a75eb7495312970b99de66ba7619a15ebd227f2bdb5153227f4aabc0999`  
		Last Modified: Fri, 17 Dec 2021 19:26:27 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:65530f037f12433ea809bae28fc24c1572737cda5126ef4745c6d32e349ac880
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49220211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4725fbe7d43e3205d4b59651b38492c470131a539294fbb5e69c6d91f44b89d0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:11:28 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 13 Nov 2021 06:11:29 GMT
ARG ASSET=ce
# Sat, 13 Nov 2021 06:11:30 GMT
ENV ASSET=ce
# Sat, 13 Nov 2021 06:11:31 GMT
ARG EE_PORTS
# Sat, 13 Nov 2021 06:11:33 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Fri, 17 Dec 2021 19:00:49 GMT
ARG KONG_VERSION=2.7.0
# Fri, 17 Dec 2021 19:00:50 GMT
ENV KONG_VERSION=2.7.0
# Fri, 17 Dec 2021 19:00:51 GMT
ARG KONG_AMD64_SHA=4caec31903319d1c09542e967e6e4d601bc469b5f28b13f83907a8115a9ff2e5
# Fri, 17 Dec 2021 19:00:52 GMT
ARG KONG_ARM64_SHA=923997ff72b52058f0c91ba09e400ea43c89f9d9e82ccb74f188a44e461a35b7
# Fri, 17 Dec 2021 19:01:19 GMT
# ARGS: KONG_AMD64_SHA=4caec31903319d1c09542e967e6e4d601bc469b5f28b13f83907a8115a9ff2e5 KONG_ARM64_SHA=923997ff72b52058f0c91ba09e400ea43c89f9d9e82ccb74f188a44e461a35b7
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Fri, 17 Dec 2021 19:01:20 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 17 Dec 2021 19:01:20 GMT
USER kong
# Fri, 17 Dec 2021 19:01:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 17 Dec 2021 19:01:22 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 17 Dec 2021 19:01:23 GMT
STOPSIGNAL SIGQUIT
# Fri, 17 Dec 2021 19:01:24 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 17 Dec 2021 19:01:25 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53315a86544ab6e48bbf724baae0beec28097187f7ffcda4174c31e3cbb0224e`  
		Last Modified: Sat, 13 Nov 2021 06:16:59 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73af152486c60eac70ed3dddb3b5f38dc02c78b8f47f4dd1b8b85a9c952099cc`  
		Last Modified: Fri, 17 Dec 2021 19:07:19 GMT  
		Size: 46.5 MB (46501501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539bcc814240d49734fbef7216ba4e444af56798b1de7719bde1aa66d7f9e38d`  
		Last Modified: Fri, 17 Dec 2021 19:07:10 GMT  
		Size: 879.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:centos`

```console
$ docker pull kong@sha256:2994d66df2c9c1be536b6ca2a5b7835fd1fbf532a4cbca34838d1660f8095375
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:centos` - linux; amd64

```console
$ docker pull kong@sha256:e64a8c7b55dad59f0428afdbc090e37f4a1b34412617f387e700928b1f24dd2b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.8 MB (167828026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af7f82237e6e981dabf88fb7e5f947940bac0edbca09cce784d467e789f2e5cc`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 15 Sep 2021 18:20:04 GMT
ADD file:805cb5e15fb6e0bb0326ca33fd2942e068863ce2a8491bb71522c652f31fb466 in / 
# Wed, 15 Sep 2021 18:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20210915
# Wed, 15 Sep 2021 18:20:05 GMT
CMD ["/bin/bash"]
# Wed, 15 Sep 2021 23:21:23 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 15 Sep 2021 23:21:23 GMT
ARG ASSET=ce
# Wed, 15 Sep 2021 23:21:23 GMT
ENV ASSET=ce
# Wed, 15 Sep 2021 23:21:24 GMT
ARG EE_PORTS
# Wed, 15 Sep 2021 23:21:24 GMT
COPY file:ff02c070e4c89f043b176279a7e41464b5fab8cb98cfcd6332fad2d2741fc41d in /tmp/kong.rpm 
# Fri, 17 Dec 2021 19:25:13 GMT
ARG KONG_VERSION=2.7.0
# Fri, 17 Dec 2021 19:25:13 GMT
ENV KONG_VERSION=2.7.0
# Fri, 17 Dec 2021 19:25:13 GMT
ARG KONG_SHA256=d69aedffbecf697482f7ef3f9ea8087e6487702e1683732205aaed108adb0c3d
# Fri, 17 Dec 2021 19:25:47 GMT
# ARGS: KONG_SHA256=d69aedffbecf697482f7ef3f9ea8087e6487702e1683732205aaed108adb0c3d
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then       curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-centos-8/Packages/k/kong-$KONG_VERSION.el8.amd64.rpm -o /tmp/kong.rpm       && echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -;     else       yum update -y       && yum upgrade -y ;     fi;     yum install -y -q unzip shadow-utils git     && yum clean all -q     && rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki     && yum install -y /tmp/kong.rpm     && yum clean all     && rm /tmp/kong.rpm     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Fri, 17 Dec 2021 19:25:48 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 17 Dec 2021 19:25:49 GMT
USER kong
# Fri, 17 Dec 2021 19:25:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 17 Dec 2021 19:25:49 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 17 Dec 2021 19:25:49 GMT
STOPSIGNAL SIGQUIT
# Fri, 17 Dec 2021 19:25:49 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 17 Dec 2021 19:25:49 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:a1d0c75327776413fa0db9ed3adcdbadedc95a662eb1d360dad82bb913f8a1d1`  
		Last Modified: Wed, 15 Sep 2021 18:21:25 GMT  
		Size: 83.5 MB (83518086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fb8a137fa2b84d66997b2207a6880267b365a0a2d08a22a00c4965ecbec7f93`  
		Last Modified: Wed, 15 Sep 2021 23:23:25 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e996b8fb0de9267b17e982ed3ce78d349259cae8470c908bb640e92ddec100a1`  
		Last Modified: Fri, 17 Dec 2021 19:27:28 GMT  
		Size: 84.3 MB (84308930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51848fd42fef75bdf5043f5c7d5f2b813b128048cb57533a1762dc5ce48490d0`  
		Last Modified: Fri, 17 Dec 2021 19:27:16 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:latest`

```console
$ docker pull kong@sha256:aa4ba1bcb806cfdd178cec95e1e4e232b0e83fc3bcb33bd1c820e482ace603b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:latest` - linux; amd64

```console
$ docker pull kong@sha256:4d3e93207305ace881fe9e95ac27717b6fbdd9e0ec1873c34e94908a4f4c9335
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.8 MB (49804489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b5e76d7c686a63026bf97ed8875443f9dd65ea60b9718701d60f46f261c8d81`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 05:49:01 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 13 Nov 2021 05:49:02 GMT
ARG ASSET=ce
# Sat, 13 Nov 2021 05:49:02 GMT
ENV ASSET=ce
# Sat, 13 Nov 2021 05:49:02 GMT
ARG EE_PORTS
# Sat, 13 Nov 2021 05:49:02 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Fri, 17 Dec 2021 19:24:11 GMT
ARG KONG_VERSION=2.7.0
# Fri, 17 Dec 2021 19:24:11 GMT
ENV KONG_VERSION=2.7.0
# Fri, 17 Dec 2021 19:24:11 GMT
ARG KONG_AMD64_SHA=4caec31903319d1c09542e967e6e4d601bc469b5f28b13f83907a8115a9ff2e5
# Fri, 17 Dec 2021 19:24:12 GMT
ARG KONG_ARM64_SHA=923997ff72b52058f0c91ba09e400ea43c89f9d9e82ccb74f188a44e461a35b7
# Fri, 17 Dec 2021 19:24:20 GMT
# ARGS: KONG_AMD64_SHA=4caec31903319d1c09542e967e6e4d601bc469b5f28b13f83907a8115a9ff2e5 KONG_ARM64_SHA=923997ff72b52058f0c91ba09e400ea43c89f9d9e82ccb74f188a44e461a35b7
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Fri, 17 Dec 2021 19:24:21 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 17 Dec 2021 19:24:21 GMT
USER kong
# Fri, 17 Dec 2021 19:24:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 17 Dec 2021 19:24:21 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 17 Dec 2021 19:24:21 GMT
STOPSIGNAL SIGQUIT
# Fri, 17 Dec 2021 19:24:22 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 17 Dec 2021 19:24:22 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e8b2c66462e7a485d21bf9baf11a6e252511cd3612b6fa68b0c1da6972f4cd`  
		Last Modified: Sat, 13 Nov 2021 05:50:42 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cffbbfa9e3c838b26474ddc1351c354216e7de77da210b380683aef16de7b7c`  
		Last Modified: Fri, 17 Dec 2021 19:26:34 GMT  
		Size: 47.0 MB (46980496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90796a75eb7495312970b99de66ba7619a15ebd227f2bdb5153227f4aabc0999`  
		Last Modified: Fri, 17 Dec 2021 19:26:27 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:latest` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:65530f037f12433ea809bae28fc24c1572737cda5126ef4745c6d32e349ac880
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49220211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4725fbe7d43e3205d4b59651b38492c470131a539294fbb5e69c6d91f44b89d0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:11:28 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 13 Nov 2021 06:11:29 GMT
ARG ASSET=ce
# Sat, 13 Nov 2021 06:11:30 GMT
ENV ASSET=ce
# Sat, 13 Nov 2021 06:11:31 GMT
ARG EE_PORTS
# Sat, 13 Nov 2021 06:11:33 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Fri, 17 Dec 2021 19:00:49 GMT
ARG KONG_VERSION=2.7.0
# Fri, 17 Dec 2021 19:00:50 GMT
ENV KONG_VERSION=2.7.0
# Fri, 17 Dec 2021 19:00:51 GMT
ARG KONG_AMD64_SHA=4caec31903319d1c09542e967e6e4d601bc469b5f28b13f83907a8115a9ff2e5
# Fri, 17 Dec 2021 19:00:52 GMT
ARG KONG_ARM64_SHA=923997ff72b52058f0c91ba09e400ea43c89f9d9e82ccb74f188a44e461a35b7
# Fri, 17 Dec 2021 19:01:19 GMT
# ARGS: KONG_AMD64_SHA=4caec31903319d1c09542e967e6e4d601bc469b5f28b13f83907a8115a9ff2e5 KONG_ARM64_SHA=923997ff72b52058f0c91ba09e400ea43c89f9d9e82ccb74f188a44e461a35b7
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Fri, 17 Dec 2021 19:01:20 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 17 Dec 2021 19:01:20 GMT
USER kong
# Fri, 17 Dec 2021 19:01:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 17 Dec 2021 19:01:22 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 17 Dec 2021 19:01:23 GMT
STOPSIGNAL SIGQUIT
# Fri, 17 Dec 2021 19:01:24 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 17 Dec 2021 19:01:25 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53315a86544ab6e48bbf724baae0beec28097187f7ffcda4174c31e3cbb0224e`  
		Last Modified: Sat, 13 Nov 2021 06:16:59 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73af152486c60eac70ed3dddb3b5f38dc02c78b8f47f4dd1b8b85a9c952099cc`  
		Last Modified: Fri, 17 Dec 2021 19:07:19 GMT  
		Size: 46.5 MB (46501501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539bcc814240d49734fbef7216ba4e444af56798b1de7719bde1aa66d7f9e38d`  
		Last Modified: Fri, 17 Dec 2021 19:07:10 GMT  
		Size: 879.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:ubuntu`

```console
$ docker pull kong@sha256:9c0af2a6cfc9a4e9da9829a0b13364ab8ad7bf7e07265ac361c5b74a57ea314d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:c0ae1dc6a1364b17f731e5ae460e9bbce6da4f728b32215aca1beaf466c17330
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (127995385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6405f15bf32e76cb7c66422c22ddc684deb2f7086d37d218542df4e99fa4f9da`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 07:37:26 GMT
ARG ASSET=ce
# Wed, 02 Feb 2022 07:37:27 GMT
ENV ASSET=ce
# Wed, 02 Feb 2022 07:37:27 GMT
ARG EE_PORTS
# Wed, 02 Feb 2022 07:37:27 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 02 Feb 2022 07:37:27 GMT
ARG KONG_VERSION=2.7.0
# Wed, 02 Feb 2022 07:37:28 GMT
ENV KONG_VERSION=2.7.0
# Wed, 02 Feb 2022 07:37:28 GMT
ARG KONG_SHA256=6c0d6091f40b2b870b75fd2429b5c1be025e6b0893b5d1f70a0698e77fe027c2
# Wed, 02 Feb 2022 07:38:39 GMT
# ARGS: KONG_SHA256=6c0d6091f40b2b870b75fd2429b5c1be025e6b0893b5d1f70a0698e77fe027c2
RUN set -ex     && apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)/pool/all/k/kong/kong_${KONG_VERSION}_amd64.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Wed, 02 Feb 2022 07:38:40 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 02 Feb 2022 07:38:40 GMT
USER kong
# Wed, 02 Feb 2022 07:38:40 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Feb 2022 07:38:41 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 02 Feb 2022 07:38:41 GMT
STOPSIGNAL SIGQUIT
# Wed, 02 Feb 2022 07:38:41 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 02 Feb 2022 07:38:41 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d35932487d0dcc4bbc7da3fcbb5c567b891759923d10b1daed30b77b8c8c10`  
		Last Modified: Wed, 02 Feb 2022 07:40:24 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145fb8793413e96ebe9b80fc283f1d27b04574f1db21bd5d78708baa43e6a5c7`  
		Last Modified: Wed, 02 Feb 2022 07:40:34 GMT  
		Size: 74.3 MB (74348451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a23060917a28e29ede5c56084d74197a1ac2cebcd3e29d82840fe9ead82f95`  
		Last Modified: Wed, 02 Feb 2022 07:40:22 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:7fb163125ba0769471c7adccc2609abcd37c3e58afcfb159ab99aa30f5ba58f2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125879708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8100ea3c312d55c4a34fcf3706f2584737cc61f1662715a6dd709d77d3f79138`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 31 Aug 2021 01:41:19 GMT
ADD file:3c6dc937cb7b4c81b42126f377d23320ec1d0a8ca34d38e7c45871f1d08dac43 in / 
# Tue, 31 Aug 2021 01:41:20 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Tue, 31 Aug 2021 01:41:20 GMT
RUN rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 01:41:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Tue, 31 Aug 2021 01:41:21 GMT
CMD ["/bin/bash"]
# Tue, 31 Aug 2021 03:13:00 GMT
ARG ASSET=ce
# Tue, 31 Aug 2021 03:13:00 GMT
ENV ASSET=ce
# Tue, 31 Aug 2021 03:13:00 GMT
ARG EE_PORTS
# Tue, 31 Aug 2021 03:13:00 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Tue, 31 Aug 2021 03:13:01 GMT
ARG KONG_VERSION=2.5.0
# Tue, 31 Aug 2021 03:13:01 GMT
ENV KONG_VERSION=2.5.0
# Tue, 31 Aug 2021 03:13:24 GMT
RUN set -ex     && apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)/pool/all/k/kong/kong_${KONG_VERSION}_$(dpkg --print-architecture).deb -o /tmp/kong.deb       && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 31 Aug 2021 03:13:25 GMT
COPY file:ae813ec19d3fef1de3793f6717c2aed3a9daa94e583e9e55448084541de3c5ff in /docker-entrypoint.sh 
# Tue, 31 Aug 2021 03:13:25 GMT
USER kong
# Tue, 31 Aug 2021 03:13:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 31 Aug 2021 03:13:25 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 31 Aug 2021 03:13:26 GMT
STOPSIGNAL SIGQUIT
# Tue, 31 Aug 2021 03:13:26 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 31 Aug 2021 03:13:26 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:828b35a09f0b2f3d1dead43aa2468ff5eba6c463423b3fff7ee6d150f6fd1b6b`  
		Last Modified: Thu, 05 Aug 2021 00:25:09 GMT  
		Size: 41.2 MB (41239253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85569e0c17003d9cf46a8b94076418863e0abfc5474bb830403acf246947fea7`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32ca509d28808ab7c61361835292ee8eddecd0c0949d658bde0ab1a77ecbf6e`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 469.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8168af71f81f1ffa234c301e9cc2ee87b560ad8b74ef4100f8ab4a6abf3a8ad3`  
		Last Modified: Tue, 31 Aug 2021 01:43:39 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eee59a359925630cd377c9610b18f7d7797349cdbabeda7b8c8685852a5ff83`  
		Last Modified: Tue, 31 Aug 2021 03:14:48 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbbe71eb414d43ff3fbf75c0de9133ebafceaf672848c6e2c17e4ab47780e97b`  
		Last Modified: Tue, 31 Aug 2021 03:15:00 GMT  
		Size: 59.6 MB (59556314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a45ed64e5c35d56c7aafb050d22218142de8f6d3142eba9294d41638844747`  
		Last Modified: Tue, 31 Aug 2021 03:14:46 GMT  
		Size: 690.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
