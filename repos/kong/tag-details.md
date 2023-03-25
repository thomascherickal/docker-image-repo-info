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
-	[`kong:alpine`](#kongalpine)
-	[`kong:latest`](#konglatest)
-	[`kong:ubuntu`](#kongubuntu)

## `kong:2.8`

```console
$ docker pull kong@sha256:adad1f4a72229fe3b1768ecc601cb875a4eecb778dc0c7b2b7dc5d7f2825a844
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.8` - linux; amd64

```console
$ docker pull kong@sha256:ae3d663f065f1a138f0656708da3990b9c2c425867ef02316a929304383bc9c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49337534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf46f5ed0fbc366915b5b4809eca9e33f2ee8f2bb157565b7b5cc29d3cbcaf41`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 14:00:20 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 11 Feb 2023 14:00:20 GMT
ARG ASSET=ce
# Sat, 11 Feb 2023 14:00:21 GMT
ENV ASSET=ce
# Sat, 11 Feb 2023 14:00:21 GMT
ARG EE_PORTS
# Sat, 11 Feb 2023 14:00:21 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Sat, 11 Feb 2023 14:00:21 GMT
ARG KONG_VERSION=2.8.3
# Sat, 11 Feb 2023 14:00:21 GMT
ENV KONG_VERSION=2.8.3
# Fri, 17 Feb 2023 21:05:31 GMT
ARG KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa
# Fri, 17 Feb 2023 21:05:31 GMT
ARG KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
# Fri, 17 Feb 2023 21:05:38 GMT
# ARGS: KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Fri, 17 Feb 2023 21:05:38 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 17 Feb 2023 21:05:38 GMT
USER kong
# Fri, 17 Feb 2023 21:05:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 17 Feb 2023 21:05:39 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 17 Feb 2023 21:05:39 GMT
STOPSIGNAL SIGQUIT
# Fri, 17 Feb 2023 21:05:39 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 17 Feb 2023 21:05:39 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:332cd90dd99acdafaf1be5f2ecbf3e7e8dbb56063cd31b47aa5c172fa53f18ba`  
		Last Modified: Sat, 11 Feb 2023 14:02:34 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34e07d8ee8b056e5949e66ecb76724024fbe556f6f36213dd16ed398f04d20db`  
		Last Modified: Fri, 17 Feb 2023 21:06:17 GMT  
		Size: 46.5 MB (46528761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baccb83225b8a3c516fb22973594a6c72238b6614bebabc09830855eab5657bf`  
		Last Modified: Fri, 17 Feb 2023 21:06:10 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.8` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:0b6ad885b3b5ebbd99cfc0c50d4584c49e1ceb1055ccbf71a01b1dfa90c5710e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.5 MB (48522073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24de28b355427f0db0e877d9a43e65156a2e3b645f19b0fbc418219e4c3360e1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:57:50 GMT
LABEL maintainer=Kong <support@konghq.com>
# Fri, 10 Feb 2023 22:57:50 GMT
ARG ASSET=ce
# Fri, 10 Feb 2023 22:57:50 GMT
ENV ASSET=ce
# Fri, 10 Feb 2023 22:57:50 GMT
ARG EE_PORTS
# Fri, 10 Feb 2023 22:57:51 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Fri, 10 Feb 2023 22:57:51 GMT
ARG KONG_VERSION=2.8.3
# Fri, 10 Feb 2023 22:57:51 GMT
ENV KONG_VERSION=2.8.3
# Fri, 17 Feb 2023 23:06:33 GMT
ARG KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa
# Fri, 17 Feb 2023 23:06:33 GMT
ARG KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
# Fri, 17 Feb 2023 23:06:39 GMT
# ARGS: KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Fri, 17 Feb 2023 23:06:40 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 17 Feb 2023 23:06:40 GMT
USER kong
# Fri, 17 Feb 2023 23:06:40 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 17 Feb 2023 23:06:40 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 17 Feb 2023 23:06:40 GMT
STOPSIGNAL SIGQUIT
# Fri, 17 Feb 2023 23:06:40 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 17 Feb 2023 23:06:40 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6251f58952598f508c63c9b905a49fd6e3eced7a7b48980335da9d6b1f66c342`  
		Last Modified: Fri, 17 Feb 2023 23:08:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237c69ba3586458df1a5d9283467b62823f7743cbe26455c26f395956626268e`  
		Last Modified: Fri, 17 Feb 2023 23:08:42 GMT  
		Size: 45.8 MB (45811562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e46fd2edc60f47ed1ba71e37abbfdc128d1208c27da478708b44e00fe588680`  
		Last Modified: Fri, 17 Feb 2023 23:08:36 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.8-ubuntu`

```console
$ docker pull kong@sha256:5001fb93806c990119edbc19ce78c847b7f0b22d89f31dd9d8025975a76efad9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.8-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:a190a0e74c2336d9accdc9d6426e954d15ec37b9482dade934de7aa3cfa78e10
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.2 MB (119176803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2942d886517f5edd5f4606c1659c0871257863b03ea3f72619f7284fa8ea075f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 08 Mar 2023 03:22:42 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:22:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:22:44 GMT
ADD file:4560926e076acae6b8396a9f1e760eee0f53e22e90ce8554dda57f1103547795 in / 
# Wed, 08 Mar 2023 03:22:44 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:54:32 GMT
ARG ASSET=ce
# Thu, 16 Mar 2023 04:54:32 GMT
ENV ASSET=ce
# Thu, 16 Mar 2023 04:54:32 GMT
ARG EE_PORTS
# Thu, 16 Mar 2023 04:54:32 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Thu, 16 Mar 2023 04:54:33 GMT
ARG KONG_VERSION=2.8.3
# Thu, 16 Mar 2023 04:54:33 GMT
ENV KONG_VERSION=2.8.3
# Thu, 16 Mar 2023 04:54:33 GMT
ARG KONG_AMD64_SHA=b52baf1caa300c3ee70ff4d58982085b1da9203c69118c885f00d13954634810
# Thu, 16 Mar 2023 04:54:33 GMT
ARG KONG_ARM64_SHA=1d5c2064d44b76fbb3cabf168dc226e91fedb991ace32915297505d089679fed
# Thu, 16 Mar 2023 04:55:30 GMT
# ARGS: KONG_AMD64_SHA=b52baf1caa300c3ee70ff4d58982085b1da9203c69118c885f00d13954634810 KONG_ARM64_SHA=1d5c2064d44b76fbb3cabf168dc226e91fedb991ace32915297505d089679fed
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Thu, 16 Mar 2023 04:55:30 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 16 Mar 2023 04:55:31 GMT
USER kong
# Thu, 16 Mar 2023 04:55:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 16 Mar 2023 04:55:31 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 16 Mar 2023 04:55:31 GMT
STOPSIGNAL SIGQUIT
# Thu, 16 Mar 2023 04:55:31 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 16 Mar 2023 04:55:31 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:cd150c608fee7837e3a5b28be5c7b540eaf4efa27b3b755d55326470691ce2df`  
		Last Modified: Sun, 12 Mar 2023 07:24:55 GMT  
		Size: 26.7 MB (26710746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c264ce00476e5586f47f4afe2421375303d74eb50bbf62aa7e469fe95b470485`  
		Last Modified: Thu, 16 Mar 2023 04:56:48 GMT  
		Size: 25.1 MB (25081962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9b782f0c05455c50ac819cc88cbf7072451e721d29a648ba17f96c9273e9c9`  
		Last Modified: Thu, 16 Mar 2023 04:56:58 GMT  
		Size: 67.4 MB (67383214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41a647953f9053c2d4350193089c38cf7b29887ad0de4a61c97d74347c1a1991`  
		Last Modified: Thu, 16 Mar 2023 04:56:47 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.8-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:951bb9d16837799ad1d89eedb46330e53c93cdf48cfb080c3d791ae4bf172fb5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.8 MB (112828230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:643936a966ffd60cdd971d4264c7dcf48d54a5e6449d0eb3e20773a5f2d72545`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 08 Mar 2023 03:25:33 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:25:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:25:35 GMT
ADD file:5f229d85bac2e85aa7ce97b2168fc61bd401d0151e8940a12d244356f984e65f in / 
# Wed, 08 Mar 2023 03:25:35 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:33:56 GMT
ARG ASSET=ce
# Thu, 16 Mar 2023 02:33:56 GMT
ENV ASSET=ce
# Thu, 16 Mar 2023 02:33:56 GMT
ARG EE_PORTS
# Thu, 16 Mar 2023 02:33:56 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Thu, 16 Mar 2023 02:33:56 GMT
ARG KONG_VERSION=2.8.3
# Thu, 16 Mar 2023 02:33:57 GMT
ENV KONG_VERSION=2.8.3
# Thu, 16 Mar 2023 02:33:57 GMT
ARG KONG_AMD64_SHA=b52baf1caa300c3ee70ff4d58982085b1da9203c69118c885f00d13954634810
# Thu, 16 Mar 2023 02:33:57 GMT
ARG KONG_ARM64_SHA=1d5c2064d44b76fbb3cabf168dc226e91fedb991ace32915297505d089679fed
# Thu, 16 Mar 2023 02:34:29 GMT
# ARGS: KONG_AMD64_SHA=b52baf1caa300c3ee70ff4d58982085b1da9203c69118c885f00d13954634810 KONG_ARM64_SHA=1d5c2064d44b76fbb3cabf168dc226e91fedb991ace32915297505d089679fed
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Thu, 16 Mar 2023 02:34:30 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 16 Mar 2023 02:34:30 GMT
USER kong
# Thu, 16 Mar 2023 02:34:30 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 16 Mar 2023 02:34:30 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 16 Mar 2023 02:34:30 GMT
STOPSIGNAL SIGQUIT
# Thu, 16 Mar 2023 02:34:30 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 16 Mar 2023 02:34:30 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:c21a0233221a76e66b6c10d2445f591bd28eb0773e6cb539474d6dca9ea0b594`  
		Last Modified: Sun, 12 Mar 2023 07:27:31 GMT  
		Size: 23.7 MB (23734706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f9a95d5aae174d1b475bd7ae3237db539e041937ba215ec5df684cee967f77`  
		Last Modified: Thu, 16 Mar 2023 02:35:40 GMT  
		Size: 25.1 MB (25081962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614f9c3cf77e1b393d10fe009e6d644bef38e718aa8220595654adfe78c2ea45`  
		Last Modified: Thu, 16 Mar 2023 02:35:48 GMT  
		Size: 64.0 MB (64010681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2888e6d56a7ff05f896b7866b11ce8896d1c9eade03af34bbebf90c41a2a9a`  
		Last Modified: Thu, 16 Mar 2023 02:35:39 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.8.3`

```console
$ docker pull kong@sha256:adad1f4a72229fe3b1768ecc601cb875a4eecb778dc0c7b2b7dc5d7f2825a844
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.8.3` - linux; amd64

```console
$ docker pull kong@sha256:ae3d663f065f1a138f0656708da3990b9c2c425867ef02316a929304383bc9c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49337534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf46f5ed0fbc366915b5b4809eca9e33f2ee8f2bb157565b7b5cc29d3cbcaf41`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 14:00:20 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 11 Feb 2023 14:00:20 GMT
ARG ASSET=ce
# Sat, 11 Feb 2023 14:00:21 GMT
ENV ASSET=ce
# Sat, 11 Feb 2023 14:00:21 GMT
ARG EE_PORTS
# Sat, 11 Feb 2023 14:00:21 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Sat, 11 Feb 2023 14:00:21 GMT
ARG KONG_VERSION=2.8.3
# Sat, 11 Feb 2023 14:00:21 GMT
ENV KONG_VERSION=2.8.3
# Fri, 17 Feb 2023 21:05:31 GMT
ARG KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa
# Fri, 17 Feb 2023 21:05:31 GMT
ARG KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
# Fri, 17 Feb 2023 21:05:38 GMT
# ARGS: KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Fri, 17 Feb 2023 21:05:38 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 17 Feb 2023 21:05:38 GMT
USER kong
# Fri, 17 Feb 2023 21:05:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 17 Feb 2023 21:05:39 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 17 Feb 2023 21:05:39 GMT
STOPSIGNAL SIGQUIT
# Fri, 17 Feb 2023 21:05:39 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 17 Feb 2023 21:05:39 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:332cd90dd99acdafaf1be5f2ecbf3e7e8dbb56063cd31b47aa5c172fa53f18ba`  
		Last Modified: Sat, 11 Feb 2023 14:02:34 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34e07d8ee8b056e5949e66ecb76724024fbe556f6f36213dd16ed398f04d20db`  
		Last Modified: Fri, 17 Feb 2023 21:06:17 GMT  
		Size: 46.5 MB (46528761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baccb83225b8a3c516fb22973594a6c72238b6614bebabc09830855eab5657bf`  
		Last Modified: Fri, 17 Feb 2023 21:06:10 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.8.3` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:0b6ad885b3b5ebbd99cfc0c50d4584c49e1ceb1055ccbf71a01b1dfa90c5710e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.5 MB (48522073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24de28b355427f0db0e877d9a43e65156a2e3b645f19b0fbc418219e4c3360e1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:57:50 GMT
LABEL maintainer=Kong <support@konghq.com>
# Fri, 10 Feb 2023 22:57:50 GMT
ARG ASSET=ce
# Fri, 10 Feb 2023 22:57:50 GMT
ENV ASSET=ce
# Fri, 10 Feb 2023 22:57:50 GMT
ARG EE_PORTS
# Fri, 10 Feb 2023 22:57:51 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Fri, 10 Feb 2023 22:57:51 GMT
ARG KONG_VERSION=2.8.3
# Fri, 10 Feb 2023 22:57:51 GMT
ENV KONG_VERSION=2.8.3
# Fri, 17 Feb 2023 23:06:33 GMT
ARG KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa
# Fri, 17 Feb 2023 23:06:33 GMT
ARG KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
# Fri, 17 Feb 2023 23:06:39 GMT
# ARGS: KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Fri, 17 Feb 2023 23:06:40 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 17 Feb 2023 23:06:40 GMT
USER kong
# Fri, 17 Feb 2023 23:06:40 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 17 Feb 2023 23:06:40 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 17 Feb 2023 23:06:40 GMT
STOPSIGNAL SIGQUIT
# Fri, 17 Feb 2023 23:06:40 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 17 Feb 2023 23:06:40 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6251f58952598f508c63c9b905a49fd6e3eced7a7b48980335da9d6b1f66c342`  
		Last Modified: Fri, 17 Feb 2023 23:08:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237c69ba3586458df1a5d9283467b62823f7743cbe26455c26f395956626268e`  
		Last Modified: Fri, 17 Feb 2023 23:08:42 GMT  
		Size: 45.8 MB (45811562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e46fd2edc60f47ed1ba71e37abbfdc128d1208c27da478708b44e00fe588680`  
		Last Modified: Fri, 17 Feb 2023 23:08:36 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.8.3-alpine`

```console
$ docker pull kong@sha256:adad1f4a72229fe3b1768ecc601cb875a4eecb778dc0c7b2b7dc5d7f2825a844
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.8.3-alpine` - linux; amd64

```console
$ docker pull kong@sha256:ae3d663f065f1a138f0656708da3990b9c2c425867ef02316a929304383bc9c0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49337534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf46f5ed0fbc366915b5b4809eca9e33f2ee8f2bb157565b7b5cc29d3cbcaf41`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 14:00:20 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 11 Feb 2023 14:00:20 GMT
ARG ASSET=ce
# Sat, 11 Feb 2023 14:00:21 GMT
ENV ASSET=ce
# Sat, 11 Feb 2023 14:00:21 GMT
ARG EE_PORTS
# Sat, 11 Feb 2023 14:00:21 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Sat, 11 Feb 2023 14:00:21 GMT
ARG KONG_VERSION=2.8.3
# Sat, 11 Feb 2023 14:00:21 GMT
ENV KONG_VERSION=2.8.3
# Fri, 17 Feb 2023 21:05:31 GMT
ARG KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa
# Fri, 17 Feb 2023 21:05:31 GMT
ARG KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
# Fri, 17 Feb 2023 21:05:38 GMT
# ARGS: KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Fri, 17 Feb 2023 21:05:38 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 17 Feb 2023 21:05:38 GMT
USER kong
# Fri, 17 Feb 2023 21:05:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 17 Feb 2023 21:05:39 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 17 Feb 2023 21:05:39 GMT
STOPSIGNAL SIGQUIT
# Fri, 17 Feb 2023 21:05:39 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 17 Feb 2023 21:05:39 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:332cd90dd99acdafaf1be5f2ecbf3e7e8dbb56063cd31b47aa5c172fa53f18ba`  
		Last Modified: Sat, 11 Feb 2023 14:02:34 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34e07d8ee8b056e5949e66ecb76724024fbe556f6f36213dd16ed398f04d20db`  
		Last Modified: Fri, 17 Feb 2023 21:06:17 GMT  
		Size: 46.5 MB (46528761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baccb83225b8a3c516fb22973594a6c72238b6614bebabc09830855eab5657bf`  
		Last Modified: Fri, 17 Feb 2023 21:06:10 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.8.3-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:0b6ad885b3b5ebbd99cfc0c50d4584c49e1ceb1055ccbf71a01b1dfa90c5710e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.5 MB (48522073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24de28b355427f0db0e877d9a43e65156a2e3b645f19b0fbc418219e4c3360e1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:57:50 GMT
LABEL maintainer=Kong <support@konghq.com>
# Fri, 10 Feb 2023 22:57:50 GMT
ARG ASSET=ce
# Fri, 10 Feb 2023 22:57:50 GMT
ENV ASSET=ce
# Fri, 10 Feb 2023 22:57:50 GMT
ARG EE_PORTS
# Fri, 10 Feb 2023 22:57:51 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Fri, 10 Feb 2023 22:57:51 GMT
ARG KONG_VERSION=2.8.3
# Fri, 10 Feb 2023 22:57:51 GMT
ENV KONG_VERSION=2.8.3
# Fri, 17 Feb 2023 23:06:33 GMT
ARG KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa
# Fri, 17 Feb 2023 23:06:33 GMT
ARG KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
# Fri, 17 Feb 2023 23:06:39 GMT
# ARGS: KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Fri, 17 Feb 2023 23:06:40 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 17 Feb 2023 23:06:40 GMT
USER kong
# Fri, 17 Feb 2023 23:06:40 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 17 Feb 2023 23:06:40 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 17 Feb 2023 23:06:40 GMT
STOPSIGNAL SIGQUIT
# Fri, 17 Feb 2023 23:06:40 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 17 Feb 2023 23:06:40 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6251f58952598f508c63c9b905a49fd6e3eced7a7b48980335da9d6b1f66c342`  
		Last Modified: Fri, 17 Feb 2023 23:08:36 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237c69ba3586458df1a5d9283467b62823f7743cbe26455c26f395956626268e`  
		Last Modified: Fri, 17 Feb 2023 23:08:42 GMT  
		Size: 45.8 MB (45811562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e46fd2edc60f47ed1ba71e37abbfdc128d1208c27da478708b44e00fe588680`  
		Last Modified: Fri, 17 Feb 2023 23:08:36 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.8.3-ubuntu`

```console
$ docker pull kong@sha256:5001fb93806c990119edbc19ce78c847b7f0b22d89f31dd9d8025975a76efad9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.8.3-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:a190a0e74c2336d9accdc9d6426e954d15ec37b9482dade934de7aa3cfa78e10
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.2 MB (119176803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2942d886517f5edd5f4606c1659c0871257863b03ea3f72619f7284fa8ea075f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 08 Mar 2023 03:22:42 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:22:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:22:42 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:22:44 GMT
ADD file:4560926e076acae6b8396a9f1e760eee0f53e22e90ce8554dda57f1103547795 in / 
# Wed, 08 Mar 2023 03:22:44 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:54:32 GMT
ARG ASSET=ce
# Thu, 16 Mar 2023 04:54:32 GMT
ENV ASSET=ce
# Thu, 16 Mar 2023 04:54:32 GMT
ARG EE_PORTS
# Thu, 16 Mar 2023 04:54:32 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Thu, 16 Mar 2023 04:54:33 GMT
ARG KONG_VERSION=2.8.3
# Thu, 16 Mar 2023 04:54:33 GMT
ENV KONG_VERSION=2.8.3
# Thu, 16 Mar 2023 04:54:33 GMT
ARG KONG_AMD64_SHA=b52baf1caa300c3ee70ff4d58982085b1da9203c69118c885f00d13954634810
# Thu, 16 Mar 2023 04:54:33 GMT
ARG KONG_ARM64_SHA=1d5c2064d44b76fbb3cabf168dc226e91fedb991ace32915297505d089679fed
# Thu, 16 Mar 2023 04:55:30 GMT
# ARGS: KONG_AMD64_SHA=b52baf1caa300c3ee70ff4d58982085b1da9203c69118c885f00d13954634810 KONG_ARM64_SHA=1d5c2064d44b76fbb3cabf168dc226e91fedb991ace32915297505d089679fed
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Thu, 16 Mar 2023 04:55:30 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 16 Mar 2023 04:55:31 GMT
USER kong
# Thu, 16 Mar 2023 04:55:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 16 Mar 2023 04:55:31 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 16 Mar 2023 04:55:31 GMT
STOPSIGNAL SIGQUIT
# Thu, 16 Mar 2023 04:55:31 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 16 Mar 2023 04:55:31 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:cd150c608fee7837e3a5b28be5c7b540eaf4efa27b3b755d55326470691ce2df`  
		Last Modified: Sun, 12 Mar 2023 07:24:55 GMT  
		Size: 26.7 MB (26710746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c264ce00476e5586f47f4afe2421375303d74eb50bbf62aa7e469fe95b470485`  
		Last Modified: Thu, 16 Mar 2023 04:56:48 GMT  
		Size: 25.1 MB (25081962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9b782f0c05455c50ac819cc88cbf7072451e721d29a648ba17f96c9273e9c9`  
		Last Modified: Thu, 16 Mar 2023 04:56:58 GMT  
		Size: 67.4 MB (67383214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41a647953f9053c2d4350193089c38cf7b29887ad0de4a61c97d74347c1a1991`  
		Last Modified: Thu, 16 Mar 2023 04:56:47 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.8.3-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:951bb9d16837799ad1d89eedb46330e53c93cdf48cfb080c3d791ae4bf172fb5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.8 MB (112828230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:643936a966ffd60cdd971d4264c7dcf48d54a5e6449d0eb3e20773a5f2d72545`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 08 Mar 2023 03:25:33 GMT
ARG RELEASE
# Wed, 08 Mar 2023 03:25:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 03:25:34 GMT
LABEL org.opencontainers.image.version=18.04
# Wed, 08 Mar 2023 03:25:35 GMT
ADD file:5f229d85bac2e85aa7ce97b2168fc61bd401d0151e8940a12d244356f984e65f in / 
# Wed, 08 Mar 2023 03:25:35 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:33:56 GMT
ARG ASSET=ce
# Thu, 16 Mar 2023 02:33:56 GMT
ENV ASSET=ce
# Thu, 16 Mar 2023 02:33:56 GMT
ARG EE_PORTS
# Thu, 16 Mar 2023 02:33:56 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Thu, 16 Mar 2023 02:33:56 GMT
ARG KONG_VERSION=2.8.3
# Thu, 16 Mar 2023 02:33:57 GMT
ENV KONG_VERSION=2.8.3
# Thu, 16 Mar 2023 02:33:57 GMT
ARG KONG_AMD64_SHA=b52baf1caa300c3ee70ff4d58982085b1da9203c69118c885f00d13954634810
# Thu, 16 Mar 2023 02:33:57 GMT
ARG KONG_ARM64_SHA=1d5c2064d44b76fbb3cabf168dc226e91fedb991ace32915297505d089679fed
# Thu, 16 Mar 2023 02:34:29 GMT
# ARGS: KONG_AMD64_SHA=b52baf1caa300c3ee70ff4d58982085b1da9203c69118c885f00d13954634810 KONG_ARM64_SHA=1d5c2064d44b76fbb3cabf168dc226e91fedb991ace32915297505d089679fed
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Thu, 16 Mar 2023 02:34:30 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 16 Mar 2023 02:34:30 GMT
USER kong
# Thu, 16 Mar 2023 02:34:30 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 16 Mar 2023 02:34:30 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 16 Mar 2023 02:34:30 GMT
STOPSIGNAL SIGQUIT
# Thu, 16 Mar 2023 02:34:30 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 16 Mar 2023 02:34:30 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:c21a0233221a76e66b6c10d2445f591bd28eb0773e6cb539474d6dca9ea0b594`  
		Last Modified: Sun, 12 Mar 2023 07:27:31 GMT  
		Size: 23.7 MB (23734706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f9a95d5aae174d1b475bd7ae3237db539e041937ba215ec5df684cee967f77`  
		Last Modified: Thu, 16 Mar 2023 02:35:40 GMT  
		Size: 25.1 MB (25081962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614f9c3cf77e1b393d10fe009e6d644bef38e718aa8220595654adfe78c2ea45`  
		Last Modified: Thu, 16 Mar 2023 02:35:48 GMT  
		Size: 64.0 MB (64010681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2888e6d56a7ff05f896b7866b11ce8896d1c9eade03af34bbebf90c41a2a9a`  
		Last Modified: Thu, 16 Mar 2023 02:35:39 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3`

```console
$ docker pull kong@sha256:79f0393caaec0a4bef96c6735520646061896b8629974ad802921f7e4af61963
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:3` - linux; amd64

```console
$ docker pull kong@sha256:e39b654c5c2fbfbfe528613dac50164fbd389a0aba712033d28c8b0e9bfc3280
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.9 MB (36926241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a67d04eb7448a9987ba1a35e28ba76e396acf9a2bdefeb7d65d28337bff1dea`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Sat, 25 Mar 2023 00:51:01 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Sat, 25 Mar 2023 00:51:01 GMT
ARG KONG_VERSION=3.2.2
# Sat, 25 Mar 2023 00:51:01 GMT
ENV KONG_VERSION=3.2.2
# Sat, 25 Mar 2023 00:51:01 GMT
ARG KONG_SHA256=a07c3bc0307e2d8fe33acb8be5fe659f348279540eaa267bc6968005094835ef
# Sat, 25 Mar 2023 00:51:01 GMT
ARG KONG_PREFIX=/usr/local/kong
# Sat, 25 Mar 2023 00:51:01 GMT
ENV KONG_PREFIX=/usr/local/kong
# Sat, 25 Mar 2023 00:51:01 GMT
ARG ASSET=remote
# Sat, 25 Mar 2023 00:51:01 GMT
ARG EE_PORTS
# Sat, 25 Mar 2023 00:51:01 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Sat, 25 Mar 2023 00:51:07 GMT
# ARGS: ASSET=remote KONG_SHA256=a07c3bc0307e2d8fe33acb8be5fe659f348279540eaa267bc6968005094835ef
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     export ARCH='amd64';     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc perl tzdata libcap zlib zlib-dev bash yaml     && adduser -S kong     && addgroup -S kong     && mkdir -p "${KONG_PREFIX}"     && chown -R kong:0 ${KONG_PREFIX}     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u ${KONG_PREFIX}     && rm -rf /tmp/kong.apk.tar.gz     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Sat, 25 Mar 2023 00:51:08 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Sat, 25 Mar 2023 00:51:08 GMT
USER kong
# Sat, 25 Mar 2023 00:51:08 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Mar 2023 00:51:08 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 25 Mar 2023 00:51:08 GMT
STOPSIGNAL SIGQUIT
# Sat, 25 Mar 2023 00:51:08 GMT
HEALTHCHECK &{["CMD-SHELL" "kong-health"] "1m0s" "10s" "0s" '\n'}
# Sat, 25 Mar 2023 00:51:08 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a260cdfa2fbd0e7eb62bccc7f6deabe23c93bb0456c841a72399e8b4d5eb4c6e`  
		Last Modified: Sat, 25 Mar 2023 00:52:31 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fa46152c72850607722b515840cf2b8eb72a29d712037b0df457beee533d4b`  
		Last Modified: Sat, 25 Mar 2023 00:52:36 GMT  
		Size: 33.6 MB (33550506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5682cda435615908fe6b508dcc0f128eb35ba3776880f51f7da735e58141379d`  
		Last Modified: Sat, 25 Mar 2023 00:52:31 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.0`

```console
$ docker pull kong@sha256:ed2dd3b2712ac3ff20dbdc82d5c20f879f379ca738dd0a922847dab51ba6f73d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.0` - linux; amd64

```console
$ docker pull kong@sha256:5c2c8369e9e86df300cd7eaf81c5e2c00e42982ce9121d7d8ce720d9c1fc4186
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75644128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd658eaac3acd2573b99af069af18e0cb6eb943b876e551be3f48078aace6dd5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 13:59:53 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Sat, 11 Feb 2023 14:00:07 GMT
ARG KONG_VERSION=3.0.2
# Sat, 11 Feb 2023 14:00:07 GMT
ENV KONG_VERSION=3.0.2
# Sat, 11 Feb 2023 14:00:07 GMT
ARG KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e
# Sat, 11 Feb 2023 14:00:07 GMT
ARG KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
# Sat, 11 Feb 2023 14:00:07 GMT
ARG ASSET=remote
# Sat, 11 Feb 2023 14:00:07 GMT
ARG EE_PORTS
# Sat, 11 Feb 2023 14:00:07 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Sat, 11 Feb 2023 14:00:15 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Sat, 11 Feb 2023 14:00:16 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Sat, 11 Feb 2023 14:00:16 GMT
USER kong
# Sat, 11 Feb 2023 14:00:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 11 Feb 2023 14:00:16 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 11 Feb 2023 14:00:16 GMT
STOPSIGNAL SIGQUIT
# Sat, 11 Feb 2023 14:00:16 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Sat, 11 Feb 2023 14:00:16 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc445c500c7e2969a0df10c742d1f08b399e9183e7dbc626be205477aee2c52`  
		Last Modified: Sat, 11 Feb 2023 14:02:13 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79380bdff2a24981734ba5da4898b9a0c18f05842cabede3f6ec945a12eb02d1`  
		Last Modified: Sat, 11 Feb 2023 14:02:21 GMT  
		Size: 72.8 MB (72835351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3695f8a90b9c4497448ae194928af5052b42aa0d708895019b4d6415d5591e1e`  
		Last Modified: Sat, 11 Feb 2023 14:02:13 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.0` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:7df485332188842c5b2c958c4e261815f187b742c9b524876444a8b9d9e9d805
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73632145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7984ea834ae8b2ade0dd8bd6b1db4e9129712bb76067b9736052f34387190e23`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:57:24 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 10 Feb 2023 22:57:37 GMT
ARG KONG_VERSION=3.0.2
# Fri, 10 Feb 2023 22:57:37 GMT
ENV KONG_VERSION=3.0.2
# Fri, 10 Feb 2023 22:57:37 GMT
ARG KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e
# Fri, 10 Feb 2023 22:57:37 GMT
ARG KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
# Fri, 10 Feb 2023 22:57:37 GMT
ARG ASSET=remote
# Fri, 10 Feb 2023 22:57:37 GMT
ARG EE_PORTS
# Fri, 10 Feb 2023 22:57:37 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Fri, 10 Feb 2023 22:57:45 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Fri, 10 Feb 2023 22:57:45 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 10 Feb 2023 22:57:45 GMT
USER kong
# Fri, 10 Feb 2023 22:57:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 10 Feb 2023 22:57:46 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 10 Feb 2023 22:57:46 GMT
STOPSIGNAL SIGQUIT
# Fri, 10 Feb 2023 22:57:46 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 10 Feb 2023 22:57:46 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab4f79effaded08ffc458dcd0b8666b376c40b38d1f8fc32e985a36e40c3d3e`  
		Last Modified: Fri, 10 Feb 2023 23:01:33 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60c99787c1181135a451bcc085437887f84003ec3641e2807e332331b11071c`  
		Last Modified: Fri, 10 Feb 2023 23:01:41 GMT  
		Size: 70.9 MB (70921631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf39f263f853308176746bf2be8939c16a2c9e1465efcdd42debcee7262357dc`  
		Last Modified: Fri, 10 Feb 2023 23:01:34 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.0-alpine`

```console
$ docker pull kong@sha256:ed2dd3b2712ac3ff20dbdc82d5c20f879f379ca738dd0a922847dab51ba6f73d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.0-alpine` - linux; amd64

```console
$ docker pull kong@sha256:5c2c8369e9e86df300cd7eaf81c5e2c00e42982ce9121d7d8ce720d9c1fc4186
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75644128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd658eaac3acd2573b99af069af18e0cb6eb943b876e551be3f48078aace6dd5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 13:59:53 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Sat, 11 Feb 2023 14:00:07 GMT
ARG KONG_VERSION=3.0.2
# Sat, 11 Feb 2023 14:00:07 GMT
ENV KONG_VERSION=3.0.2
# Sat, 11 Feb 2023 14:00:07 GMT
ARG KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e
# Sat, 11 Feb 2023 14:00:07 GMT
ARG KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
# Sat, 11 Feb 2023 14:00:07 GMT
ARG ASSET=remote
# Sat, 11 Feb 2023 14:00:07 GMT
ARG EE_PORTS
# Sat, 11 Feb 2023 14:00:07 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Sat, 11 Feb 2023 14:00:15 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Sat, 11 Feb 2023 14:00:16 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Sat, 11 Feb 2023 14:00:16 GMT
USER kong
# Sat, 11 Feb 2023 14:00:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 11 Feb 2023 14:00:16 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 11 Feb 2023 14:00:16 GMT
STOPSIGNAL SIGQUIT
# Sat, 11 Feb 2023 14:00:16 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Sat, 11 Feb 2023 14:00:16 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc445c500c7e2969a0df10c742d1f08b399e9183e7dbc626be205477aee2c52`  
		Last Modified: Sat, 11 Feb 2023 14:02:13 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79380bdff2a24981734ba5da4898b9a0c18f05842cabede3f6ec945a12eb02d1`  
		Last Modified: Sat, 11 Feb 2023 14:02:21 GMT  
		Size: 72.8 MB (72835351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3695f8a90b9c4497448ae194928af5052b42aa0d708895019b4d6415d5591e1e`  
		Last Modified: Sat, 11 Feb 2023 14:02:13 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.0-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:7df485332188842c5b2c958c4e261815f187b742c9b524876444a8b9d9e9d805
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73632145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7984ea834ae8b2ade0dd8bd6b1db4e9129712bb76067b9736052f34387190e23`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:57:24 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 10 Feb 2023 22:57:37 GMT
ARG KONG_VERSION=3.0.2
# Fri, 10 Feb 2023 22:57:37 GMT
ENV KONG_VERSION=3.0.2
# Fri, 10 Feb 2023 22:57:37 GMT
ARG KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e
# Fri, 10 Feb 2023 22:57:37 GMT
ARG KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
# Fri, 10 Feb 2023 22:57:37 GMT
ARG ASSET=remote
# Fri, 10 Feb 2023 22:57:37 GMT
ARG EE_PORTS
# Fri, 10 Feb 2023 22:57:37 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Fri, 10 Feb 2023 22:57:45 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Fri, 10 Feb 2023 22:57:45 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 10 Feb 2023 22:57:45 GMT
USER kong
# Fri, 10 Feb 2023 22:57:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 10 Feb 2023 22:57:46 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 10 Feb 2023 22:57:46 GMT
STOPSIGNAL SIGQUIT
# Fri, 10 Feb 2023 22:57:46 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 10 Feb 2023 22:57:46 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab4f79effaded08ffc458dcd0b8666b376c40b38d1f8fc32e985a36e40c3d3e`  
		Last Modified: Fri, 10 Feb 2023 23:01:33 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60c99787c1181135a451bcc085437887f84003ec3641e2807e332331b11071c`  
		Last Modified: Fri, 10 Feb 2023 23:01:41 GMT  
		Size: 70.9 MB (70921631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf39f263f853308176746bf2be8939c16a2c9e1465efcdd42debcee7262357dc`  
		Last Modified: Fri, 10 Feb 2023 23:01:34 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.0-ubuntu`

```console
$ docker pull kong@sha256:b1315b4930a17790a731bf39dbaf753158ff81f5d682ed176ca1b10da37aeb1e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.0-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:cf36c2ce52780db49268cfb74e4e3a3c46250d6bccba79d4faa5ee62399eab38
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.7 MB (101695556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d7ede3ebd282e831d3adc64358caeb4d0f90972ef2b6159aff6a8bea41f4990`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:41:26 GMT
ADD file:20f2ff22b9a8ca9bec5178036c9ebc525a12cd4312daf5d14a9a631a30be20e1 in / 
# Wed, 08 Mar 2023 04:41:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:52:49 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 16 Mar 2023 04:52:49 GMT
ARG ASSET=ce
# Thu, 16 Mar 2023 04:52:49 GMT
ENV ASSET=ce
# Thu, 16 Mar 2023 04:52:49 GMT
ARG EE_PORTS
# Thu, 16 Mar 2023 04:52:49 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Thu, 16 Mar 2023 04:54:01 GMT
ARG KONG_VERSION=3.0.2
# Thu, 16 Mar 2023 04:54:01 GMT
ENV KONG_VERSION=3.0.2
# Thu, 16 Mar 2023 04:54:01 GMT
ARG KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396
# Thu, 16 Mar 2023 04:54:01 GMT
ARG KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
# Thu, 16 Mar 2023 04:54:23 GMT
# ARGS: KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396 KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Thu, 16 Mar 2023 04:54:24 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 16 Mar 2023 04:54:24 GMT
USER kong
# Thu, 16 Mar 2023 04:54:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 16 Mar 2023 04:54:24 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 16 Mar 2023 04:54:24 GMT
STOPSIGNAL SIGQUIT
# Thu, 16 Mar 2023 04:54:24 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 16 Mar 2023 04:54:24 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:5544ebdc0c7b82aa6901eae124b1d220914d2629a9bde25396d7ee9cfd273a8f`  
		Last Modified: Wed, 08 Mar 2023 09:02:58 GMT  
		Size: 28.6 MB (28578068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0310ac76a75b3413c8efa68949fbf815db82ac8624b9d1ca500280c0722969f`  
		Last Modified: Thu, 16 Mar 2023 04:56:02 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c081dda2d728a2bcb14aa145bc47b32465be7ac4386c1eab0d9038e88f017fa`  
		Last Modified: Thu, 16 Mar 2023 04:56:37 GMT  
		Size: 73.1 MB (73116481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5daa755535d2d64c240f9c2c483544fa058c572eca788ecf128771dc70bf27`  
		Last Modified: Thu, 16 Mar 2023 04:56:25 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.0-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:7e0367d33fe0f054ffd29b2a469ab7c7cb09257bd962ffc1897314bafeaa12b1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.9 MB (98936932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55d2be0b24917e50d2eab58f26ef173167fd3e79fd4cf75ecb4edb5f0a125a5d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 08 Mar 2023 04:34:20 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:34:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:34:24 GMT
ADD file:e73d5d005a3ba2c2fb3d8585a1f19daf5ea9ed75af5a2f97b1cc6f7f03db0cdc in / 
# Wed, 08 Mar 2023 04:34:24 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:32:55 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 16 Mar 2023 02:32:55 GMT
ARG ASSET=ce
# Thu, 16 Mar 2023 02:32:55 GMT
ENV ASSET=ce
# Thu, 16 Mar 2023 02:32:55 GMT
ARG EE_PORTS
# Thu, 16 Mar 2023 02:32:56 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Thu, 16 Mar 2023 02:33:31 GMT
ARG KONG_VERSION=3.0.2
# Thu, 16 Mar 2023 02:33:31 GMT
ENV KONG_VERSION=3.0.2
# Thu, 16 Mar 2023 02:33:31 GMT
ARG KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396
# Thu, 16 Mar 2023 02:33:31 GMT
ARG KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
# Thu, 16 Mar 2023 02:33:47 GMT
# ARGS: KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396 KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Thu, 16 Mar 2023 02:33:48 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 16 Mar 2023 02:33:48 GMT
USER kong
# Thu, 16 Mar 2023 02:33:48 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 16 Mar 2023 02:33:49 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 16 Mar 2023 02:33:49 GMT
STOPSIGNAL SIGQUIT
# Thu, 16 Mar 2023 02:33:49 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 16 Mar 2023 02:33:49 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:0c68957c744181d1b5cae80a96971c651cec74faeade53191985b92abff361da`  
		Last Modified: Wed, 08 Mar 2023 20:37:17 GMT  
		Size: 27.2 MB (27196161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e58bbdc23e3f7ce51624faf13094ccd5a8b2bc147310d449308170aaea47858`  
		Last Modified: Thu, 16 Mar 2023 02:34:59 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6eea3d777ba00cecabfd931e6359202bbd38bedc9f4ef929dfe5bff8d69edf`  
		Last Modified: Thu, 16 Mar 2023 02:35:28 GMT  
		Size: 71.7 MB (71739763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93319c3075950636fd68326675331a1392e90a3704eaddc6350957f4167d2fc9`  
		Last Modified: Thu, 16 Mar 2023 02:35:20 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.0.2`

```console
$ docker pull kong@sha256:ed2dd3b2712ac3ff20dbdc82d5c20f879f379ca738dd0a922847dab51ba6f73d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.0.2` - linux; amd64

```console
$ docker pull kong@sha256:5c2c8369e9e86df300cd7eaf81c5e2c00e42982ce9121d7d8ce720d9c1fc4186
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75644128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd658eaac3acd2573b99af069af18e0cb6eb943b876e551be3f48078aace6dd5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 13:59:53 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Sat, 11 Feb 2023 14:00:07 GMT
ARG KONG_VERSION=3.0.2
# Sat, 11 Feb 2023 14:00:07 GMT
ENV KONG_VERSION=3.0.2
# Sat, 11 Feb 2023 14:00:07 GMT
ARG KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e
# Sat, 11 Feb 2023 14:00:07 GMT
ARG KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
# Sat, 11 Feb 2023 14:00:07 GMT
ARG ASSET=remote
# Sat, 11 Feb 2023 14:00:07 GMT
ARG EE_PORTS
# Sat, 11 Feb 2023 14:00:07 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Sat, 11 Feb 2023 14:00:15 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Sat, 11 Feb 2023 14:00:16 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Sat, 11 Feb 2023 14:00:16 GMT
USER kong
# Sat, 11 Feb 2023 14:00:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 11 Feb 2023 14:00:16 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 11 Feb 2023 14:00:16 GMT
STOPSIGNAL SIGQUIT
# Sat, 11 Feb 2023 14:00:16 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Sat, 11 Feb 2023 14:00:16 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc445c500c7e2969a0df10c742d1f08b399e9183e7dbc626be205477aee2c52`  
		Last Modified: Sat, 11 Feb 2023 14:02:13 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79380bdff2a24981734ba5da4898b9a0c18f05842cabede3f6ec945a12eb02d1`  
		Last Modified: Sat, 11 Feb 2023 14:02:21 GMT  
		Size: 72.8 MB (72835351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3695f8a90b9c4497448ae194928af5052b42aa0d708895019b4d6415d5591e1e`  
		Last Modified: Sat, 11 Feb 2023 14:02:13 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.0.2` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:7df485332188842c5b2c958c4e261815f187b742c9b524876444a8b9d9e9d805
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73632145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7984ea834ae8b2ade0dd8bd6b1db4e9129712bb76067b9736052f34387190e23`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:57:24 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 10 Feb 2023 22:57:37 GMT
ARG KONG_VERSION=3.0.2
# Fri, 10 Feb 2023 22:57:37 GMT
ENV KONG_VERSION=3.0.2
# Fri, 10 Feb 2023 22:57:37 GMT
ARG KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e
# Fri, 10 Feb 2023 22:57:37 GMT
ARG KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
# Fri, 10 Feb 2023 22:57:37 GMT
ARG ASSET=remote
# Fri, 10 Feb 2023 22:57:37 GMT
ARG EE_PORTS
# Fri, 10 Feb 2023 22:57:37 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Fri, 10 Feb 2023 22:57:45 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Fri, 10 Feb 2023 22:57:45 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 10 Feb 2023 22:57:45 GMT
USER kong
# Fri, 10 Feb 2023 22:57:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 10 Feb 2023 22:57:46 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 10 Feb 2023 22:57:46 GMT
STOPSIGNAL SIGQUIT
# Fri, 10 Feb 2023 22:57:46 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 10 Feb 2023 22:57:46 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab4f79effaded08ffc458dcd0b8666b376c40b38d1f8fc32e985a36e40c3d3e`  
		Last Modified: Fri, 10 Feb 2023 23:01:33 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60c99787c1181135a451bcc085437887f84003ec3641e2807e332331b11071c`  
		Last Modified: Fri, 10 Feb 2023 23:01:41 GMT  
		Size: 70.9 MB (70921631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf39f263f853308176746bf2be8939c16a2c9e1465efcdd42debcee7262357dc`  
		Last Modified: Fri, 10 Feb 2023 23:01:34 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.0.2-alpine`

```console
$ docker pull kong@sha256:ed2dd3b2712ac3ff20dbdc82d5c20f879f379ca738dd0a922847dab51ba6f73d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.0.2-alpine` - linux; amd64

```console
$ docker pull kong@sha256:5c2c8369e9e86df300cd7eaf81c5e2c00e42982ce9121d7d8ce720d9c1fc4186
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75644128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd658eaac3acd2573b99af069af18e0cb6eb943b876e551be3f48078aace6dd5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 13:59:53 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Sat, 11 Feb 2023 14:00:07 GMT
ARG KONG_VERSION=3.0.2
# Sat, 11 Feb 2023 14:00:07 GMT
ENV KONG_VERSION=3.0.2
# Sat, 11 Feb 2023 14:00:07 GMT
ARG KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e
# Sat, 11 Feb 2023 14:00:07 GMT
ARG KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
# Sat, 11 Feb 2023 14:00:07 GMT
ARG ASSET=remote
# Sat, 11 Feb 2023 14:00:07 GMT
ARG EE_PORTS
# Sat, 11 Feb 2023 14:00:07 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Sat, 11 Feb 2023 14:00:15 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Sat, 11 Feb 2023 14:00:16 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Sat, 11 Feb 2023 14:00:16 GMT
USER kong
# Sat, 11 Feb 2023 14:00:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 11 Feb 2023 14:00:16 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 11 Feb 2023 14:00:16 GMT
STOPSIGNAL SIGQUIT
# Sat, 11 Feb 2023 14:00:16 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Sat, 11 Feb 2023 14:00:16 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc445c500c7e2969a0df10c742d1f08b399e9183e7dbc626be205477aee2c52`  
		Last Modified: Sat, 11 Feb 2023 14:02:13 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79380bdff2a24981734ba5da4898b9a0c18f05842cabede3f6ec945a12eb02d1`  
		Last Modified: Sat, 11 Feb 2023 14:02:21 GMT  
		Size: 72.8 MB (72835351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3695f8a90b9c4497448ae194928af5052b42aa0d708895019b4d6415d5591e1e`  
		Last Modified: Sat, 11 Feb 2023 14:02:13 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.0.2-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:7df485332188842c5b2c958c4e261815f187b742c9b524876444a8b9d9e9d805
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73632145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7984ea834ae8b2ade0dd8bd6b1db4e9129712bb76067b9736052f34387190e23`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:57:24 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 10 Feb 2023 22:57:37 GMT
ARG KONG_VERSION=3.0.2
# Fri, 10 Feb 2023 22:57:37 GMT
ENV KONG_VERSION=3.0.2
# Fri, 10 Feb 2023 22:57:37 GMT
ARG KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e
# Fri, 10 Feb 2023 22:57:37 GMT
ARG KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
# Fri, 10 Feb 2023 22:57:37 GMT
ARG ASSET=remote
# Fri, 10 Feb 2023 22:57:37 GMT
ARG EE_PORTS
# Fri, 10 Feb 2023 22:57:37 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Fri, 10 Feb 2023 22:57:45 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Fri, 10 Feb 2023 22:57:45 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 10 Feb 2023 22:57:45 GMT
USER kong
# Fri, 10 Feb 2023 22:57:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 10 Feb 2023 22:57:46 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 10 Feb 2023 22:57:46 GMT
STOPSIGNAL SIGQUIT
# Fri, 10 Feb 2023 22:57:46 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 10 Feb 2023 22:57:46 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab4f79effaded08ffc458dcd0b8666b376c40b38d1f8fc32e985a36e40c3d3e`  
		Last Modified: Fri, 10 Feb 2023 23:01:33 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60c99787c1181135a451bcc085437887f84003ec3641e2807e332331b11071c`  
		Last Modified: Fri, 10 Feb 2023 23:01:41 GMT  
		Size: 70.9 MB (70921631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf39f263f853308176746bf2be8939c16a2c9e1465efcdd42debcee7262357dc`  
		Last Modified: Fri, 10 Feb 2023 23:01:34 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.0.2-ubuntu`

```console
$ docker pull kong@sha256:b1315b4930a17790a731bf39dbaf753158ff81f5d682ed176ca1b10da37aeb1e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.0.2-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:cf36c2ce52780db49268cfb74e4e3a3c46250d6bccba79d4faa5ee62399eab38
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.7 MB (101695556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d7ede3ebd282e831d3adc64358caeb4d0f90972ef2b6159aff6a8bea41f4990`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:41:26 GMT
ADD file:20f2ff22b9a8ca9bec5178036c9ebc525a12cd4312daf5d14a9a631a30be20e1 in / 
# Wed, 08 Mar 2023 04:41:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:52:49 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 16 Mar 2023 04:52:49 GMT
ARG ASSET=ce
# Thu, 16 Mar 2023 04:52:49 GMT
ENV ASSET=ce
# Thu, 16 Mar 2023 04:52:49 GMT
ARG EE_PORTS
# Thu, 16 Mar 2023 04:52:49 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Thu, 16 Mar 2023 04:54:01 GMT
ARG KONG_VERSION=3.0.2
# Thu, 16 Mar 2023 04:54:01 GMT
ENV KONG_VERSION=3.0.2
# Thu, 16 Mar 2023 04:54:01 GMT
ARG KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396
# Thu, 16 Mar 2023 04:54:01 GMT
ARG KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
# Thu, 16 Mar 2023 04:54:23 GMT
# ARGS: KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396 KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Thu, 16 Mar 2023 04:54:24 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 16 Mar 2023 04:54:24 GMT
USER kong
# Thu, 16 Mar 2023 04:54:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 16 Mar 2023 04:54:24 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 16 Mar 2023 04:54:24 GMT
STOPSIGNAL SIGQUIT
# Thu, 16 Mar 2023 04:54:24 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 16 Mar 2023 04:54:24 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:5544ebdc0c7b82aa6901eae124b1d220914d2629a9bde25396d7ee9cfd273a8f`  
		Last Modified: Wed, 08 Mar 2023 09:02:58 GMT  
		Size: 28.6 MB (28578068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0310ac76a75b3413c8efa68949fbf815db82ac8624b9d1ca500280c0722969f`  
		Last Modified: Thu, 16 Mar 2023 04:56:02 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c081dda2d728a2bcb14aa145bc47b32465be7ac4386c1eab0d9038e88f017fa`  
		Last Modified: Thu, 16 Mar 2023 04:56:37 GMT  
		Size: 73.1 MB (73116481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5daa755535d2d64c240f9c2c483544fa058c572eca788ecf128771dc70bf27`  
		Last Modified: Thu, 16 Mar 2023 04:56:25 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.0.2-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:7e0367d33fe0f054ffd29b2a469ab7c7cb09257bd962ffc1897314bafeaa12b1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.9 MB (98936932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55d2be0b24917e50d2eab58f26ef173167fd3e79fd4cf75ecb4edb5f0a125a5d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 08 Mar 2023 04:34:20 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:34:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:34:24 GMT
ADD file:e73d5d005a3ba2c2fb3d8585a1f19daf5ea9ed75af5a2f97b1cc6f7f03db0cdc in / 
# Wed, 08 Mar 2023 04:34:24 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:32:55 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 16 Mar 2023 02:32:55 GMT
ARG ASSET=ce
# Thu, 16 Mar 2023 02:32:55 GMT
ENV ASSET=ce
# Thu, 16 Mar 2023 02:32:55 GMT
ARG EE_PORTS
# Thu, 16 Mar 2023 02:32:56 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Thu, 16 Mar 2023 02:33:31 GMT
ARG KONG_VERSION=3.0.2
# Thu, 16 Mar 2023 02:33:31 GMT
ENV KONG_VERSION=3.0.2
# Thu, 16 Mar 2023 02:33:31 GMT
ARG KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396
# Thu, 16 Mar 2023 02:33:31 GMT
ARG KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
# Thu, 16 Mar 2023 02:33:47 GMT
# ARGS: KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396 KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Thu, 16 Mar 2023 02:33:48 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 16 Mar 2023 02:33:48 GMT
USER kong
# Thu, 16 Mar 2023 02:33:48 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 16 Mar 2023 02:33:49 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 16 Mar 2023 02:33:49 GMT
STOPSIGNAL SIGQUIT
# Thu, 16 Mar 2023 02:33:49 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 16 Mar 2023 02:33:49 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:0c68957c744181d1b5cae80a96971c651cec74faeade53191985b92abff361da`  
		Last Modified: Wed, 08 Mar 2023 20:37:17 GMT  
		Size: 27.2 MB (27196161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e58bbdc23e3f7ce51624faf13094ccd5a8b2bc147310d449308170aaea47858`  
		Last Modified: Thu, 16 Mar 2023 02:34:59 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6eea3d777ba00cecabfd931e6359202bbd38bedc9f4ef929dfe5bff8d69edf`  
		Last Modified: Thu, 16 Mar 2023 02:35:28 GMT  
		Size: 71.7 MB (71739763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93319c3075950636fd68326675331a1392e90a3704eaddc6350957f4167d2fc9`  
		Last Modified: Thu, 16 Mar 2023 02:35:20 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.1`

```console
$ docker pull kong@sha256:f97a5087ba9331c9ae2e78707df9eed51954f28d83f04358a120e2440ef05eca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.1` - linux; amd64

```console
$ docker pull kong@sha256:36258c1d9dd6f5da8cc0403af4650f5d95296e48f83e330ec8f5fd3e3883f162
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75689080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b76469f8b580bfa16be2cce693e879f0c97cf21dab83dca21aa46b9597ed0747`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 13:59:53 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Sat, 11 Feb 2023 13:59:53 GMT
ARG KONG_VERSION=3.1.1
# Sat, 11 Feb 2023 13:59:53 GMT
ENV KONG_VERSION=3.1.1
# Sat, 11 Feb 2023 13:59:53 GMT
ARG KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c
# Sat, 11 Feb 2023 13:59:53 GMT
ARG KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
# Sat, 11 Feb 2023 13:59:53 GMT
ARG ASSET=remote
# Sat, 11 Feb 2023 13:59:53 GMT
ARG EE_PORTS
# Sat, 11 Feb 2023 13:59:53 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Sat, 11 Feb 2023 14:00:01 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Sat, 11 Feb 2023 14:00:01 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Sat, 11 Feb 2023 14:00:01 GMT
USER kong
# Sat, 11 Feb 2023 14:00:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 11 Feb 2023 14:00:01 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 11 Feb 2023 14:00:01 GMT
STOPSIGNAL SIGQUIT
# Sat, 11 Feb 2023 14:00:02 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Sat, 11 Feb 2023 14:00:02 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256d8d79435b0bcc04e2462111b09b5a21093f05b20ff38b484036c091891ff2`  
		Last Modified: Sat, 11 Feb 2023 14:01:47 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8a6c1e7dd831b077e9ed68a8dd90af0a86718c8e0873c8c3dd6f877dc08ded`  
		Last Modified: Sat, 11 Feb 2023 14:01:56 GMT  
		Size: 72.9 MB (72880307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce630ba9f4f76fa8c33b114ce2e01fe176acd00019a99c6e2c8d9f95c2157de`  
		Last Modified: Sat, 11 Feb 2023 14:01:47 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.1` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:6cb2e58647fc834e751ed3ff2618757f854e8eea6baa9872b241a5b4922cd2f9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.7 MB (73705071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b194d85727fe1e9c5e8b3df6cfc7434c14b7c9f32b9a179c5b02f56eeced8861`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:57:24 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 10 Feb 2023 22:57:24 GMT
ARG KONG_VERSION=3.1.1
# Fri, 10 Feb 2023 22:57:24 GMT
ENV KONG_VERSION=3.1.1
# Fri, 10 Feb 2023 22:57:24 GMT
ARG KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c
# Fri, 10 Feb 2023 22:57:24 GMT
ARG KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
# Fri, 10 Feb 2023 22:57:24 GMT
ARG ASSET=remote
# Fri, 10 Feb 2023 22:57:25 GMT
ARG EE_PORTS
# Fri, 10 Feb 2023 22:57:25 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Fri, 10 Feb 2023 22:57:31 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Fri, 10 Feb 2023 22:57:32 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 10 Feb 2023 22:57:32 GMT
USER kong
# Fri, 10 Feb 2023 22:57:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 10 Feb 2023 22:57:32 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 10 Feb 2023 22:57:32 GMT
STOPSIGNAL SIGQUIT
# Fri, 10 Feb 2023 22:57:32 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 10 Feb 2023 22:57:32 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7d673d809eb0c188ffdf72da404979eec54eac371b562252cfc579c3d1663f`  
		Last Modified: Fri, 10 Feb 2023 23:01:05 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fc02867f544f9cde11ef414aceb1bdd1235a8da723f6795fe0d358ecd90638`  
		Last Modified: Fri, 10 Feb 2023 23:01:13 GMT  
		Size: 71.0 MB (70994554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ecf15059d665b9ba5f1604f250bc942cb91274a0115c4067ea8cc0887869519`  
		Last Modified: Fri, 10 Feb 2023 23:01:05 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.1-ubuntu`

```console
$ docker pull kong@sha256:975961b67d0fbc8c196a6b5793a6dd37c31bc178ab6203f1c6f904b9607e8e8b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.1-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:8ed9bd110f3da4288bdbeea1e304bad5871743e77bb8c64c47a3e61672777ee0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.7 MB (101726780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33890cc7473f3e37ff7fca779b2a0f56eeba8c5dc3fe6f0262e000b3c57eb911`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:41:26 GMT
ADD file:20f2ff22b9a8ca9bec5178036c9ebc525a12cd4312daf5d14a9a631a30be20e1 in / 
# Wed, 08 Mar 2023 04:41:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:52:49 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 16 Mar 2023 04:52:49 GMT
ARG ASSET=ce
# Thu, 16 Mar 2023 04:52:49 GMT
ENV ASSET=ce
# Thu, 16 Mar 2023 04:52:49 GMT
ARG EE_PORTS
# Thu, 16 Mar 2023 04:52:49 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Thu, 16 Mar 2023 04:52:49 GMT
ARG KONG_VERSION=3.1.1
# Thu, 16 Mar 2023 04:52:50 GMT
ENV KONG_VERSION=3.1.1
# Thu, 16 Mar 2023 04:52:50 GMT
ARG KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b
# Thu, 16 Mar 2023 04:52:50 GMT
ARG KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
# Thu, 16 Mar 2023 04:53:44 GMT
# ARGS: KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Thu, 16 Mar 2023 04:53:45 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 16 Mar 2023 04:53:45 GMT
USER kong
# Thu, 16 Mar 2023 04:53:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 16 Mar 2023 04:53:45 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 16 Mar 2023 04:53:45 GMT
STOPSIGNAL SIGQUIT
# Thu, 16 Mar 2023 04:53:45 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 16 Mar 2023 04:53:45 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:5544ebdc0c7b82aa6901eae124b1d220914d2629a9bde25396d7ee9cfd273a8f`  
		Last Modified: Wed, 08 Mar 2023 09:02:58 GMT  
		Size: 28.6 MB (28578068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0310ac76a75b3413c8efa68949fbf815db82ac8624b9d1ca500280c0722969f`  
		Last Modified: Thu, 16 Mar 2023 04:56:02 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a7f03c733975322bd977f20abb1e6abb79a4c3d9b211be3afa32f6e14d522ac`  
		Last Modified: Thu, 16 Mar 2023 04:56:13 GMT  
		Size: 73.1 MB (73147706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31059c935546737773cd25b29801a0113c45428a34a09cc5676aa03f11aeff8f`  
		Last Modified: Thu, 16 Mar 2023 04:56:02 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.1-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:9f9955f0bdc78ba76c52a2eba62efede56b47fb645ec01b4356579f5eddfeb51
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.0 MB (98966357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38ae7460b241a3710fe8abe5f21fea1620f771abbed7d26aeaef4b916de33c55`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 08 Mar 2023 04:34:20 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:34:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:34:24 GMT
ADD file:e73d5d005a3ba2c2fb3d8585a1f19daf5ea9ed75af5a2f97b1cc6f7f03db0cdc in / 
# Wed, 08 Mar 2023 04:34:24 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:32:55 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 16 Mar 2023 02:32:55 GMT
ARG ASSET=ce
# Thu, 16 Mar 2023 02:32:55 GMT
ENV ASSET=ce
# Thu, 16 Mar 2023 02:32:55 GMT
ARG EE_PORTS
# Thu, 16 Mar 2023 02:32:56 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Thu, 16 Mar 2023 02:32:56 GMT
ARG KONG_VERSION=3.1.1
# Thu, 16 Mar 2023 02:32:56 GMT
ENV KONG_VERSION=3.1.1
# Thu, 16 Mar 2023 02:32:56 GMT
ARG KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b
# Thu, 16 Mar 2023 02:32:56 GMT
ARG KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
# Thu, 16 Mar 2023 02:33:24 GMT
# ARGS: KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Thu, 16 Mar 2023 02:33:25 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 16 Mar 2023 02:33:25 GMT
USER kong
# Thu, 16 Mar 2023 02:33:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 16 Mar 2023 02:33:26 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 16 Mar 2023 02:33:26 GMT
STOPSIGNAL SIGQUIT
# Thu, 16 Mar 2023 02:33:26 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 16 Mar 2023 02:33:26 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:0c68957c744181d1b5cae80a96971c651cec74faeade53191985b92abff361da`  
		Last Modified: Wed, 08 Mar 2023 20:37:17 GMT  
		Size: 27.2 MB (27196161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e58bbdc23e3f7ce51624faf13094ccd5a8b2bc147310d449308170aaea47858`  
		Last Modified: Thu, 16 Mar 2023 02:34:59 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e646675e52dfdb0a044814d6b6639b18f1ca2b8c611012f3505e0d58e12d98da`  
		Last Modified: Thu, 16 Mar 2023 02:35:07 GMT  
		Size: 71.8 MB (71769188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4789db6cc6108aa4834e2b9b21406a3dcba608a8dd70f6868fb008f1882368`  
		Last Modified: Thu, 16 Mar 2023 02:34:59 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.1.1`

```console
$ docker pull kong@sha256:f97a5087ba9331c9ae2e78707df9eed51954f28d83f04358a120e2440ef05eca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.1.1` - linux; amd64

```console
$ docker pull kong@sha256:36258c1d9dd6f5da8cc0403af4650f5d95296e48f83e330ec8f5fd3e3883f162
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75689080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b76469f8b580bfa16be2cce693e879f0c97cf21dab83dca21aa46b9597ed0747`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 13:59:53 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Sat, 11 Feb 2023 13:59:53 GMT
ARG KONG_VERSION=3.1.1
# Sat, 11 Feb 2023 13:59:53 GMT
ENV KONG_VERSION=3.1.1
# Sat, 11 Feb 2023 13:59:53 GMT
ARG KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c
# Sat, 11 Feb 2023 13:59:53 GMT
ARG KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
# Sat, 11 Feb 2023 13:59:53 GMT
ARG ASSET=remote
# Sat, 11 Feb 2023 13:59:53 GMT
ARG EE_PORTS
# Sat, 11 Feb 2023 13:59:53 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Sat, 11 Feb 2023 14:00:01 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Sat, 11 Feb 2023 14:00:01 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Sat, 11 Feb 2023 14:00:01 GMT
USER kong
# Sat, 11 Feb 2023 14:00:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 11 Feb 2023 14:00:01 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 11 Feb 2023 14:00:01 GMT
STOPSIGNAL SIGQUIT
# Sat, 11 Feb 2023 14:00:02 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Sat, 11 Feb 2023 14:00:02 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256d8d79435b0bcc04e2462111b09b5a21093f05b20ff38b484036c091891ff2`  
		Last Modified: Sat, 11 Feb 2023 14:01:47 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8a6c1e7dd831b077e9ed68a8dd90af0a86718c8e0873c8c3dd6f877dc08ded`  
		Last Modified: Sat, 11 Feb 2023 14:01:56 GMT  
		Size: 72.9 MB (72880307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce630ba9f4f76fa8c33b114ce2e01fe176acd00019a99c6e2c8d9f95c2157de`  
		Last Modified: Sat, 11 Feb 2023 14:01:47 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.1.1` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:6cb2e58647fc834e751ed3ff2618757f854e8eea6baa9872b241a5b4922cd2f9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.7 MB (73705071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b194d85727fe1e9c5e8b3df6cfc7434c14b7c9f32b9a179c5b02f56eeced8861`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:57:24 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 10 Feb 2023 22:57:24 GMT
ARG KONG_VERSION=3.1.1
# Fri, 10 Feb 2023 22:57:24 GMT
ENV KONG_VERSION=3.1.1
# Fri, 10 Feb 2023 22:57:24 GMT
ARG KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c
# Fri, 10 Feb 2023 22:57:24 GMT
ARG KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
# Fri, 10 Feb 2023 22:57:24 GMT
ARG ASSET=remote
# Fri, 10 Feb 2023 22:57:25 GMT
ARG EE_PORTS
# Fri, 10 Feb 2023 22:57:25 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Fri, 10 Feb 2023 22:57:31 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Fri, 10 Feb 2023 22:57:32 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 10 Feb 2023 22:57:32 GMT
USER kong
# Fri, 10 Feb 2023 22:57:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 10 Feb 2023 22:57:32 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 10 Feb 2023 22:57:32 GMT
STOPSIGNAL SIGQUIT
# Fri, 10 Feb 2023 22:57:32 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 10 Feb 2023 22:57:32 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7d673d809eb0c188ffdf72da404979eec54eac371b562252cfc579c3d1663f`  
		Last Modified: Fri, 10 Feb 2023 23:01:05 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fc02867f544f9cde11ef414aceb1bdd1235a8da723f6795fe0d358ecd90638`  
		Last Modified: Fri, 10 Feb 2023 23:01:13 GMT  
		Size: 71.0 MB (70994554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ecf15059d665b9ba5f1604f250bc942cb91274a0115c4067ea8cc0887869519`  
		Last Modified: Fri, 10 Feb 2023 23:01:05 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.1.1-alpine`

```console
$ docker pull kong@sha256:f97a5087ba9331c9ae2e78707df9eed51954f28d83f04358a120e2440ef05eca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.1.1-alpine` - linux; amd64

```console
$ docker pull kong@sha256:36258c1d9dd6f5da8cc0403af4650f5d95296e48f83e330ec8f5fd3e3883f162
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75689080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b76469f8b580bfa16be2cce693e879f0c97cf21dab83dca21aa46b9597ed0747`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 13:59:53 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Sat, 11 Feb 2023 13:59:53 GMT
ARG KONG_VERSION=3.1.1
# Sat, 11 Feb 2023 13:59:53 GMT
ENV KONG_VERSION=3.1.1
# Sat, 11 Feb 2023 13:59:53 GMT
ARG KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c
# Sat, 11 Feb 2023 13:59:53 GMT
ARG KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
# Sat, 11 Feb 2023 13:59:53 GMT
ARG ASSET=remote
# Sat, 11 Feb 2023 13:59:53 GMT
ARG EE_PORTS
# Sat, 11 Feb 2023 13:59:53 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Sat, 11 Feb 2023 14:00:01 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Sat, 11 Feb 2023 14:00:01 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Sat, 11 Feb 2023 14:00:01 GMT
USER kong
# Sat, 11 Feb 2023 14:00:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 11 Feb 2023 14:00:01 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 11 Feb 2023 14:00:01 GMT
STOPSIGNAL SIGQUIT
# Sat, 11 Feb 2023 14:00:02 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Sat, 11 Feb 2023 14:00:02 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256d8d79435b0bcc04e2462111b09b5a21093f05b20ff38b484036c091891ff2`  
		Last Modified: Sat, 11 Feb 2023 14:01:47 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8a6c1e7dd831b077e9ed68a8dd90af0a86718c8e0873c8c3dd6f877dc08ded`  
		Last Modified: Sat, 11 Feb 2023 14:01:56 GMT  
		Size: 72.9 MB (72880307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce630ba9f4f76fa8c33b114ce2e01fe176acd00019a99c6e2c8d9f95c2157de`  
		Last Modified: Sat, 11 Feb 2023 14:01:47 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.1.1-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:6cb2e58647fc834e751ed3ff2618757f854e8eea6baa9872b241a5b4922cd2f9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.7 MB (73705071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b194d85727fe1e9c5e8b3df6cfc7434c14b7c9f32b9a179c5b02f56eeced8861`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:57:24 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 10 Feb 2023 22:57:24 GMT
ARG KONG_VERSION=3.1.1
# Fri, 10 Feb 2023 22:57:24 GMT
ENV KONG_VERSION=3.1.1
# Fri, 10 Feb 2023 22:57:24 GMT
ARG KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c
# Fri, 10 Feb 2023 22:57:24 GMT
ARG KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
# Fri, 10 Feb 2023 22:57:24 GMT
ARG ASSET=remote
# Fri, 10 Feb 2023 22:57:25 GMT
ARG EE_PORTS
# Fri, 10 Feb 2023 22:57:25 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Fri, 10 Feb 2023 22:57:31 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Fri, 10 Feb 2023 22:57:32 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Fri, 10 Feb 2023 22:57:32 GMT
USER kong
# Fri, 10 Feb 2023 22:57:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 10 Feb 2023 22:57:32 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 10 Feb 2023 22:57:32 GMT
STOPSIGNAL SIGQUIT
# Fri, 10 Feb 2023 22:57:32 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 10 Feb 2023 22:57:32 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7d673d809eb0c188ffdf72da404979eec54eac371b562252cfc579c3d1663f`  
		Last Modified: Fri, 10 Feb 2023 23:01:05 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fc02867f544f9cde11ef414aceb1bdd1235a8da723f6795fe0d358ecd90638`  
		Last Modified: Fri, 10 Feb 2023 23:01:13 GMT  
		Size: 71.0 MB (70994554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ecf15059d665b9ba5f1604f250bc942cb91274a0115c4067ea8cc0887869519`  
		Last Modified: Fri, 10 Feb 2023 23:01:05 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.1.1-ubuntu`

```console
$ docker pull kong@sha256:975961b67d0fbc8c196a6b5793a6dd37c31bc178ab6203f1c6f904b9607e8e8b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.1.1-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:8ed9bd110f3da4288bdbeea1e304bad5871743e77bb8c64c47a3e61672777ee0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.7 MB (101726780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33890cc7473f3e37ff7fca779b2a0f56eeba8c5dc3fe6f0262e000b3c57eb911`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 08 Mar 2023 04:41:24 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:41:24 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:41:24 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:41:26 GMT
ADD file:20f2ff22b9a8ca9bec5178036c9ebc525a12cd4312daf5d14a9a631a30be20e1 in / 
# Wed, 08 Mar 2023 04:41:27 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 04:52:49 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 16 Mar 2023 04:52:49 GMT
ARG ASSET=ce
# Thu, 16 Mar 2023 04:52:49 GMT
ENV ASSET=ce
# Thu, 16 Mar 2023 04:52:49 GMT
ARG EE_PORTS
# Thu, 16 Mar 2023 04:52:49 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Thu, 16 Mar 2023 04:52:49 GMT
ARG KONG_VERSION=3.1.1
# Thu, 16 Mar 2023 04:52:50 GMT
ENV KONG_VERSION=3.1.1
# Thu, 16 Mar 2023 04:52:50 GMT
ARG KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b
# Thu, 16 Mar 2023 04:52:50 GMT
ARG KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
# Thu, 16 Mar 2023 04:53:44 GMT
# ARGS: KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Thu, 16 Mar 2023 04:53:45 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 16 Mar 2023 04:53:45 GMT
USER kong
# Thu, 16 Mar 2023 04:53:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 16 Mar 2023 04:53:45 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 16 Mar 2023 04:53:45 GMT
STOPSIGNAL SIGQUIT
# Thu, 16 Mar 2023 04:53:45 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 16 Mar 2023 04:53:45 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:5544ebdc0c7b82aa6901eae124b1d220914d2629a9bde25396d7ee9cfd273a8f`  
		Last Modified: Wed, 08 Mar 2023 09:02:58 GMT  
		Size: 28.6 MB (28578068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0310ac76a75b3413c8efa68949fbf815db82ac8624b9d1ca500280c0722969f`  
		Last Modified: Thu, 16 Mar 2023 04:56:02 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a7f03c733975322bd977f20abb1e6abb79a4c3d9b211be3afa32f6e14d522ac`  
		Last Modified: Thu, 16 Mar 2023 04:56:13 GMT  
		Size: 73.1 MB (73147706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31059c935546737773cd25b29801a0113c45428a34a09cc5676aa03f11aeff8f`  
		Last Modified: Thu, 16 Mar 2023 04:56:02 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.1.1-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:9f9955f0bdc78ba76c52a2eba62efede56b47fb645ec01b4356579f5eddfeb51
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.0 MB (98966357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38ae7460b241a3710fe8abe5f21fea1620f771abbed7d26aeaef4b916de33c55`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 08 Mar 2023 04:34:20 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:34:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:34:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 08 Mar 2023 04:34:24 GMT
ADD file:e73d5d005a3ba2c2fb3d8585a1f19daf5ea9ed75af5a2f97b1cc6f7f03db0cdc in / 
# Wed, 08 Mar 2023 04:34:24 GMT
CMD ["/bin/bash"]
# Thu, 16 Mar 2023 02:32:55 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 16 Mar 2023 02:32:55 GMT
ARG ASSET=ce
# Thu, 16 Mar 2023 02:32:55 GMT
ENV ASSET=ce
# Thu, 16 Mar 2023 02:32:55 GMT
ARG EE_PORTS
# Thu, 16 Mar 2023 02:32:56 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Thu, 16 Mar 2023 02:32:56 GMT
ARG KONG_VERSION=3.1.1
# Thu, 16 Mar 2023 02:32:56 GMT
ENV KONG_VERSION=3.1.1
# Thu, 16 Mar 2023 02:32:56 GMT
ARG KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b
# Thu, 16 Mar 2023 02:32:56 GMT
ARG KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
# Thu, 16 Mar 2023 02:33:24 GMT
# ARGS: KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Thu, 16 Mar 2023 02:33:25 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 16 Mar 2023 02:33:25 GMT
USER kong
# Thu, 16 Mar 2023 02:33:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 16 Mar 2023 02:33:26 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 16 Mar 2023 02:33:26 GMT
STOPSIGNAL SIGQUIT
# Thu, 16 Mar 2023 02:33:26 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 16 Mar 2023 02:33:26 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:0c68957c744181d1b5cae80a96971c651cec74faeade53191985b92abff361da`  
		Last Modified: Wed, 08 Mar 2023 20:37:17 GMT  
		Size: 27.2 MB (27196161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e58bbdc23e3f7ce51624faf13094ccd5a8b2bc147310d449308170aaea47858`  
		Last Modified: Thu, 16 Mar 2023 02:34:59 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e646675e52dfdb0a044814d6b6639b18f1ca2b8c611012f3505e0d58e12d98da`  
		Last Modified: Thu, 16 Mar 2023 02:35:07 GMT  
		Size: 71.8 MB (71769188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4789db6cc6108aa4834e2b9b21406a3dcba608a8dd70f6868fb008f1882368`  
		Last Modified: Thu, 16 Mar 2023 02:34:59 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.2`

```console
$ docker pull kong@sha256:79f0393caaec0a4bef96c6735520646061896b8629974ad802921f7e4af61963
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:3.2` - linux; amd64

```console
$ docker pull kong@sha256:e39b654c5c2fbfbfe528613dac50164fbd389a0aba712033d28c8b0e9bfc3280
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.9 MB (36926241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a67d04eb7448a9987ba1a35e28ba76e396acf9a2bdefeb7d65d28337bff1dea`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Sat, 25 Mar 2023 00:51:01 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Sat, 25 Mar 2023 00:51:01 GMT
ARG KONG_VERSION=3.2.2
# Sat, 25 Mar 2023 00:51:01 GMT
ENV KONG_VERSION=3.2.2
# Sat, 25 Mar 2023 00:51:01 GMT
ARG KONG_SHA256=a07c3bc0307e2d8fe33acb8be5fe659f348279540eaa267bc6968005094835ef
# Sat, 25 Mar 2023 00:51:01 GMT
ARG KONG_PREFIX=/usr/local/kong
# Sat, 25 Mar 2023 00:51:01 GMT
ENV KONG_PREFIX=/usr/local/kong
# Sat, 25 Mar 2023 00:51:01 GMT
ARG ASSET=remote
# Sat, 25 Mar 2023 00:51:01 GMT
ARG EE_PORTS
# Sat, 25 Mar 2023 00:51:01 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Sat, 25 Mar 2023 00:51:07 GMT
# ARGS: ASSET=remote KONG_SHA256=a07c3bc0307e2d8fe33acb8be5fe659f348279540eaa267bc6968005094835ef
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     export ARCH='amd64';     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc perl tzdata libcap zlib zlib-dev bash yaml     && adduser -S kong     && addgroup -S kong     && mkdir -p "${KONG_PREFIX}"     && chown -R kong:0 ${KONG_PREFIX}     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u ${KONG_PREFIX}     && rm -rf /tmp/kong.apk.tar.gz     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Sat, 25 Mar 2023 00:51:08 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Sat, 25 Mar 2023 00:51:08 GMT
USER kong
# Sat, 25 Mar 2023 00:51:08 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Mar 2023 00:51:08 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 25 Mar 2023 00:51:08 GMT
STOPSIGNAL SIGQUIT
# Sat, 25 Mar 2023 00:51:08 GMT
HEALTHCHECK &{["CMD-SHELL" "kong-health"] "1m0s" "10s" "0s" '\n'}
# Sat, 25 Mar 2023 00:51:08 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a260cdfa2fbd0e7eb62bccc7f6deabe23c93bb0456c841a72399e8b4d5eb4c6e`  
		Last Modified: Sat, 25 Mar 2023 00:52:31 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fa46152c72850607722b515840cf2b8eb72a29d712037b0df457beee533d4b`  
		Last Modified: Sat, 25 Mar 2023 00:52:36 GMT  
		Size: 33.6 MB (33550506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5682cda435615908fe6b508dcc0f128eb35ba3776880f51f7da735e58141379d`  
		Last Modified: Sat, 25 Mar 2023 00:52:31 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.2-ubuntu`

```console
$ docker pull kong@sha256:86f9b1e316dcddeb30dc045cedd239d8573bff4d8acbf231f7d11902c1a83adf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.2-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:f5f51af49fa1f5a7600e60bb51ebd760b16fd020bb16bba2b70d36a54f3d6ac8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.4 MB (74381601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b5a4a92323976685af4f320261472e8c4575583169192c82d27e246681fc216`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 08 Mar 2023 04:44:25 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:44:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:44:27 GMT
ADD file:c8ef6447752cab2541ffca9e3cfa27d581f3491bc8f356f6eafd951243609341 in / 
# Wed, 08 Mar 2023 04:44:27 GMT
CMD ["/bin/bash"]
# Sat, 25 Mar 2023 00:51:10 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Sat, 25 Mar 2023 00:51:10 GMT
ARG ASSET=ce
# Sat, 25 Mar 2023 00:51:10 GMT
ENV ASSET=ce
# Sat, 25 Mar 2023 00:51:10 GMT
ARG EE_PORTS
# Sat, 25 Mar 2023 00:51:11 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Sat, 25 Mar 2023 00:51:11 GMT
ARG KONG_VERSION=3.2.2
# Sat, 25 Mar 2023 00:51:11 GMT
ENV KONG_VERSION=3.2.2
# Sat, 25 Mar 2023 00:51:11 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Sat, 25 Mar 2023 00:51:11 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Sat, 25 Mar 2023 00:52:03 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Sat, 25 Mar 2023 00:52:04 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Sat, 25 Mar 2023 00:52:04 GMT
USER kong
# Sat, 25 Mar 2023 00:52:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Mar 2023 00:52:04 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 25 Mar 2023 00:52:04 GMT
STOPSIGNAL SIGQUIT
# Sat, 25 Mar 2023 00:52:04 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Sat, 25 Mar 2023 00:52:04 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:74ac377868f863e123f24c409f79709f7563fa464557c36a09cf6f85c8b92b7f`  
		Last Modified: Wed, 08 Mar 2023 09:03:15 GMT  
		Size: 30.4 MB (30429963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a798f30a08e58465197ea53af5348cb1920b409dce739c8c1191fa526b779c26`  
		Last Modified: Sat, 25 Mar 2023 00:52:51 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:192c4afa29b67585a708114ac6e302a8de969f95b6037af093514f0b41e1a873`  
		Last Modified: Sat, 25 Mar 2023 00:52:58 GMT  
		Size: 44.0 MB (43950354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8497c811ba9ee1b3aa10434828370b73152317680fd95a5b7718672c3cfb2b2c`  
		Last Modified: Sat, 25 Mar 2023 00:52:51 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.2-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:4d0e6518979970d7795ebfd3996daa3f6f2414ed7a2282ba15c35ac299dc4f50
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.5 MB (78466508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad2ac3aea873b6b79878a75119e8b9481f7bb257b98bccb497854f6567a738bc`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
# Fri, 24 Mar 2023 23:39:31 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 24 Mar 2023 23:39:31 GMT
ARG ASSET=ce
# Fri, 24 Mar 2023 23:39:31 GMT
ENV ASSET=ce
# Fri, 24 Mar 2023 23:39:31 GMT
ARG EE_PORTS
# Fri, 24 Mar 2023 23:39:31 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 24 Mar 2023 23:39:32 GMT
ARG KONG_VERSION=3.2.2
# Fri, 24 Mar 2023 23:39:32 GMT
ENV KONG_VERSION=3.2.2
# Fri, 24 Mar 2023 23:39:32 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Fri, 24 Mar 2023 23:39:32 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Fri, 24 Mar 2023 23:40:38 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 24 Mar 2023 23:40:38 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 24 Mar 2023 23:40:39 GMT
USER kong
# Fri, 24 Mar 2023 23:40:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Mar 2023 23:40:39 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 24 Mar 2023 23:40:39 GMT
STOPSIGNAL SIGQUIT
# Fri, 24 Mar 2023 23:40:39 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 24 Mar 2023 23:40:39 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:b2ddfd337773edbf5766dce2fdbeef139ba8c42724e29eda157c84e9f97f1bce`  
		Last Modified: Wed, 08 Mar 2023 12:37:24 GMT  
		Size: 28.4 MB (28387554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc7b355e64c2bd4ae186d762e75dcf38abb3a3a38feca3d07c5de89f24c54b6`  
		Last Modified: Fri, 24 Mar 2023 23:41:11 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15cca0f56b895a7954dcff8ef25eac39c8aaa299cee84f520714508573ee2cee`  
		Last Modified: Fri, 24 Mar 2023 23:41:17 GMT  
		Size: 50.1 MB (50077673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09190020715369973a3868d7c33a1e59d33c39a77be8a68ed47d9a875256f22`  
		Last Modified: Fri, 24 Mar 2023 23:41:11 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.2.2`

```console
$ docker pull kong@sha256:79f0393caaec0a4bef96c6735520646061896b8629974ad802921f7e4af61963
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:3.2.2` - linux; amd64

```console
$ docker pull kong@sha256:e39b654c5c2fbfbfe528613dac50164fbd389a0aba712033d28c8b0e9bfc3280
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.9 MB (36926241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a67d04eb7448a9987ba1a35e28ba76e396acf9a2bdefeb7d65d28337bff1dea`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Sat, 25 Mar 2023 00:51:01 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Sat, 25 Mar 2023 00:51:01 GMT
ARG KONG_VERSION=3.2.2
# Sat, 25 Mar 2023 00:51:01 GMT
ENV KONG_VERSION=3.2.2
# Sat, 25 Mar 2023 00:51:01 GMT
ARG KONG_SHA256=a07c3bc0307e2d8fe33acb8be5fe659f348279540eaa267bc6968005094835ef
# Sat, 25 Mar 2023 00:51:01 GMT
ARG KONG_PREFIX=/usr/local/kong
# Sat, 25 Mar 2023 00:51:01 GMT
ENV KONG_PREFIX=/usr/local/kong
# Sat, 25 Mar 2023 00:51:01 GMT
ARG ASSET=remote
# Sat, 25 Mar 2023 00:51:01 GMT
ARG EE_PORTS
# Sat, 25 Mar 2023 00:51:01 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Sat, 25 Mar 2023 00:51:07 GMT
# ARGS: ASSET=remote KONG_SHA256=a07c3bc0307e2d8fe33acb8be5fe659f348279540eaa267bc6968005094835ef
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     export ARCH='amd64';     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc perl tzdata libcap zlib zlib-dev bash yaml     && adduser -S kong     && addgroup -S kong     && mkdir -p "${KONG_PREFIX}"     && chown -R kong:0 ${KONG_PREFIX}     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u ${KONG_PREFIX}     && rm -rf /tmp/kong.apk.tar.gz     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Sat, 25 Mar 2023 00:51:08 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Sat, 25 Mar 2023 00:51:08 GMT
USER kong
# Sat, 25 Mar 2023 00:51:08 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Mar 2023 00:51:08 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 25 Mar 2023 00:51:08 GMT
STOPSIGNAL SIGQUIT
# Sat, 25 Mar 2023 00:51:08 GMT
HEALTHCHECK &{["CMD-SHELL" "kong-health"] "1m0s" "10s" "0s" '\n'}
# Sat, 25 Mar 2023 00:51:08 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a260cdfa2fbd0e7eb62bccc7f6deabe23c93bb0456c841a72399e8b4d5eb4c6e`  
		Last Modified: Sat, 25 Mar 2023 00:52:31 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fa46152c72850607722b515840cf2b8eb72a29d712037b0df457beee533d4b`  
		Last Modified: Sat, 25 Mar 2023 00:52:36 GMT  
		Size: 33.6 MB (33550506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5682cda435615908fe6b508dcc0f128eb35ba3776880f51f7da735e58141379d`  
		Last Modified: Sat, 25 Mar 2023 00:52:31 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.2.2-alpine`

```console
$ docker pull kong@sha256:79f0393caaec0a4bef96c6735520646061896b8629974ad802921f7e4af61963
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:3.2.2-alpine` - linux; amd64

```console
$ docker pull kong@sha256:e39b654c5c2fbfbfe528613dac50164fbd389a0aba712033d28c8b0e9bfc3280
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.9 MB (36926241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a67d04eb7448a9987ba1a35e28ba76e396acf9a2bdefeb7d65d28337bff1dea`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Sat, 25 Mar 2023 00:51:01 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Sat, 25 Mar 2023 00:51:01 GMT
ARG KONG_VERSION=3.2.2
# Sat, 25 Mar 2023 00:51:01 GMT
ENV KONG_VERSION=3.2.2
# Sat, 25 Mar 2023 00:51:01 GMT
ARG KONG_SHA256=a07c3bc0307e2d8fe33acb8be5fe659f348279540eaa267bc6968005094835ef
# Sat, 25 Mar 2023 00:51:01 GMT
ARG KONG_PREFIX=/usr/local/kong
# Sat, 25 Mar 2023 00:51:01 GMT
ENV KONG_PREFIX=/usr/local/kong
# Sat, 25 Mar 2023 00:51:01 GMT
ARG ASSET=remote
# Sat, 25 Mar 2023 00:51:01 GMT
ARG EE_PORTS
# Sat, 25 Mar 2023 00:51:01 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Sat, 25 Mar 2023 00:51:07 GMT
# ARGS: ASSET=remote KONG_SHA256=a07c3bc0307e2d8fe33acb8be5fe659f348279540eaa267bc6968005094835ef
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     export ARCH='amd64';     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc perl tzdata libcap zlib zlib-dev bash yaml     && adduser -S kong     && addgroup -S kong     && mkdir -p "${KONG_PREFIX}"     && chown -R kong:0 ${KONG_PREFIX}     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u ${KONG_PREFIX}     && rm -rf /tmp/kong.apk.tar.gz     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Sat, 25 Mar 2023 00:51:08 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Sat, 25 Mar 2023 00:51:08 GMT
USER kong
# Sat, 25 Mar 2023 00:51:08 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Mar 2023 00:51:08 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 25 Mar 2023 00:51:08 GMT
STOPSIGNAL SIGQUIT
# Sat, 25 Mar 2023 00:51:08 GMT
HEALTHCHECK &{["CMD-SHELL" "kong-health"] "1m0s" "10s" "0s" '\n'}
# Sat, 25 Mar 2023 00:51:08 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a260cdfa2fbd0e7eb62bccc7f6deabe23c93bb0456c841a72399e8b4d5eb4c6e`  
		Last Modified: Sat, 25 Mar 2023 00:52:31 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fa46152c72850607722b515840cf2b8eb72a29d712037b0df457beee533d4b`  
		Last Modified: Sat, 25 Mar 2023 00:52:36 GMT  
		Size: 33.6 MB (33550506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5682cda435615908fe6b508dcc0f128eb35ba3776880f51f7da735e58141379d`  
		Last Modified: Sat, 25 Mar 2023 00:52:31 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.2.2-ubuntu`

```console
$ docker pull kong@sha256:86f9b1e316dcddeb30dc045cedd239d8573bff4d8acbf231f7d11902c1a83adf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.2.2-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:f5f51af49fa1f5a7600e60bb51ebd760b16fd020bb16bba2b70d36a54f3d6ac8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.4 MB (74381601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b5a4a92323976685af4f320261472e8c4575583169192c82d27e246681fc216`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 08 Mar 2023 04:44:25 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:44:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:44:27 GMT
ADD file:c8ef6447752cab2541ffca9e3cfa27d581f3491bc8f356f6eafd951243609341 in / 
# Wed, 08 Mar 2023 04:44:27 GMT
CMD ["/bin/bash"]
# Sat, 25 Mar 2023 00:51:10 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Sat, 25 Mar 2023 00:51:10 GMT
ARG ASSET=ce
# Sat, 25 Mar 2023 00:51:10 GMT
ENV ASSET=ce
# Sat, 25 Mar 2023 00:51:10 GMT
ARG EE_PORTS
# Sat, 25 Mar 2023 00:51:11 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Sat, 25 Mar 2023 00:51:11 GMT
ARG KONG_VERSION=3.2.2
# Sat, 25 Mar 2023 00:51:11 GMT
ENV KONG_VERSION=3.2.2
# Sat, 25 Mar 2023 00:51:11 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Sat, 25 Mar 2023 00:51:11 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Sat, 25 Mar 2023 00:52:03 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Sat, 25 Mar 2023 00:52:04 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Sat, 25 Mar 2023 00:52:04 GMT
USER kong
# Sat, 25 Mar 2023 00:52:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Mar 2023 00:52:04 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 25 Mar 2023 00:52:04 GMT
STOPSIGNAL SIGQUIT
# Sat, 25 Mar 2023 00:52:04 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Sat, 25 Mar 2023 00:52:04 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:74ac377868f863e123f24c409f79709f7563fa464557c36a09cf6f85c8b92b7f`  
		Last Modified: Wed, 08 Mar 2023 09:03:15 GMT  
		Size: 30.4 MB (30429963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a798f30a08e58465197ea53af5348cb1920b409dce739c8c1191fa526b779c26`  
		Last Modified: Sat, 25 Mar 2023 00:52:51 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:192c4afa29b67585a708114ac6e302a8de969f95b6037af093514f0b41e1a873`  
		Last Modified: Sat, 25 Mar 2023 00:52:58 GMT  
		Size: 44.0 MB (43950354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8497c811ba9ee1b3aa10434828370b73152317680fd95a5b7718672c3cfb2b2c`  
		Last Modified: Sat, 25 Mar 2023 00:52:51 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.2.2-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:4d0e6518979970d7795ebfd3996daa3f6f2414ed7a2282ba15c35ac299dc4f50
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.5 MB (78466508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad2ac3aea873b6b79878a75119e8b9481f7bb257b98bccb497854f6567a738bc`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
# Fri, 24 Mar 2023 23:39:31 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 24 Mar 2023 23:39:31 GMT
ARG ASSET=ce
# Fri, 24 Mar 2023 23:39:31 GMT
ENV ASSET=ce
# Fri, 24 Mar 2023 23:39:31 GMT
ARG EE_PORTS
# Fri, 24 Mar 2023 23:39:31 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 24 Mar 2023 23:39:32 GMT
ARG KONG_VERSION=3.2.2
# Fri, 24 Mar 2023 23:39:32 GMT
ENV KONG_VERSION=3.2.2
# Fri, 24 Mar 2023 23:39:32 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Fri, 24 Mar 2023 23:39:32 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Fri, 24 Mar 2023 23:40:38 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 24 Mar 2023 23:40:38 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 24 Mar 2023 23:40:39 GMT
USER kong
# Fri, 24 Mar 2023 23:40:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Mar 2023 23:40:39 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 24 Mar 2023 23:40:39 GMT
STOPSIGNAL SIGQUIT
# Fri, 24 Mar 2023 23:40:39 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 24 Mar 2023 23:40:39 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:b2ddfd337773edbf5766dce2fdbeef139ba8c42724e29eda157c84e9f97f1bce`  
		Last Modified: Wed, 08 Mar 2023 12:37:24 GMT  
		Size: 28.4 MB (28387554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc7b355e64c2bd4ae186d762e75dcf38abb3a3a38feca3d07c5de89f24c54b6`  
		Last Modified: Fri, 24 Mar 2023 23:41:11 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15cca0f56b895a7954dcff8ef25eac39c8aaa299cee84f520714508573ee2cee`  
		Last Modified: Fri, 24 Mar 2023 23:41:17 GMT  
		Size: 50.1 MB (50077673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09190020715369973a3868d7c33a1e59d33c39a77be8a68ed47d9a875256f22`  
		Last Modified: Fri, 24 Mar 2023 23:41:11 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:alpine`

```console
$ docker pull kong@sha256:79f0393caaec0a4bef96c6735520646061896b8629974ad802921f7e4af61963
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:alpine` - linux; amd64

```console
$ docker pull kong@sha256:e39b654c5c2fbfbfe528613dac50164fbd389a0aba712033d28c8b0e9bfc3280
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.9 MB (36926241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a67d04eb7448a9987ba1a35e28ba76e396acf9a2bdefeb7d65d28337bff1dea`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Sat, 25 Mar 2023 00:51:01 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Sat, 25 Mar 2023 00:51:01 GMT
ARG KONG_VERSION=3.2.2
# Sat, 25 Mar 2023 00:51:01 GMT
ENV KONG_VERSION=3.2.2
# Sat, 25 Mar 2023 00:51:01 GMT
ARG KONG_SHA256=a07c3bc0307e2d8fe33acb8be5fe659f348279540eaa267bc6968005094835ef
# Sat, 25 Mar 2023 00:51:01 GMT
ARG KONG_PREFIX=/usr/local/kong
# Sat, 25 Mar 2023 00:51:01 GMT
ENV KONG_PREFIX=/usr/local/kong
# Sat, 25 Mar 2023 00:51:01 GMT
ARG ASSET=remote
# Sat, 25 Mar 2023 00:51:01 GMT
ARG EE_PORTS
# Sat, 25 Mar 2023 00:51:01 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Sat, 25 Mar 2023 00:51:07 GMT
# ARGS: ASSET=remote KONG_SHA256=a07c3bc0307e2d8fe33acb8be5fe659f348279540eaa267bc6968005094835ef
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     export ARCH='amd64';     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc perl tzdata libcap zlib zlib-dev bash yaml     && adduser -S kong     && addgroup -S kong     && mkdir -p "${KONG_PREFIX}"     && chown -R kong:0 ${KONG_PREFIX}     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u ${KONG_PREFIX}     && rm -rf /tmp/kong.apk.tar.gz     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Sat, 25 Mar 2023 00:51:08 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Sat, 25 Mar 2023 00:51:08 GMT
USER kong
# Sat, 25 Mar 2023 00:51:08 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Mar 2023 00:51:08 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 25 Mar 2023 00:51:08 GMT
STOPSIGNAL SIGQUIT
# Sat, 25 Mar 2023 00:51:08 GMT
HEALTHCHECK &{["CMD-SHELL" "kong-health"] "1m0s" "10s" "0s" '\n'}
# Sat, 25 Mar 2023 00:51:08 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a260cdfa2fbd0e7eb62bccc7f6deabe23c93bb0456c841a72399e8b4d5eb4c6e`  
		Last Modified: Sat, 25 Mar 2023 00:52:31 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fa46152c72850607722b515840cf2b8eb72a29d712037b0df457beee533d4b`  
		Last Modified: Sat, 25 Mar 2023 00:52:36 GMT  
		Size: 33.6 MB (33550506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5682cda435615908fe6b508dcc0f128eb35ba3776880f51f7da735e58141379d`  
		Last Modified: Sat, 25 Mar 2023 00:52:31 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:latest`

```console
$ docker pull kong@sha256:79f0393caaec0a4bef96c6735520646061896b8629974ad802921f7e4af61963
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:latest` - linux; amd64

```console
$ docker pull kong@sha256:e39b654c5c2fbfbfe528613dac50164fbd389a0aba712033d28c8b0e9bfc3280
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.9 MB (36926241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a67d04eb7448a9987ba1a35e28ba76e396acf9a2bdefeb7d65d28337bff1dea`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Sat, 25 Mar 2023 00:51:01 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Sat, 25 Mar 2023 00:51:01 GMT
ARG KONG_VERSION=3.2.2
# Sat, 25 Mar 2023 00:51:01 GMT
ENV KONG_VERSION=3.2.2
# Sat, 25 Mar 2023 00:51:01 GMT
ARG KONG_SHA256=a07c3bc0307e2d8fe33acb8be5fe659f348279540eaa267bc6968005094835ef
# Sat, 25 Mar 2023 00:51:01 GMT
ARG KONG_PREFIX=/usr/local/kong
# Sat, 25 Mar 2023 00:51:01 GMT
ENV KONG_PREFIX=/usr/local/kong
# Sat, 25 Mar 2023 00:51:01 GMT
ARG ASSET=remote
# Sat, 25 Mar 2023 00:51:01 GMT
ARG EE_PORTS
# Sat, 25 Mar 2023 00:51:01 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Sat, 25 Mar 2023 00:51:07 GMT
# ARGS: ASSET=remote KONG_SHA256=a07c3bc0307e2d8fe33acb8be5fe659f348279540eaa267bc6968005094835ef
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     export ARCH='amd64';     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc perl tzdata libcap zlib zlib-dev bash yaml     && adduser -S kong     && addgroup -S kong     && mkdir -p "${KONG_PREFIX}"     && chown -R kong:0 ${KONG_PREFIX}     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u ${KONG_PREFIX}     && rm -rf /tmp/kong.apk.tar.gz     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Sat, 25 Mar 2023 00:51:08 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Sat, 25 Mar 2023 00:51:08 GMT
USER kong
# Sat, 25 Mar 2023 00:51:08 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Mar 2023 00:51:08 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 25 Mar 2023 00:51:08 GMT
STOPSIGNAL SIGQUIT
# Sat, 25 Mar 2023 00:51:08 GMT
HEALTHCHECK &{["CMD-SHELL" "kong-health"] "1m0s" "10s" "0s" '\n'}
# Sat, 25 Mar 2023 00:51:08 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a260cdfa2fbd0e7eb62bccc7f6deabe23c93bb0456c841a72399e8b4d5eb4c6e`  
		Last Modified: Sat, 25 Mar 2023 00:52:31 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fa46152c72850607722b515840cf2b8eb72a29d712037b0df457beee533d4b`  
		Last Modified: Sat, 25 Mar 2023 00:52:36 GMT  
		Size: 33.6 MB (33550506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5682cda435615908fe6b508dcc0f128eb35ba3776880f51f7da735e58141379d`  
		Last Modified: Sat, 25 Mar 2023 00:52:31 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:ubuntu`

```console
$ docker pull kong@sha256:86f9b1e316dcddeb30dc045cedd239d8573bff4d8acbf231f7d11902c1a83adf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:f5f51af49fa1f5a7600e60bb51ebd760b16fd020bb16bba2b70d36a54f3d6ac8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.4 MB (74381601 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b5a4a92323976685af4f320261472e8c4575583169192c82d27e246681fc216`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 08 Mar 2023 04:44:25 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:44:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:44:25 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:44:27 GMT
ADD file:c8ef6447752cab2541ffca9e3cfa27d581f3491bc8f356f6eafd951243609341 in / 
# Wed, 08 Mar 2023 04:44:27 GMT
CMD ["/bin/bash"]
# Sat, 25 Mar 2023 00:51:10 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Sat, 25 Mar 2023 00:51:10 GMT
ARG ASSET=ce
# Sat, 25 Mar 2023 00:51:10 GMT
ENV ASSET=ce
# Sat, 25 Mar 2023 00:51:10 GMT
ARG EE_PORTS
# Sat, 25 Mar 2023 00:51:11 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Sat, 25 Mar 2023 00:51:11 GMT
ARG KONG_VERSION=3.2.2
# Sat, 25 Mar 2023 00:51:11 GMT
ENV KONG_VERSION=3.2.2
# Sat, 25 Mar 2023 00:51:11 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Sat, 25 Mar 2023 00:51:11 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Sat, 25 Mar 2023 00:52:03 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Sat, 25 Mar 2023 00:52:04 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Sat, 25 Mar 2023 00:52:04 GMT
USER kong
# Sat, 25 Mar 2023 00:52:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Mar 2023 00:52:04 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 25 Mar 2023 00:52:04 GMT
STOPSIGNAL SIGQUIT
# Sat, 25 Mar 2023 00:52:04 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Sat, 25 Mar 2023 00:52:04 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:74ac377868f863e123f24c409f79709f7563fa464557c36a09cf6f85c8b92b7f`  
		Last Modified: Wed, 08 Mar 2023 09:03:15 GMT  
		Size: 30.4 MB (30429963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a798f30a08e58465197ea53af5348cb1920b409dce739c8c1191fa526b779c26`  
		Last Modified: Sat, 25 Mar 2023 00:52:51 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:192c4afa29b67585a708114ac6e302a8de969f95b6037af093514f0b41e1a873`  
		Last Modified: Sat, 25 Mar 2023 00:52:58 GMT  
		Size: 44.0 MB (43950354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8497c811ba9ee1b3aa10434828370b73152317680fd95a5b7718672c3cfb2b2c`  
		Last Modified: Sat, 25 Mar 2023 00:52:51 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:4d0e6518979970d7795ebfd3996daa3f6f2414ed7a2282ba15c35ac299dc4f50
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.5 MB (78466508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad2ac3aea873b6b79878a75119e8b9481f7bb257b98bccb497854f6567a738bc`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 08 Mar 2023 04:32:38 GMT
ARG RELEASE
# Wed, 08 Mar 2023 04:32:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 08 Mar 2023 04:32:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 08 Mar 2023 04:32:39 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 08 Mar 2023 04:32:40 GMT
ADD file:79b36308bc382d9cae7197b4cecc21430f4e8f3e8bec3547d0f00bcff7681e60 in / 
# Wed, 08 Mar 2023 04:32:41 GMT
CMD ["/bin/bash"]
# Fri, 24 Mar 2023 23:39:31 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Fri, 24 Mar 2023 23:39:31 GMT
ARG ASSET=ce
# Fri, 24 Mar 2023 23:39:31 GMT
ENV ASSET=ce
# Fri, 24 Mar 2023 23:39:31 GMT
ARG EE_PORTS
# Fri, 24 Mar 2023 23:39:31 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Fri, 24 Mar 2023 23:39:32 GMT
ARG KONG_VERSION=3.2.2
# Fri, 24 Mar 2023 23:39:32 GMT
ENV KONG_VERSION=3.2.2
# Fri, 24 Mar 2023 23:39:32 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Fri, 24 Mar 2023 23:39:32 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Fri, 24 Mar 2023 23:40:38 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Fri, 24 Mar 2023 23:40:38 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Fri, 24 Mar 2023 23:40:39 GMT
USER kong
# Fri, 24 Mar 2023 23:40:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 24 Mar 2023 23:40:39 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 24 Mar 2023 23:40:39 GMT
STOPSIGNAL SIGQUIT
# Fri, 24 Mar 2023 23:40:39 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Fri, 24 Mar 2023 23:40:39 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:b2ddfd337773edbf5766dce2fdbeef139ba8c42724e29eda157c84e9f97f1bce`  
		Last Modified: Wed, 08 Mar 2023 12:37:24 GMT  
		Size: 28.4 MB (28387554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc7b355e64c2bd4ae186d762e75dcf38abb3a3a38feca3d07c5de89f24c54b6`  
		Last Modified: Fri, 24 Mar 2023 23:41:11 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15cca0f56b895a7954dcff8ef25eac39c8aaa299cee84f520714508573ee2cee`  
		Last Modified: Fri, 24 Mar 2023 23:41:17 GMT  
		Size: 50.1 MB (50077673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09190020715369973a3868d7c33a1e59d33c39a77be8a68ed47d9a875256f22`  
		Last Modified: Fri, 24 Mar 2023 23:41:11 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
