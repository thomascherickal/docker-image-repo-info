<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kong`

-	[`kong:2.8`](#kong28)
-	[`kong:2.8-ubuntu`](#kong28-ubuntu)
-	[`kong:2.8.4`](#kong284)
-	[`kong:2.8.4-alpine`](#kong284-alpine)
-	[`kong:2.8.4-ubuntu`](#kong284-ubuntu)
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
-	[`kong:3.4`](#kong34)
-	[`kong:3.4-ubuntu`](#kong34-ubuntu)
-	[`kong:3.4.2`](#kong342)
-	[`kong:3.4.2-ubuntu`](#kong342-ubuntu)
-	[`kong:alpine`](#kongalpine)
-	[`kong:latest`](#konglatest)
-	[`kong:ubuntu`](#kongubuntu)

## `kong:2.8`

```console
$ docker pull kong@sha256:f23efb982519a4a2ad3585b374a11308fe45662706b7b70a09de06747ea81772
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.8` - linux; amd64

```console
$ docker pull kong@sha256:cf00e57a4a1b1f1cd5fb625e417a00fc8c6540fb57143f2e025b0ef264d586e2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48111526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c73b0a6c49643c6efe73acaed269e1db4c2bc0c2e3f3f32cb5c301d3d1ff856`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Wed, 04 Oct 2023 22:33:04 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 04 Oct 2023 22:33:05 GMT
ARG ASSET=ce
# Wed, 04 Oct 2023 22:33:05 GMT
ENV ASSET=ce
# Wed, 04 Oct 2023 22:33:05 GMT
ARG EE_PORTS
# Wed, 04 Oct 2023 22:33:05 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 04 Oct 2023 22:33:05 GMT
ARG KONG_VERSION=2.8.4
# Wed, 04 Oct 2023 22:33:05 GMT
ENV KONG_VERSION=2.8.4
# Wed, 04 Oct 2023 22:33:05 GMT
ARG KONG_AMD64_SHA=930b3b933b6c3f0393700433a919745900485d19e0cd8aba2d70aa066ccd10d2
# Wed, 04 Oct 2023 22:33:05 GMT
ARG KONG_ARM64_SHA=9027da2a4df477b462f34da9450412012ffdc0f9019e33ed7ff8e88f3df062c6
# Wed, 04 Oct 2023 22:33:14 GMT
# ARGS: KONG_AMD64_SHA=930b3b933b6c3f0393700433a919745900485d19e0cd8aba2d70aa066ccd10d2 KONG_ARM64_SHA=9027da2a4df477b462f34da9450412012ffdc0f9019e33ed7ff8e88f3df062c6
RUN set -eux;     arch="$(apk --print-arch)";     major_minor="$(echo "${KONG_VERSION%.*}" | tr -d '.')";     case "${arch}" in       x86_64) KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://packages.konghq.com/public/gateway-${major_minor}/raw/names/kong-${arch}/versions/${KONG_VERSION}/kong-${KONG_VERSION}.${arch}.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi     && mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Wed, 04 Oct 2023 22:33:15 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 04 Oct 2023 22:33:15 GMT
USER kong
# Wed, 04 Oct 2023 22:33:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 04 Oct 2023 22:33:15 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 04 Oct 2023 22:33:15 GMT
STOPSIGNAL SIGQUIT
# Wed, 04 Oct 2023 22:33:15 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "1m0s" "10s" "0s" '\n'}
# Wed, 04 Oct 2023 22:33:15 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fcf1971154a7cd0aa3e3d8903b45868c7b1e6d818b0caa3e17b6266e7cf2bd2`  
		Last Modified: Wed, 04 Oct 2023 22:35:05 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597c955e473f0dd0b2e5594aa721bc26451a355293b2c1609750968ce4027f5c`  
		Last Modified: Wed, 04 Oct 2023 22:35:11 GMT  
		Size: 44.7 MB (44708548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708ee02a72a39ebcc864778605e174c850ad93415d55423428aa1477da763843`  
		Last Modified: Wed, 04 Oct 2023 22:35:05 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.8` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:76a29bf815fe374566b837ef6f5694610f4ee97d1d0d8bd42c9f4321175e2252
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47431460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9383d141d52c248b85b37a5be7afccb459f7536ebf46adf9d2044526cc85270`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Wed, 04 Oct 2023 23:02:29 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 04 Oct 2023 23:02:29 GMT
ARG ASSET=ce
# Wed, 04 Oct 2023 23:02:29 GMT
ENV ASSET=ce
# Wed, 04 Oct 2023 23:02:29 GMT
ARG EE_PORTS
# Wed, 04 Oct 2023 23:02:29 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 04 Oct 2023 23:02:29 GMT
ARG KONG_VERSION=2.8.4
# Wed, 04 Oct 2023 23:02:29 GMT
ENV KONG_VERSION=2.8.4
# Wed, 04 Oct 2023 23:02:29 GMT
ARG KONG_AMD64_SHA=930b3b933b6c3f0393700433a919745900485d19e0cd8aba2d70aa066ccd10d2
# Wed, 04 Oct 2023 23:02:29 GMT
ARG KONG_ARM64_SHA=9027da2a4df477b462f34da9450412012ffdc0f9019e33ed7ff8e88f3df062c6
# Wed, 04 Oct 2023 23:02:38 GMT
# ARGS: KONG_AMD64_SHA=930b3b933b6c3f0393700433a919745900485d19e0cd8aba2d70aa066ccd10d2 KONG_ARM64_SHA=9027da2a4df477b462f34da9450412012ffdc0f9019e33ed7ff8e88f3df062c6
RUN set -eux;     arch="$(apk --print-arch)";     major_minor="$(echo "${KONG_VERSION%.*}" | tr -d '.')";     case "${arch}" in       x86_64) KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://packages.konghq.com/public/gateway-${major_minor}/raw/names/kong-${arch}/versions/${KONG_VERSION}/kong-${KONG_VERSION}.${arch}.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi     && mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Wed, 04 Oct 2023 23:02:38 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 04 Oct 2023 23:02:38 GMT
USER kong
# Wed, 04 Oct 2023 23:02:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 04 Oct 2023 23:02:39 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 04 Oct 2023 23:02:39 GMT
STOPSIGNAL SIGQUIT
# Wed, 04 Oct 2023 23:02:39 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "1m0s" "10s" "0s" '\n'}
# Wed, 04 Oct 2023 23:02:39 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01232959ebe8ac5e069edd0acf45fad85258df0f47c9864713209f8677dcc0bc`  
		Last Modified: Wed, 04 Oct 2023 23:04:10 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad9c2723eaf90728924ef882ba1a55263ff32c7fdafe9b3e437ee89ce971bab`  
		Last Modified: Wed, 04 Oct 2023 23:04:16 GMT  
		Size: 44.1 MB (44098619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8565503849b9d9c0b4e078ba8e6d3f00f923ed8c8d74cc19259451c80e26ae6d`  
		Last Modified: Wed, 04 Oct 2023 23:04:10 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.8-ubuntu`

```console
$ docker pull kong@sha256:1baf4542e28b389267fc93287c8007eae4408359c3ed20653d942fff87dec420
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.8-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:3976e71d53aac1481668e60228de4f89df5e64bf3308274d98d70f825ac84777
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.5 MB (116549583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb56012c6f3087fe21ea7da9bae0691a244e08f6ece3e940896da1e8d27939b2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 05 Oct 2023 07:33:30 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:33:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:33:32 GMT
ADD file:63d5ab3ef0aab308c0e71cb67292c5467f60deafa9b0418cbb220affcd078444 in / 
# Thu, 05 Oct 2023 07:33:32 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:31:02 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 07:31:03 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 07:31:03 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 07:31:03 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Fri, 13 Oct 2023 07:31:03 GMT
ARG KONG_VERSION=2.8.4
# Fri, 13 Oct 2023 07:31:03 GMT
ENV KONG_VERSION=2.8.4
# Fri, 13 Oct 2023 07:31:03 GMT
ARG KONG_AMD64_SHA=e4bc62c80f717114cc486776ee453931c5de0e8eaf0901ac11dbb4b2bae14534
# Fri, 13 Oct 2023 07:31:03 GMT
ARG KONG_ARM64_SHA=4fff44f9a0c7b06469591b7d1499a99a100109bc3f08dc412dd0eb38ff383d35
# Fri, 13 Oct 2023 07:31:25 GMT
# ARGS: KONG_AMD64_SHA=e4bc62c80f717114cc486776ee453931c5de0e8eaf0901ac11dbb4b2bae14534 KONG_ARM64_SHA=4fff44f9a0c7b06469591b7d1499a99a100109bc3f08dc412dd0eb38ff383d35
RUN set -ex;     arch=$(dpkg --print-architecture);     major_minor="$(echo "${KONG_VERSION%.*}" | tr -d '.')";     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       CODENAME=$(grep -m1 VERSION_CODENAME /etc/os-release | cut -d = -f 2);       apt-get install -y curl       && curl -fL "https://packages.konghq.com/public/gateway-${major_minor}/deb/ubuntu/pool/${CODENAME}/main/k/ko/kong_${KONG_VERSION}/kong_${KONG_VERSION}_${arch}.deb" -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi     && apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 07:31:26 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 07:31:26 GMT
USER kong
# Fri, 13 Oct 2023 07:31:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 07:31:26 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 07:31:26 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 07:31:26 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "1m0s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 07:31:26 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:43f89b94cd7df92a2f7e565b8fb1b7f502eff2cd225508cbd7ea2d36a9a3a601`  
		Last Modified: Thu, 05 Oct 2023 08:42:10 GMT  
		Size: 30.4 MB (30439111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe49fa7c25e2b7288668afcb8e156156114bef7b251cbf24faf391312eb8645e`  
		Last Modified: Fri, 13 Oct 2023 07:33:49 GMT  
		Size: 25.1 MB (25081963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1702d02c7856b0fde47caf2b899db523915489381171d8fd6aa171282d09a234`  
		Last Modified: Fri, 13 Oct 2023 07:33:57 GMT  
		Size: 61.0 MB (61027628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346776669b322c49e8351b6e84b0f5ee3825040e93c33b31ae2551c23e23eac8`  
		Last Modified: Fri, 13 Oct 2023 07:33:47 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.8-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:9734a2a340d635f6befaaa254c954797bdddff8e6a780046eb06c2f1a59f63c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.1 MB (113122623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4b39e558275ca6f1acb6b9018a446d9660761f1d3e7d36e31e7cfe34354750c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 05 Oct 2023 07:32:20 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:32:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:32:22 GMT
ADD file:f8594e26831508c318e42c8dfd9942041031087b8de1bf3fec11fd75b8b30fd4 in / 
# Thu, 05 Oct 2023 07:32:22 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 03:54:06 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 03:54:06 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 03:54:06 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 03:54:06 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Fri, 13 Oct 2023 03:54:06 GMT
ARG KONG_VERSION=2.8.4
# Fri, 13 Oct 2023 03:54:06 GMT
ENV KONG_VERSION=2.8.4
# Fri, 13 Oct 2023 03:54:06 GMT
ARG KONG_AMD64_SHA=e4bc62c80f717114cc486776ee453931c5de0e8eaf0901ac11dbb4b2bae14534
# Fri, 13 Oct 2023 03:54:07 GMT
ARG KONG_ARM64_SHA=4fff44f9a0c7b06469591b7d1499a99a100109bc3f08dc412dd0eb38ff383d35
# Fri, 13 Oct 2023 03:54:25 GMT
# ARGS: KONG_AMD64_SHA=e4bc62c80f717114cc486776ee453931c5de0e8eaf0901ac11dbb4b2bae14534 KONG_ARM64_SHA=4fff44f9a0c7b06469591b7d1499a99a100109bc3f08dc412dd0eb38ff383d35
RUN set -ex;     arch=$(dpkg --print-architecture);     major_minor="$(echo "${KONG_VERSION%.*}" | tr -d '.')";     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       CODENAME=$(grep -m1 VERSION_CODENAME /etc/os-release | cut -d = -f 2);       apt-get install -y curl       && curl -fL "https://packages.konghq.com/public/gateway-${major_minor}/deb/ubuntu/pool/${CODENAME}/main/k/ko/kong_${KONG_VERSION}/kong_${KONG_VERSION}_${arch}.deb" -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi     && apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 03:54:26 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 03:54:26 GMT
USER kong
# Fri, 13 Oct 2023 03:54:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 03:54:26 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 03:54:26 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 03:54:26 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "1m0s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 03:54:26 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:895d322e8e5957c04af3ab7b3431f2a562182d34167c6e159e02044150a66967`  
		Last Modified: Thu, 05 Oct 2023 08:57:30 GMT  
		Size: 28.4 MB (28391939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26665eea29a322fbd469277b677a4c57c88ecdccf02e8fb59023360990f21914`  
		Last Modified: Fri, 13 Oct 2023 03:56:32 GMT  
		Size: 25.1 MB (25081963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34aee2bba0788003261dfa6d49a1c327134e6e4d564cca5e2978f1bd6f837c7`  
		Last Modified: Fri, 13 Oct 2023 03:56:38 GMT  
		Size: 59.6 MB (59647841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91d817f3c9375cb458d1eedca17a71433308121e8796a328d92903aeb88ae652`  
		Last Modified: Fri, 13 Oct 2023 03:56:30 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.8.4`

```console
$ docker pull kong@sha256:f23efb982519a4a2ad3585b374a11308fe45662706b7b70a09de06747ea81772
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.8.4` - linux; amd64

```console
$ docker pull kong@sha256:cf00e57a4a1b1f1cd5fb625e417a00fc8c6540fb57143f2e025b0ef264d586e2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48111526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c73b0a6c49643c6efe73acaed269e1db4c2bc0c2e3f3f32cb5c301d3d1ff856`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Wed, 04 Oct 2023 22:33:04 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 04 Oct 2023 22:33:05 GMT
ARG ASSET=ce
# Wed, 04 Oct 2023 22:33:05 GMT
ENV ASSET=ce
# Wed, 04 Oct 2023 22:33:05 GMT
ARG EE_PORTS
# Wed, 04 Oct 2023 22:33:05 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 04 Oct 2023 22:33:05 GMT
ARG KONG_VERSION=2.8.4
# Wed, 04 Oct 2023 22:33:05 GMT
ENV KONG_VERSION=2.8.4
# Wed, 04 Oct 2023 22:33:05 GMT
ARG KONG_AMD64_SHA=930b3b933b6c3f0393700433a919745900485d19e0cd8aba2d70aa066ccd10d2
# Wed, 04 Oct 2023 22:33:05 GMT
ARG KONG_ARM64_SHA=9027da2a4df477b462f34da9450412012ffdc0f9019e33ed7ff8e88f3df062c6
# Wed, 04 Oct 2023 22:33:14 GMT
# ARGS: KONG_AMD64_SHA=930b3b933b6c3f0393700433a919745900485d19e0cd8aba2d70aa066ccd10d2 KONG_ARM64_SHA=9027da2a4df477b462f34da9450412012ffdc0f9019e33ed7ff8e88f3df062c6
RUN set -eux;     arch="$(apk --print-arch)";     major_minor="$(echo "${KONG_VERSION%.*}" | tr -d '.')";     case "${arch}" in       x86_64) KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://packages.konghq.com/public/gateway-${major_minor}/raw/names/kong-${arch}/versions/${KONG_VERSION}/kong-${KONG_VERSION}.${arch}.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi     && mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Wed, 04 Oct 2023 22:33:15 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 04 Oct 2023 22:33:15 GMT
USER kong
# Wed, 04 Oct 2023 22:33:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 04 Oct 2023 22:33:15 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 04 Oct 2023 22:33:15 GMT
STOPSIGNAL SIGQUIT
# Wed, 04 Oct 2023 22:33:15 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "1m0s" "10s" "0s" '\n'}
# Wed, 04 Oct 2023 22:33:15 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fcf1971154a7cd0aa3e3d8903b45868c7b1e6d818b0caa3e17b6266e7cf2bd2`  
		Last Modified: Wed, 04 Oct 2023 22:35:05 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597c955e473f0dd0b2e5594aa721bc26451a355293b2c1609750968ce4027f5c`  
		Last Modified: Wed, 04 Oct 2023 22:35:11 GMT  
		Size: 44.7 MB (44708548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708ee02a72a39ebcc864778605e174c850ad93415d55423428aa1477da763843`  
		Last Modified: Wed, 04 Oct 2023 22:35:05 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.8.4` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:76a29bf815fe374566b837ef6f5694610f4ee97d1d0d8bd42c9f4321175e2252
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47431460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9383d141d52c248b85b37a5be7afccb459f7536ebf46adf9d2044526cc85270`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Wed, 04 Oct 2023 23:02:29 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 04 Oct 2023 23:02:29 GMT
ARG ASSET=ce
# Wed, 04 Oct 2023 23:02:29 GMT
ENV ASSET=ce
# Wed, 04 Oct 2023 23:02:29 GMT
ARG EE_PORTS
# Wed, 04 Oct 2023 23:02:29 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 04 Oct 2023 23:02:29 GMT
ARG KONG_VERSION=2.8.4
# Wed, 04 Oct 2023 23:02:29 GMT
ENV KONG_VERSION=2.8.4
# Wed, 04 Oct 2023 23:02:29 GMT
ARG KONG_AMD64_SHA=930b3b933b6c3f0393700433a919745900485d19e0cd8aba2d70aa066ccd10d2
# Wed, 04 Oct 2023 23:02:29 GMT
ARG KONG_ARM64_SHA=9027da2a4df477b462f34da9450412012ffdc0f9019e33ed7ff8e88f3df062c6
# Wed, 04 Oct 2023 23:02:38 GMT
# ARGS: KONG_AMD64_SHA=930b3b933b6c3f0393700433a919745900485d19e0cd8aba2d70aa066ccd10d2 KONG_ARM64_SHA=9027da2a4df477b462f34da9450412012ffdc0f9019e33ed7ff8e88f3df062c6
RUN set -eux;     arch="$(apk --print-arch)";     major_minor="$(echo "${KONG_VERSION%.*}" | tr -d '.')";     case "${arch}" in       x86_64) KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://packages.konghq.com/public/gateway-${major_minor}/raw/names/kong-${arch}/versions/${KONG_VERSION}/kong-${KONG_VERSION}.${arch}.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi     && mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Wed, 04 Oct 2023 23:02:38 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 04 Oct 2023 23:02:38 GMT
USER kong
# Wed, 04 Oct 2023 23:02:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 04 Oct 2023 23:02:39 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 04 Oct 2023 23:02:39 GMT
STOPSIGNAL SIGQUIT
# Wed, 04 Oct 2023 23:02:39 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "1m0s" "10s" "0s" '\n'}
# Wed, 04 Oct 2023 23:02:39 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01232959ebe8ac5e069edd0acf45fad85258df0f47c9864713209f8677dcc0bc`  
		Last Modified: Wed, 04 Oct 2023 23:04:10 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad9c2723eaf90728924ef882ba1a55263ff32c7fdafe9b3e437ee89ce971bab`  
		Last Modified: Wed, 04 Oct 2023 23:04:16 GMT  
		Size: 44.1 MB (44098619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8565503849b9d9c0b4e078ba8e6d3f00f923ed8c8d74cc19259451c80e26ae6d`  
		Last Modified: Wed, 04 Oct 2023 23:04:10 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.8.4-alpine`

```console
$ docker pull kong@sha256:f23efb982519a4a2ad3585b374a11308fe45662706b7b70a09de06747ea81772
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.8.4-alpine` - linux; amd64

```console
$ docker pull kong@sha256:cf00e57a4a1b1f1cd5fb625e417a00fc8c6540fb57143f2e025b0ef264d586e2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48111526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c73b0a6c49643c6efe73acaed269e1db4c2bc0c2e3f3f32cb5c301d3d1ff856`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Wed, 04 Oct 2023 22:33:04 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 04 Oct 2023 22:33:05 GMT
ARG ASSET=ce
# Wed, 04 Oct 2023 22:33:05 GMT
ENV ASSET=ce
# Wed, 04 Oct 2023 22:33:05 GMT
ARG EE_PORTS
# Wed, 04 Oct 2023 22:33:05 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 04 Oct 2023 22:33:05 GMT
ARG KONG_VERSION=2.8.4
# Wed, 04 Oct 2023 22:33:05 GMT
ENV KONG_VERSION=2.8.4
# Wed, 04 Oct 2023 22:33:05 GMT
ARG KONG_AMD64_SHA=930b3b933b6c3f0393700433a919745900485d19e0cd8aba2d70aa066ccd10d2
# Wed, 04 Oct 2023 22:33:05 GMT
ARG KONG_ARM64_SHA=9027da2a4df477b462f34da9450412012ffdc0f9019e33ed7ff8e88f3df062c6
# Wed, 04 Oct 2023 22:33:14 GMT
# ARGS: KONG_AMD64_SHA=930b3b933b6c3f0393700433a919745900485d19e0cd8aba2d70aa066ccd10d2 KONG_ARM64_SHA=9027da2a4df477b462f34da9450412012ffdc0f9019e33ed7ff8e88f3df062c6
RUN set -eux;     arch="$(apk --print-arch)";     major_minor="$(echo "${KONG_VERSION%.*}" | tr -d '.')";     case "${arch}" in       x86_64) KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://packages.konghq.com/public/gateway-${major_minor}/raw/names/kong-${arch}/versions/${KONG_VERSION}/kong-${KONG_VERSION}.${arch}.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi     && mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Wed, 04 Oct 2023 22:33:15 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 04 Oct 2023 22:33:15 GMT
USER kong
# Wed, 04 Oct 2023 22:33:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 04 Oct 2023 22:33:15 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 04 Oct 2023 22:33:15 GMT
STOPSIGNAL SIGQUIT
# Wed, 04 Oct 2023 22:33:15 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "1m0s" "10s" "0s" '\n'}
# Wed, 04 Oct 2023 22:33:15 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fcf1971154a7cd0aa3e3d8903b45868c7b1e6d818b0caa3e17b6266e7cf2bd2`  
		Last Modified: Wed, 04 Oct 2023 22:35:05 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597c955e473f0dd0b2e5594aa721bc26451a355293b2c1609750968ce4027f5c`  
		Last Modified: Wed, 04 Oct 2023 22:35:11 GMT  
		Size: 44.7 MB (44708548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708ee02a72a39ebcc864778605e174c850ad93415d55423428aa1477da763843`  
		Last Modified: Wed, 04 Oct 2023 22:35:05 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.8.4-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:76a29bf815fe374566b837ef6f5694610f4ee97d1d0d8bd42c9f4321175e2252
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47431460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9383d141d52c248b85b37a5be7afccb459f7536ebf46adf9d2044526cc85270`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Wed, 04 Oct 2023 23:02:29 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 04 Oct 2023 23:02:29 GMT
ARG ASSET=ce
# Wed, 04 Oct 2023 23:02:29 GMT
ENV ASSET=ce
# Wed, 04 Oct 2023 23:02:29 GMT
ARG EE_PORTS
# Wed, 04 Oct 2023 23:02:29 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 04 Oct 2023 23:02:29 GMT
ARG KONG_VERSION=2.8.4
# Wed, 04 Oct 2023 23:02:29 GMT
ENV KONG_VERSION=2.8.4
# Wed, 04 Oct 2023 23:02:29 GMT
ARG KONG_AMD64_SHA=930b3b933b6c3f0393700433a919745900485d19e0cd8aba2d70aa066ccd10d2
# Wed, 04 Oct 2023 23:02:29 GMT
ARG KONG_ARM64_SHA=9027da2a4df477b462f34da9450412012ffdc0f9019e33ed7ff8e88f3df062c6
# Wed, 04 Oct 2023 23:02:38 GMT
# ARGS: KONG_AMD64_SHA=930b3b933b6c3f0393700433a919745900485d19e0cd8aba2d70aa066ccd10d2 KONG_ARM64_SHA=9027da2a4df477b462f34da9450412012ffdc0f9019e33ed7ff8e88f3df062c6
RUN set -eux;     arch="$(apk --print-arch)";     major_minor="$(echo "${KONG_VERSION%.*}" | tr -d '.')";     case "${arch}" in       x86_64) KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://packages.konghq.com/public/gateway-${major_minor}/raw/names/kong-${arch}/versions/${KONG_VERSION}/kong-${KONG_VERSION}.${arch}.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi     && mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Wed, 04 Oct 2023 23:02:38 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 04 Oct 2023 23:02:38 GMT
USER kong
# Wed, 04 Oct 2023 23:02:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 04 Oct 2023 23:02:39 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 04 Oct 2023 23:02:39 GMT
STOPSIGNAL SIGQUIT
# Wed, 04 Oct 2023 23:02:39 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "1m0s" "10s" "0s" '\n'}
# Wed, 04 Oct 2023 23:02:39 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01232959ebe8ac5e069edd0acf45fad85258df0f47c9864713209f8677dcc0bc`  
		Last Modified: Wed, 04 Oct 2023 23:04:10 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad9c2723eaf90728924ef882ba1a55263ff32c7fdafe9b3e437ee89ce971bab`  
		Last Modified: Wed, 04 Oct 2023 23:04:16 GMT  
		Size: 44.1 MB (44098619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8565503849b9d9c0b4e078ba8e6d3f00f923ed8c8d74cc19259451c80e26ae6d`  
		Last Modified: Wed, 04 Oct 2023 23:04:10 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.8.4-ubuntu`

```console
$ docker pull kong@sha256:1baf4542e28b389267fc93287c8007eae4408359c3ed20653d942fff87dec420
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.8.4-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:3976e71d53aac1481668e60228de4f89df5e64bf3308274d98d70f825ac84777
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.5 MB (116549583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb56012c6f3087fe21ea7da9bae0691a244e08f6ece3e940896da1e8d27939b2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 05 Oct 2023 07:33:30 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:33:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:33:32 GMT
ADD file:63d5ab3ef0aab308c0e71cb67292c5467f60deafa9b0418cbb220affcd078444 in / 
# Thu, 05 Oct 2023 07:33:32 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:31:02 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 07:31:03 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 07:31:03 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 07:31:03 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Fri, 13 Oct 2023 07:31:03 GMT
ARG KONG_VERSION=2.8.4
# Fri, 13 Oct 2023 07:31:03 GMT
ENV KONG_VERSION=2.8.4
# Fri, 13 Oct 2023 07:31:03 GMT
ARG KONG_AMD64_SHA=e4bc62c80f717114cc486776ee453931c5de0e8eaf0901ac11dbb4b2bae14534
# Fri, 13 Oct 2023 07:31:03 GMT
ARG KONG_ARM64_SHA=4fff44f9a0c7b06469591b7d1499a99a100109bc3f08dc412dd0eb38ff383d35
# Fri, 13 Oct 2023 07:31:25 GMT
# ARGS: KONG_AMD64_SHA=e4bc62c80f717114cc486776ee453931c5de0e8eaf0901ac11dbb4b2bae14534 KONG_ARM64_SHA=4fff44f9a0c7b06469591b7d1499a99a100109bc3f08dc412dd0eb38ff383d35
RUN set -ex;     arch=$(dpkg --print-architecture);     major_minor="$(echo "${KONG_VERSION%.*}" | tr -d '.')";     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       CODENAME=$(grep -m1 VERSION_CODENAME /etc/os-release | cut -d = -f 2);       apt-get install -y curl       && curl -fL "https://packages.konghq.com/public/gateway-${major_minor}/deb/ubuntu/pool/${CODENAME}/main/k/ko/kong_${KONG_VERSION}/kong_${KONG_VERSION}_${arch}.deb" -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi     && apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 07:31:26 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 07:31:26 GMT
USER kong
# Fri, 13 Oct 2023 07:31:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 07:31:26 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 07:31:26 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 07:31:26 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "1m0s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 07:31:26 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:43f89b94cd7df92a2f7e565b8fb1b7f502eff2cd225508cbd7ea2d36a9a3a601`  
		Last Modified: Thu, 05 Oct 2023 08:42:10 GMT  
		Size: 30.4 MB (30439111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe49fa7c25e2b7288668afcb8e156156114bef7b251cbf24faf391312eb8645e`  
		Last Modified: Fri, 13 Oct 2023 07:33:49 GMT  
		Size: 25.1 MB (25081963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1702d02c7856b0fde47caf2b899db523915489381171d8fd6aa171282d09a234`  
		Last Modified: Fri, 13 Oct 2023 07:33:57 GMT  
		Size: 61.0 MB (61027628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346776669b322c49e8351b6e84b0f5ee3825040e93c33b31ae2551c23e23eac8`  
		Last Modified: Fri, 13 Oct 2023 07:33:47 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.8.4-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:9734a2a340d635f6befaaa254c954797bdddff8e6a780046eb06c2f1a59f63c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.1 MB (113122623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4b39e558275ca6f1acb6b9018a446d9660761f1d3e7d36e31e7cfe34354750c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 05 Oct 2023 07:32:20 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:32:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:32:22 GMT
ADD file:f8594e26831508c318e42c8dfd9942041031087b8de1bf3fec11fd75b8b30fd4 in / 
# Thu, 05 Oct 2023 07:32:22 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 03:54:06 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 03:54:06 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 03:54:06 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 03:54:06 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Fri, 13 Oct 2023 03:54:06 GMT
ARG KONG_VERSION=2.8.4
# Fri, 13 Oct 2023 03:54:06 GMT
ENV KONG_VERSION=2.8.4
# Fri, 13 Oct 2023 03:54:06 GMT
ARG KONG_AMD64_SHA=e4bc62c80f717114cc486776ee453931c5de0e8eaf0901ac11dbb4b2bae14534
# Fri, 13 Oct 2023 03:54:07 GMT
ARG KONG_ARM64_SHA=4fff44f9a0c7b06469591b7d1499a99a100109bc3f08dc412dd0eb38ff383d35
# Fri, 13 Oct 2023 03:54:25 GMT
# ARGS: KONG_AMD64_SHA=e4bc62c80f717114cc486776ee453931c5de0e8eaf0901ac11dbb4b2bae14534 KONG_ARM64_SHA=4fff44f9a0c7b06469591b7d1499a99a100109bc3f08dc412dd0eb38ff383d35
RUN set -ex;     arch=$(dpkg --print-architecture);     major_minor="$(echo "${KONG_VERSION%.*}" | tr -d '.')";     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       CODENAME=$(grep -m1 VERSION_CODENAME /etc/os-release | cut -d = -f 2);       apt-get install -y curl       && curl -fL "https://packages.konghq.com/public/gateway-${major_minor}/deb/ubuntu/pool/${CODENAME}/main/k/ko/kong_${KONG_VERSION}/kong_${KONG_VERSION}_${arch}.deb" -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi     && apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 03:54:26 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 03:54:26 GMT
USER kong
# Fri, 13 Oct 2023 03:54:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 03:54:26 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 03:54:26 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 03:54:26 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "1m0s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 03:54:26 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:895d322e8e5957c04af3ab7b3431f2a562182d34167c6e159e02044150a66967`  
		Last Modified: Thu, 05 Oct 2023 08:57:30 GMT  
		Size: 28.4 MB (28391939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26665eea29a322fbd469277b677a4c57c88ecdccf02e8fb59023360990f21914`  
		Last Modified: Fri, 13 Oct 2023 03:56:32 GMT  
		Size: 25.1 MB (25081963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34aee2bba0788003261dfa6d49a1c327134e6e4d564cca5e2978f1bd6f837c7`  
		Last Modified: Fri, 13 Oct 2023 03:56:38 GMT  
		Size: 59.6 MB (59647841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91d817f3c9375cb458d1eedca17a71433308121e8796a328d92903aeb88ae652`  
		Last Modified: Fri, 13 Oct 2023 03:56:30 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3`

```console
$ docker pull kong@sha256:6b5506ae271bc252fe9594a808db7146b488e0a88966c640d320abd6dedc1ef2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3` - linux; amd64

```console
$ docker pull kong@sha256:11116706f624bd4cf92a18c9ae614628db8bd5788b7406eb07896862ddb1da4f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93175019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7fabd29ce8cdbab7ae27f755052f60f1cf548d07f4f7f2dff8614946a3a07c4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 05 Oct 2023 07:33:30 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:33:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:33:32 GMT
ADD file:63d5ab3ef0aab308c0e71cb67292c5467f60deafa9b0418cbb220affcd078444 in / 
# Thu, 05 Oct 2023 07:33:32 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:28:30 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 13 Oct 2023 07:28:30 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 07:28:30 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 07:28:30 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 07:28:30 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 13 Oct 2023 07:28:30 GMT
ARG KONG_VERSION=3.4.2
# Fri, 13 Oct 2023 07:28:31 GMT
ENV KONG_VERSION=3.4.2
# Fri, 13 Oct 2023 07:28:31 GMT
ARG KONG_AMD64_SHA=b6bf56a5088660e7cac748a005af8d977be7177e64b0abfe1e7f77d797cdc0e2
# Fri, 13 Oct 2023 07:28:31 GMT
ARG KONG_ARM64_SHA=8bca79a6337a6299316cca4e2f9a766df09268359292686498db18a48d883689
# Fri, 13 Oct 2023 07:28:49 GMT
# ARGS: KONG_AMD64_SHA=b6bf56a5088660e7cac748a005af8d977be7177e64b0abfe1e7f77d797cdc0e2 KONG_ARM64_SHA=8bca79a6337a6299316cca4e2f9a766df09268359292686498db18a48d883689
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y --no-install-recommends curl ca-certificates       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes --no-install-recommends /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 07:28:50 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 07:28:50 GMT
USER kong
# Fri, 13 Oct 2023 07:28:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 07:28:50 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 07:28:50 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 07:28:50 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 07:28:50 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:43f89b94cd7df92a2f7e565b8fb1b7f502eff2cd225508cbd7ea2d36a9a3a601`  
		Last Modified: Thu, 05 Oct 2023 08:42:10 GMT  
		Size: 30.4 MB (30439111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676526cf23951612fff170db505ac909b79f87739dc8b7dd9ed856ae710da9b6`  
		Last Modified: Fri, 13 Oct 2023 07:31:52 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d5013df765c3cd670061a26110d49400b487e4b8cf32dc3064f2015f0a3c7e`  
		Last Modified: Fri, 13 Oct 2023 07:32:02 GMT  
		Size: 62.7 MB (62734627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df25283763c84405dba67bbe987e73bee45b491a7db05c40f3f6fe23fbf66b22`  
		Last Modified: Fri, 13 Oct 2023 07:31:52 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:f57a09ff69a0d431c58fbf856358804a776aed167cb093231840722d2a68a317
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.6 MB (89561608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74f7cdc7bf980ab8c7a02630be0dceaace6a4d23886be7fd1ab4774398f82503`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 05 Oct 2023 07:32:20 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:32:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:32:22 GMT
ADD file:f8594e26831508c318e42c8dfd9942041031087b8de1bf3fec11fd75b8b30fd4 in / 
# Thu, 05 Oct 2023 07:32:22 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 03:52:02 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 13 Oct 2023 03:52:02 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 03:52:02 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 03:52:02 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 03:52:02 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 13 Oct 2023 03:52:02 GMT
ARG KONG_VERSION=3.4.2
# Fri, 13 Oct 2023 03:52:02 GMT
ENV KONG_VERSION=3.4.2
# Fri, 13 Oct 2023 03:52:02 GMT
ARG KONG_AMD64_SHA=b6bf56a5088660e7cac748a005af8d977be7177e64b0abfe1e7f77d797cdc0e2
# Fri, 13 Oct 2023 03:52:02 GMT
ARG KONG_ARM64_SHA=8bca79a6337a6299316cca4e2f9a766df09268359292686498db18a48d883689
# Fri, 13 Oct 2023 03:52:20 GMT
# ARGS: KONG_AMD64_SHA=b6bf56a5088660e7cac748a005af8d977be7177e64b0abfe1e7f77d797cdc0e2 KONG_ARM64_SHA=8bca79a6337a6299316cca4e2f9a766df09268359292686498db18a48d883689
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y --no-install-recommends curl ca-certificates       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes --no-install-recommends /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 03:52:21 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 03:52:21 GMT
USER kong
# Fri, 13 Oct 2023 03:52:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 03:52:21 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 03:52:22 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 03:52:22 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 03:52:22 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:895d322e8e5957c04af3ab7b3431f2a562182d34167c6e159e02044150a66967`  
		Last Modified: Thu, 05 Oct 2023 08:57:30 GMT  
		Size: 28.4 MB (28391939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4eb9336ac11e4c267c309924d9e2989161e7930966c2b551b0de49623951691`  
		Last Modified: Fri, 13 Oct 2023 03:54:48 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72627dd6b77fdc810bbd21463b5c05d892e09189e42be4c8d7c71e1b06e5a7b7`  
		Last Modified: Fri, 13 Oct 2023 03:54:56 GMT  
		Size: 61.2 MB (61168390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba1271a9a34893cea35e4c19b85ca607fef78046cb6baa5ad6f2936ae009043`  
		Last Modified: Fri, 13 Oct 2023 03:54:48 GMT  
		Size: 1.2 KB (1156 bytes)  
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
$ docker pull kong@sha256:99c7d653c0bfd368e1cb5d811dc1be295acf5c519b4461e0f5b086e71b4cee0f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.0-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:cd0fc578d7b3fa5d1574426d54d89a173773f0caed7d961f165ac608474d5154
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101878925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29d52165577d37d93609b41a37f9ea288e06e2826b56b6cabf5ce30d0ba3fff3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 03 Oct 2023 10:45:50 GMT
ARG RELEASE
# Tue, 03 Oct 2023 10:45:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 10:45:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 10:45:50 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 10:45:51 GMT
ADD file:4809da414c2d478b4d991cbdaa2df457f2b3d07d0ff6cf673f09a66f90833e81 in / 
# Tue, 03 Oct 2023 10:45:52 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:30:00 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 13 Oct 2023 07:30:00 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 07:30:00 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 07:30:00 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 07:30:00 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 13 Oct 2023 07:30:31 GMT
ARG KONG_VERSION=3.0.2
# Fri, 13 Oct 2023 07:30:31 GMT
ENV KONG_VERSION=3.0.2
# Fri, 13 Oct 2023 07:30:31 GMT
ARG KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396
# Fri, 13 Oct 2023 07:30:31 GMT
ARG KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
# Fri, 13 Oct 2023 07:30:54 GMT
# ARGS: KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396 KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 07:30:55 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 07:30:55 GMT
USER kong
# Fri, 13 Oct 2023 07:30:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 07:30:55 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 07:30:55 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 07:30:55 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 07:30:55 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:7a2c559011895d255fce249c00396abff5ae7e0c0a92931d0ed493e71de78e3a`  
		Last Modified: Tue, 03 Oct 2023 17:02:08 GMT  
		Size: 28.6 MB (28580681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d353d9e29f4083dc54fb8aaa3c2a8c3acd2b323e46c6e661530332f0d0de4f5b`  
		Last Modified: Fri, 13 Oct 2023 07:33:05 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdc2e2de06e7a5c2b76d72d73abb37ed8f039f1fb7ff342c1b22ffb4c9ba013`  
		Last Modified: Fri, 13 Oct 2023 07:33:38 GMT  
		Size: 73.3 MB (73297239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f1cc1e36ab8890a8c98443b8be385f77876df3b458fcb415bd354ef513e769`  
		Last Modified: Fri, 13 Oct 2023 07:33:27 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.0-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:ce796693cb43d768a5db05af72831253ab15371e2a3f701a808a4008a796cd02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99134607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb1d33a12407ecf5fc716353f1cd087774822c2f71ba754d280aa990f4eec104`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 03 Oct 2023 11:04:09 GMT
ARG RELEASE
# Tue, 03 Oct 2023 11:04:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 11:04:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 11:04:10 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 11:04:16 GMT
ADD file:f70cc2610ea8fcd25e6e9ae727eb9345d5b7198102f6a6d8e458ab8f99efefc3 in / 
# Tue, 03 Oct 2023 11:04:17 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 03:53:06 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 13 Oct 2023 03:53:06 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 03:53:06 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 03:53:06 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 03:53:06 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 13 Oct 2023 03:53:41 GMT
ARG KONG_VERSION=3.0.2
# Fri, 13 Oct 2023 03:53:41 GMT
ENV KONG_VERSION=3.0.2
# Fri, 13 Oct 2023 03:53:41 GMT
ARG KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396
# Fri, 13 Oct 2023 03:53:41 GMT
ARG KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
# Fri, 13 Oct 2023 03:54:00 GMT
# ARGS: KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396 KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 03:54:01 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 03:54:01 GMT
USER kong
# Fri, 13 Oct 2023 03:54:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 03:54:01 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 03:54:01 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 03:54:01 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 03:54:01 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:6cba4020c0a193cd551ed8edf368670967e3546345b52c4ec66cb0931436e9b9`  
		Last Modified: Thu, 05 Oct 2023 12:12:17 GMT  
		Size: 27.2 MB (27199503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56cd9e4c848af2df3b1f46417e685175dbea6cea79b54605c2eb3a08143e050`  
		Last Modified: Fri, 13 Oct 2023 03:55:53 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3433a78a7e7d0abfe4b6020c5b65e1b354ea85dec48ded07756e9436a8f77bfd`  
		Last Modified: Fri, 13 Oct 2023 03:56:20 GMT  
		Size: 71.9 MB (71934100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de778c7694e3f2d671397e209b131152cb07cd95c3f1624b87529b586946b7e`  
		Last Modified: Fri, 13 Oct 2023 03:56:11 GMT  
		Size: 879.0 B  
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
$ docker pull kong@sha256:99c7d653c0bfd368e1cb5d811dc1be295acf5c519b4461e0f5b086e71b4cee0f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.0.2-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:cd0fc578d7b3fa5d1574426d54d89a173773f0caed7d961f165ac608474d5154
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101878925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29d52165577d37d93609b41a37f9ea288e06e2826b56b6cabf5ce30d0ba3fff3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 03 Oct 2023 10:45:50 GMT
ARG RELEASE
# Tue, 03 Oct 2023 10:45:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 10:45:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 10:45:50 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 10:45:51 GMT
ADD file:4809da414c2d478b4d991cbdaa2df457f2b3d07d0ff6cf673f09a66f90833e81 in / 
# Tue, 03 Oct 2023 10:45:52 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:30:00 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 13 Oct 2023 07:30:00 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 07:30:00 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 07:30:00 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 07:30:00 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 13 Oct 2023 07:30:31 GMT
ARG KONG_VERSION=3.0.2
# Fri, 13 Oct 2023 07:30:31 GMT
ENV KONG_VERSION=3.0.2
# Fri, 13 Oct 2023 07:30:31 GMT
ARG KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396
# Fri, 13 Oct 2023 07:30:31 GMT
ARG KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
# Fri, 13 Oct 2023 07:30:54 GMT
# ARGS: KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396 KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 07:30:55 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 07:30:55 GMT
USER kong
# Fri, 13 Oct 2023 07:30:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 07:30:55 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 07:30:55 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 07:30:55 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 07:30:55 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:7a2c559011895d255fce249c00396abff5ae7e0c0a92931d0ed493e71de78e3a`  
		Last Modified: Tue, 03 Oct 2023 17:02:08 GMT  
		Size: 28.6 MB (28580681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d353d9e29f4083dc54fb8aaa3c2a8c3acd2b323e46c6e661530332f0d0de4f5b`  
		Last Modified: Fri, 13 Oct 2023 07:33:05 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdc2e2de06e7a5c2b76d72d73abb37ed8f039f1fb7ff342c1b22ffb4c9ba013`  
		Last Modified: Fri, 13 Oct 2023 07:33:38 GMT  
		Size: 73.3 MB (73297239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96f1cc1e36ab8890a8c98443b8be385f77876df3b458fcb415bd354ef513e769`  
		Last Modified: Fri, 13 Oct 2023 07:33:27 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.0.2-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:ce796693cb43d768a5db05af72831253ab15371e2a3f701a808a4008a796cd02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.1 MB (99134607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb1d33a12407ecf5fc716353f1cd087774822c2f71ba754d280aa990f4eec104`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 03 Oct 2023 11:04:09 GMT
ARG RELEASE
# Tue, 03 Oct 2023 11:04:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 11:04:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 11:04:10 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 11:04:16 GMT
ADD file:f70cc2610ea8fcd25e6e9ae727eb9345d5b7198102f6a6d8e458ab8f99efefc3 in / 
# Tue, 03 Oct 2023 11:04:17 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 03:53:06 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 13 Oct 2023 03:53:06 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 03:53:06 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 03:53:06 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 03:53:06 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 13 Oct 2023 03:53:41 GMT
ARG KONG_VERSION=3.0.2
# Fri, 13 Oct 2023 03:53:41 GMT
ENV KONG_VERSION=3.0.2
# Fri, 13 Oct 2023 03:53:41 GMT
ARG KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396
# Fri, 13 Oct 2023 03:53:41 GMT
ARG KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
# Fri, 13 Oct 2023 03:54:00 GMT
# ARGS: KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396 KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 03:54:01 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 03:54:01 GMT
USER kong
# Fri, 13 Oct 2023 03:54:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 03:54:01 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 03:54:01 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 03:54:01 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 03:54:01 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:6cba4020c0a193cd551ed8edf368670967e3546345b52c4ec66cb0931436e9b9`  
		Last Modified: Thu, 05 Oct 2023 12:12:17 GMT  
		Size: 27.2 MB (27199503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56cd9e4c848af2df3b1f46417e685175dbea6cea79b54605c2eb3a08143e050`  
		Last Modified: Fri, 13 Oct 2023 03:55:53 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3433a78a7e7d0abfe4b6020c5b65e1b354ea85dec48ded07756e9436a8f77bfd`  
		Last Modified: Fri, 13 Oct 2023 03:56:20 GMT  
		Size: 71.9 MB (71934100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de778c7694e3f2d671397e209b131152cb07cd95c3f1624b87529b586946b7e`  
		Last Modified: Fri, 13 Oct 2023 03:56:11 GMT  
		Size: 879.0 B  
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
$ docker pull kong@sha256:f12138e78e74be62291f2c7509df262cb48c0ee8a1cca43b4204a5172615e05c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.1-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:9d918ec2750493a7005d50fc538c5f71692d89736b5ac145ab113f663044918e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101908651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:001ee1c1c185ad9c273e99227c7aa06834c2807378d8802fe229284056877dba`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 03 Oct 2023 10:45:50 GMT
ARG RELEASE
# Tue, 03 Oct 2023 10:45:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 10:45:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 10:45:50 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 10:45:51 GMT
ADD file:4809da414c2d478b4d991cbdaa2df457f2b3d07d0ff6cf673f09a66f90833e81 in / 
# Tue, 03 Oct 2023 10:45:52 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:30:00 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 13 Oct 2023 07:30:00 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 07:30:00 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 07:30:00 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 07:30:00 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 13 Oct 2023 07:30:00 GMT
ARG KONG_VERSION=3.1.1
# Fri, 13 Oct 2023 07:30:00 GMT
ENV KONG_VERSION=3.1.1
# Fri, 13 Oct 2023 07:30:00 GMT
ARG KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b
# Fri, 13 Oct 2023 07:30:01 GMT
ARG KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
# Fri, 13 Oct 2023 07:30:24 GMT
# ARGS: KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 07:30:25 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 07:30:25 GMT
USER kong
# Fri, 13 Oct 2023 07:30:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 07:30:26 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 07:30:26 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 07:30:26 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 07:30:26 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:7a2c559011895d255fce249c00396abff5ae7e0c0a92931d0ed493e71de78e3a`  
		Last Modified: Tue, 03 Oct 2023 17:02:08 GMT  
		Size: 28.6 MB (28580681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d353d9e29f4083dc54fb8aaa3c2a8c3acd2b323e46c6e661530332f0d0de4f5b`  
		Last Modified: Fri, 13 Oct 2023 07:33:05 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b8665cbf5d23d5120327135c9176afec4fe6a44241ee7d509b6db82d85941e`  
		Last Modified: Fri, 13 Oct 2023 07:33:17 GMT  
		Size: 73.3 MB (73326965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2055abc93184439b0ae50dbbed41d87c14e5f42d869f2860a7a928109c64dbe3`  
		Last Modified: Fri, 13 Oct 2023 07:33:06 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.1-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:91d6576396659ee01577a7fdad7f40be9a70a3544e02e0f52161640b2eef8176
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99162663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:013a974ce75706d181cd7a8619840d30932b2f281303962d9b1ca0a68836f586`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 03 Oct 2023 11:04:09 GMT
ARG RELEASE
# Tue, 03 Oct 2023 11:04:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 11:04:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 11:04:10 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 11:04:16 GMT
ADD file:f70cc2610ea8fcd25e6e9ae727eb9345d5b7198102f6a6d8e458ab8f99efefc3 in / 
# Tue, 03 Oct 2023 11:04:17 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 03:53:06 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 13 Oct 2023 03:53:06 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 03:53:06 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 03:53:06 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 03:53:06 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 13 Oct 2023 03:53:06 GMT
ARG KONG_VERSION=3.1.1
# Fri, 13 Oct 2023 03:53:06 GMT
ENV KONG_VERSION=3.1.1
# Fri, 13 Oct 2023 03:53:06 GMT
ARG KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b
# Fri, 13 Oct 2023 03:53:06 GMT
ARG KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
# Fri, 13 Oct 2023 03:53:35 GMT
# ARGS: KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 03:53:36 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 03:53:36 GMT
USER kong
# Fri, 13 Oct 2023 03:53:36 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 03:53:36 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 03:53:36 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 03:53:36 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 03:53:36 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:6cba4020c0a193cd551ed8edf368670967e3546345b52c4ec66cb0931436e9b9`  
		Last Modified: Thu, 05 Oct 2023 12:12:17 GMT  
		Size: 27.2 MB (27199503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56cd9e4c848af2df3b1f46417e685175dbea6cea79b54605c2eb3a08143e050`  
		Last Modified: Fri, 13 Oct 2023 03:55:53 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39053bd209e78485f7075fc7537de10de2fd04c583501936d9497ee1b353f756`  
		Last Modified: Fri, 13 Oct 2023 03:56:02 GMT  
		Size: 72.0 MB (71962154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:591a220d51bd7d1e993bbbbcd6be269108168dfd7090833c24079c52d4ca9803`  
		Last Modified: Fri, 13 Oct 2023 03:55:53 GMT  
		Size: 881.0 B  
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
$ docker pull kong@sha256:f12138e78e74be62291f2c7509df262cb48c0ee8a1cca43b4204a5172615e05c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.1.1-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:9d918ec2750493a7005d50fc538c5f71692d89736b5ac145ab113f663044918e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.9 MB (101908651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:001ee1c1c185ad9c273e99227c7aa06834c2807378d8802fe229284056877dba`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 03 Oct 2023 10:45:50 GMT
ARG RELEASE
# Tue, 03 Oct 2023 10:45:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 10:45:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 10:45:50 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 10:45:51 GMT
ADD file:4809da414c2d478b4d991cbdaa2df457f2b3d07d0ff6cf673f09a66f90833e81 in / 
# Tue, 03 Oct 2023 10:45:52 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:30:00 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 13 Oct 2023 07:30:00 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 07:30:00 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 07:30:00 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 07:30:00 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 13 Oct 2023 07:30:00 GMT
ARG KONG_VERSION=3.1.1
# Fri, 13 Oct 2023 07:30:00 GMT
ENV KONG_VERSION=3.1.1
# Fri, 13 Oct 2023 07:30:00 GMT
ARG KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b
# Fri, 13 Oct 2023 07:30:01 GMT
ARG KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
# Fri, 13 Oct 2023 07:30:24 GMT
# ARGS: KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 07:30:25 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 07:30:25 GMT
USER kong
# Fri, 13 Oct 2023 07:30:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 07:30:26 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 07:30:26 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 07:30:26 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 07:30:26 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:7a2c559011895d255fce249c00396abff5ae7e0c0a92931d0ed493e71de78e3a`  
		Last Modified: Tue, 03 Oct 2023 17:02:08 GMT  
		Size: 28.6 MB (28580681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d353d9e29f4083dc54fb8aaa3c2a8c3acd2b323e46c6e661530332f0d0de4f5b`  
		Last Modified: Fri, 13 Oct 2023 07:33:05 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b8665cbf5d23d5120327135c9176afec4fe6a44241ee7d509b6db82d85941e`  
		Last Modified: Fri, 13 Oct 2023 07:33:17 GMT  
		Size: 73.3 MB (73326965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2055abc93184439b0ae50dbbed41d87c14e5f42d869f2860a7a928109c64dbe3`  
		Last Modified: Fri, 13 Oct 2023 07:33:06 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.1.1-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:91d6576396659ee01577a7fdad7f40be9a70a3544e02e0f52161640b2eef8176
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99162663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:013a974ce75706d181cd7a8619840d30932b2f281303962d9b1ca0a68836f586`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 03 Oct 2023 11:04:09 GMT
ARG RELEASE
# Tue, 03 Oct 2023 11:04:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 11:04:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 11:04:10 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 11:04:16 GMT
ADD file:f70cc2610ea8fcd25e6e9ae727eb9345d5b7198102f6a6d8e458ab8f99efefc3 in / 
# Tue, 03 Oct 2023 11:04:17 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 03:53:06 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 13 Oct 2023 03:53:06 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 03:53:06 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 03:53:06 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 03:53:06 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 13 Oct 2023 03:53:06 GMT
ARG KONG_VERSION=3.1.1
# Fri, 13 Oct 2023 03:53:06 GMT
ENV KONG_VERSION=3.1.1
# Fri, 13 Oct 2023 03:53:06 GMT
ARG KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b
# Fri, 13 Oct 2023 03:53:06 GMT
ARG KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
# Fri, 13 Oct 2023 03:53:35 GMT
# ARGS: KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 03:53:36 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 03:53:36 GMT
USER kong
# Fri, 13 Oct 2023 03:53:36 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 03:53:36 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 03:53:36 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 03:53:36 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 03:53:36 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:6cba4020c0a193cd551ed8edf368670967e3546345b52c4ec66cb0931436e9b9`  
		Last Modified: Thu, 05 Oct 2023 12:12:17 GMT  
		Size: 27.2 MB (27199503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56cd9e4c848af2df3b1f46417e685175dbea6cea79b54605c2eb3a08143e050`  
		Last Modified: Fri, 13 Oct 2023 03:55:53 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39053bd209e78485f7075fc7537de10de2fd04c583501936d9497ee1b353f756`  
		Last Modified: Fri, 13 Oct 2023 03:56:02 GMT  
		Size: 72.0 MB (71962154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:591a220d51bd7d1e993bbbbcd6be269108168dfd7090833c24079c52d4ca9803`  
		Last Modified: Fri, 13 Oct 2023 03:55:53 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.2`

```console
$ docker pull kong@sha256:40ba22637e7e2c9cb5289f4b35cae77698c56eee2a900229c6209d593115d3ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.2` - linux; amd64

```console
$ docker pull kong@sha256:1cf3925fdda3705e8cd9e8a943ec9b8154544e7b60894c2b2e9018c5f5d6f16b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.5 MB (74497345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e03bf0667a84cea37f31e1b62949273e7031073d721b55a6dfc3f7adeb11f103`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 05 Oct 2023 07:33:30 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:33:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:33:32 GMT
ADD file:63d5ab3ef0aab308c0e71cb67292c5467f60deafa9b0418cbb220affcd078444 in / 
# Thu, 05 Oct 2023 07:33:32 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:28:30 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 13 Oct 2023 07:28:30 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 07:28:30 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 07:28:30 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 07:28:30 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 13 Oct 2023 07:29:33 GMT
ARG KONG_VERSION=3.2.2
# Fri, 13 Oct 2023 07:29:33 GMT
ENV KONG_VERSION=3.2.2
# Fri, 13 Oct 2023 07:29:33 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Fri, 13 Oct 2023 07:29:34 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Fri, 13 Oct 2023 07:29:51 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 07:29:52 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 07:29:52 GMT
USER kong
# Fri, 13 Oct 2023 07:29:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 07:29:52 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 07:29:52 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 07:29:52 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 07:29:53 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:43f89b94cd7df92a2f7e565b8fb1b7f502eff2cd225508cbd7ea2d36a9a3a601`  
		Last Modified: Thu, 05 Oct 2023 08:42:10 GMT  
		Size: 30.4 MB (30439111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676526cf23951612fff170db505ac909b79f87739dc8b7dd9ed856ae710da9b6`  
		Last Modified: Fri, 13 Oct 2023 07:31:52 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:213c776f6936ac9434ef008dfbc93c88aef4f06dd0d1c1ae38de8edc45dd56ed`  
		Last Modified: Fri, 13 Oct 2023 07:32:48 GMT  
		Size: 44.1 MB (44056956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e40245655de1b28c9980b4e731666b7cdb155bb251533cd1f27919d3778d38fc`  
		Last Modified: Fri, 13 Oct 2023 07:32:41 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.2` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:a6848eb55034ae60d631b33a533fb343d87de6b03df99255fbd091106bda98f5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.6 MB (78616304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b0b86db1f7e9d2288644536ce43f03c3175677b0c0a698c3ee59765415f6b75`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 05 Oct 2023 07:32:20 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:32:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:32:22 GMT
ADD file:f8594e26831508c318e42c8dfd9942041031087b8de1bf3fec11fd75b8b30fd4 in / 
# Thu, 05 Oct 2023 07:32:22 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 03:52:02 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 13 Oct 2023 03:52:02 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 03:52:02 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 03:52:02 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 03:52:02 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 13 Oct 2023 03:52:45 GMT
ARG KONG_VERSION=3.2.2
# Fri, 13 Oct 2023 03:52:45 GMT
ENV KONG_VERSION=3.2.2
# Fri, 13 Oct 2023 03:52:45 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Fri, 13 Oct 2023 03:52:45 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Fri, 13 Oct 2023 03:53:01 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 03:53:02 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 03:53:02 GMT
USER kong
# Fri, 13 Oct 2023 03:53:02 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 03:53:02 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 03:53:02 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 03:53:02 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 03:53:02 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:895d322e8e5957c04af3ab7b3431f2a562182d34167c6e159e02044150a66967`  
		Last Modified: Thu, 05 Oct 2023 08:57:30 GMT  
		Size: 28.4 MB (28391939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4eb9336ac11e4c267c309924d9e2989161e7930966c2b551b0de49623951691`  
		Last Modified: Fri, 13 Oct 2023 03:54:48 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2559520ef4c4dd535afa82720395f3cc00b685bafa1a5f11b54c960a21fcfbb8`  
		Last Modified: Fri, 13 Oct 2023 03:55:39 GMT  
		Size: 50.2 MB (50223089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:861df4f16e7b6e722a718ecc89581dcbf13b711802b225d1c2f169f07b6d05d1`  
		Last Modified: Fri, 13 Oct 2023 03:55:33 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.2-ubuntu`

```console
$ docker pull kong@sha256:40ba22637e7e2c9cb5289f4b35cae77698c56eee2a900229c6209d593115d3ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.2-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:1cf3925fdda3705e8cd9e8a943ec9b8154544e7b60894c2b2e9018c5f5d6f16b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.5 MB (74497345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e03bf0667a84cea37f31e1b62949273e7031073d721b55a6dfc3f7adeb11f103`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 05 Oct 2023 07:33:30 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:33:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:33:32 GMT
ADD file:63d5ab3ef0aab308c0e71cb67292c5467f60deafa9b0418cbb220affcd078444 in / 
# Thu, 05 Oct 2023 07:33:32 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:28:30 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 13 Oct 2023 07:28:30 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 07:28:30 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 07:28:30 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 07:28:30 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 13 Oct 2023 07:29:33 GMT
ARG KONG_VERSION=3.2.2
# Fri, 13 Oct 2023 07:29:33 GMT
ENV KONG_VERSION=3.2.2
# Fri, 13 Oct 2023 07:29:33 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Fri, 13 Oct 2023 07:29:34 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Fri, 13 Oct 2023 07:29:51 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 07:29:52 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 07:29:52 GMT
USER kong
# Fri, 13 Oct 2023 07:29:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 07:29:52 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 07:29:52 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 07:29:52 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 07:29:53 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:43f89b94cd7df92a2f7e565b8fb1b7f502eff2cd225508cbd7ea2d36a9a3a601`  
		Last Modified: Thu, 05 Oct 2023 08:42:10 GMT  
		Size: 30.4 MB (30439111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676526cf23951612fff170db505ac909b79f87739dc8b7dd9ed856ae710da9b6`  
		Last Modified: Fri, 13 Oct 2023 07:31:52 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:213c776f6936ac9434ef008dfbc93c88aef4f06dd0d1c1ae38de8edc45dd56ed`  
		Last Modified: Fri, 13 Oct 2023 07:32:48 GMT  
		Size: 44.1 MB (44056956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e40245655de1b28c9980b4e731666b7cdb155bb251533cd1f27919d3778d38fc`  
		Last Modified: Fri, 13 Oct 2023 07:32:41 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.2-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:a6848eb55034ae60d631b33a533fb343d87de6b03df99255fbd091106bda98f5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.6 MB (78616304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b0b86db1f7e9d2288644536ce43f03c3175677b0c0a698c3ee59765415f6b75`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 05 Oct 2023 07:32:20 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:32:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:32:22 GMT
ADD file:f8594e26831508c318e42c8dfd9942041031087b8de1bf3fec11fd75b8b30fd4 in / 
# Thu, 05 Oct 2023 07:32:22 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 03:52:02 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 13 Oct 2023 03:52:02 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 03:52:02 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 03:52:02 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 03:52:02 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 13 Oct 2023 03:52:45 GMT
ARG KONG_VERSION=3.2.2
# Fri, 13 Oct 2023 03:52:45 GMT
ENV KONG_VERSION=3.2.2
# Fri, 13 Oct 2023 03:52:45 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Fri, 13 Oct 2023 03:52:45 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Fri, 13 Oct 2023 03:53:01 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 03:53:02 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 03:53:02 GMT
USER kong
# Fri, 13 Oct 2023 03:53:02 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 03:53:02 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 03:53:02 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 03:53:02 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 03:53:02 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:895d322e8e5957c04af3ab7b3431f2a562182d34167c6e159e02044150a66967`  
		Last Modified: Thu, 05 Oct 2023 08:57:30 GMT  
		Size: 28.4 MB (28391939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4eb9336ac11e4c267c309924d9e2989161e7930966c2b551b0de49623951691`  
		Last Modified: Fri, 13 Oct 2023 03:54:48 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2559520ef4c4dd535afa82720395f3cc00b685bafa1a5f11b54c960a21fcfbb8`  
		Last Modified: Fri, 13 Oct 2023 03:55:39 GMT  
		Size: 50.2 MB (50223089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:861df4f16e7b6e722a718ecc89581dcbf13b711802b225d1c2f169f07b6d05d1`  
		Last Modified: Fri, 13 Oct 2023 03:55:33 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.2.2`

```console
$ docker pull kong@sha256:40ba22637e7e2c9cb5289f4b35cae77698c56eee2a900229c6209d593115d3ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.2.2` - linux; amd64

```console
$ docker pull kong@sha256:1cf3925fdda3705e8cd9e8a943ec9b8154544e7b60894c2b2e9018c5f5d6f16b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.5 MB (74497345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e03bf0667a84cea37f31e1b62949273e7031073d721b55a6dfc3f7adeb11f103`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 05 Oct 2023 07:33:30 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:33:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:33:32 GMT
ADD file:63d5ab3ef0aab308c0e71cb67292c5467f60deafa9b0418cbb220affcd078444 in / 
# Thu, 05 Oct 2023 07:33:32 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:28:30 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 13 Oct 2023 07:28:30 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 07:28:30 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 07:28:30 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 07:28:30 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 13 Oct 2023 07:29:33 GMT
ARG KONG_VERSION=3.2.2
# Fri, 13 Oct 2023 07:29:33 GMT
ENV KONG_VERSION=3.2.2
# Fri, 13 Oct 2023 07:29:33 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Fri, 13 Oct 2023 07:29:34 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Fri, 13 Oct 2023 07:29:51 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 07:29:52 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 07:29:52 GMT
USER kong
# Fri, 13 Oct 2023 07:29:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 07:29:52 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 07:29:52 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 07:29:52 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 07:29:53 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:43f89b94cd7df92a2f7e565b8fb1b7f502eff2cd225508cbd7ea2d36a9a3a601`  
		Last Modified: Thu, 05 Oct 2023 08:42:10 GMT  
		Size: 30.4 MB (30439111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676526cf23951612fff170db505ac909b79f87739dc8b7dd9ed856ae710da9b6`  
		Last Modified: Fri, 13 Oct 2023 07:31:52 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:213c776f6936ac9434ef008dfbc93c88aef4f06dd0d1c1ae38de8edc45dd56ed`  
		Last Modified: Fri, 13 Oct 2023 07:32:48 GMT  
		Size: 44.1 MB (44056956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e40245655de1b28c9980b4e731666b7cdb155bb251533cd1f27919d3778d38fc`  
		Last Modified: Fri, 13 Oct 2023 07:32:41 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.2.2` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:a6848eb55034ae60d631b33a533fb343d87de6b03df99255fbd091106bda98f5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.6 MB (78616304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b0b86db1f7e9d2288644536ce43f03c3175677b0c0a698c3ee59765415f6b75`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 05 Oct 2023 07:32:20 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:32:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:32:22 GMT
ADD file:f8594e26831508c318e42c8dfd9942041031087b8de1bf3fec11fd75b8b30fd4 in / 
# Thu, 05 Oct 2023 07:32:22 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 03:52:02 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 13 Oct 2023 03:52:02 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 03:52:02 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 03:52:02 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 03:52:02 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 13 Oct 2023 03:52:45 GMT
ARG KONG_VERSION=3.2.2
# Fri, 13 Oct 2023 03:52:45 GMT
ENV KONG_VERSION=3.2.2
# Fri, 13 Oct 2023 03:52:45 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Fri, 13 Oct 2023 03:52:45 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Fri, 13 Oct 2023 03:53:01 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 03:53:02 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 03:53:02 GMT
USER kong
# Fri, 13 Oct 2023 03:53:02 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 03:53:02 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 03:53:02 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 03:53:02 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 03:53:02 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:895d322e8e5957c04af3ab7b3431f2a562182d34167c6e159e02044150a66967`  
		Last Modified: Thu, 05 Oct 2023 08:57:30 GMT  
		Size: 28.4 MB (28391939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4eb9336ac11e4c267c309924d9e2989161e7930966c2b551b0de49623951691`  
		Last Modified: Fri, 13 Oct 2023 03:54:48 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2559520ef4c4dd535afa82720395f3cc00b685bafa1a5f11b54c960a21fcfbb8`  
		Last Modified: Fri, 13 Oct 2023 03:55:39 GMT  
		Size: 50.2 MB (50223089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:861df4f16e7b6e722a718ecc89581dcbf13b711802b225d1c2f169f07b6d05d1`  
		Last Modified: Fri, 13 Oct 2023 03:55:33 GMT  
		Size: 1.2 KB (1153 bytes)  
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
$ docker pull kong@sha256:40ba22637e7e2c9cb5289f4b35cae77698c56eee2a900229c6209d593115d3ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.2.2-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:1cf3925fdda3705e8cd9e8a943ec9b8154544e7b60894c2b2e9018c5f5d6f16b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.5 MB (74497345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e03bf0667a84cea37f31e1b62949273e7031073d721b55a6dfc3f7adeb11f103`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 05 Oct 2023 07:33:30 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:33:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:33:32 GMT
ADD file:63d5ab3ef0aab308c0e71cb67292c5467f60deafa9b0418cbb220affcd078444 in / 
# Thu, 05 Oct 2023 07:33:32 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:28:30 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 13 Oct 2023 07:28:30 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 07:28:30 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 07:28:30 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 07:28:30 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 13 Oct 2023 07:29:33 GMT
ARG KONG_VERSION=3.2.2
# Fri, 13 Oct 2023 07:29:33 GMT
ENV KONG_VERSION=3.2.2
# Fri, 13 Oct 2023 07:29:33 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Fri, 13 Oct 2023 07:29:34 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Fri, 13 Oct 2023 07:29:51 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 07:29:52 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 07:29:52 GMT
USER kong
# Fri, 13 Oct 2023 07:29:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 07:29:52 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 07:29:52 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 07:29:52 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 07:29:53 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:43f89b94cd7df92a2f7e565b8fb1b7f502eff2cd225508cbd7ea2d36a9a3a601`  
		Last Modified: Thu, 05 Oct 2023 08:42:10 GMT  
		Size: 30.4 MB (30439111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676526cf23951612fff170db505ac909b79f87739dc8b7dd9ed856ae710da9b6`  
		Last Modified: Fri, 13 Oct 2023 07:31:52 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:213c776f6936ac9434ef008dfbc93c88aef4f06dd0d1c1ae38de8edc45dd56ed`  
		Last Modified: Fri, 13 Oct 2023 07:32:48 GMT  
		Size: 44.1 MB (44056956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e40245655de1b28c9980b4e731666b7cdb155bb251533cd1f27919d3778d38fc`  
		Last Modified: Fri, 13 Oct 2023 07:32:41 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.2.2-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:a6848eb55034ae60d631b33a533fb343d87de6b03df99255fbd091106bda98f5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.6 MB (78616304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b0b86db1f7e9d2288644536ce43f03c3175677b0c0a698c3ee59765415f6b75`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 05 Oct 2023 07:32:20 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:32:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:32:22 GMT
ADD file:f8594e26831508c318e42c8dfd9942041031087b8de1bf3fec11fd75b8b30fd4 in / 
# Thu, 05 Oct 2023 07:32:22 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 03:52:02 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 13 Oct 2023 03:52:02 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 03:52:02 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 03:52:02 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 03:52:02 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 13 Oct 2023 03:52:45 GMT
ARG KONG_VERSION=3.2.2
# Fri, 13 Oct 2023 03:52:45 GMT
ENV KONG_VERSION=3.2.2
# Fri, 13 Oct 2023 03:52:45 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Fri, 13 Oct 2023 03:52:45 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Fri, 13 Oct 2023 03:53:01 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 03:53:02 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 03:53:02 GMT
USER kong
# Fri, 13 Oct 2023 03:53:02 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 03:53:02 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 03:53:02 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 03:53:02 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 03:53:02 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:895d322e8e5957c04af3ab7b3431f2a562182d34167c6e159e02044150a66967`  
		Last Modified: Thu, 05 Oct 2023 08:57:30 GMT  
		Size: 28.4 MB (28391939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4eb9336ac11e4c267c309924d9e2989161e7930966c2b551b0de49623951691`  
		Last Modified: Fri, 13 Oct 2023 03:54:48 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2559520ef4c4dd535afa82720395f3cc00b685bafa1a5f11b54c960a21fcfbb8`  
		Last Modified: Fri, 13 Oct 2023 03:55:39 GMT  
		Size: 50.2 MB (50223089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:861df4f16e7b6e722a718ecc89581dcbf13b711802b225d1c2f169f07b6d05d1`  
		Last Modified: Fri, 13 Oct 2023 03:55:33 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.3`

```console
$ docker pull kong@sha256:cef6b14b25cd30a090fa0692e9ded6e7debe8db961f08ef7d54fb383346768c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.3` - linux; amd64

```console
$ docker pull kong@sha256:284d5f410d44c40b8e3793d5c23321a76e44ff6c2ac2aa356d0e5bea7d1c2166
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.4 MB (81350005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c66031a94022bbd56c6fee05c159bb917a175d557b2fa53aea66934f9a94c5fc`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 05 Oct 2023 07:33:30 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:33:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:33:32 GMT
ADD file:63d5ab3ef0aab308c0e71cb67292c5467f60deafa9b0418cbb220affcd078444 in / 
# Thu, 05 Oct 2023 07:33:32 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:28:30 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 13 Oct 2023 07:28:30 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 07:28:30 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 07:28:30 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 07:28:30 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 13 Oct 2023 07:28:57 GMT
ARG KONG_VERSION=3.3.1
# Fri, 13 Oct 2023 07:28:57 GMT
ENV KONG_VERSION=3.3.1
# Fri, 13 Oct 2023 07:28:57 GMT
ARG KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20
# Fri, 13 Oct 2023 07:28:57 GMT
ARG KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
# Fri, 13 Oct 2023 07:29:25 GMT
# ARGS: KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20 KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 07:29:26 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 07:29:26 GMT
USER kong
# Fri, 13 Oct 2023 07:29:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 07:29:26 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 07:29:26 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 07:29:27 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 07:29:27 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:43f89b94cd7df92a2f7e565b8fb1b7f502eff2cd225508cbd7ea2d36a9a3a601`  
		Last Modified: Thu, 05 Oct 2023 08:42:10 GMT  
		Size: 30.4 MB (30439111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676526cf23951612fff170db505ac909b79f87739dc8b7dd9ed856ae710da9b6`  
		Last Modified: Fri, 13 Oct 2023 07:31:52 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4def0d602c5984e4453aa39b7e3e3e1e896cbd21c1f6bdf5d8c5b6f9d7f408d9`  
		Last Modified: Fri, 13 Oct 2023 07:32:27 GMT  
		Size: 50.9 MB (50909614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:277217efd2742c7f82e9389429a9bfa2ddcbf4347fb992ba93f051e47c9fb025`  
		Last Modified: Fri, 13 Oct 2023 07:32:20 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.3` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:7d14713d357aeaab02ceeaa45d5f0ed89e2230235ed3b780d99f004f3c9aa60f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.8 MB (75769288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0884155d3564ce1d9c0ccda4ac3753a48929dee3f423320bd6ddd490c135723`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 05 Oct 2023 07:32:20 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:32:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:32:22 GMT
ADD file:f8594e26831508c318e42c8dfd9942041031087b8de1bf3fec11fd75b8b30fd4 in / 
# Thu, 05 Oct 2023 07:32:22 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 03:52:02 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 13 Oct 2023 03:52:02 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 03:52:02 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 03:52:02 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 03:52:02 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 13 Oct 2023 03:52:25 GMT
ARG KONG_VERSION=3.3.1
# Fri, 13 Oct 2023 03:52:25 GMT
ENV KONG_VERSION=3.3.1
# Fri, 13 Oct 2023 03:52:25 GMT
ARG KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20
# Fri, 13 Oct 2023 03:52:25 GMT
ARG KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
# Fri, 13 Oct 2023 03:52:41 GMT
# ARGS: KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20 KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 03:52:42 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 03:52:42 GMT
USER kong
# Fri, 13 Oct 2023 03:52:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 03:52:42 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 03:52:42 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 03:52:42 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 03:52:42 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:895d322e8e5957c04af3ab7b3431f2a562182d34167c6e159e02044150a66967`  
		Last Modified: Thu, 05 Oct 2023 08:57:30 GMT  
		Size: 28.4 MB (28391939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4eb9336ac11e4c267c309924d9e2989161e7930966c2b551b0de49623951691`  
		Last Modified: Fri, 13 Oct 2023 03:54:48 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0996f4d7bc2002dad66156c70889f5c98f7b663458df7a8e18f03b51439dda`  
		Last Modified: Fri, 13 Oct 2023 03:55:20 GMT  
		Size: 47.4 MB (47376070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c0a200877adb59005e5dd2713d041b397fd7d777d45b251b368347c6f47969`  
		Last Modified: Fri, 13 Oct 2023 03:55:14 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.3-ubuntu`

```console
$ docker pull kong@sha256:cef6b14b25cd30a090fa0692e9ded6e7debe8db961f08ef7d54fb383346768c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.3-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:284d5f410d44c40b8e3793d5c23321a76e44ff6c2ac2aa356d0e5bea7d1c2166
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.4 MB (81350005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c66031a94022bbd56c6fee05c159bb917a175d557b2fa53aea66934f9a94c5fc`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 05 Oct 2023 07:33:30 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:33:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:33:32 GMT
ADD file:63d5ab3ef0aab308c0e71cb67292c5467f60deafa9b0418cbb220affcd078444 in / 
# Thu, 05 Oct 2023 07:33:32 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:28:30 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 13 Oct 2023 07:28:30 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 07:28:30 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 07:28:30 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 07:28:30 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 13 Oct 2023 07:28:57 GMT
ARG KONG_VERSION=3.3.1
# Fri, 13 Oct 2023 07:28:57 GMT
ENV KONG_VERSION=3.3.1
# Fri, 13 Oct 2023 07:28:57 GMT
ARG KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20
# Fri, 13 Oct 2023 07:28:57 GMT
ARG KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
# Fri, 13 Oct 2023 07:29:25 GMT
# ARGS: KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20 KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 07:29:26 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 07:29:26 GMT
USER kong
# Fri, 13 Oct 2023 07:29:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 07:29:26 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 07:29:26 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 07:29:27 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 07:29:27 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:43f89b94cd7df92a2f7e565b8fb1b7f502eff2cd225508cbd7ea2d36a9a3a601`  
		Last Modified: Thu, 05 Oct 2023 08:42:10 GMT  
		Size: 30.4 MB (30439111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676526cf23951612fff170db505ac909b79f87739dc8b7dd9ed856ae710da9b6`  
		Last Modified: Fri, 13 Oct 2023 07:31:52 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4def0d602c5984e4453aa39b7e3e3e1e896cbd21c1f6bdf5d8c5b6f9d7f408d9`  
		Last Modified: Fri, 13 Oct 2023 07:32:27 GMT  
		Size: 50.9 MB (50909614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:277217efd2742c7f82e9389429a9bfa2ddcbf4347fb992ba93f051e47c9fb025`  
		Last Modified: Fri, 13 Oct 2023 07:32:20 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.3-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:7d14713d357aeaab02ceeaa45d5f0ed89e2230235ed3b780d99f004f3c9aa60f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.8 MB (75769288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0884155d3564ce1d9c0ccda4ac3753a48929dee3f423320bd6ddd490c135723`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 05 Oct 2023 07:32:20 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:32:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:32:22 GMT
ADD file:f8594e26831508c318e42c8dfd9942041031087b8de1bf3fec11fd75b8b30fd4 in / 
# Thu, 05 Oct 2023 07:32:22 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 03:52:02 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 13 Oct 2023 03:52:02 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 03:52:02 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 03:52:02 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 03:52:02 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 13 Oct 2023 03:52:25 GMT
ARG KONG_VERSION=3.3.1
# Fri, 13 Oct 2023 03:52:25 GMT
ENV KONG_VERSION=3.3.1
# Fri, 13 Oct 2023 03:52:25 GMT
ARG KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20
# Fri, 13 Oct 2023 03:52:25 GMT
ARG KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
# Fri, 13 Oct 2023 03:52:41 GMT
# ARGS: KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20 KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 03:52:42 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 03:52:42 GMT
USER kong
# Fri, 13 Oct 2023 03:52:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 03:52:42 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 03:52:42 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 03:52:42 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 03:52:42 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:895d322e8e5957c04af3ab7b3431f2a562182d34167c6e159e02044150a66967`  
		Last Modified: Thu, 05 Oct 2023 08:57:30 GMT  
		Size: 28.4 MB (28391939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4eb9336ac11e4c267c309924d9e2989161e7930966c2b551b0de49623951691`  
		Last Modified: Fri, 13 Oct 2023 03:54:48 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0996f4d7bc2002dad66156c70889f5c98f7b663458df7a8e18f03b51439dda`  
		Last Modified: Fri, 13 Oct 2023 03:55:20 GMT  
		Size: 47.4 MB (47376070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c0a200877adb59005e5dd2713d041b397fd7d777d45b251b368347c6f47969`  
		Last Modified: Fri, 13 Oct 2023 03:55:14 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.3.1`

```console
$ docker pull kong@sha256:cef6b14b25cd30a090fa0692e9ded6e7debe8db961f08ef7d54fb383346768c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.3.1` - linux; amd64

```console
$ docker pull kong@sha256:284d5f410d44c40b8e3793d5c23321a76e44ff6c2ac2aa356d0e5bea7d1c2166
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.4 MB (81350005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c66031a94022bbd56c6fee05c159bb917a175d557b2fa53aea66934f9a94c5fc`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 05 Oct 2023 07:33:30 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:33:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:33:32 GMT
ADD file:63d5ab3ef0aab308c0e71cb67292c5467f60deafa9b0418cbb220affcd078444 in / 
# Thu, 05 Oct 2023 07:33:32 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:28:30 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 13 Oct 2023 07:28:30 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 07:28:30 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 07:28:30 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 07:28:30 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 13 Oct 2023 07:28:57 GMT
ARG KONG_VERSION=3.3.1
# Fri, 13 Oct 2023 07:28:57 GMT
ENV KONG_VERSION=3.3.1
# Fri, 13 Oct 2023 07:28:57 GMT
ARG KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20
# Fri, 13 Oct 2023 07:28:57 GMT
ARG KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
# Fri, 13 Oct 2023 07:29:25 GMT
# ARGS: KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20 KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 07:29:26 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 07:29:26 GMT
USER kong
# Fri, 13 Oct 2023 07:29:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 07:29:26 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 07:29:26 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 07:29:27 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 07:29:27 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:43f89b94cd7df92a2f7e565b8fb1b7f502eff2cd225508cbd7ea2d36a9a3a601`  
		Last Modified: Thu, 05 Oct 2023 08:42:10 GMT  
		Size: 30.4 MB (30439111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676526cf23951612fff170db505ac909b79f87739dc8b7dd9ed856ae710da9b6`  
		Last Modified: Fri, 13 Oct 2023 07:31:52 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4def0d602c5984e4453aa39b7e3e3e1e896cbd21c1f6bdf5d8c5b6f9d7f408d9`  
		Last Modified: Fri, 13 Oct 2023 07:32:27 GMT  
		Size: 50.9 MB (50909614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:277217efd2742c7f82e9389429a9bfa2ddcbf4347fb992ba93f051e47c9fb025`  
		Last Modified: Fri, 13 Oct 2023 07:32:20 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.3.1` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:7d14713d357aeaab02ceeaa45d5f0ed89e2230235ed3b780d99f004f3c9aa60f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.8 MB (75769288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0884155d3564ce1d9c0ccda4ac3753a48929dee3f423320bd6ddd490c135723`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 05 Oct 2023 07:32:20 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:32:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:32:22 GMT
ADD file:f8594e26831508c318e42c8dfd9942041031087b8de1bf3fec11fd75b8b30fd4 in / 
# Thu, 05 Oct 2023 07:32:22 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 03:52:02 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 13 Oct 2023 03:52:02 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 03:52:02 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 03:52:02 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 03:52:02 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 13 Oct 2023 03:52:25 GMT
ARG KONG_VERSION=3.3.1
# Fri, 13 Oct 2023 03:52:25 GMT
ENV KONG_VERSION=3.3.1
# Fri, 13 Oct 2023 03:52:25 GMT
ARG KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20
# Fri, 13 Oct 2023 03:52:25 GMT
ARG KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
# Fri, 13 Oct 2023 03:52:41 GMT
# ARGS: KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20 KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 03:52:42 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 03:52:42 GMT
USER kong
# Fri, 13 Oct 2023 03:52:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 03:52:42 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 03:52:42 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 03:52:42 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 03:52:42 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:895d322e8e5957c04af3ab7b3431f2a562182d34167c6e159e02044150a66967`  
		Last Modified: Thu, 05 Oct 2023 08:57:30 GMT  
		Size: 28.4 MB (28391939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4eb9336ac11e4c267c309924d9e2989161e7930966c2b551b0de49623951691`  
		Last Modified: Fri, 13 Oct 2023 03:54:48 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0996f4d7bc2002dad66156c70889f5c98f7b663458df7a8e18f03b51439dda`  
		Last Modified: Fri, 13 Oct 2023 03:55:20 GMT  
		Size: 47.4 MB (47376070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c0a200877adb59005e5dd2713d041b397fd7d777d45b251b368347c6f47969`  
		Last Modified: Fri, 13 Oct 2023 03:55:14 GMT  
		Size: 1.2 KB (1156 bytes)  
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
$ docker pull kong@sha256:cef6b14b25cd30a090fa0692e9ded6e7debe8db961f08ef7d54fb383346768c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.3.1-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:284d5f410d44c40b8e3793d5c23321a76e44ff6c2ac2aa356d0e5bea7d1c2166
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.4 MB (81350005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c66031a94022bbd56c6fee05c159bb917a175d557b2fa53aea66934f9a94c5fc`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 05 Oct 2023 07:33:30 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:33:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:33:32 GMT
ADD file:63d5ab3ef0aab308c0e71cb67292c5467f60deafa9b0418cbb220affcd078444 in / 
# Thu, 05 Oct 2023 07:33:32 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:28:30 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 13 Oct 2023 07:28:30 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 07:28:30 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 07:28:30 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 07:28:30 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 13 Oct 2023 07:28:57 GMT
ARG KONG_VERSION=3.3.1
# Fri, 13 Oct 2023 07:28:57 GMT
ENV KONG_VERSION=3.3.1
# Fri, 13 Oct 2023 07:28:57 GMT
ARG KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20
# Fri, 13 Oct 2023 07:28:57 GMT
ARG KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
# Fri, 13 Oct 2023 07:29:25 GMT
# ARGS: KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20 KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 07:29:26 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 07:29:26 GMT
USER kong
# Fri, 13 Oct 2023 07:29:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 07:29:26 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 07:29:26 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 07:29:27 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 07:29:27 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:43f89b94cd7df92a2f7e565b8fb1b7f502eff2cd225508cbd7ea2d36a9a3a601`  
		Last Modified: Thu, 05 Oct 2023 08:42:10 GMT  
		Size: 30.4 MB (30439111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676526cf23951612fff170db505ac909b79f87739dc8b7dd9ed856ae710da9b6`  
		Last Modified: Fri, 13 Oct 2023 07:31:52 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4def0d602c5984e4453aa39b7e3e3e1e896cbd21c1f6bdf5d8c5b6f9d7f408d9`  
		Last Modified: Fri, 13 Oct 2023 07:32:27 GMT  
		Size: 50.9 MB (50909614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:277217efd2742c7f82e9389429a9bfa2ddcbf4347fb992ba93f051e47c9fb025`  
		Last Modified: Fri, 13 Oct 2023 07:32:20 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.3.1-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:7d14713d357aeaab02ceeaa45d5f0ed89e2230235ed3b780d99f004f3c9aa60f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.8 MB (75769288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0884155d3564ce1d9c0ccda4ac3753a48929dee3f423320bd6ddd490c135723`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 05 Oct 2023 07:32:20 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:32:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:32:22 GMT
ADD file:f8594e26831508c318e42c8dfd9942041031087b8de1bf3fec11fd75b8b30fd4 in / 
# Thu, 05 Oct 2023 07:32:22 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 03:52:02 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 13 Oct 2023 03:52:02 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 03:52:02 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 03:52:02 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 03:52:02 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 13 Oct 2023 03:52:25 GMT
ARG KONG_VERSION=3.3.1
# Fri, 13 Oct 2023 03:52:25 GMT
ENV KONG_VERSION=3.3.1
# Fri, 13 Oct 2023 03:52:25 GMT
ARG KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20
# Fri, 13 Oct 2023 03:52:25 GMT
ARG KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
# Fri, 13 Oct 2023 03:52:41 GMT
# ARGS: KONG_AMD64_SHA=3aa6625933b60c8a4669a3623bcd3a3d736dfd807bbc314ea8989cd63c117a20 KONG_ARM64_SHA=3fd20cd0e45e81d858b54d3e40992d73ac9d7d11e398c0d02854ff69988657dd
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 03:52:42 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 03:52:42 GMT
USER kong
# Fri, 13 Oct 2023 03:52:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 03:52:42 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 03:52:42 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 03:52:42 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 03:52:42 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:895d322e8e5957c04af3ab7b3431f2a562182d34167c6e159e02044150a66967`  
		Last Modified: Thu, 05 Oct 2023 08:57:30 GMT  
		Size: 28.4 MB (28391939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4eb9336ac11e4c267c309924d9e2989161e7930966c2b551b0de49623951691`  
		Last Modified: Fri, 13 Oct 2023 03:54:48 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0996f4d7bc2002dad66156c70889f5c98f7b663458df7a8e18f03b51439dda`  
		Last Modified: Fri, 13 Oct 2023 03:55:20 GMT  
		Size: 47.4 MB (47376070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c0a200877adb59005e5dd2713d041b397fd7d777d45b251b368347c6f47969`  
		Last Modified: Fri, 13 Oct 2023 03:55:14 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.4`

```console
$ docker pull kong@sha256:6b5506ae271bc252fe9594a808db7146b488e0a88966c640d320abd6dedc1ef2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.4` - linux; amd64

```console
$ docker pull kong@sha256:11116706f624bd4cf92a18c9ae614628db8bd5788b7406eb07896862ddb1da4f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93175019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7fabd29ce8cdbab7ae27f755052f60f1cf548d07f4f7f2dff8614946a3a07c4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 05 Oct 2023 07:33:30 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:33:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:33:32 GMT
ADD file:63d5ab3ef0aab308c0e71cb67292c5467f60deafa9b0418cbb220affcd078444 in / 
# Thu, 05 Oct 2023 07:33:32 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:28:30 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 13 Oct 2023 07:28:30 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 07:28:30 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 07:28:30 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 07:28:30 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 13 Oct 2023 07:28:30 GMT
ARG KONG_VERSION=3.4.2
# Fri, 13 Oct 2023 07:28:31 GMT
ENV KONG_VERSION=3.4.2
# Fri, 13 Oct 2023 07:28:31 GMT
ARG KONG_AMD64_SHA=b6bf56a5088660e7cac748a005af8d977be7177e64b0abfe1e7f77d797cdc0e2
# Fri, 13 Oct 2023 07:28:31 GMT
ARG KONG_ARM64_SHA=8bca79a6337a6299316cca4e2f9a766df09268359292686498db18a48d883689
# Fri, 13 Oct 2023 07:28:49 GMT
# ARGS: KONG_AMD64_SHA=b6bf56a5088660e7cac748a005af8d977be7177e64b0abfe1e7f77d797cdc0e2 KONG_ARM64_SHA=8bca79a6337a6299316cca4e2f9a766df09268359292686498db18a48d883689
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y --no-install-recommends curl ca-certificates       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes --no-install-recommends /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 07:28:50 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 07:28:50 GMT
USER kong
# Fri, 13 Oct 2023 07:28:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 07:28:50 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 07:28:50 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 07:28:50 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 07:28:50 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:43f89b94cd7df92a2f7e565b8fb1b7f502eff2cd225508cbd7ea2d36a9a3a601`  
		Last Modified: Thu, 05 Oct 2023 08:42:10 GMT  
		Size: 30.4 MB (30439111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676526cf23951612fff170db505ac909b79f87739dc8b7dd9ed856ae710da9b6`  
		Last Modified: Fri, 13 Oct 2023 07:31:52 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d5013df765c3cd670061a26110d49400b487e4b8cf32dc3064f2015f0a3c7e`  
		Last Modified: Fri, 13 Oct 2023 07:32:02 GMT  
		Size: 62.7 MB (62734627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df25283763c84405dba67bbe987e73bee45b491a7db05c40f3f6fe23fbf66b22`  
		Last Modified: Fri, 13 Oct 2023 07:31:52 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.4` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:f57a09ff69a0d431c58fbf856358804a776aed167cb093231840722d2a68a317
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.6 MB (89561608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74f7cdc7bf980ab8c7a02630be0dceaace6a4d23886be7fd1ab4774398f82503`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 05 Oct 2023 07:32:20 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:32:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:32:22 GMT
ADD file:f8594e26831508c318e42c8dfd9942041031087b8de1bf3fec11fd75b8b30fd4 in / 
# Thu, 05 Oct 2023 07:32:22 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 03:52:02 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 13 Oct 2023 03:52:02 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 03:52:02 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 03:52:02 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 03:52:02 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 13 Oct 2023 03:52:02 GMT
ARG KONG_VERSION=3.4.2
# Fri, 13 Oct 2023 03:52:02 GMT
ENV KONG_VERSION=3.4.2
# Fri, 13 Oct 2023 03:52:02 GMT
ARG KONG_AMD64_SHA=b6bf56a5088660e7cac748a005af8d977be7177e64b0abfe1e7f77d797cdc0e2
# Fri, 13 Oct 2023 03:52:02 GMT
ARG KONG_ARM64_SHA=8bca79a6337a6299316cca4e2f9a766df09268359292686498db18a48d883689
# Fri, 13 Oct 2023 03:52:20 GMT
# ARGS: KONG_AMD64_SHA=b6bf56a5088660e7cac748a005af8d977be7177e64b0abfe1e7f77d797cdc0e2 KONG_ARM64_SHA=8bca79a6337a6299316cca4e2f9a766df09268359292686498db18a48d883689
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y --no-install-recommends curl ca-certificates       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes --no-install-recommends /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 03:52:21 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 03:52:21 GMT
USER kong
# Fri, 13 Oct 2023 03:52:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 03:52:21 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 03:52:22 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 03:52:22 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 03:52:22 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:895d322e8e5957c04af3ab7b3431f2a562182d34167c6e159e02044150a66967`  
		Last Modified: Thu, 05 Oct 2023 08:57:30 GMT  
		Size: 28.4 MB (28391939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4eb9336ac11e4c267c309924d9e2989161e7930966c2b551b0de49623951691`  
		Last Modified: Fri, 13 Oct 2023 03:54:48 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72627dd6b77fdc810bbd21463b5c05d892e09189e42be4c8d7c71e1b06e5a7b7`  
		Last Modified: Fri, 13 Oct 2023 03:54:56 GMT  
		Size: 61.2 MB (61168390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba1271a9a34893cea35e4c19b85ca607fef78046cb6baa5ad6f2936ae009043`  
		Last Modified: Fri, 13 Oct 2023 03:54:48 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.4-ubuntu`

```console
$ docker pull kong@sha256:6b5506ae271bc252fe9594a808db7146b488e0a88966c640d320abd6dedc1ef2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.4-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:11116706f624bd4cf92a18c9ae614628db8bd5788b7406eb07896862ddb1da4f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93175019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7fabd29ce8cdbab7ae27f755052f60f1cf548d07f4f7f2dff8614946a3a07c4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 05 Oct 2023 07:33:30 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:33:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:33:32 GMT
ADD file:63d5ab3ef0aab308c0e71cb67292c5467f60deafa9b0418cbb220affcd078444 in / 
# Thu, 05 Oct 2023 07:33:32 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:28:30 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 13 Oct 2023 07:28:30 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 07:28:30 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 07:28:30 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 07:28:30 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 13 Oct 2023 07:28:30 GMT
ARG KONG_VERSION=3.4.2
# Fri, 13 Oct 2023 07:28:31 GMT
ENV KONG_VERSION=3.4.2
# Fri, 13 Oct 2023 07:28:31 GMT
ARG KONG_AMD64_SHA=b6bf56a5088660e7cac748a005af8d977be7177e64b0abfe1e7f77d797cdc0e2
# Fri, 13 Oct 2023 07:28:31 GMT
ARG KONG_ARM64_SHA=8bca79a6337a6299316cca4e2f9a766df09268359292686498db18a48d883689
# Fri, 13 Oct 2023 07:28:49 GMT
# ARGS: KONG_AMD64_SHA=b6bf56a5088660e7cac748a005af8d977be7177e64b0abfe1e7f77d797cdc0e2 KONG_ARM64_SHA=8bca79a6337a6299316cca4e2f9a766df09268359292686498db18a48d883689
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y --no-install-recommends curl ca-certificates       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes --no-install-recommends /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 07:28:50 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 07:28:50 GMT
USER kong
# Fri, 13 Oct 2023 07:28:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 07:28:50 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 07:28:50 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 07:28:50 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 07:28:50 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:43f89b94cd7df92a2f7e565b8fb1b7f502eff2cd225508cbd7ea2d36a9a3a601`  
		Last Modified: Thu, 05 Oct 2023 08:42:10 GMT  
		Size: 30.4 MB (30439111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676526cf23951612fff170db505ac909b79f87739dc8b7dd9ed856ae710da9b6`  
		Last Modified: Fri, 13 Oct 2023 07:31:52 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d5013df765c3cd670061a26110d49400b487e4b8cf32dc3064f2015f0a3c7e`  
		Last Modified: Fri, 13 Oct 2023 07:32:02 GMT  
		Size: 62.7 MB (62734627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df25283763c84405dba67bbe987e73bee45b491a7db05c40f3f6fe23fbf66b22`  
		Last Modified: Fri, 13 Oct 2023 07:31:52 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.4-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:f57a09ff69a0d431c58fbf856358804a776aed167cb093231840722d2a68a317
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.6 MB (89561608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74f7cdc7bf980ab8c7a02630be0dceaace6a4d23886be7fd1ab4774398f82503`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 05 Oct 2023 07:32:20 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:32:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:32:22 GMT
ADD file:f8594e26831508c318e42c8dfd9942041031087b8de1bf3fec11fd75b8b30fd4 in / 
# Thu, 05 Oct 2023 07:32:22 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 03:52:02 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 13 Oct 2023 03:52:02 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 03:52:02 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 03:52:02 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 03:52:02 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 13 Oct 2023 03:52:02 GMT
ARG KONG_VERSION=3.4.2
# Fri, 13 Oct 2023 03:52:02 GMT
ENV KONG_VERSION=3.4.2
# Fri, 13 Oct 2023 03:52:02 GMT
ARG KONG_AMD64_SHA=b6bf56a5088660e7cac748a005af8d977be7177e64b0abfe1e7f77d797cdc0e2
# Fri, 13 Oct 2023 03:52:02 GMT
ARG KONG_ARM64_SHA=8bca79a6337a6299316cca4e2f9a766df09268359292686498db18a48d883689
# Fri, 13 Oct 2023 03:52:20 GMT
# ARGS: KONG_AMD64_SHA=b6bf56a5088660e7cac748a005af8d977be7177e64b0abfe1e7f77d797cdc0e2 KONG_ARM64_SHA=8bca79a6337a6299316cca4e2f9a766df09268359292686498db18a48d883689
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y --no-install-recommends curl ca-certificates       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes --no-install-recommends /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 03:52:21 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 03:52:21 GMT
USER kong
# Fri, 13 Oct 2023 03:52:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 03:52:21 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 03:52:22 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 03:52:22 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 03:52:22 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:895d322e8e5957c04af3ab7b3431f2a562182d34167c6e159e02044150a66967`  
		Last Modified: Thu, 05 Oct 2023 08:57:30 GMT  
		Size: 28.4 MB (28391939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4eb9336ac11e4c267c309924d9e2989161e7930966c2b551b0de49623951691`  
		Last Modified: Fri, 13 Oct 2023 03:54:48 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72627dd6b77fdc810bbd21463b5c05d892e09189e42be4c8d7c71e1b06e5a7b7`  
		Last Modified: Fri, 13 Oct 2023 03:54:56 GMT  
		Size: 61.2 MB (61168390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba1271a9a34893cea35e4c19b85ca607fef78046cb6baa5ad6f2936ae009043`  
		Last Modified: Fri, 13 Oct 2023 03:54:48 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.4.2`

```console
$ docker pull kong@sha256:6b5506ae271bc252fe9594a808db7146b488e0a88966c640d320abd6dedc1ef2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.4.2` - linux; amd64

```console
$ docker pull kong@sha256:11116706f624bd4cf92a18c9ae614628db8bd5788b7406eb07896862ddb1da4f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93175019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7fabd29ce8cdbab7ae27f755052f60f1cf548d07f4f7f2dff8614946a3a07c4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 05 Oct 2023 07:33:30 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:33:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:33:32 GMT
ADD file:63d5ab3ef0aab308c0e71cb67292c5467f60deafa9b0418cbb220affcd078444 in / 
# Thu, 05 Oct 2023 07:33:32 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:28:30 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 13 Oct 2023 07:28:30 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 07:28:30 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 07:28:30 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 07:28:30 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 13 Oct 2023 07:28:30 GMT
ARG KONG_VERSION=3.4.2
# Fri, 13 Oct 2023 07:28:31 GMT
ENV KONG_VERSION=3.4.2
# Fri, 13 Oct 2023 07:28:31 GMT
ARG KONG_AMD64_SHA=b6bf56a5088660e7cac748a005af8d977be7177e64b0abfe1e7f77d797cdc0e2
# Fri, 13 Oct 2023 07:28:31 GMT
ARG KONG_ARM64_SHA=8bca79a6337a6299316cca4e2f9a766df09268359292686498db18a48d883689
# Fri, 13 Oct 2023 07:28:49 GMT
# ARGS: KONG_AMD64_SHA=b6bf56a5088660e7cac748a005af8d977be7177e64b0abfe1e7f77d797cdc0e2 KONG_ARM64_SHA=8bca79a6337a6299316cca4e2f9a766df09268359292686498db18a48d883689
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y --no-install-recommends curl ca-certificates       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes --no-install-recommends /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 07:28:50 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 07:28:50 GMT
USER kong
# Fri, 13 Oct 2023 07:28:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 07:28:50 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 07:28:50 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 07:28:50 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 07:28:50 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:43f89b94cd7df92a2f7e565b8fb1b7f502eff2cd225508cbd7ea2d36a9a3a601`  
		Last Modified: Thu, 05 Oct 2023 08:42:10 GMT  
		Size: 30.4 MB (30439111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676526cf23951612fff170db505ac909b79f87739dc8b7dd9ed856ae710da9b6`  
		Last Modified: Fri, 13 Oct 2023 07:31:52 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d5013df765c3cd670061a26110d49400b487e4b8cf32dc3064f2015f0a3c7e`  
		Last Modified: Fri, 13 Oct 2023 07:32:02 GMT  
		Size: 62.7 MB (62734627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df25283763c84405dba67bbe987e73bee45b491a7db05c40f3f6fe23fbf66b22`  
		Last Modified: Fri, 13 Oct 2023 07:31:52 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.4.2` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:f57a09ff69a0d431c58fbf856358804a776aed167cb093231840722d2a68a317
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.6 MB (89561608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74f7cdc7bf980ab8c7a02630be0dceaace6a4d23886be7fd1ab4774398f82503`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 05 Oct 2023 07:32:20 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:32:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:32:22 GMT
ADD file:f8594e26831508c318e42c8dfd9942041031087b8de1bf3fec11fd75b8b30fd4 in / 
# Thu, 05 Oct 2023 07:32:22 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 03:52:02 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 13 Oct 2023 03:52:02 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 03:52:02 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 03:52:02 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 03:52:02 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 13 Oct 2023 03:52:02 GMT
ARG KONG_VERSION=3.4.2
# Fri, 13 Oct 2023 03:52:02 GMT
ENV KONG_VERSION=3.4.2
# Fri, 13 Oct 2023 03:52:02 GMT
ARG KONG_AMD64_SHA=b6bf56a5088660e7cac748a005af8d977be7177e64b0abfe1e7f77d797cdc0e2
# Fri, 13 Oct 2023 03:52:02 GMT
ARG KONG_ARM64_SHA=8bca79a6337a6299316cca4e2f9a766df09268359292686498db18a48d883689
# Fri, 13 Oct 2023 03:52:20 GMT
# ARGS: KONG_AMD64_SHA=b6bf56a5088660e7cac748a005af8d977be7177e64b0abfe1e7f77d797cdc0e2 KONG_ARM64_SHA=8bca79a6337a6299316cca4e2f9a766df09268359292686498db18a48d883689
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y --no-install-recommends curl ca-certificates       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes --no-install-recommends /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 03:52:21 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 03:52:21 GMT
USER kong
# Fri, 13 Oct 2023 03:52:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 03:52:21 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 03:52:22 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 03:52:22 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 03:52:22 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:895d322e8e5957c04af3ab7b3431f2a562182d34167c6e159e02044150a66967`  
		Last Modified: Thu, 05 Oct 2023 08:57:30 GMT  
		Size: 28.4 MB (28391939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4eb9336ac11e4c267c309924d9e2989161e7930966c2b551b0de49623951691`  
		Last Modified: Fri, 13 Oct 2023 03:54:48 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72627dd6b77fdc810bbd21463b5c05d892e09189e42be4c8d7c71e1b06e5a7b7`  
		Last Modified: Fri, 13 Oct 2023 03:54:56 GMT  
		Size: 61.2 MB (61168390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba1271a9a34893cea35e4c19b85ca607fef78046cb6baa5ad6f2936ae009043`  
		Last Modified: Fri, 13 Oct 2023 03:54:48 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.4.2-ubuntu`

```console
$ docker pull kong@sha256:6b5506ae271bc252fe9594a808db7146b488e0a88966c640d320abd6dedc1ef2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.4.2-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:11116706f624bd4cf92a18c9ae614628db8bd5788b7406eb07896862ddb1da4f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93175019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7fabd29ce8cdbab7ae27f755052f60f1cf548d07f4f7f2dff8614946a3a07c4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 05 Oct 2023 07:33:30 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:33:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:33:32 GMT
ADD file:63d5ab3ef0aab308c0e71cb67292c5467f60deafa9b0418cbb220affcd078444 in / 
# Thu, 05 Oct 2023 07:33:32 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:28:30 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 13 Oct 2023 07:28:30 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 07:28:30 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 07:28:30 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 07:28:30 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 13 Oct 2023 07:28:30 GMT
ARG KONG_VERSION=3.4.2
# Fri, 13 Oct 2023 07:28:31 GMT
ENV KONG_VERSION=3.4.2
# Fri, 13 Oct 2023 07:28:31 GMT
ARG KONG_AMD64_SHA=b6bf56a5088660e7cac748a005af8d977be7177e64b0abfe1e7f77d797cdc0e2
# Fri, 13 Oct 2023 07:28:31 GMT
ARG KONG_ARM64_SHA=8bca79a6337a6299316cca4e2f9a766df09268359292686498db18a48d883689
# Fri, 13 Oct 2023 07:28:49 GMT
# ARGS: KONG_AMD64_SHA=b6bf56a5088660e7cac748a005af8d977be7177e64b0abfe1e7f77d797cdc0e2 KONG_ARM64_SHA=8bca79a6337a6299316cca4e2f9a766df09268359292686498db18a48d883689
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y --no-install-recommends curl ca-certificates       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes --no-install-recommends /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 07:28:50 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 07:28:50 GMT
USER kong
# Fri, 13 Oct 2023 07:28:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 07:28:50 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 07:28:50 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 07:28:50 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 07:28:50 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:43f89b94cd7df92a2f7e565b8fb1b7f502eff2cd225508cbd7ea2d36a9a3a601`  
		Last Modified: Thu, 05 Oct 2023 08:42:10 GMT  
		Size: 30.4 MB (30439111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676526cf23951612fff170db505ac909b79f87739dc8b7dd9ed856ae710da9b6`  
		Last Modified: Fri, 13 Oct 2023 07:31:52 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d5013df765c3cd670061a26110d49400b487e4b8cf32dc3064f2015f0a3c7e`  
		Last Modified: Fri, 13 Oct 2023 07:32:02 GMT  
		Size: 62.7 MB (62734627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df25283763c84405dba67bbe987e73bee45b491a7db05c40f3f6fe23fbf66b22`  
		Last Modified: Fri, 13 Oct 2023 07:31:52 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.4.2-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:f57a09ff69a0d431c58fbf856358804a776aed167cb093231840722d2a68a317
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.6 MB (89561608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74f7cdc7bf980ab8c7a02630be0dceaace6a4d23886be7fd1ab4774398f82503`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 05 Oct 2023 07:32:20 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:32:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:32:22 GMT
ADD file:f8594e26831508c318e42c8dfd9942041031087b8de1bf3fec11fd75b8b30fd4 in / 
# Thu, 05 Oct 2023 07:32:22 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 03:52:02 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 13 Oct 2023 03:52:02 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 03:52:02 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 03:52:02 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 03:52:02 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 13 Oct 2023 03:52:02 GMT
ARG KONG_VERSION=3.4.2
# Fri, 13 Oct 2023 03:52:02 GMT
ENV KONG_VERSION=3.4.2
# Fri, 13 Oct 2023 03:52:02 GMT
ARG KONG_AMD64_SHA=b6bf56a5088660e7cac748a005af8d977be7177e64b0abfe1e7f77d797cdc0e2
# Fri, 13 Oct 2023 03:52:02 GMT
ARG KONG_ARM64_SHA=8bca79a6337a6299316cca4e2f9a766df09268359292686498db18a48d883689
# Fri, 13 Oct 2023 03:52:20 GMT
# ARGS: KONG_AMD64_SHA=b6bf56a5088660e7cac748a005af8d977be7177e64b0abfe1e7f77d797cdc0e2 KONG_ARM64_SHA=8bca79a6337a6299316cca4e2f9a766df09268359292686498db18a48d883689
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y --no-install-recommends curl ca-certificates       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes --no-install-recommends /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 03:52:21 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 03:52:21 GMT
USER kong
# Fri, 13 Oct 2023 03:52:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 03:52:21 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 03:52:22 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 03:52:22 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 03:52:22 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:895d322e8e5957c04af3ab7b3431f2a562182d34167c6e159e02044150a66967`  
		Last Modified: Thu, 05 Oct 2023 08:57:30 GMT  
		Size: 28.4 MB (28391939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4eb9336ac11e4c267c309924d9e2989161e7930966c2b551b0de49623951691`  
		Last Modified: Fri, 13 Oct 2023 03:54:48 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72627dd6b77fdc810bbd21463b5c05d892e09189e42be4c8d7c71e1b06e5a7b7`  
		Last Modified: Fri, 13 Oct 2023 03:54:56 GMT  
		Size: 61.2 MB (61168390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba1271a9a34893cea35e4c19b85ca607fef78046cb6baa5ad6f2936ae009043`  
		Last Modified: Fri, 13 Oct 2023 03:54:48 GMT  
		Size: 1.2 KB (1156 bytes)  
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
$ docker pull kong@sha256:6b5506ae271bc252fe9594a808db7146b488e0a88966c640d320abd6dedc1ef2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:latest` - linux; amd64

```console
$ docker pull kong@sha256:11116706f624bd4cf92a18c9ae614628db8bd5788b7406eb07896862ddb1da4f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93175019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7fabd29ce8cdbab7ae27f755052f60f1cf548d07f4f7f2dff8614946a3a07c4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 05 Oct 2023 07:33:30 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:33:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:33:32 GMT
ADD file:63d5ab3ef0aab308c0e71cb67292c5467f60deafa9b0418cbb220affcd078444 in / 
# Thu, 05 Oct 2023 07:33:32 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:28:30 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 13 Oct 2023 07:28:30 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 07:28:30 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 07:28:30 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 07:28:30 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 13 Oct 2023 07:28:30 GMT
ARG KONG_VERSION=3.4.2
# Fri, 13 Oct 2023 07:28:31 GMT
ENV KONG_VERSION=3.4.2
# Fri, 13 Oct 2023 07:28:31 GMT
ARG KONG_AMD64_SHA=b6bf56a5088660e7cac748a005af8d977be7177e64b0abfe1e7f77d797cdc0e2
# Fri, 13 Oct 2023 07:28:31 GMT
ARG KONG_ARM64_SHA=8bca79a6337a6299316cca4e2f9a766df09268359292686498db18a48d883689
# Fri, 13 Oct 2023 07:28:49 GMT
# ARGS: KONG_AMD64_SHA=b6bf56a5088660e7cac748a005af8d977be7177e64b0abfe1e7f77d797cdc0e2 KONG_ARM64_SHA=8bca79a6337a6299316cca4e2f9a766df09268359292686498db18a48d883689
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y --no-install-recommends curl ca-certificates       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes --no-install-recommends /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 07:28:50 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 07:28:50 GMT
USER kong
# Fri, 13 Oct 2023 07:28:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 07:28:50 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 07:28:50 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 07:28:50 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 07:28:50 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:43f89b94cd7df92a2f7e565b8fb1b7f502eff2cd225508cbd7ea2d36a9a3a601`  
		Last Modified: Thu, 05 Oct 2023 08:42:10 GMT  
		Size: 30.4 MB (30439111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676526cf23951612fff170db505ac909b79f87739dc8b7dd9ed856ae710da9b6`  
		Last Modified: Fri, 13 Oct 2023 07:31:52 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d5013df765c3cd670061a26110d49400b487e4b8cf32dc3064f2015f0a3c7e`  
		Last Modified: Fri, 13 Oct 2023 07:32:02 GMT  
		Size: 62.7 MB (62734627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df25283763c84405dba67bbe987e73bee45b491a7db05c40f3f6fe23fbf66b22`  
		Last Modified: Fri, 13 Oct 2023 07:31:52 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:latest` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:f57a09ff69a0d431c58fbf856358804a776aed167cb093231840722d2a68a317
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.6 MB (89561608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74f7cdc7bf980ab8c7a02630be0dceaace6a4d23886be7fd1ab4774398f82503`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 05 Oct 2023 07:32:20 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:32:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:32:22 GMT
ADD file:f8594e26831508c318e42c8dfd9942041031087b8de1bf3fec11fd75b8b30fd4 in / 
# Thu, 05 Oct 2023 07:32:22 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 03:52:02 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 13 Oct 2023 03:52:02 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 03:52:02 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 03:52:02 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 03:52:02 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 13 Oct 2023 03:52:02 GMT
ARG KONG_VERSION=3.4.2
# Fri, 13 Oct 2023 03:52:02 GMT
ENV KONG_VERSION=3.4.2
# Fri, 13 Oct 2023 03:52:02 GMT
ARG KONG_AMD64_SHA=b6bf56a5088660e7cac748a005af8d977be7177e64b0abfe1e7f77d797cdc0e2
# Fri, 13 Oct 2023 03:52:02 GMT
ARG KONG_ARM64_SHA=8bca79a6337a6299316cca4e2f9a766df09268359292686498db18a48d883689
# Fri, 13 Oct 2023 03:52:20 GMT
# ARGS: KONG_AMD64_SHA=b6bf56a5088660e7cac748a005af8d977be7177e64b0abfe1e7f77d797cdc0e2 KONG_ARM64_SHA=8bca79a6337a6299316cca4e2f9a766df09268359292686498db18a48d883689
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y --no-install-recommends curl ca-certificates       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes --no-install-recommends /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 03:52:21 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 03:52:21 GMT
USER kong
# Fri, 13 Oct 2023 03:52:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 03:52:21 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 03:52:22 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 03:52:22 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 03:52:22 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:895d322e8e5957c04af3ab7b3431f2a562182d34167c6e159e02044150a66967`  
		Last Modified: Thu, 05 Oct 2023 08:57:30 GMT  
		Size: 28.4 MB (28391939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4eb9336ac11e4c267c309924d9e2989161e7930966c2b551b0de49623951691`  
		Last Modified: Fri, 13 Oct 2023 03:54:48 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72627dd6b77fdc810bbd21463b5c05d892e09189e42be4c8d7c71e1b06e5a7b7`  
		Last Modified: Fri, 13 Oct 2023 03:54:56 GMT  
		Size: 61.2 MB (61168390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba1271a9a34893cea35e4c19b85ca607fef78046cb6baa5ad6f2936ae009043`  
		Last Modified: Fri, 13 Oct 2023 03:54:48 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:ubuntu`

```console
$ docker pull kong@sha256:6b5506ae271bc252fe9594a808db7146b488e0a88966c640d320abd6dedc1ef2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:11116706f624bd4cf92a18c9ae614628db8bd5788b7406eb07896862ddb1da4f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93175019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7fabd29ce8cdbab7ae27f755052f60f1cf548d07f4f7f2dff8614946a3a07c4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 05 Oct 2023 07:33:30 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:33:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:33:32 GMT
ADD file:63d5ab3ef0aab308c0e71cb67292c5467f60deafa9b0418cbb220affcd078444 in / 
# Thu, 05 Oct 2023 07:33:32 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:28:30 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 13 Oct 2023 07:28:30 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 07:28:30 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 07:28:30 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 07:28:30 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 13 Oct 2023 07:28:30 GMT
ARG KONG_VERSION=3.4.2
# Fri, 13 Oct 2023 07:28:31 GMT
ENV KONG_VERSION=3.4.2
# Fri, 13 Oct 2023 07:28:31 GMT
ARG KONG_AMD64_SHA=b6bf56a5088660e7cac748a005af8d977be7177e64b0abfe1e7f77d797cdc0e2
# Fri, 13 Oct 2023 07:28:31 GMT
ARG KONG_ARM64_SHA=8bca79a6337a6299316cca4e2f9a766df09268359292686498db18a48d883689
# Fri, 13 Oct 2023 07:28:49 GMT
# ARGS: KONG_AMD64_SHA=b6bf56a5088660e7cac748a005af8d977be7177e64b0abfe1e7f77d797cdc0e2 KONG_ARM64_SHA=8bca79a6337a6299316cca4e2f9a766df09268359292686498db18a48d883689
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y --no-install-recommends curl ca-certificates       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes --no-install-recommends /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 07:28:50 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 07:28:50 GMT
USER kong
# Fri, 13 Oct 2023 07:28:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 07:28:50 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 07:28:50 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 07:28:50 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 07:28:50 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:43f89b94cd7df92a2f7e565b8fb1b7f502eff2cd225508cbd7ea2d36a9a3a601`  
		Last Modified: Thu, 05 Oct 2023 08:42:10 GMT  
		Size: 30.4 MB (30439111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676526cf23951612fff170db505ac909b79f87739dc8b7dd9ed856ae710da9b6`  
		Last Modified: Fri, 13 Oct 2023 07:31:52 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d5013df765c3cd670061a26110d49400b487e4b8cf32dc3064f2015f0a3c7e`  
		Last Modified: Fri, 13 Oct 2023 07:32:02 GMT  
		Size: 62.7 MB (62734627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df25283763c84405dba67bbe987e73bee45b491a7db05c40f3f6fe23fbf66b22`  
		Last Modified: Fri, 13 Oct 2023 07:31:52 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:f57a09ff69a0d431c58fbf856358804a776aed167cb093231840722d2a68a317
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.6 MB (89561608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74f7cdc7bf980ab8c7a02630be0dceaace6a4d23886be7fd1ab4774398f82503`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 05 Oct 2023 07:32:20 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:32:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:32:22 GMT
ADD file:f8594e26831508c318e42c8dfd9942041031087b8de1bf3fec11fd75b8b30fd4 in / 
# Thu, 05 Oct 2023 07:32:22 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 03:52:02 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 13 Oct 2023 03:52:02 GMT
ARG ASSET=ce
# Fri, 13 Oct 2023 03:52:02 GMT
ENV ASSET=ce
# Fri, 13 Oct 2023 03:52:02 GMT
ARG EE_PORTS
# Fri, 13 Oct 2023 03:52:02 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 13 Oct 2023 03:52:02 GMT
ARG KONG_VERSION=3.4.2
# Fri, 13 Oct 2023 03:52:02 GMT
ENV KONG_VERSION=3.4.2
# Fri, 13 Oct 2023 03:52:02 GMT
ARG KONG_AMD64_SHA=b6bf56a5088660e7cac748a005af8d977be7177e64b0abfe1e7f77d797cdc0e2
# Fri, 13 Oct 2023 03:52:02 GMT
ARG KONG_ARM64_SHA=8bca79a6337a6299316cca4e2f9a766df09268359292686498db18a48d883689
# Fri, 13 Oct 2023 03:52:20 GMT
# ARGS: KONG_AMD64_SHA=b6bf56a5088660e7cac748a005af8d977be7177e64b0abfe1e7f77d797cdc0e2 KONG_ARM64_SHA=8bca79a6337a6299316cca4e2f9a766df09268359292686498db18a48d883689
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y --no-install-recommends curl ca-certificates       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes --no-install-recommends /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 13 Oct 2023 03:52:21 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 13 Oct 2023 03:52:21 GMT
USER kong
# Fri, 13 Oct 2023 03:52:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 13 Oct 2023 03:52:21 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 13 Oct 2023 03:52:22 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 Oct 2023 03:52:22 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 13 Oct 2023 03:52:22 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:895d322e8e5957c04af3ab7b3431f2a562182d34167c6e159e02044150a66967`  
		Last Modified: Thu, 05 Oct 2023 08:57:30 GMT  
		Size: 28.4 MB (28391939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4eb9336ac11e4c267c309924d9e2989161e7930966c2b551b0de49623951691`  
		Last Modified: Fri, 13 Oct 2023 03:54:48 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72627dd6b77fdc810bbd21463b5c05d892e09189e42be4c8d7c71e1b06e5a7b7`  
		Last Modified: Fri, 13 Oct 2023 03:54:56 GMT  
		Size: 61.2 MB (61168390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba1271a9a34893cea35e4c19b85ca607fef78046cb6baa5ad6f2936ae009043`  
		Last Modified: Fri, 13 Oct 2023 03:54:48 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
