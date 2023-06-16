<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kong`

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
-	[`kong:3.2`](#kong32)
-	[`kong:3.2-ubuntu`](#kong32-ubuntu)
-	[`kong:3.2.2`](#kong322)
-	[`kong:3.2.2-alpine`](#kong322-alpine)
-	[`kong:3.2.2-ubuntu`](#kong322-ubuntu)
-	[`kong:3.3`](#kong33)
-	[`kong:3.3-ubuntu`](#kong33-ubuntu)
-	[`kong:3.3.0`](#kong330)
-	[`kong:3.3.0-alpine`](#kong330-alpine)
-	[`kong:3.3.0-ubuntu`](#kong330-ubuntu)
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

## `kong:2.8-ubuntu`

```console
$ docker pull kong@sha256:bca947da1904c3f562c39dc0cd39c38b42ffe80ebf9e7e32394ef1c0c0c055cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.8-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:acf28d896192bb0a0d763bd71344dc50b464d791351fceb99870b43c48c41ad7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.4 MB (119387329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acde46139b2824b356768d354ecbef753dde3f5921acc03a1191d1cbe6123db8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 30 May 2023 09:32:07 GMT
ARG RELEASE
# Tue, 30 May 2023 09:32:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:32:09 GMT
ADD file:3c74e7e08cbf9a87694ce6fa541af617599680fa54d9e48556fc0fbc120b4a83 in / 
# Tue, 30 May 2023 09:32:09 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 01:32:26 GMT
ARG ASSET=ce
# Fri, 02 Jun 2023 01:32:26 GMT
ENV ASSET=ce
# Fri, 02 Jun 2023 01:32:26 GMT
ARG EE_PORTS
# Fri, 02 Jun 2023 01:32:27 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Fri, 02 Jun 2023 01:32:27 GMT
ARG KONG_VERSION=2.8.3
# Fri, 02 Jun 2023 01:32:27 GMT
ENV KONG_VERSION=2.8.3
# Fri, 02 Jun 2023 01:32:27 GMT
ARG KONG_AMD64_SHA=b52baf1caa300c3ee70ff4d58982085b1da9203c69118c885f00d13954634810
# Fri, 02 Jun 2023 01:32:27 GMT
ARG KONG_ARM64_SHA=1d5c2064d44b76fbb3cabf168dc226e91fedb991ace32915297505d089679fed
# Fri, 02 Jun 2023 01:32:53 GMT
# ARGS: KONG_AMD64_SHA=b52baf1caa300c3ee70ff4d58982085b1da9203c69118c885f00d13954634810 KONG_ARM64_SHA=1d5c2064d44b76fbb3cabf168dc226e91fedb991ace32915297505d089679fed
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 02 Jun 2023 01:32:54 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 02 Jun 2023 01:32:54 GMT
USER kong
# Fri, 02 Jun 2023 01:32:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 02 Jun 2023 01:32:54 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 02 Jun 2023 01:32:54 GMT
STOPSIGNAL SIGQUIT
# Fri, 02 Jun 2023 01:32:54 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 02 Jun 2023 01:32:54 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:41af1b5f0f51947706ae712999cf098bef968a7799e7cb4bb2268829e62a6ab3`  
		Last Modified: Fri, 02 Jun 2023 00:09:06 GMT  
		Size: 26.7 MB (26717357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6118fa5af40da97195ae6cab7e2e8f9cc05b50459ee1e1448a4e6474bf74bc29`  
		Last Modified: Fri, 02 Jun 2023 01:34:04 GMT  
		Size: 25.1 MB (25081969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe58ac5f781db246f24e1a10d7d157bcce0277b0108cf5f1bdd73d566b4b229d`  
		Last Modified: Fri, 02 Jun 2023 01:34:13 GMT  
		Size: 67.6 MB (67587122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6bf88b49502f0db3e88ad85f37e8933423e31d293b64c98163e2c711ef40ab8`  
		Last Modified: Fri, 02 Jun 2023 01:34:02 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.8-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:5cefac7b46d6ad7744555399726f2787e9283ea4b582080d3e61ea2a369c6d08
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.0 MB (113033786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:954b1f32c76863ec51999ae69faa00474e4e8f7b2fce5e298720423e5ac9aed4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 30 May 2023 09:39:04 GMT
ARG RELEASE
# Tue, 30 May 2023 09:39:04 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:39:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:39:04 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:39:09 GMT
ADD file:f56078e320535ad36864a2a30efa5b760ae65dd324cea9d75f01388b17e1183c in / 
# Tue, 30 May 2023 09:39:10 GMT
CMD ["/bin/bash"]
# Thu, 01 Jun 2023 23:38:53 GMT
ARG ASSET=ce
# Thu, 01 Jun 2023 23:38:53 GMT
ENV ASSET=ce
# Thu, 01 Jun 2023 23:38:54 GMT
ARG EE_PORTS
# Thu, 01 Jun 2023 23:38:54 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Thu, 01 Jun 2023 23:38:54 GMT
ARG KONG_VERSION=2.8.3
# Thu, 01 Jun 2023 23:38:54 GMT
ENV KONG_VERSION=2.8.3
# Thu, 01 Jun 2023 23:38:54 GMT
ARG KONG_AMD64_SHA=b52baf1caa300c3ee70ff4d58982085b1da9203c69118c885f00d13954634810
# Thu, 01 Jun 2023 23:38:54 GMT
ARG KONG_ARM64_SHA=1d5c2064d44b76fbb3cabf168dc226e91fedb991ace32915297505d089679fed
# Thu, 01 Jun 2023 23:39:26 GMT
# ARGS: KONG_AMD64_SHA=b52baf1caa300c3ee70ff4d58982085b1da9203c69118c885f00d13954634810 KONG_ARM64_SHA=1d5c2064d44b76fbb3cabf168dc226e91fedb991ace32915297505d089679fed
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Thu, 01 Jun 2023 23:39:27 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 01 Jun 2023 23:39:27 GMT
USER kong
# Thu, 01 Jun 2023 23:39:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 01 Jun 2023 23:39:27 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 01 Jun 2023 23:39:27 GMT
STOPSIGNAL SIGQUIT
# Thu, 01 Jun 2023 23:39:28 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 01 Jun 2023 23:39:28 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:7f8ef08e85adb2e0a8e170480033b585598619a5675768da9972914138e520de`  
		Last Modified: Thu, 01 Jun 2023 23:17:46 GMT  
		Size: 23.7 MB (23740900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db1ef3d318ed811633bd8f4e109c8c3dbf7f911d5f83b67b3222b01ec4e4b0c9`  
		Last Modified: Thu, 01 Jun 2023 23:40:33 GMT  
		Size: 25.1 MB (25081963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2d1b7e8ca60037ae9795efc4985a841e2024c768ad28489971a8b39b5b8de9`  
		Last Modified: Thu, 01 Jun 2023 23:40:40 GMT  
		Size: 64.2 MB (64210045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155334a315c5daddf675e0a0421864216ef9d5b62fcfa758780ce23bc563f651`  
		Last Modified: Thu, 01 Jun 2023 23:40:31 GMT  
		Size: 878.0 B  
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

## `kong:2.8.3-ubuntu`

```console
$ docker pull kong@sha256:bca947da1904c3f562c39dc0cd39c38b42ffe80ebf9e7e32394ef1c0c0c055cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.8.3-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:acf28d896192bb0a0d763bd71344dc50b464d791351fceb99870b43c48c41ad7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.4 MB (119387329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acde46139b2824b356768d354ecbef753dde3f5921acc03a1191d1cbe6123db8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 30 May 2023 09:32:07 GMT
ARG RELEASE
# Tue, 30 May 2023 09:32:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:32:07 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:32:09 GMT
ADD file:3c74e7e08cbf9a87694ce6fa541af617599680fa54d9e48556fc0fbc120b4a83 in / 
# Tue, 30 May 2023 09:32:09 GMT
CMD ["/bin/bash"]
# Fri, 02 Jun 2023 01:32:26 GMT
ARG ASSET=ce
# Fri, 02 Jun 2023 01:32:26 GMT
ENV ASSET=ce
# Fri, 02 Jun 2023 01:32:26 GMT
ARG EE_PORTS
# Fri, 02 Jun 2023 01:32:27 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Fri, 02 Jun 2023 01:32:27 GMT
ARG KONG_VERSION=2.8.3
# Fri, 02 Jun 2023 01:32:27 GMT
ENV KONG_VERSION=2.8.3
# Fri, 02 Jun 2023 01:32:27 GMT
ARG KONG_AMD64_SHA=b52baf1caa300c3ee70ff4d58982085b1da9203c69118c885f00d13954634810
# Fri, 02 Jun 2023 01:32:27 GMT
ARG KONG_ARM64_SHA=1d5c2064d44b76fbb3cabf168dc226e91fedb991ace32915297505d089679fed
# Fri, 02 Jun 2023 01:32:53 GMT
# ARGS: KONG_AMD64_SHA=b52baf1caa300c3ee70ff4d58982085b1da9203c69118c885f00d13954634810 KONG_ARM64_SHA=1d5c2064d44b76fbb3cabf168dc226e91fedb991ace32915297505d089679fed
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 02 Jun 2023 01:32:54 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 02 Jun 2023 01:32:54 GMT
USER kong
# Fri, 02 Jun 2023 01:32:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 02 Jun 2023 01:32:54 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 02 Jun 2023 01:32:54 GMT
STOPSIGNAL SIGQUIT
# Fri, 02 Jun 2023 01:32:54 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 02 Jun 2023 01:32:54 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:41af1b5f0f51947706ae712999cf098bef968a7799e7cb4bb2268829e62a6ab3`  
		Last Modified: Fri, 02 Jun 2023 00:09:06 GMT  
		Size: 26.7 MB (26717357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6118fa5af40da97195ae6cab7e2e8f9cc05b50459ee1e1448a4e6474bf74bc29`  
		Last Modified: Fri, 02 Jun 2023 01:34:04 GMT  
		Size: 25.1 MB (25081969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe58ac5f781db246f24e1a10d7d157bcce0277b0108cf5f1bdd73d566b4b229d`  
		Last Modified: Fri, 02 Jun 2023 01:34:13 GMT  
		Size: 67.6 MB (67587122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6bf88b49502f0db3e88ad85f37e8933423e31d293b64c98163e2c711ef40ab8`  
		Last Modified: Fri, 02 Jun 2023 01:34:02 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.8.3-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:5cefac7b46d6ad7744555399726f2787e9283ea4b582080d3e61ea2a369c6d08
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.0 MB (113033786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:954b1f32c76863ec51999ae69faa00474e4e8f7b2fce5e298720423e5ac9aed4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 30 May 2023 09:39:04 GMT
ARG RELEASE
# Tue, 30 May 2023 09:39:04 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 30 May 2023 09:39:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 30 May 2023 09:39:04 GMT
LABEL org.opencontainers.image.version=18.04
# Tue, 30 May 2023 09:39:09 GMT
ADD file:f56078e320535ad36864a2a30efa5b760ae65dd324cea9d75f01388b17e1183c in / 
# Tue, 30 May 2023 09:39:10 GMT
CMD ["/bin/bash"]
# Thu, 01 Jun 2023 23:38:53 GMT
ARG ASSET=ce
# Thu, 01 Jun 2023 23:38:53 GMT
ENV ASSET=ce
# Thu, 01 Jun 2023 23:38:54 GMT
ARG EE_PORTS
# Thu, 01 Jun 2023 23:38:54 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Thu, 01 Jun 2023 23:38:54 GMT
ARG KONG_VERSION=2.8.3
# Thu, 01 Jun 2023 23:38:54 GMT
ENV KONG_VERSION=2.8.3
# Thu, 01 Jun 2023 23:38:54 GMT
ARG KONG_AMD64_SHA=b52baf1caa300c3ee70ff4d58982085b1da9203c69118c885f00d13954634810
# Thu, 01 Jun 2023 23:38:54 GMT
ARG KONG_ARM64_SHA=1d5c2064d44b76fbb3cabf168dc226e91fedb991ace32915297505d089679fed
# Thu, 01 Jun 2023 23:39:26 GMT
# ARGS: KONG_AMD64_SHA=b52baf1caa300c3ee70ff4d58982085b1da9203c69118c885f00d13954634810 KONG_ARM64_SHA=1d5c2064d44b76fbb3cabf168dc226e91fedb991ace32915297505d089679fed
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Thu, 01 Jun 2023 23:39:27 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 01 Jun 2023 23:39:27 GMT
USER kong
# Thu, 01 Jun 2023 23:39:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 01 Jun 2023 23:39:27 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 01 Jun 2023 23:39:27 GMT
STOPSIGNAL SIGQUIT
# Thu, 01 Jun 2023 23:39:28 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 01 Jun 2023 23:39:28 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:7f8ef08e85adb2e0a8e170480033b585598619a5675768da9972914138e520de`  
		Last Modified: Thu, 01 Jun 2023 23:17:46 GMT  
		Size: 23.7 MB (23740900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db1ef3d318ed811633bd8f4e109c8c3dbf7f911d5f83b67b3222b01ec4e4b0c9`  
		Last Modified: Thu, 01 Jun 2023 23:40:33 GMT  
		Size: 25.1 MB (25081963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2d1b7e8ca60037ae9795efc4985a841e2024c768ad28489971a8b39b5b8de9`  
		Last Modified: Thu, 01 Jun 2023 23:40:40 GMT  
		Size: 64.2 MB (64210045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155334a315c5daddf675e0a0421864216ef9d5b62fcfa758780ce23bc563f651`  
		Last Modified: Thu, 01 Jun 2023 23:40:31 GMT  
		Size: 878.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3`

```console
$ docker pull kong@sha256:09787b545ddd942214f97241433d5c22ad30124396d1c74333adc3e12b301481
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3` - linux; amd64

```console
$ docker pull kong@sha256:74fd7d02fc80426128220c844b649ee80e078e0dcb4b2684c06b83636f4492e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81324591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46ac5c3d6929b19e745f738a7e38ffe7aac08c148cc07f5778b221c9c276ed78`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:02:20 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 16 Jun 2023 03:02:20 GMT
ARG ASSET=ce
# Fri, 16 Jun 2023 03:02:20 GMT
ENV ASSET=ce
# Fri, 16 Jun 2023 03:02:20 GMT
ARG EE_PORTS
# Fri, 16 Jun 2023 03:02:20 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 16 Jun 2023 03:02:20 GMT
ARG KONG_VERSION=3.3.0
# Fri, 16 Jun 2023 03:02:20 GMT
ENV KONG_VERSION=3.3.0
# Fri, 16 Jun 2023 03:02:20 GMT
ARG KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b
# Fri, 16 Jun 2023 03:02:20 GMT
ARG KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
# Fri, 16 Jun 2023 03:03:00 GMT
# ARGS: KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 16 Jun 2023 03:03:01 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 16 Jun 2023 03:03:01 GMT
USER kong
# Fri, 16 Jun 2023 03:03:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 16 Jun 2023 03:03:01 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 16 Jun 2023 03:03:01 GMT
STOPSIGNAL SIGQUIT
# Fri, 16 Jun 2023 03:03:01 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 16 Jun 2023 03:03:01 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:3f94e4e483ea634d7ab0b63649b8f72f8b721d4c626297fd0edae0abea1df9e9`  
		Last Modified: Tue, 06 Jun 2023 11:46:33 GMT  
		Size: 30.4 MB (30431039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b770a78ff719726efe345cf12823afe49c4f5dcfdb7c5592748ab9952e0bc087`  
		Last Modified: Fri, 16 Jun 2023 03:05:00 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d8f511e7f8d6ec0ce9cbb5237ebd5f850a99daf26f983923273a4faf566e0a`  
		Last Modified: Fri, 16 Jun 2023 03:05:07 GMT  
		Size: 50.9 MB (50892272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f2a3e4dd7fc95c394ec37022ac3067a0f4831948c64a4417681a6d38b54a8a`  
		Last Modified: Fri, 16 Jun 2023 03:04:59 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:53004538dca8b628e4b41158806a88cb29436e78740b745e13dfa5e8b0a178b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75745127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f031d6ecb97c9cd35f241a18a86551ee1ba7caa78e70932024c32a5edf17acd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:12:49 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 16 Jun 2023 03:12:50 GMT
ARG ASSET=ce
# Fri, 16 Jun 2023 03:12:50 GMT
ENV ASSET=ce
# Fri, 16 Jun 2023 03:12:50 GMT
ARG EE_PORTS
# Fri, 16 Jun 2023 03:12:50 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 16 Jun 2023 03:12:50 GMT
ARG KONG_VERSION=3.3.0
# Fri, 16 Jun 2023 03:12:50 GMT
ENV KONG_VERSION=3.3.0
# Fri, 16 Jun 2023 03:12:50 GMT
ARG KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b
# Fri, 16 Jun 2023 03:12:50 GMT
ARG KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
# Fri, 16 Jun 2023 03:13:20 GMT
# ARGS: KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 16 Jun 2023 03:13:21 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 16 Jun 2023 03:13:21 GMT
USER kong
# Fri, 16 Jun 2023 03:13:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 16 Jun 2023 03:13:21 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 16 Jun 2023 03:13:21 GMT
STOPSIGNAL SIGQUIT
# Fri, 16 Jun 2023 03:13:21 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 16 Jun 2023 03:13:21 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680f9a455927f5d901583f8890fea5cbb4c3293cae5709bd9e7df249a73f51b8`  
		Last Modified: Fri, 16 Jun 2023 03:15:15 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b2c1ee90db6284b0543979c2c3eec98e8d43362b7c6356ece9a0e8ecf99cec`  
		Last Modified: Fri, 16 Jun 2023 03:15:21 GMT  
		Size: 47.4 MB (47354643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052afa3d593dfd6a129bfa53bf0016759dbb5ed2f7324b6cfcc7200698e0ed03`  
		Last Modified: Fri, 16 Jun 2023 03:15:15 GMT  
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
$ docker pull kong@sha256:f202527d6a18b904bf15938d3c6cf5101e0ea3f4e94876fa3705a69b438468a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.0-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:2e17f2edc0f7e2ff4a8ff8893894fea2988682d0308da354b933157884402a85
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101885664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e1b4462b09d329103288ab569791bd11ded09d0b5a3aa841ae1c0a6ad80c7ea`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:57 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:58 GMT
ADD file:655d373cb551d0dd5d7867f88a4f98908dc3f16190986f693e88c423e6f21b8d in / 
# Mon, 05 Jun 2023 17:08:58 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:03:33 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 16 Jun 2023 03:03:33 GMT
ARG ASSET=ce
# Fri, 16 Jun 2023 03:03:33 GMT
ENV ASSET=ce
# Fri, 16 Jun 2023 03:03:33 GMT
ARG EE_PORTS
# Fri, 16 Jun 2023 03:03:34 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 16 Jun 2023 03:04:10 GMT
ARG KONG_VERSION=3.0.2
# Fri, 16 Jun 2023 03:04:10 GMT
ENV KONG_VERSION=3.0.2
# Fri, 16 Jun 2023 03:04:10 GMT
ARG KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396
# Fri, 16 Jun 2023 03:04:10 GMT
ARG KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
# Fri, 16 Jun 2023 03:04:32 GMT
# ARGS: KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396 KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 16 Jun 2023 03:04:32 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 16 Jun 2023 03:04:32 GMT
USER kong
# Fri, 16 Jun 2023 03:04:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 16 Jun 2023 03:04:33 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 16 Jun 2023 03:04:33 GMT
STOPSIGNAL SIGQUIT
# Fri, 16 Jun 2023 03:04:33 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 16 Jun 2023 03:04:33 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:f0412dfb1aaea4892c13dab6f771bcd79641a4bdcb521ce881f5dcfc0df9a7a5`  
		Last Modified: Tue, 06 Jun 2023 09:20:27 GMT  
		Size: 28.6 MB (28580519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c66323755fe369ed51bc005bc9b488c538dbfaa2406cb5150d0d3abbdb2e8179`  
		Last Modified: Fri, 16 Jun 2023 03:05:43 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9c47ed825e77bc437d906d6c0e93a80d53756f7c8b6dca684c2204ff88ad4b`  
		Last Modified: Fri, 16 Jun 2023 03:06:14 GMT  
		Size: 73.3 MB (73304139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ec2ed682710092d8b187780a34cd4807b72bbd85148b6e5015114fa840e3ef`  
		Last Modified: Fri, 16 Jun 2023 03:06:03 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.0-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:cce88f22b6793a6fe64b9071ef9c08c415fb6d2af3d14c61210696637e60158e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99135316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:060f4ad2e5bffa94060235dce9b86675e0106aa5df0e7635c6b61649abc659da`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 05 Jun 2023 17:07:59 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:07:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:02 GMT
ADD file:6c0661b94e27ede70ca2a8842bdab5bc26b9ae4760b17870eda9d595672795ff in / 
# Mon, 05 Jun 2023 17:08:02 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:13:50 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 16 Jun 2023 03:13:50 GMT
ARG ASSET=ce
# Fri, 16 Jun 2023 03:13:50 GMT
ENV ASSET=ce
# Fri, 16 Jun 2023 03:13:50 GMT
ARG EE_PORTS
# Fri, 16 Jun 2023 03:13:50 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 16 Jun 2023 03:14:32 GMT
ARG KONG_VERSION=3.0.2
# Fri, 16 Jun 2023 03:14:32 GMT
ENV KONG_VERSION=3.0.2
# Fri, 16 Jun 2023 03:14:32 GMT
ARG KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396
# Fri, 16 Jun 2023 03:14:32 GMT
ARG KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
# Fri, 16 Jun 2023 03:14:50 GMT
# ARGS: KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396 KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 16 Jun 2023 03:14:51 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 16 Jun 2023 03:14:51 GMT
USER kong
# Fri, 16 Jun 2023 03:14:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 16 Jun 2023 03:14:51 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 16 Jun 2023 03:14:51 GMT
STOPSIGNAL SIGQUIT
# Fri, 16 Jun 2023 03:14:51 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 16 Jun 2023 03:14:52 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:29c851dfb906fc3c51d9a9d53a0cfa8ea88e10040baaf47155e04bf87ce3f3a5`  
		Last Modified: Fri, 09 Jun 2023 02:40:24 GMT  
		Size: 27.2 MB (27200436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4132d1158ebf52a1f799a119d7078f80a510b5d6439d9273cd3ec246617ed89`  
		Last Modified: Fri, 16 Jun 2023 03:15:59 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9390ad2480a4cbb5cff05c8fe107b405dc5fce950692e4ee19e4c24cf4ced5fa`  
		Last Modified: Fri, 16 Jun 2023 03:16:27 GMT  
		Size: 71.9 MB (71933874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1d4ed2abfb7a877f2f718c61cb0a9f120b86d3235c3a695aa09f5cf594df02`  
		Last Modified: Fri, 16 Jun 2023 03:16:18 GMT  
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
$ docker pull kong@sha256:f202527d6a18b904bf15938d3c6cf5101e0ea3f4e94876fa3705a69b438468a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.0.2-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:2e17f2edc0f7e2ff4a8ff8893894fea2988682d0308da354b933157884402a85
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101885664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e1b4462b09d329103288ab569791bd11ded09d0b5a3aa841ae1c0a6ad80c7ea`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:57 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:58 GMT
ADD file:655d373cb551d0dd5d7867f88a4f98908dc3f16190986f693e88c423e6f21b8d in / 
# Mon, 05 Jun 2023 17:08:58 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:03:33 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 16 Jun 2023 03:03:33 GMT
ARG ASSET=ce
# Fri, 16 Jun 2023 03:03:33 GMT
ENV ASSET=ce
# Fri, 16 Jun 2023 03:03:33 GMT
ARG EE_PORTS
# Fri, 16 Jun 2023 03:03:34 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 16 Jun 2023 03:04:10 GMT
ARG KONG_VERSION=3.0.2
# Fri, 16 Jun 2023 03:04:10 GMT
ENV KONG_VERSION=3.0.2
# Fri, 16 Jun 2023 03:04:10 GMT
ARG KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396
# Fri, 16 Jun 2023 03:04:10 GMT
ARG KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
# Fri, 16 Jun 2023 03:04:32 GMT
# ARGS: KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396 KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 16 Jun 2023 03:04:32 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 16 Jun 2023 03:04:32 GMT
USER kong
# Fri, 16 Jun 2023 03:04:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 16 Jun 2023 03:04:33 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 16 Jun 2023 03:04:33 GMT
STOPSIGNAL SIGQUIT
# Fri, 16 Jun 2023 03:04:33 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 16 Jun 2023 03:04:33 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:f0412dfb1aaea4892c13dab6f771bcd79641a4bdcb521ce881f5dcfc0df9a7a5`  
		Last Modified: Tue, 06 Jun 2023 09:20:27 GMT  
		Size: 28.6 MB (28580519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c66323755fe369ed51bc005bc9b488c538dbfaa2406cb5150d0d3abbdb2e8179`  
		Last Modified: Fri, 16 Jun 2023 03:05:43 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9c47ed825e77bc437d906d6c0e93a80d53756f7c8b6dca684c2204ff88ad4b`  
		Last Modified: Fri, 16 Jun 2023 03:06:14 GMT  
		Size: 73.3 MB (73304139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ec2ed682710092d8b187780a34cd4807b72bbd85148b6e5015114fa840e3ef`  
		Last Modified: Fri, 16 Jun 2023 03:06:03 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.0.2-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:cce88f22b6793a6fe64b9071ef9c08c415fb6d2af3d14c61210696637e60158e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99135316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:060f4ad2e5bffa94060235dce9b86675e0106aa5df0e7635c6b61649abc659da`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 05 Jun 2023 17:07:59 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:07:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:02 GMT
ADD file:6c0661b94e27ede70ca2a8842bdab5bc26b9ae4760b17870eda9d595672795ff in / 
# Mon, 05 Jun 2023 17:08:02 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:13:50 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 16 Jun 2023 03:13:50 GMT
ARG ASSET=ce
# Fri, 16 Jun 2023 03:13:50 GMT
ENV ASSET=ce
# Fri, 16 Jun 2023 03:13:50 GMT
ARG EE_PORTS
# Fri, 16 Jun 2023 03:13:50 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 16 Jun 2023 03:14:32 GMT
ARG KONG_VERSION=3.0.2
# Fri, 16 Jun 2023 03:14:32 GMT
ENV KONG_VERSION=3.0.2
# Fri, 16 Jun 2023 03:14:32 GMT
ARG KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396
# Fri, 16 Jun 2023 03:14:32 GMT
ARG KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
# Fri, 16 Jun 2023 03:14:50 GMT
# ARGS: KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396 KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 16 Jun 2023 03:14:51 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 16 Jun 2023 03:14:51 GMT
USER kong
# Fri, 16 Jun 2023 03:14:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 16 Jun 2023 03:14:51 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 16 Jun 2023 03:14:51 GMT
STOPSIGNAL SIGQUIT
# Fri, 16 Jun 2023 03:14:51 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 16 Jun 2023 03:14:52 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:29c851dfb906fc3c51d9a9d53a0cfa8ea88e10040baaf47155e04bf87ce3f3a5`  
		Last Modified: Fri, 09 Jun 2023 02:40:24 GMT  
		Size: 27.2 MB (27200436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4132d1158ebf52a1f799a119d7078f80a510b5d6439d9273cd3ec246617ed89`  
		Last Modified: Fri, 16 Jun 2023 03:15:59 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9390ad2480a4cbb5cff05c8fe107b405dc5fce950692e4ee19e4c24cf4ced5fa`  
		Last Modified: Fri, 16 Jun 2023 03:16:27 GMT  
		Size: 71.9 MB (71933874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1d4ed2abfb7a877f2f718c61cb0a9f120b86d3235c3a695aa09f5cf594df02`  
		Last Modified: Fri, 16 Jun 2023 03:16:18 GMT  
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
$ docker pull kong@sha256:cd187e49b7907c08ae9c94d678dc3d25d4420d3cec99e3cef7155b35fec96427
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.1-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:2e8971a50718976310afeeed80b09bed29698bdaf86cd384b5a60c3ffc8640c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101910319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab956c364d9458476b36360b3e4d0883ab54ef77a8cca39c142e90f58059524b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:57 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:58 GMT
ADD file:655d373cb551d0dd5d7867f88a4f98908dc3f16190986f693e88c423e6f21b8d in / 
# Mon, 05 Jun 2023 17:08:58 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:03:33 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 16 Jun 2023 03:03:33 GMT
ARG ASSET=ce
# Fri, 16 Jun 2023 03:03:33 GMT
ENV ASSET=ce
# Fri, 16 Jun 2023 03:03:33 GMT
ARG EE_PORTS
# Fri, 16 Jun 2023 03:03:34 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 16 Jun 2023 03:03:34 GMT
ARG KONG_VERSION=3.1.1
# Fri, 16 Jun 2023 03:03:34 GMT
ENV KONG_VERSION=3.1.1
# Fri, 16 Jun 2023 03:03:34 GMT
ARG KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b
# Fri, 16 Jun 2023 03:03:34 GMT
ARG KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
# Fri, 16 Jun 2023 03:04:00 GMT
# ARGS: KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 16 Jun 2023 03:04:01 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 16 Jun 2023 03:04:01 GMT
USER kong
# Fri, 16 Jun 2023 03:04:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 16 Jun 2023 03:04:01 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 16 Jun 2023 03:04:01 GMT
STOPSIGNAL SIGQUIT
# Fri, 16 Jun 2023 03:04:01 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 16 Jun 2023 03:04:02 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:f0412dfb1aaea4892c13dab6f771bcd79641a4bdcb521ce881f5dcfc0df9a7a5`  
		Last Modified: Tue, 06 Jun 2023 09:20:27 GMT  
		Size: 28.6 MB (28580519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c66323755fe369ed51bc005bc9b488c538dbfaa2406cb5150d0d3abbdb2e8179`  
		Last Modified: Fri, 16 Jun 2023 03:05:43 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34806bc389bc099811617cf1b7cb0d2fcc8b0ef86ab57ae00ab3b2a648e2ff7a`  
		Last Modified: Fri, 16 Jun 2023 03:05:54 GMT  
		Size: 73.3 MB (73328794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d77c172b87ec9898cdbcfd906eb25b2e1b8620e7c178f9779e4ef1473a5ff7`  
		Last Modified: Fri, 16 Jun 2023 03:05:43 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.1-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:8af4562c870648b02ce93ab3db637921d357d477013c5e474b4d360ebdad940f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99168591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b37aacdb1e08c690286ccb79ddd725e8f4a10ed29e4df8bafac3de4f4754cfef`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 05 Jun 2023 17:07:59 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:07:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:02 GMT
ADD file:6c0661b94e27ede70ca2a8842bdab5bc26b9ae4760b17870eda9d595672795ff in / 
# Mon, 05 Jun 2023 17:08:02 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:13:50 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 16 Jun 2023 03:13:50 GMT
ARG ASSET=ce
# Fri, 16 Jun 2023 03:13:50 GMT
ENV ASSET=ce
# Fri, 16 Jun 2023 03:13:50 GMT
ARG EE_PORTS
# Fri, 16 Jun 2023 03:13:50 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 16 Jun 2023 03:13:51 GMT
ARG KONG_VERSION=3.1.1
# Fri, 16 Jun 2023 03:13:51 GMT
ENV KONG_VERSION=3.1.1
# Fri, 16 Jun 2023 03:13:51 GMT
ARG KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b
# Fri, 16 Jun 2023 03:13:51 GMT
ARG KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
# Fri, 16 Jun 2023 03:14:26 GMT
# ARGS: KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 16 Jun 2023 03:14:27 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 16 Jun 2023 03:14:27 GMT
USER kong
# Fri, 16 Jun 2023 03:14:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 16 Jun 2023 03:14:28 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 16 Jun 2023 03:14:28 GMT
STOPSIGNAL SIGQUIT
# Fri, 16 Jun 2023 03:14:28 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 16 Jun 2023 03:14:28 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:29c851dfb906fc3c51d9a9d53a0cfa8ea88e10040baaf47155e04bf87ce3f3a5`  
		Last Modified: Fri, 09 Jun 2023 02:40:24 GMT  
		Size: 27.2 MB (27200436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4132d1158ebf52a1f799a119d7078f80a510b5d6439d9273cd3ec246617ed89`  
		Last Modified: Fri, 16 Jun 2023 03:15:59 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5ad5666b5995cc296e5d09a3db172524425a4eaacfb67cda5a865e307cdb26`  
		Last Modified: Fri, 16 Jun 2023 03:16:08 GMT  
		Size: 72.0 MB (71967148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2390196ed1427fbc91ccf67634ded741b90f592c1e3f03d6a3475c31a4a1f3`  
		Last Modified: Fri, 16 Jun 2023 03:15:59 GMT  
		Size: 881.0 B  
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
$ docker pull kong@sha256:cd187e49b7907c08ae9c94d678dc3d25d4420d3cec99e3cef7155b35fec96427
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.1.1-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:2e8971a50718976310afeeed80b09bed29698bdaf86cd384b5a60c3ffc8640c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101910319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab956c364d9458476b36360b3e4d0883ab54ef77a8cca39c142e90f58059524b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 05 Jun 2023 17:08:57 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:08:57 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:08:57 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:58 GMT
ADD file:655d373cb551d0dd5d7867f88a4f98908dc3f16190986f693e88c423e6f21b8d in / 
# Mon, 05 Jun 2023 17:08:58 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:03:33 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 16 Jun 2023 03:03:33 GMT
ARG ASSET=ce
# Fri, 16 Jun 2023 03:03:33 GMT
ENV ASSET=ce
# Fri, 16 Jun 2023 03:03:33 GMT
ARG EE_PORTS
# Fri, 16 Jun 2023 03:03:34 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 16 Jun 2023 03:03:34 GMT
ARG KONG_VERSION=3.1.1
# Fri, 16 Jun 2023 03:03:34 GMT
ENV KONG_VERSION=3.1.1
# Fri, 16 Jun 2023 03:03:34 GMT
ARG KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b
# Fri, 16 Jun 2023 03:03:34 GMT
ARG KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
# Fri, 16 Jun 2023 03:04:00 GMT
# ARGS: KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 16 Jun 2023 03:04:01 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 16 Jun 2023 03:04:01 GMT
USER kong
# Fri, 16 Jun 2023 03:04:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 16 Jun 2023 03:04:01 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 16 Jun 2023 03:04:01 GMT
STOPSIGNAL SIGQUIT
# Fri, 16 Jun 2023 03:04:01 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 16 Jun 2023 03:04:02 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:f0412dfb1aaea4892c13dab6f771bcd79641a4bdcb521ce881f5dcfc0df9a7a5`  
		Last Modified: Tue, 06 Jun 2023 09:20:27 GMT  
		Size: 28.6 MB (28580519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c66323755fe369ed51bc005bc9b488c538dbfaa2406cb5150d0d3abbdb2e8179`  
		Last Modified: Fri, 16 Jun 2023 03:05:43 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34806bc389bc099811617cf1b7cb0d2fcc8b0ef86ab57ae00ab3b2a648e2ff7a`  
		Last Modified: Fri, 16 Jun 2023 03:05:54 GMT  
		Size: 73.3 MB (73328794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d77c172b87ec9898cdbcfd906eb25b2e1b8620e7c178f9779e4ef1473a5ff7`  
		Last Modified: Fri, 16 Jun 2023 03:05:43 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.1.1-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:8af4562c870648b02ce93ab3db637921d357d477013c5e474b4d360ebdad940f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99168591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b37aacdb1e08c690286ccb79ddd725e8f4a10ed29e4df8bafac3de4f4754cfef`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 05 Jun 2023 17:07:59 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:07:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:07:59 GMT
LABEL org.opencontainers.image.version=20.04
# Mon, 05 Jun 2023 17:08:02 GMT
ADD file:6c0661b94e27ede70ca2a8842bdab5bc26b9ae4760b17870eda9d595672795ff in / 
# Mon, 05 Jun 2023 17:08:02 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:13:50 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 16 Jun 2023 03:13:50 GMT
ARG ASSET=ce
# Fri, 16 Jun 2023 03:13:50 GMT
ENV ASSET=ce
# Fri, 16 Jun 2023 03:13:50 GMT
ARG EE_PORTS
# Fri, 16 Jun 2023 03:13:50 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 16 Jun 2023 03:13:51 GMT
ARG KONG_VERSION=3.1.1
# Fri, 16 Jun 2023 03:13:51 GMT
ENV KONG_VERSION=3.1.1
# Fri, 16 Jun 2023 03:13:51 GMT
ARG KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b
# Fri, 16 Jun 2023 03:13:51 GMT
ARG KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
# Fri, 16 Jun 2023 03:14:26 GMT
# ARGS: KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 16 Jun 2023 03:14:27 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 16 Jun 2023 03:14:27 GMT
USER kong
# Fri, 16 Jun 2023 03:14:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 16 Jun 2023 03:14:28 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 16 Jun 2023 03:14:28 GMT
STOPSIGNAL SIGQUIT
# Fri, 16 Jun 2023 03:14:28 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 16 Jun 2023 03:14:28 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:29c851dfb906fc3c51d9a9d53a0cfa8ea88e10040baaf47155e04bf87ce3f3a5`  
		Last Modified: Fri, 09 Jun 2023 02:40:24 GMT  
		Size: 27.2 MB (27200436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4132d1158ebf52a1f799a119d7078f80a510b5d6439d9273cd3ec246617ed89`  
		Last Modified: Fri, 16 Jun 2023 03:15:59 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5ad5666b5995cc296e5d09a3db172524425a4eaacfb67cda5a865e307cdb26`  
		Last Modified: Fri, 16 Jun 2023 03:16:08 GMT  
		Size: 72.0 MB (71967148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2390196ed1427fbc91ccf67634ded741b90f592c1e3f03d6a3475c31a4a1f3`  
		Last Modified: Fri, 16 Jun 2023 03:15:59 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.2`

```console
$ docker pull kong@sha256:16b4dcef1715fdcc4aca5443986b53eef37f1f96c594fbdcc8eb9772c7c346d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.2` - linux; amd64

```console
$ docker pull kong@sha256:0ecd93ecf2e1335859e9c57b7baf43f97a63906df220cbd8334bc20af0f80bf5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.5 MB (74472801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae120a7aadefee3a861b2ed3852748d742d1a4a73827569ba2bcc3281010753e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:02:20 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 16 Jun 2023 03:02:20 GMT
ARG ASSET=ce
# Fri, 16 Jun 2023 03:02:20 GMT
ENV ASSET=ce
# Fri, 16 Jun 2023 03:02:20 GMT
ARG EE_PORTS
# Fri, 16 Jun 2023 03:02:20 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 16 Jun 2023 03:03:11 GMT
ARG KONG_VERSION=3.2.2
# Fri, 16 Jun 2023 03:03:11 GMT
ENV KONG_VERSION=3.2.2
# Fri, 16 Jun 2023 03:03:11 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Fri, 16 Jun 2023 03:03:11 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Fri, 16 Jun 2023 03:03:28 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 16 Jun 2023 03:03:28 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 16 Jun 2023 03:03:28 GMT
USER kong
# Fri, 16 Jun 2023 03:03:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 16 Jun 2023 03:03:28 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 16 Jun 2023 03:03:28 GMT
STOPSIGNAL SIGQUIT
# Fri, 16 Jun 2023 03:03:29 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 16 Jun 2023 03:03:29 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:3f94e4e483ea634d7ab0b63649b8f72f8b721d4c626297fd0edae0abea1df9e9`  
		Last Modified: Tue, 06 Jun 2023 11:46:33 GMT  
		Size: 30.4 MB (30431039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b770a78ff719726efe345cf12823afe49c4f5dcfdb7c5592748ab9952e0bc087`  
		Last Modified: Fri, 16 Jun 2023 03:05:00 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb458c6178f039c53c57aa3854d6622861de2dd8d113dc4bc4b84f87459b565`  
		Last Modified: Fri, 16 Jun 2023 03:05:31 GMT  
		Size: 44.0 MB (44040482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db3c40feea8806cfd68f3828341b796708edb32d8df206ab2782c132c417a6e`  
		Last Modified: Fri, 16 Jun 2023 03:05:24 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.2` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:95231e853c3bbaf822916ea77416405b00c605604dc0cc7050460f7da094f95c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.6 MB (78594233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cc9b33bb4d41040be5eebb54d43f48cc7f7577c68d9a3cd87060a37c30a6db0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:12:49 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 16 Jun 2023 03:12:50 GMT
ARG ASSET=ce
# Fri, 16 Jun 2023 03:12:50 GMT
ENV ASSET=ce
# Fri, 16 Jun 2023 03:12:50 GMT
ARG EE_PORTS
# Fri, 16 Jun 2023 03:12:50 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 16 Jun 2023 03:13:29 GMT
ARG KONG_VERSION=3.2.2
# Fri, 16 Jun 2023 03:13:30 GMT
ENV KONG_VERSION=3.2.2
# Fri, 16 Jun 2023 03:13:30 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Fri, 16 Jun 2023 03:13:30 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Fri, 16 Jun 2023 03:13:45 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 16 Jun 2023 03:13:46 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 16 Jun 2023 03:13:46 GMT
USER kong
# Fri, 16 Jun 2023 03:13:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 16 Jun 2023 03:13:46 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 16 Jun 2023 03:13:46 GMT
STOPSIGNAL SIGQUIT
# Fri, 16 Jun 2023 03:13:46 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 16 Jun 2023 03:13:46 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680f9a455927f5d901583f8890fea5cbb4c3293cae5709bd9e7df249a73f51b8`  
		Last Modified: Fri, 16 Jun 2023 03:15:15 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4975afdaf40a1f95130a051e2ecdbdc8f0dd2c6218c0e8a3cd4e2e5a16a8699`  
		Last Modified: Fri, 16 Jun 2023 03:15:46 GMT  
		Size: 50.2 MB (50203748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cecee8e33e2df7873eca389980df7b82ff9908e00896f9c527864202eee67a3`  
		Last Modified: Fri, 16 Jun 2023 03:15:39 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.2-ubuntu`

```console
$ docker pull kong@sha256:16b4dcef1715fdcc4aca5443986b53eef37f1f96c594fbdcc8eb9772c7c346d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.2-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:0ecd93ecf2e1335859e9c57b7baf43f97a63906df220cbd8334bc20af0f80bf5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.5 MB (74472801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae120a7aadefee3a861b2ed3852748d742d1a4a73827569ba2bcc3281010753e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:02:20 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 16 Jun 2023 03:02:20 GMT
ARG ASSET=ce
# Fri, 16 Jun 2023 03:02:20 GMT
ENV ASSET=ce
# Fri, 16 Jun 2023 03:02:20 GMT
ARG EE_PORTS
# Fri, 16 Jun 2023 03:02:20 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 16 Jun 2023 03:03:11 GMT
ARG KONG_VERSION=3.2.2
# Fri, 16 Jun 2023 03:03:11 GMT
ENV KONG_VERSION=3.2.2
# Fri, 16 Jun 2023 03:03:11 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Fri, 16 Jun 2023 03:03:11 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Fri, 16 Jun 2023 03:03:28 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 16 Jun 2023 03:03:28 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 16 Jun 2023 03:03:28 GMT
USER kong
# Fri, 16 Jun 2023 03:03:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 16 Jun 2023 03:03:28 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 16 Jun 2023 03:03:28 GMT
STOPSIGNAL SIGQUIT
# Fri, 16 Jun 2023 03:03:29 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 16 Jun 2023 03:03:29 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:3f94e4e483ea634d7ab0b63649b8f72f8b721d4c626297fd0edae0abea1df9e9`  
		Last Modified: Tue, 06 Jun 2023 11:46:33 GMT  
		Size: 30.4 MB (30431039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b770a78ff719726efe345cf12823afe49c4f5dcfdb7c5592748ab9952e0bc087`  
		Last Modified: Fri, 16 Jun 2023 03:05:00 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb458c6178f039c53c57aa3854d6622861de2dd8d113dc4bc4b84f87459b565`  
		Last Modified: Fri, 16 Jun 2023 03:05:31 GMT  
		Size: 44.0 MB (44040482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db3c40feea8806cfd68f3828341b796708edb32d8df206ab2782c132c417a6e`  
		Last Modified: Fri, 16 Jun 2023 03:05:24 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.2-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:95231e853c3bbaf822916ea77416405b00c605604dc0cc7050460f7da094f95c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.6 MB (78594233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cc9b33bb4d41040be5eebb54d43f48cc7f7577c68d9a3cd87060a37c30a6db0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:12:49 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 16 Jun 2023 03:12:50 GMT
ARG ASSET=ce
# Fri, 16 Jun 2023 03:12:50 GMT
ENV ASSET=ce
# Fri, 16 Jun 2023 03:12:50 GMT
ARG EE_PORTS
# Fri, 16 Jun 2023 03:12:50 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 16 Jun 2023 03:13:29 GMT
ARG KONG_VERSION=3.2.2
# Fri, 16 Jun 2023 03:13:30 GMT
ENV KONG_VERSION=3.2.2
# Fri, 16 Jun 2023 03:13:30 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Fri, 16 Jun 2023 03:13:30 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Fri, 16 Jun 2023 03:13:45 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 16 Jun 2023 03:13:46 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 16 Jun 2023 03:13:46 GMT
USER kong
# Fri, 16 Jun 2023 03:13:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 16 Jun 2023 03:13:46 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 16 Jun 2023 03:13:46 GMT
STOPSIGNAL SIGQUIT
# Fri, 16 Jun 2023 03:13:46 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 16 Jun 2023 03:13:46 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680f9a455927f5d901583f8890fea5cbb4c3293cae5709bd9e7df249a73f51b8`  
		Last Modified: Fri, 16 Jun 2023 03:15:15 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4975afdaf40a1f95130a051e2ecdbdc8f0dd2c6218c0e8a3cd4e2e5a16a8699`  
		Last Modified: Fri, 16 Jun 2023 03:15:46 GMT  
		Size: 50.2 MB (50203748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cecee8e33e2df7873eca389980df7b82ff9908e00896f9c527864202eee67a3`  
		Last Modified: Fri, 16 Jun 2023 03:15:39 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.2.2`

```console
$ docker pull kong@sha256:16b4dcef1715fdcc4aca5443986b53eef37f1f96c594fbdcc8eb9772c7c346d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.2.2` - linux; amd64

```console
$ docker pull kong@sha256:0ecd93ecf2e1335859e9c57b7baf43f97a63906df220cbd8334bc20af0f80bf5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.5 MB (74472801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae120a7aadefee3a861b2ed3852748d742d1a4a73827569ba2bcc3281010753e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:02:20 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 16 Jun 2023 03:02:20 GMT
ARG ASSET=ce
# Fri, 16 Jun 2023 03:02:20 GMT
ENV ASSET=ce
# Fri, 16 Jun 2023 03:02:20 GMT
ARG EE_PORTS
# Fri, 16 Jun 2023 03:02:20 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 16 Jun 2023 03:03:11 GMT
ARG KONG_VERSION=3.2.2
# Fri, 16 Jun 2023 03:03:11 GMT
ENV KONG_VERSION=3.2.2
# Fri, 16 Jun 2023 03:03:11 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Fri, 16 Jun 2023 03:03:11 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Fri, 16 Jun 2023 03:03:28 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 16 Jun 2023 03:03:28 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 16 Jun 2023 03:03:28 GMT
USER kong
# Fri, 16 Jun 2023 03:03:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 16 Jun 2023 03:03:28 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 16 Jun 2023 03:03:28 GMT
STOPSIGNAL SIGQUIT
# Fri, 16 Jun 2023 03:03:29 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 16 Jun 2023 03:03:29 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:3f94e4e483ea634d7ab0b63649b8f72f8b721d4c626297fd0edae0abea1df9e9`  
		Last Modified: Tue, 06 Jun 2023 11:46:33 GMT  
		Size: 30.4 MB (30431039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b770a78ff719726efe345cf12823afe49c4f5dcfdb7c5592748ab9952e0bc087`  
		Last Modified: Fri, 16 Jun 2023 03:05:00 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb458c6178f039c53c57aa3854d6622861de2dd8d113dc4bc4b84f87459b565`  
		Last Modified: Fri, 16 Jun 2023 03:05:31 GMT  
		Size: 44.0 MB (44040482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db3c40feea8806cfd68f3828341b796708edb32d8df206ab2782c132c417a6e`  
		Last Modified: Fri, 16 Jun 2023 03:05:24 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.2.2` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:95231e853c3bbaf822916ea77416405b00c605604dc0cc7050460f7da094f95c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.6 MB (78594233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cc9b33bb4d41040be5eebb54d43f48cc7f7577c68d9a3cd87060a37c30a6db0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:12:49 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 16 Jun 2023 03:12:50 GMT
ARG ASSET=ce
# Fri, 16 Jun 2023 03:12:50 GMT
ENV ASSET=ce
# Fri, 16 Jun 2023 03:12:50 GMT
ARG EE_PORTS
# Fri, 16 Jun 2023 03:12:50 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 16 Jun 2023 03:13:29 GMT
ARG KONG_VERSION=3.2.2
# Fri, 16 Jun 2023 03:13:30 GMT
ENV KONG_VERSION=3.2.2
# Fri, 16 Jun 2023 03:13:30 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Fri, 16 Jun 2023 03:13:30 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Fri, 16 Jun 2023 03:13:45 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 16 Jun 2023 03:13:46 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 16 Jun 2023 03:13:46 GMT
USER kong
# Fri, 16 Jun 2023 03:13:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 16 Jun 2023 03:13:46 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 16 Jun 2023 03:13:46 GMT
STOPSIGNAL SIGQUIT
# Fri, 16 Jun 2023 03:13:46 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 16 Jun 2023 03:13:46 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680f9a455927f5d901583f8890fea5cbb4c3293cae5709bd9e7df249a73f51b8`  
		Last Modified: Fri, 16 Jun 2023 03:15:15 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4975afdaf40a1f95130a051e2ecdbdc8f0dd2c6218c0e8a3cd4e2e5a16a8699`  
		Last Modified: Fri, 16 Jun 2023 03:15:46 GMT  
		Size: 50.2 MB (50203748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cecee8e33e2df7873eca389980df7b82ff9908e00896f9c527864202eee67a3`  
		Last Modified: Fri, 16 Jun 2023 03:15:39 GMT  
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
$ docker pull kong@sha256:16b4dcef1715fdcc4aca5443986b53eef37f1f96c594fbdcc8eb9772c7c346d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.2.2-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:0ecd93ecf2e1335859e9c57b7baf43f97a63906df220cbd8334bc20af0f80bf5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.5 MB (74472801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae120a7aadefee3a861b2ed3852748d742d1a4a73827569ba2bcc3281010753e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:02:20 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 16 Jun 2023 03:02:20 GMT
ARG ASSET=ce
# Fri, 16 Jun 2023 03:02:20 GMT
ENV ASSET=ce
# Fri, 16 Jun 2023 03:02:20 GMT
ARG EE_PORTS
# Fri, 16 Jun 2023 03:02:20 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 16 Jun 2023 03:03:11 GMT
ARG KONG_VERSION=3.2.2
# Fri, 16 Jun 2023 03:03:11 GMT
ENV KONG_VERSION=3.2.2
# Fri, 16 Jun 2023 03:03:11 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Fri, 16 Jun 2023 03:03:11 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Fri, 16 Jun 2023 03:03:28 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 16 Jun 2023 03:03:28 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 16 Jun 2023 03:03:28 GMT
USER kong
# Fri, 16 Jun 2023 03:03:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 16 Jun 2023 03:03:28 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 16 Jun 2023 03:03:28 GMT
STOPSIGNAL SIGQUIT
# Fri, 16 Jun 2023 03:03:29 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 16 Jun 2023 03:03:29 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:3f94e4e483ea634d7ab0b63649b8f72f8b721d4c626297fd0edae0abea1df9e9`  
		Last Modified: Tue, 06 Jun 2023 11:46:33 GMT  
		Size: 30.4 MB (30431039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b770a78ff719726efe345cf12823afe49c4f5dcfdb7c5592748ab9952e0bc087`  
		Last Modified: Fri, 16 Jun 2023 03:05:00 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb458c6178f039c53c57aa3854d6622861de2dd8d113dc4bc4b84f87459b565`  
		Last Modified: Fri, 16 Jun 2023 03:05:31 GMT  
		Size: 44.0 MB (44040482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db3c40feea8806cfd68f3828341b796708edb32d8df206ab2782c132c417a6e`  
		Last Modified: Fri, 16 Jun 2023 03:05:24 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.2.2-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:95231e853c3bbaf822916ea77416405b00c605604dc0cc7050460f7da094f95c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.6 MB (78594233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cc9b33bb4d41040be5eebb54d43f48cc7f7577c68d9a3cd87060a37c30a6db0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:12:49 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 16 Jun 2023 03:12:50 GMT
ARG ASSET=ce
# Fri, 16 Jun 2023 03:12:50 GMT
ENV ASSET=ce
# Fri, 16 Jun 2023 03:12:50 GMT
ARG EE_PORTS
# Fri, 16 Jun 2023 03:12:50 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 16 Jun 2023 03:13:29 GMT
ARG KONG_VERSION=3.2.2
# Fri, 16 Jun 2023 03:13:30 GMT
ENV KONG_VERSION=3.2.2
# Fri, 16 Jun 2023 03:13:30 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Fri, 16 Jun 2023 03:13:30 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Fri, 16 Jun 2023 03:13:45 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 16 Jun 2023 03:13:46 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 16 Jun 2023 03:13:46 GMT
USER kong
# Fri, 16 Jun 2023 03:13:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 16 Jun 2023 03:13:46 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 16 Jun 2023 03:13:46 GMT
STOPSIGNAL SIGQUIT
# Fri, 16 Jun 2023 03:13:46 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 16 Jun 2023 03:13:46 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680f9a455927f5d901583f8890fea5cbb4c3293cae5709bd9e7df249a73f51b8`  
		Last Modified: Fri, 16 Jun 2023 03:15:15 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4975afdaf40a1f95130a051e2ecdbdc8f0dd2c6218c0e8a3cd4e2e5a16a8699`  
		Last Modified: Fri, 16 Jun 2023 03:15:46 GMT  
		Size: 50.2 MB (50203748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cecee8e33e2df7873eca389980df7b82ff9908e00896f9c527864202eee67a3`  
		Last Modified: Fri, 16 Jun 2023 03:15:39 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.3`

```console
$ docker pull kong@sha256:09787b545ddd942214f97241433d5c22ad30124396d1c74333adc3e12b301481
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.3` - linux; amd64

```console
$ docker pull kong@sha256:74fd7d02fc80426128220c844b649ee80e078e0dcb4b2684c06b83636f4492e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81324591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46ac5c3d6929b19e745f738a7e38ffe7aac08c148cc07f5778b221c9c276ed78`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:02:20 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 16 Jun 2023 03:02:20 GMT
ARG ASSET=ce
# Fri, 16 Jun 2023 03:02:20 GMT
ENV ASSET=ce
# Fri, 16 Jun 2023 03:02:20 GMT
ARG EE_PORTS
# Fri, 16 Jun 2023 03:02:20 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 16 Jun 2023 03:02:20 GMT
ARG KONG_VERSION=3.3.0
# Fri, 16 Jun 2023 03:02:20 GMT
ENV KONG_VERSION=3.3.0
# Fri, 16 Jun 2023 03:02:20 GMT
ARG KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b
# Fri, 16 Jun 2023 03:02:20 GMT
ARG KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
# Fri, 16 Jun 2023 03:03:00 GMT
# ARGS: KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 16 Jun 2023 03:03:01 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 16 Jun 2023 03:03:01 GMT
USER kong
# Fri, 16 Jun 2023 03:03:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 16 Jun 2023 03:03:01 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 16 Jun 2023 03:03:01 GMT
STOPSIGNAL SIGQUIT
# Fri, 16 Jun 2023 03:03:01 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 16 Jun 2023 03:03:01 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:3f94e4e483ea634d7ab0b63649b8f72f8b721d4c626297fd0edae0abea1df9e9`  
		Last Modified: Tue, 06 Jun 2023 11:46:33 GMT  
		Size: 30.4 MB (30431039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b770a78ff719726efe345cf12823afe49c4f5dcfdb7c5592748ab9952e0bc087`  
		Last Modified: Fri, 16 Jun 2023 03:05:00 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d8f511e7f8d6ec0ce9cbb5237ebd5f850a99daf26f983923273a4faf566e0a`  
		Last Modified: Fri, 16 Jun 2023 03:05:07 GMT  
		Size: 50.9 MB (50892272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f2a3e4dd7fc95c394ec37022ac3067a0f4831948c64a4417681a6d38b54a8a`  
		Last Modified: Fri, 16 Jun 2023 03:04:59 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.3` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:53004538dca8b628e4b41158806a88cb29436e78740b745e13dfa5e8b0a178b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75745127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f031d6ecb97c9cd35f241a18a86551ee1ba7caa78e70932024c32a5edf17acd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:12:49 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 16 Jun 2023 03:12:50 GMT
ARG ASSET=ce
# Fri, 16 Jun 2023 03:12:50 GMT
ENV ASSET=ce
# Fri, 16 Jun 2023 03:12:50 GMT
ARG EE_PORTS
# Fri, 16 Jun 2023 03:12:50 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 16 Jun 2023 03:12:50 GMT
ARG KONG_VERSION=3.3.0
# Fri, 16 Jun 2023 03:12:50 GMT
ENV KONG_VERSION=3.3.0
# Fri, 16 Jun 2023 03:12:50 GMT
ARG KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b
# Fri, 16 Jun 2023 03:12:50 GMT
ARG KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
# Fri, 16 Jun 2023 03:13:20 GMT
# ARGS: KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 16 Jun 2023 03:13:21 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 16 Jun 2023 03:13:21 GMT
USER kong
# Fri, 16 Jun 2023 03:13:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 16 Jun 2023 03:13:21 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 16 Jun 2023 03:13:21 GMT
STOPSIGNAL SIGQUIT
# Fri, 16 Jun 2023 03:13:21 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 16 Jun 2023 03:13:21 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680f9a455927f5d901583f8890fea5cbb4c3293cae5709bd9e7df249a73f51b8`  
		Last Modified: Fri, 16 Jun 2023 03:15:15 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b2c1ee90db6284b0543979c2c3eec98e8d43362b7c6356ece9a0e8ecf99cec`  
		Last Modified: Fri, 16 Jun 2023 03:15:21 GMT  
		Size: 47.4 MB (47354643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052afa3d593dfd6a129bfa53bf0016759dbb5ed2f7324b6cfcc7200698e0ed03`  
		Last Modified: Fri, 16 Jun 2023 03:15:15 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.3-ubuntu`

```console
$ docker pull kong@sha256:09787b545ddd942214f97241433d5c22ad30124396d1c74333adc3e12b301481
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.3-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:74fd7d02fc80426128220c844b649ee80e078e0dcb4b2684c06b83636f4492e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81324591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46ac5c3d6929b19e745f738a7e38ffe7aac08c148cc07f5778b221c9c276ed78`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:02:20 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 16 Jun 2023 03:02:20 GMT
ARG ASSET=ce
# Fri, 16 Jun 2023 03:02:20 GMT
ENV ASSET=ce
# Fri, 16 Jun 2023 03:02:20 GMT
ARG EE_PORTS
# Fri, 16 Jun 2023 03:02:20 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 16 Jun 2023 03:02:20 GMT
ARG KONG_VERSION=3.3.0
# Fri, 16 Jun 2023 03:02:20 GMT
ENV KONG_VERSION=3.3.0
# Fri, 16 Jun 2023 03:02:20 GMT
ARG KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b
# Fri, 16 Jun 2023 03:02:20 GMT
ARG KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
# Fri, 16 Jun 2023 03:03:00 GMT
# ARGS: KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 16 Jun 2023 03:03:01 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 16 Jun 2023 03:03:01 GMT
USER kong
# Fri, 16 Jun 2023 03:03:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 16 Jun 2023 03:03:01 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 16 Jun 2023 03:03:01 GMT
STOPSIGNAL SIGQUIT
# Fri, 16 Jun 2023 03:03:01 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 16 Jun 2023 03:03:01 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:3f94e4e483ea634d7ab0b63649b8f72f8b721d4c626297fd0edae0abea1df9e9`  
		Last Modified: Tue, 06 Jun 2023 11:46:33 GMT  
		Size: 30.4 MB (30431039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b770a78ff719726efe345cf12823afe49c4f5dcfdb7c5592748ab9952e0bc087`  
		Last Modified: Fri, 16 Jun 2023 03:05:00 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d8f511e7f8d6ec0ce9cbb5237ebd5f850a99daf26f983923273a4faf566e0a`  
		Last Modified: Fri, 16 Jun 2023 03:05:07 GMT  
		Size: 50.9 MB (50892272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f2a3e4dd7fc95c394ec37022ac3067a0f4831948c64a4417681a6d38b54a8a`  
		Last Modified: Fri, 16 Jun 2023 03:04:59 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.3-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:53004538dca8b628e4b41158806a88cb29436e78740b745e13dfa5e8b0a178b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75745127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f031d6ecb97c9cd35f241a18a86551ee1ba7caa78e70932024c32a5edf17acd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:12:49 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 16 Jun 2023 03:12:50 GMT
ARG ASSET=ce
# Fri, 16 Jun 2023 03:12:50 GMT
ENV ASSET=ce
# Fri, 16 Jun 2023 03:12:50 GMT
ARG EE_PORTS
# Fri, 16 Jun 2023 03:12:50 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 16 Jun 2023 03:12:50 GMT
ARG KONG_VERSION=3.3.0
# Fri, 16 Jun 2023 03:12:50 GMT
ENV KONG_VERSION=3.3.0
# Fri, 16 Jun 2023 03:12:50 GMT
ARG KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b
# Fri, 16 Jun 2023 03:12:50 GMT
ARG KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
# Fri, 16 Jun 2023 03:13:20 GMT
# ARGS: KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 16 Jun 2023 03:13:21 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 16 Jun 2023 03:13:21 GMT
USER kong
# Fri, 16 Jun 2023 03:13:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 16 Jun 2023 03:13:21 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 16 Jun 2023 03:13:21 GMT
STOPSIGNAL SIGQUIT
# Fri, 16 Jun 2023 03:13:21 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 16 Jun 2023 03:13:21 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680f9a455927f5d901583f8890fea5cbb4c3293cae5709bd9e7df249a73f51b8`  
		Last Modified: Fri, 16 Jun 2023 03:15:15 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b2c1ee90db6284b0543979c2c3eec98e8d43362b7c6356ece9a0e8ecf99cec`  
		Last Modified: Fri, 16 Jun 2023 03:15:21 GMT  
		Size: 47.4 MB (47354643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052afa3d593dfd6a129bfa53bf0016759dbb5ed2f7324b6cfcc7200698e0ed03`  
		Last Modified: Fri, 16 Jun 2023 03:15:15 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.3.0`

```console
$ docker pull kong@sha256:09787b545ddd942214f97241433d5c22ad30124396d1c74333adc3e12b301481
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.3.0` - linux; amd64

```console
$ docker pull kong@sha256:74fd7d02fc80426128220c844b649ee80e078e0dcb4b2684c06b83636f4492e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81324591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46ac5c3d6929b19e745f738a7e38ffe7aac08c148cc07f5778b221c9c276ed78`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:02:20 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 16 Jun 2023 03:02:20 GMT
ARG ASSET=ce
# Fri, 16 Jun 2023 03:02:20 GMT
ENV ASSET=ce
# Fri, 16 Jun 2023 03:02:20 GMT
ARG EE_PORTS
# Fri, 16 Jun 2023 03:02:20 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 16 Jun 2023 03:02:20 GMT
ARG KONG_VERSION=3.3.0
# Fri, 16 Jun 2023 03:02:20 GMT
ENV KONG_VERSION=3.3.0
# Fri, 16 Jun 2023 03:02:20 GMT
ARG KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b
# Fri, 16 Jun 2023 03:02:20 GMT
ARG KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
# Fri, 16 Jun 2023 03:03:00 GMT
# ARGS: KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 16 Jun 2023 03:03:01 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 16 Jun 2023 03:03:01 GMT
USER kong
# Fri, 16 Jun 2023 03:03:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 16 Jun 2023 03:03:01 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 16 Jun 2023 03:03:01 GMT
STOPSIGNAL SIGQUIT
# Fri, 16 Jun 2023 03:03:01 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 16 Jun 2023 03:03:01 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:3f94e4e483ea634d7ab0b63649b8f72f8b721d4c626297fd0edae0abea1df9e9`  
		Last Modified: Tue, 06 Jun 2023 11:46:33 GMT  
		Size: 30.4 MB (30431039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b770a78ff719726efe345cf12823afe49c4f5dcfdb7c5592748ab9952e0bc087`  
		Last Modified: Fri, 16 Jun 2023 03:05:00 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d8f511e7f8d6ec0ce9cbb5237ebd5f850a99daf26f983923273a4faf566e0a`  
		Last Modified: Fri, 16 Jun 2023 03:05:07 GMT  
		Size: 50.9 MB (50892272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f2a3e4dd7fc95c394ec37022ac3067a0f4831948c64a4417681a6d38b54a8a`  
		Last Modified: Fri, 16 Jun 2023 03:04:59 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.3.0` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:53004538dca8b628e4b41158806a88cb29436e78740b745e13dfa5e8b0a178b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75745127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f031d6ecb97c9cd35f241a18a86551ee1ba7caa78e70932024c32a5edf17acd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:12:49 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 16 Jun 2023 03:12:50 GMT
ARG ASSET=ce
# Fri, 16 Jun 2023 03:12:50 GMT
ENV ASSET=ce
# Fri, 16 Jun 2023 03:12:50 GMT
ARG EE_PORTS
# Fri, 16 Jun 2023 03:12:50 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 16 Jun 2023 03:12:50 GMT
ARG KONG_VERSION=3.3.0
# Fri, 16 Jun 2023 03:12:50 GMT
ENV KONG_VERSION=3.3.0
# Fri, 16 Jun 2023 03:12:50 GMT
ARG KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b
# Fri, 16 Jun 2023 03:12:50 GMT
ARG KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
# Fri, 16 Jun 2023 03:13:20 GMT
# ARGS: KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 16 Jun 2023 03:13:21 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 16 Jun 2023 03:13:21 GMT
USER kong
# Fri, 16 Jun 2023 03:13:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 16 Jun 2023 03:13:21 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 16 Jun 2023 03:13:21 GMT
STOPSIGNAL SIGQUIT
# Fri, 16 Jun 2023 03:13:21 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 16 Jun 2023 03:13:21 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680f9a455927f5d901583f8890fea5cbb4c3293cae5709bd9e7df249a73f51b8`  
		Last Modified: Fri, 16 Jun 2023 03:15:15 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b2c1ee90db6284b0543979c2c3eec98e8d43362b7c6356ece9a0e8ecf99cec`  
		Last Modified: Fri, 16 Jun 2023 03:15:21 GMT  
		Size: 47.4 MB (47354643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052afa3d593dfd6a129bfa53bf0016759dbb5ed2f7324b6cfcc7200698e0ed03`  
		Last Modified: Fri, 16 Jun 2023 03:15:15 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.3.0-alpine`

```console
$ docker pull kong@sha256:aae539892ee4f08d979274768504d5e592928b1d57a824e3436d627a8588fe6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:3.3.0-alpine` - linux; amd64

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

## `kong:3.3.0-ubuntu`

```console
$ docker pull kong@sha256:09787b545ddd942214f97241433d5c22ad30124396d1c74333adc3e12b301481
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.3.0-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:74fd7d02fc80426128220c844b649ee80e078e0dcb4b2684c06b83636f4492e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81324591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46ac5c3d6929b19e745f738a7e38ffe7aac08c148cc07f5778b221c9c276ed78`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:02:20 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 16 Jun 2023 03:02:20 GMT
ARG ASSET=ce
# Fri, 16 Jun 2023 03:02:20 GMT
ENV ASSET=ce
# Fri, 16 Jun 2023 03:02:20 GMT
ARG EE_PORTS
# Fri, 16 Jun 2023 03:02:20 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 16 Jun 2023 03:02:20 GMT
ARG KONG_VERSION=3.3.0
# Fri, 16 Jun 2023 03:02:20 GMT
ENV KONG_VERSION=3.3.0
# Fri, 16 Jun 2023 03:02:20 GMT
ARG KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b
# Fri, 16 Jun 2023 03:02:20 GMT
ARG KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
# Fri, 16 Jun 2023 03:03:00 GMT
# ARGS: KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 16 Jun 2023 03:03:01 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 16 Jun 2023 03:03:01 GMT
USER kong
# Fri, 16 Jun 2023 03:03:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 16 Jun 2023 03:03:01 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 16 Jun 2023 03:03:01 GMT
STOPSIGNAL SIGQUIT
# Fri, 16 Jun 2023 03:03:01 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 16 Jun 2023 03:03:01 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:3f94e4e483ea634d7ab0b63649b8f72f8b721d4c626297fd0edae0abea1df9e9`  
		Last Modified: Tue, 06 Jun 2023 11:46:33 GMT  
		Size: 30.4 MB (30431039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b770a78ff719726efe345cf12823afe49c4f5dcfdb7c5592748ab9952e0bc087`  
		Last Modified: Fri, 16 Jun 2023 03:05:00 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d8f511e7f8d6ec0ce9cbb5237ebd5f850a99daf26f983923273a4faf566e0a`  
		Last Modified: Fri, 16 Jun 2023 03:05:07 GMT  
		Size: 50.9 MB (50892272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f2a3e4dd7fc95c394ec37022ac3067a0f4831948c64a4417681a6d38b54a8a`  
		Last Modified: Fri, 16 Jun 2023 03:04:59 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.3.0-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:53004538dca8b628e4b41158806a88cb29436e78740b745e13dfa5e8b0a178b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75745127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f031d6ecb97c9cd35f241a18a86551ee1ba7caa78e70932024c32a5edf17acd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:12:49 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 16 Jun 2023 03:12:50 GMT
ARG ASSET=ce
# Fri, 16 Jun 2023 03:12:50 GMT
ENV ASSET=ce
# Fri, 16 Jun 2023 03:12:50 GMT
ARG EE_PORTS
# Fri, 16 Jun 2023 03:12:50 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 16 Jun 2023 03:12:50 GMT
ARG KONG_VERSION=3.3.0
# Fri, 16 Jun 2023 03:12:50 GMT
ENV KONG_VERSION=3.3.0
# Fri, 16 Jun 2023 03:12:50 GMT
ARG KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b
# Fri, 16 Jun 2023 03:12:50 GMT
ARG KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
# Fri, 16 Jun 2023 03:13:20 GMT
# ARGS: KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 16 Jun 2023 03:13:21 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 16 Jun 2023 03:13:21 GMT
USER kong
# Fri, 16 Jun 2023 03:13:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 16 Jun 2023 03:13:21 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 16 Jun 2023 03:13:21 GMT
STOPSIGNAL SIGQUIT
# Fri, 16 Jun 2023 03:13:21 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 16 Jun 2023 03:13:21 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680f9a455927f5d901583f8890fea5cbb4c3293cae5709bd9e7df249a73f51b8`  
		Last Modified: Fri, 16 Jun 2023 03:15:15 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b2c1ee90db6284b0543979c2c3eec98e8d43362b7c6356ece9a0e8ecf99cec`  
		Last Modified: Fri, 16 Jun 2023 03:15:21 GMT  
		Size: 47.4 MB (47354643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052afa3d593dfd6a129bfa53bf0016759dbb5ed2f7324b6cfcc7200698e0ed03`  
		Last Modified: Fri, 16 Jun 2023 03:15:15 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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
$ docker pull kong@sha256:09787b545ddd942214f97241433d5c22ad30124396d1c74333adc3e12b301481
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:latest` - linux; amd64

```console
$ docker pull kong@sha256:74fd7d02fc80426128220c844b649ee80e078e0dcb4b2684c06b83636f4492e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81324591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46ac5c3d6929b19e745f738a7e38ffe7aac08c148cc07f5778b221c9c276ed78`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:02:20 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 16 Jun 2023 03:02:20 GMT
ARG ASSET=ce
# Fri, 16 Jun 2023 03:02:20 GMT
ENV ASSET=ce
# Fri, 16 Jun 2023 03:02:20 GMT
ARG EE_PORTS
# Fri, 16 Jun 2023 03:02:20 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 16 Jun 2023 03:02:20 GMT
ARG KONG_VERSION=3.3.0
# Fri, 16 Jun 2023 03:02:20 GMT
ENV KONG_VERSION=3.3.0
# Fri, 16 Jun 2023 03:02:20 GMT
ARG KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b
# Fri, 16 Jun 2023 03:02:20 GMT
ARG KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
# Fri, 16 Jun 2023 03:03:00 GMT
# ARGS: KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 16 Jun 2023 03:03:01 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 16 Jun 2023 03:03:01 GMT
USER kong
# Fri, 16 Jun 2023 03:03:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 16 Jun 2023 03:03:01 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 16 Jun 2023 03:03:01 GMT
STOPSIGNAL SIGQUIT
# Fri, 16 Jun 2023 03:03:01 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 16 Jun 2023 03:03:01 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:3f94e4e483ea634d7ab0b63649b8f72f8b721d4c626297fd0edae0abea1df9e9`  
		Last Modified: Tue, 06 Jun 2023 11:46:33 GMT  
		Size: 30.4 MB (30431039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b770a78ff719726efe345cf12823afe49c4f5dcfdb7c5592748ab9952e0bc087`  
		Last Modified: Fri, 16 Jun 2023 03:05:00 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d8f511e7f8d6ec0ce9cbb5237ebd5f850a99daf26f983923273a4faf566e0a`  
		Last Modified: Fri, 16 Jun 2023 03:05:07 GMT  
		Size: 50.9 MB (50892272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f2a3e4dd7fc95c394ec37022ac3067a0f4831948c64a4417681a6d38b54a8a`  
		Last Modified: Fri, 16 Jun 2023 03:04:59 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:latest` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:53004538dca8b628e4b41158806a88cb29436e78740b745e13dfa5e8b0a178b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75745127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f031d6ecb97c9cd35f241a18a86551ee1ba7caa78e70932024c32a5edf17acd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:12:49 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 16 Jun 2023 03:12:50 GMT
ARG ASSET=ce
# Fri, 16 Jun 2023 03:12:50 GMT
ENV ASSET=ce
# Fri, 16 Jun 2023 03:12:50 GMT
ARG EE_PORTS
# Fri, 16 Jun 2023 03:12:50 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 16 Jun 2023 03:12:50 GMT
ARG KONG_VERSION=3.3.0
# Fri, 16 Jun 2023 03:12:50 GMT
ENV KONG_VERSION=3.3.0
# Fri, 16 Jun 2023 03:12:50 GMT
ARG KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b
# Fri, 16 Jun 2023 03:12:50 GMT
ARG KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
# Fri, 16 Jun 2023 03:13:20 GMT
# ARGS: KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 16 Jun 2023 03:13:21 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 16 Jun 2023 03:13:21 GMT
USER kong
# Fri, 16 Jun 2023 03:13:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 16 Jun 2023 03:13:21 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 16 Jun 2023 03:13:21 GMT
STOPSIGNAL SIGQUIT
# Fri, 16 Jun 2023 03:13:21 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 16 Jun 2023 03:13:21 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680f9a455927f5d901583f8890fea5cbb4c3293cae5709bd9e7df249a73f51b8`  
		Last Modified: Fri, 16 Jun 2023 03:15:15 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b2c1ee90db6284b0543979c2c3eec98e8d43362b7c6356ece9a0e8ecf99cec`  
		Last Modified: Fri, 16 Jun 2023 03:15:21 GMT  
		Size: 47.4 MB (47354643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052afa3d593dfd6a129bfa53bf0016759dbb5ed2f7324b6cfcc7200698e0ed03`  
		Last Modified: Fri, 16 Jun 2023 03:15:15 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:ubuntu`

```console
$ docker pull kong@sha256:09787b545ddd942214f97241433d5c22ad30124396d1c74333adc3e12b301481
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:74fd7d02fc80426128220c844b649ee80e078e0dcb4b2684c06b83636f4492e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81324591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46ac5c3d6929b19e745f738a7e38ffe7aac08c148cc07f5778b221c9c276ed78`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 05 Jun 2023 17:00:37 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:00:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:00:37 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:00:39 GMT
ADD file:0ad2ee2cfb186802f49c9bf4148674d1c6fc201f83478ec01ffaa7086d491323 in / 
# Mon, 05 Jun 2023 17:00:39 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:02:20 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 16 Jun 2023 03:02:20 GMT
ARG ASSET=ce
# Fri, 16 Jun 2023 03:02:20 GMT
ENV ASSET=ce
# Fri, 16 Jun 2023 03:02:20 GMT
ARG EE_PORTS
# Fri, 16 Jun 2023 03:02:20 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 16 Jun 2023 03:02:20 GMT
ARG KONG_VERSION=3.3.0
# Fri, 16 Jun 2023 03:02:20 GMT
ENV KONG_VERSION=3.3.0
# Fri, 16 Jun 2023 03:02:20 GMT
ARG KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b
# Fri, 16 Jun 2023 03:02:20 GMT
ARG KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
# Fri, 16 Jun 2023 03:03:00 GMT
# ARGS: KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 16 Jun 2023 03:03:01 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 16 Jun 2023 03:03:01 GMT
USER kong
# Fri, 16 Jun 2023 03:03:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 16 Jun 2023 03:03:01 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 16 Jun 2023 03:03:01 GMT
STOPSIGNAL SIGQUIT
# Fri, 16 Jun 2023 03:03:01 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 16 Jun 2023 03:03:01 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:3f94e4e483ea634d7ab0b63649b8f72f8b721d4c626297fd0edae0abea1df9e9`  
		Last Modified: Tue, 06 Jun 2023 11:46:33 GMT  
		Size: 30.4 MB (30431039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b770a78ff719726efe345cf12823afe49c4f5dcfdb7c5592748ab9952e0bc087`  
		Last Modified: Fri, 16 Jun 2023 03:05:00 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d8f511e7f8d6ec0ce9cbb5237ebd5f850a99daf26f983923273a4faf566e0a`  
		Last Modified: Fri, 16 Jun 2023 03:05:07 GMT  
		Size: 50.9 MB (50892272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f2a3e4dd7fc95c394ec37022ac3067a0f4831948c64a4417681a6d38b54a8a`  
		Last Modified: Fri, 16 Jun 2023 03:04:59 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:53004538dca8b628e4b41158806a88cb29436e78740b745e13dfa5e8b0a178b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75745127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f031d6ecb97c9cd35f241a18a86551ee1ba7caa78e70932024c32a5edf17acd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 05 Jun 2023 17:11:17 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:11:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:11:17 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 05 Jun 2023 17:11:19 GMT
ADD file:1043594b482384e967c94378b65ec4bc7a38190649a94f0325b7fb00be0a623e in / 
# Mon, 05 Jun 2023 17:11:19 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 03:12:49 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 16 Jun 2023 03:12:50 GMT
ARG ASSET=ce
# Fri, 16 Jun 2023 03:12:50 GMT
ENV ASSET=ce
# Fri, 16 Jun 2023 03:12:50 GMT
ARG EE_PORTS
# Fri, 16 Jun 2023 03:12:50 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 16 Jun 2023 03:12:50 GMT
ARG KONG_VERSION=3.3.0
# Fri, 16 Jun 2023 03:12:50 GMT
ENV KONG_VERSION=3.3.0
# Fri, 16 Jun 2023 03:12:50 GMT
ARG KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b
# Fri, 16 Jun 2023 03:12:50 GMT
ARG KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
# Fri, 16 Jun 2023 03:13:20 GMT
# ARGS: KONG_AMD64_SHA=e8c5fe8cacf19477d37a3b16375a263183f0c87c9ec217c4ead0c774d286be5b KONG_ARM64_SHA=2d918f7dd1ca5d54a6832cc370892a99af8e39fc4040df66d2d7ca6d97b9a2b5
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 16 Jun 2023 03:13:21 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 16 Jun 2023 03:13:21 GMT
USER kong
# Fri, 16 Jun 2023 03:13:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 16 Jun 2023 03:13:21 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 16 Jun 2023 03:13:21 GMT
STOPSIGNAL SIGQUIT
# Fri, 16 Jun 2023 03:13:21 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 16 Jun 2023 03:13:21 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:a1df1d4a17c6a461a5967be8a40f1158e55e0ae4dc3b3b7ae64f57cae69eb7e7`  
		Last Modified: Wed, 07 Jun 2023 02:07:18 GMT  
		Size: 28.4 MB (28389201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680f9a455927f5d901583f8890fea5cbb4c3293cae5709bd9e7df249a73f51b8`  
		Last Modified: Fri, 16 Jun 2023 03:15:15 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b2c1ee90db6284b0543979c2c3eec98e8d43362b7c6356ece9a0e8ecf99cec`  
		Last Modified: Fri, 16 Jun 2023 03:15:21 GMT  
		Size: 47.4 MB (47354643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052afa3d593dfd6a129bfa53bf0016759dbb5ed2f7324b6cfcc7200698e0ed03`  
		Last Modified: Fri, 16 Jun 2023 03:15:15 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
