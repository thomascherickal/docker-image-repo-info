<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kong`

-	[`kong:2.5`](#kong25)
-	[`kong:2.5-ubuntu`](#kong25-ubuntu)
-	[`kong:2.5.1`](#kong251)
-	[`kong:2.5.1-alpine`](#kong251-alpine)
-	[`kong:2.5.1-ubuntu`](#kong251-ubuntu)
-	[`kong:2.6`](#kong26)
-	[`kong:2.6-ubuntu`](#kong26-ubuntu)
-	[`kong:2.6.0`](#kong260)
-	[`kong:2.6.0-alpine`](#kong260-alpine)
-	[`kong:2.6.0-ubuntu`](#kong260-ubuntu)
-	[`kong:2.7`](#kong27)
-	[`kong:2.7-ubuntu`](#kong27-ubuntu)
-	[`kong:2.7.1`](#kong271)
-	[`kong:2.7.1-alpine`](#kong271-alpine)
-	[`kong:2.7.1-ubuntu`](#kong271-ubuntu)
-	[`kong:2.8`](#kong28)
-	[`kong:2.8-ubuntu`](#kong28-ubuntu)
-	[`kong:2.8.0`](#kong280)
-	[`kong:2.8.0-alpine`](#kong280-alpine)
-	[`kong:2.8.0-ubuntu`](#kong280-ubuntu)
-	[`kong:alpine`](#kongalpine)
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
$ docker pull kong@sha256:96af327e86bdf9f163ba69b3ad3fd2df9c416ac9cf13c0c932db39f48a6cd7cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.7` - linux; amd64

```console
$ docker pull kong@sha256:64702704f1b85bffdc0f159382805cd113dfe341c138c07e3784e1601e4ddfda
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50075195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8431176d93b6a2783635b718ca928b11090d149c224bbc930e70b16ac1b0d5bd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Fri, 04 Feb 2022 20:19:55 GMT
LABEL maintainer=Kong <support@konghq.com>
# Fri, 04 Feb 2022 20:19:55 GMT
ARG ASSET=ce
# Fri, 04 Feb 2022 20:19:55 GMT
ENV ASSET=ce
# Fri, 04 Feb 2022 20:19:55 GMT
ARG EE_PORTS
# Fri, 04 Feb 2022 20:19:55 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Fri, 04 Feb 2022 20:19:55 GMT
ARG KONG_VERSION=2.7.1
# Fri, 04 Feb 2022 20:19:56 GMT
ENV KONG_VERSION=2.7.1
# Fri, 04 Feb 2022 20:19:56 GMT
ARG KONG_AMD64_SHA=7ccd12a15f357dea4d9bea2a5c06c1efe05dcaa0bc8b937f00619e31634715c4
# Fri, 04 Feb 2022 20:19:56 GMT
ARG KONG_ARM64_SHA=00f6c3af15418af07d7429e15762db2355a5f9cdbf278f198c59b5fd34e80abc
# Fri, 04 Feb 2022 20:20:04 GMT
# ARGS: KONG_AMD64_SHA=7ccd12a15f357dea4d9bea2a5c06c1efe05dcaa0bc8b937f00619e31634715c4 KONG_ARM64_SHA=00f6c3af15418af07d7429e15762db2355a5f9cdbf278f198c59b5fd34e80abc
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Fri, 04 Feb 2022 20:20:05 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 04 Feb 2022 20:20:05 GMT
USER kong
# Fri, 04 Feb 2022 20:20:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 04 Feb 2022 20:20:05 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 04 Feb 2022 20:20:06 GMT
STOPSIGNAL SIGQUIT
# Fri, 04 Feb 2022 20:20:06 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 04 Feb 2022 20:20:06 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbc91fb05d0b42d1f1f4b4f99a82dd5445c43c4189aab98fb71228437396e73`  
		Last Modified: Fri, 04 Feb 2022 20:24:49 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c6b74e1d01a5699a36c4042485729e9bf85518b40223fe38397fc6c8837400`  
		Last Modified: Fri, 04 Feb 2022 20:24:57 GMT  
		Size: 47.3 MB (47255773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b84f5d788f2ac167f17d0e21e12bc455b256b8ea0c40cc507e7bfdcaf73d09`  
		Last Modified: Fri, 04 Feb 2022 20:24:49 GMT  
		Size: 879.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.7` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:750e6a4272de6a6cdf995bd2d1129c61b8f0b50d23b50b372a55eb8c91022bb8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49478275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3488a1912608619edd9623b089e502c805c4f9b4d4fb66c40d4ac93fd5cac4e1`
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
# Fri, 04 Feb 2022 20:40:23 GMT
ARG KONG_VERSION=2.7.1
# Fri, 04 Feb 2022 20:40:24 GMT
ENV KONG_VERSION=2.7.1
# Fri, 04 Feb 2022 20:40:25 GMT
ARG KONG_AMD64_SHA=7ccd12a15f357dea4d9bea2a5c06c1efe05dcaa0bc8b937f00619e31634715c4
# Fri, 04 Feb 2022 20:40:26 GMT
ARG KONG_ARM64_SHA=00f6c3af15418af07d7429e15762db2355a5f9cdbf278f198c59b5fd34e80abc
# Fri, 04 Feb 2022 20:40:53 GMT
# ARGS: KONG_AMD64_SHA=7ccd12a15f357dea4d9bea2a5c06c1efe05dcaa0bc8b937f00619e31634715c4 KONG_ARM64_SHA=00f6c3af15418af07d7429e15762db2355a5f9cdbf278f198c59b5fd34e80abc
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Fri, 04 Feb 2022 20:40:55 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 04 Feb 2022 20:40:55 GMT
USER kong
# Fri, 04 Feb 2022 20:40:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 04 Feb 2022 20:40:57 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 04 Feb 2022 20:40:58 GMT
STOPSIGNAL SIGQUIT
# Fri, 04 Feb 2022 20:40:59 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 04 Feb 2022 20:41:00 GMT
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
	-	`sha256:77aa1523c2af572e45166cc1092442469dee6ed9869b66f0f9fc71964b3fee9a`  
		Last Modified: Fri, 04 Feb 2022 20:47:01 GMT  
		Size: 46.8 MB (46761830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348575b5ca4c666e734b84e7713f293475df6df5f4c46261f95555dd2873a1be`  
		Last Modified: Fri, 04 Feb 2022 20:46:52 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.7-ubuntu`

```console
$ docker pull kong@sha256:68f1b94e35ecc3bcda01d49e19cd7e14331b82c3d460228b6abbf47a73d89baf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:2.7-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:dc42868d4cd45050e0e09fdb9e460704000f956955fed5a2ee5c82729e2f1eba
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (127997410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6cf58201aa5f25a7917e4a7da57a3c5997d993f2b2e8f9f051d548ec5ab1f36`
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
# Fri, 04 Feb 2022 20:20:09 GMT
ARG KONG_VERSION=2.7.1
# Fri, 04 Feb 2022 20:20:10 GMT
ENV KONG_VERSION=2.7.1
# Fri, 04 Feb 2022 20:20:10 GMT
ARG KONG_SHA256=feeee661bbe44cf3ca2d4b748291dd3f9153f355fbc13ffeccb6fbc036249a89
# Fri, 04 Feb 2022 20:21:02 GMT
# ARGS: KONG_SHA256=feeee661bbe44cf3ca2d4b748291dd3f9153f355fbc13ffeccb6fbc036249a89
RUN set -ex     && apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_amd64.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 04 Feb 2022 20:21:03 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 04 Feb 2022 20:21:03 GMT
USER kong
# Fri, 04 Feb 2022 20:21:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 04 Feb 2022 20:21:03 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 04 Feb 2022 20:21:04 GMT
STOPSIGNAL SIGQUIT
# Fri, 04 Feb 2022 20:21:04 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 04 Feb 2022 20:21:04 GMT
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
	-	`sha256:98d4135a56578f94e10fdd1215590128a99383ea6104ad50882e07e2764063cc`  
		Last Modified: Fri, 04 Feb 2022 20:25:31 GMT  
		Size: 74.4 MB (74350478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f7e8848ec863e11869e0b3fbb9a0f57aef8c564df825fcc3ce3282c988b890`  
		Last Modified: Fri, 04 Feb 2022 20:25:19 GMT  
		Size: 879.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.7.1`

```console
$ docker pull kong@sha256:96af327e86bdf9f163ba69b3ad3fd2df9c416ac9cf13c0c932db39f48a6cd7cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.7.1` - linux; amd64

```console
$ docker pull kong@sha256:64702704f1b85bffdc0f159382805cd113dfe341c138c07e3784e1601e4ddfda
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50075195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8431176d93b6a2783635b718ca928b11090d149c224bbc930e70b16ac1b0d5bd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Fri, 04 Feb 2022 20:19:55 GMT
LABEL maintainer=Kong <support@konghq.com>
# Fri, 04 Feb 2022 20:19:55 GMT
ARG ASSET=ce
# Fri, 04 Feb 2022 20:19:55 GMT
ENV ASSET=ce
# Fri, 04 Feb 2022 20:19:55 GMT
ARG EE_PORTS
# Fri, 04 Feb 2022 20:19:55 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Fri, 04 Feb 2022 20:19:55 GMT
ARG KONG_VERSION=2.7.1
# Fri, 04 Feb 2022 20:19:56 GMT
ENV KONG_VERSION=2.7.1
# Fri, 04 Feb 2022 20:19:56 GMT
ARG KONG_AMD64_SHA=7ccd12a15f357dea4d9bea2a5c06c1efe05dcaa0bc8b937f00619e31634715c4
# Fri, 04 Feb 2022 20:19:56 GMT
ARG KONG_ARM64_SHA=00f6c3af15418af07d7429e15762db2355a5f9cdbf278f198c59b5fd34e80abc
# Fri, 04 Feb 2022 20:20:04 GMT
# ARGS: KONG_AMD64_SHA=7ccd12a15f357dea4d9bea2a5c06c1efe05dcaa0bc8b937f00619e31634715c4 KONG_ARM64_SHA=00f6c3af15418af07d7429e15762db2355a5f9cdbf278f198c59b5fd34e80abc
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Fri, 04 Feb 2022 20:20:05 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 04 Feb 2022 20:20:05 GMT
USER kong
# Fri, 04 Feb 2022 20:20:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 04 Feb 2022 20:20:05 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 04 Feb 2022 20:20:06 GMT
STOPSIGNAL SIGQUIT
# Fri, 04 Feb 2022 20:20:06 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 04 Feb 2022 20:20:06 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbc91fb05d0b42d1f1f4b4f99a82dd5445c43c4189aab98fb71228437396e73`  
		Last Modified: Fri, 04 Feb 2022 20:24:49 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c6b74e1d01a5699a36c4042485729e9bf85518b40223fe38397fc6c8837400`  
		Last Modified: Fri, 04 Feb 2022 20:24:57 GMT  
		Size: 47.3 MB (47255773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b84f5d788f2ac167f17d0e21e12bc455b256b8ea0c40cc507e7bfdcaf73d09`  
		Last Modified: Fri, 04 Feb 2022 20:24:49 GMT  
		Size: 879.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.7.1` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:750e6a4272de6a6cdf995bd2d1129c61b8f0b50d23b50b372a55eb8c91022bb8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49478275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3488a1912608619edd9623b089e502c805c4f9b4d4fb66c40d4ac93fd5cac4e1`
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
# Fri, 04 Feb 2022 20:40:23 GMT
ARG KONG_VERSION=2.7.1
# Fri, 04 Feb 2022 20:40:24 GMT
ENV KONG_VERSION=2.7.1
# Fri, 04 Feb 2022 20:40:25 GMT
ARG KONG_AMD64_SHA=7ccd12a15f357dea4d9bea2a5c06c1efe05dcaa0bc8b937f00619e31634715c4
# Fri, 04 Feb 2022 20:40:26 GMT
ARG KONG_ARM64_SHA=00f6c3af15418af07d7429e15762db2355a5f9cdbf278f198c59b5fd34e80abc
# Fri, 04 Feb 2022 20:40:53 GMT
# ARGS: KONG_AMD64_SHA=7ccd12a15f357dea4d9bea2a5c06c1efe05dcaa0bc8b937f00619e31634715c4 KONG_ARM64_SHA=00f6c3af15418af07d7429e15762db2355a5f9cdbf278f198c59b5fd34e80abc
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Fri, 04 Feb 2022 20:40:55 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 04 Feb 2022 20:40:55 GMT
USER kong
# Fri, 04 Feb 2022 20:40:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 04 Feb 2022 20:40:57 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 04 Feb 2022 20:40:58 GMT
STOPSIGNAL SIGQUIT
# Fri, 04 Feb 2022 20:40:59 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 04 Feb 2022 20:41:00 GMT
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
	-	`sha256:77aa1523c2af572e45166cc1092442469dee6ed9869b66f0f9fc71964b3fee9a`  
		Last Modified: Fri, 04 Feb 2022 20:47:01 GMT  
		Size: 46.8 MB (46761830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348575b5ca4c666e734b84e7713f293475df6df5f4c46261f95555dd2873a1be`  
		Last Modified: Fri, 04 Feb 2022 20:46:52 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.7.1-alpine`

```console
$ docker pull kong@sha256:96af327e86bdf9f163ba69b3ad3fd2df9c416ac9cf13c0c932db39f48a6cd7cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.7.1-alpine` - linux; amd64

```console
$ docker pull kong@sha256:64702704f1b85bffdc0f159382805cd113dfe341c138c07e3784e1601e4ddfda
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50075195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8431176d93b6a2783635b718ca928b11090d149c224bbc930e70b16ac1b0d5bd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Fri, 04 Feb 2022 20:19:55 GMT
LABEL maintainer=Kong <support@konghq.com>
# Fri, 04 Feb 2022 20:19:55 GMT
ARG ASSET=ce
# Fri, 04 Feb 2022 20:19:55 GMT
ENV ASSET=ce
# Fri, 04 Feb 2022 20:19:55 GMT
ARG EE_PORTS
# Fri, 04 Feb 2022 20:19:55 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Fri, 04 Feb 2022 20:19:55 GMT
ARG KONG_VERSION=2.7.1
# Fri, 04 Feb 2022 20:19:56 GMT
ENV KONG_VERSION=2.7.1
# Fri, 04 Feb 2022 20:19:56 GMT
ARG KONG_AMD64_SHA=7ccd12a15f357dea4d9bea2a5c06c1efe05dcaa0bc8b937f00619e31634715c4
# Fri, 04 Feb 2022 20:19:56 GMT
ARG KONG_ARM64_SHA=00f6c3af15418af07d7429e15762db2355a5f9cdbf278f198c59b5fd34e80abc
# Fri, 04 Feb 2022 20:20:04 GMT
# ARGS: KONG_AMD64_SHA=7ccd12a15f357dea4d9bea2a5c06c1efe05dcaa0bc8b937f00619e31634715c4 KONG_ARM64_SHA=00f6c3af15418af07d7429e15762db2355a5f9cdbf278f198c59b5fd34e80abc
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Fri, 04 Feb 2022 20:20:05 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 04 Feb 2022 20:20:05 GMT
USER kong
# Fri, 04 Feb 2022 20:20:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 04 Feb 2022 20:20:05 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 04 Feb 2022 20:20:06 GMT
STOPSIGNAL SIGQUIT
# Fri, 04 Feb 2022 20:20:06 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 04 Feb 2022 20:20:06 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbc91fb05d0b42d1f1f4b4f99a82dd5445c43c4189aab98fb71228437396e73`  
		Last Modified: Fri, 04 Feb 2022 20:24:49 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c6b74e1d01a5699a36c4042485729e9bf85518b40223fe38397fc6c8837400`  
		Last Modified: Fri, 04 Feb 2022 20:24:57 GMT  
		Size: 47.3 MB (47255773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b84f5d788f2ac167f17d0e21e12bc455b256b8ea0c40cc507e7bfdcaf73d09`  
		Last Modified: Fri, 04 Feb 2022 20:24:49 GMT  
		Size: 879.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.7.1-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:750e6a4272de6a6cdf995bd2d1129c61b8f0b50d23b50b372a55eb8c91022bb8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49478275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3488a1912608619edd9623b089e502c805c4f9b4d4fb66c40d4ac93fd5cac4e1`
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
# Fri, 04 Feb 2022 20:40:23 GMT
ARG KONG_VERSION=2.7.1
# Fri, 04 Feb 2022 20:40:24 GMT
ENV KONG_VERSION=2.7.1
# Fri, 04 Feb 2022 20:40:25 GMT
ARG KONG_AMD64_SHA=7ccd12a15f357dea4d9bea2a5c06c1efe05dcaa0bc8b937f00619e31634715c4
# Fri, 04 Feb 2022 20:40:26 GMT
ARG KONG_ARM64_SHA=00f6c3af15418af07d7429e15762db2355a5f9cdbf278f198c59b5fd34e80abc
# Fri, 04 Feb 2022 20:40:53 GMT
# ARGS: KONG_AMD64_SHA=7ccd12a15f357dea4d9bea2a5c06c1efe05dcaa0bc8b937f00619e31634715c4 KONG_ARM64_SHA=00f6c3af15418af07d7429e15762db2355a5f9cdbf278f198c59b5fd34e80abc
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Fri, 04 Feb 2022 20:40:55 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 04 Feb 2022 20:40:55 GMT
USER kong
# Fri, 04 Feb 2022 20:40:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 04 Feb 2022 20:40:57 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 04 Feb 2022 20:40:58 GMT
STOPSIGNAL SIGQUIT
# Fri, 04 Feb 2022 20:40:59 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 04 Feb 2022 20:41:00 GMT
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
	-	`sha256:77aa1523c2af572e45166cc1092442469dee6ed9869b66f0f9fc71964b3fee9a`  
		Last Modified: Fri, 04 Feb 2022 20:47:01 GMT  
		Size: 46.8 MB (46761830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348575b5ca4c666e734b84e7713f293475df6df5f4c46261f95555dd2873a1be`  
		Last Modified: Fri, 04 Feb 2022 20:46:52 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.7.1-ubuntu`

```console
$ docker pull kong@sha256:68f1b94e35ecc3bcda01d49e19cd7e14331b82c3d460228b6abbf47a73d89baf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:2.7.1-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:dc42868d4cd45050e0e09fdb9e460704000f956955fed5a2ee5c82729e2f1eba
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (127997410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6cf58201aa5f25a7917e4a7da57a3c5997d993f2b2e8f9f051d548ec5ab1f36`
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
# Fri, 04 Feb 2022 20:20:09 GMT
ARG KONG_VERSION=2.7.1
# Fri, 04 Feb 2022 20:20:10 GMT
ENV KONG_VERSION=2.7.1
# Fri, 04 Feb 2022 20:20:10 GMT
ARG KONG_SHA256=feeee661bbe44cf3ca2d4b748291dd3f9153f355fbc13ffeccb6fbc036249a89
# Fri, 04 Feb 2022 20:21:02 GMT
# ARGS: KONG_SHA256=feeee661bbe44cf3ca2d4b748291dd3f9153f355fbc13ffeccb6fbc036249a89
RUN set -ex     && apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_amd64.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 04 Feb 2022 20:21:03 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 04 Feb 2022 20:21:03 GMT
USER kong
# Fri, 04 Feb 2022 20:21:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 04 Feb 2022 20:21:03 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 04 Feb 2022 20:21:04 GMT
STOPSIGNAL SIGQUIT
# Fri, 04 Feb 2022 20:21:04 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 04 Feb 2022 20:21:04 GMT
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
	-	`sha256:98d4135a56578f94e10fdd1215590128a99383ea6104ad50882e07e2764063cc`  
		Last Modified: Fri, 04 Feb 2022 20:25:31 GMT  
		Size: 74.4 MB (74350478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f7e8848ec863e11869e0b3fbb9a0f57aef8c564df825fcc3ce3282c988b890`  
		Last Modified: Fri, 04 Feb 2022 20:25:19 GMT  
		Size: 879.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.8`

```console
$ docker pull kong@sha256:61f482c7e149f8617d153e06331d6498b361e3db8646269fd63768089a28cc2d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `kong:2.8` - linux; arm64 variant v8

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

## `kong:2.8-ubuntu`

```console
$ docker pull kong@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 0

## `kong:2.8.0`

```console
$ docker pull kong@sha256:61f482c7e149f8617d153e06331d6498b361e3db8646269fd63768089a28cc2d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `kong:2.8.0` - linux; arm64 variant v8

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

## `kong:2.8.0-alpine`

```console
$ docker pull kong@sha256:61f482c7e149f8617d153e06331d6498b361e3db8646269fd63768089a28cc2d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm64 variant v8

### `kong:2.8.0-alpine` - linux; arm64 variant v8

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

## `kong:2.8.0-ubuntu`

```console
$ docker pull kong@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 0

## `kong:alpine`

```console
$ docker pull kong@sha256:13667591684662db75a938a58775faff84ac7c72eb48a41d608ad0f717d188c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:alpine` - linux; amd64

```console
$ docker pull kong@sha256:64702704f1b85bffdc0f159382805cd113dfe341c138c07e3784e1601e4ddfda
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50075195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8431176d93b6a2783635b718ca928b11090d149c224bbc930e70b16ac1b0d5bd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Fri, 04 Feb 2022 20:19:55 GMT
LABEL maintainer=Kong <support@konghq.com>
# Fri, 04 Feb 2022 20:19:55 GMT
ARG ASSET=ce
# Fri, 04 Feb 2022 20:19:55 GMT
ENV ASSET=ce
# Fri, 04 Feb 2022 20:19:55 GMT
ARG EE_PORTS
# Fri, 04 Feb 2022 20:19:55 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Fri, 04 Feb 2022 20:19:55 GMT
ARG KONG_VERSION=2.7.1
# Fri, 04 Feb 2022 20:19:56 GMT
ENV KONG_VERSION=2.7.1
# Fri, 04 Feb 2022 20:19:56 GMT
ARG KONG_AMD64_SHA=7ccd12a15f357dea4d9bea2a5c06c1efe05dcaa0bc8b937f00619e31634715c4
# Fri, 04 Feb 2022 20:19:56 GMT
ARG KONG_ARM64_SHA=00f6c3af15418af07d7429e15762db2355a5f9cdbf278f198c59b5fd34e80abc
# Fri, 04 Feb 2022 20:20:04 GMT
# ARGS: KONG_AMD64_SHA=7ccd12a15f357dea4d9bea2a5c06c1efe05dcaa0bc8b937f00619e31634715c4 KONG_ARM64_SHA=00f6c3af15418af07d7429e15762db2355a5f9cdbf278f198c59b5fd34e80abc
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Fri, 04 Feb 2022 20:20:05 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 04 Feb 2022 20:20:05 GMT
USER kong
# Fri, 04 Feb 2022 20:20:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 04 Feb 2022 20:20:05 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 04 Feb 2022 20:20:06 GMT
STOPSIGNAL SIGQUIT
# Fri, 04 Feb 2022 20:20:06 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 04 Feb 2022 20:20:06 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbc91fb05d0b42d1f1f4b4f99a82dd5445c43c4189aab98fb71228437396e73`  
		Last Modified: Fri, 04 Feb 2022 20:24:49 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c6b74e1d01a5699a36c4042485729e9bf85518b40223fe38397fc6c8837400`  
		Last Modified: Fri, 04 Feb 2022 20:24:57 GMT  
		Size: 47.3 MB (47255773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b84f5d788f2ac167f17d0e21e12bc455b256b8ea0c40cc507e7bfdcaf73d09`  
		Last Modified: Fri, 04 Feb 2022 20:24:49 GMT  
		Size: 879.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:alpine` - linux; arm64 variant v8

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

## `kong:latest`

```console
$ docker pull kong@sha256:13667591684662db75a938a58775faff84ac7c72eb48a41d608ad0f717d188c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:latest` - linux; amd64

```console
$ docker pull kong@sha256:64702704f1b85bffdc0f159382805cd113dfe341c138c07e3784e1601e4ddfda
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50075195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8431176d93b6a2783635b718ca928b11090d149c224bbc930e70b16ac1b0d5bd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Fri, 04 Feb 2022 20:19:55 GMT
LABEL maintainer=Kong <support@konghq.com>
# Fri, 04 Feb 2022 20:19:55 GMT
ARG ASSET=ce
# Fri, 04 Feb 2022 20:19:55 GMT
ENV ASSET=ce
# Fri, 04 Feb 2022 20:19:55 GMT
ARG EE_PORTS
# Fri, 04 Feb 2022 20:19:55 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Fri, 04 Feb 2022 20:19:55 GMT
ARG KONG_VERSION=2.7.1
# Fri, 04 Feb 2022 20:19:56 GMT
ENV KONG_VERSION=2.7.1
# Fri, 04 Feb 2022 20:19:56 GMT
ARG KONG_AMD64_SHA=7ccd12a15f357dea4d9bea2a5c06c1efe05dcaa0bc8b937f00619e31634715c4
# Fri, 04 Feb 2022 20:19:56 GMT
ARG KONG_ARM64_SHA=00f6c3af15418af07d7429e15762db2355a5f9cdbf278f198c59b5fd34e80abc
# Fri, 04 Feb 2022 20:20:04 GMT
# ARGS: KONG_AMD64_SHA=7ccd12a15f357dea4d9bea2a5c06c1efe05dcaa0bc8b937f00619e31634715c4 KONG_ARM64_SHA=00f6c3af15418af07d7429e15762db2355a5f9cdbf278f198c59b5fd34e80abc
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Fri, 04 Feb 2022 20:20:05 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 04 Feb 2022 20:20:05 GMT
USER kong
# Fri, 04 Feb 2022 20:20:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 04 Feb 2022 20:20:05 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 04 Feb 2022 20:20:06 GMT
STOPSIGNAL SIGQUIT
# Fri, 04 Feb 2022 20:20:06 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 04 Feb 2022 20:20:06 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbc91fb05d0b42d1f1f4b4f99a82dd5445c43c4189aab98fb71228437396e73`  
		Last Modified: Fri, 04 Feb 2022 20:24:49 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2c6b74e1d01a5699a36c4042485729e9bf85518b40223fe38397fc6c8837400`  
		Last Modified: Fri, 04 Feb 2022 20:24:57 GMT  
		Size: 47.3 MB (47255773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b84f5d788f2ac167f17d0e21e12bc455b256b8ea0c40cc507e7bfdcaf73d09`  
		Last Modified: Fri, 04 Feb 2022 20:24:49 GMT  
		Size: 879.0 B  
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

## `kong:ubuntu`

```console
$ docker pull kong@sha256:2db93db046eff9283f02757c73953a9996434e07e37e3e90459c8d4e95879d3d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:dc42868d4cd45050e0e09fdb9e460704000f956955fed5a2ee5c82729e2f1eba
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.0 MB (127997410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6cf58201aa5f25a7917e4a7da57a3c5997d993f2b2e8f9f051d548ec5ab1f36`
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
# Fri, 04 Feb 2022 20:20:09 GMT
ARG KONG_VERSION=2.7.1
# Fri, 04 Feb 2022 20:20:10 GMT
ENV KONG_VERSION=2.7.1
# Fri, 04 Feb 2022 20:20:10 GMT
ARG KONG_SHA256=feeee661bbe44cf3ca2d4b748291dd3f9153f355fbc13ffeccb6fbc036249a89
# Fri, 04 Feb 2022 20:21:02 GMT
# ARGS: KONG_SHA256=feeee661bbe44cf3ca2d4b748291dd3f9153f355fbc13ffeccb6fbc036249a89
RUN set -ex     && apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_amd64.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 04 Feb 2022 20:21:03 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 04 Feb 2022 20:21:03 GMT
USER kong
# Fri, 04 Feb 2022 20:21:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 04 Feb 2022 20:21:03 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 04 Feb 2022 20:21:04 GMT
STOPSIGNAL SIGQUIT
# Fri, 04 Feb 2022 20:21:04 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 04 Feb 2022 20:21:04 GMT
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
	-	`sha256:98d4135a56578f94e10fdd1215590128a99383ea6104ad50882e07e2764063cc`  
		Last Modified: Fri, 04 Feb 2022 20:25:31 GMT  
		Size: 74.4 MB (74350478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f7e8848ec863e11869e0b3fbb9a0f57aef8c564df825fcc3ce3282c988b890`  
		Last Modified: Fri, 04 Feb 2022 20:25:19 GMT  
		Size: 879.0 B  
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
