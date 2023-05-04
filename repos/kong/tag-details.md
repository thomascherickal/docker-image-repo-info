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
$ docker pull kong@sha256:83b7264156246a942c1bc1c95d9409603d9fc71f578d13731bc77824388f0e21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.8` - linux; amd64

```console
$ docker pull kong@sha256:b767f991a30f9cac433865b63e465ccd0e485c104329391815372789b475f7a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49336669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f08d55de6605e1ff87d4bb5bf3bee1589e87b5390041fdeff55c501a60dbc5db`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:11:26 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 29 Mar 2023 22:11:26 GMT
ARG ASSET=ce
# Wed, 29 Mar 2023 22:11:26 GMT
ENV ASSET=ce
# Wed, 29 Mar 2023 22:11:26 GMT
ARG EE_PORTS
# Wed, 29 Mar 2023 22:11:26 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 29 Mar 2023 22:11:26 GMT
ARG KONG_VERSION=2.8.3
# Wed, 29 Mar 2023 22:11:27 GMT
ENV KONG_VERSION=2.8.3
# Wed, 29 Mar 2023 22:11:27 GMT
ARG KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa
# Wed, 29 Mar 2023 22:11:27 GMT
ARG KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
# Wed, 29 Mar 2023 22:11:33 GMT
# ARGS: KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Wed, 29 Mar 2023 22:11:33 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 29 Mar 2023 22:11:34 GMT
USER kong
# Wed, 29 Mar 2023 22:11:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 29 Mar 2023 22:11:34 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 29 Mar 2023 22:11:34 GMT
STOPSIGNAL SIGQUIT
# Wed, 29 Mar 2023 22:11:34 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 29 Mar 2023 22:11:34 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:91d30c5bc19582de1415b18f1ec5bcbf52a558b62cf6cc201c9669df9f748c22`  
		Last Modified: Wed, 29 Mar 2023 18:20:09 GMT  
		Size: 2.8 MB (2807803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c6c1798758d52be09614fa8ec90799ee184e137bc78da7792dcfd727d51c26`  
		Last Modified: Wed, 29 Mar 2023 22:12:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd40f0f27d03b3579307957241a10fe96137a75555eb4ceb5f0436ebcc48a735`  
		Last Modified: Wed, 29 Mar 2023 22:12:49 GMT  
		Size: 46.5 MB (46527857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae3de81c97825904984d09363568c9ac780869f6bc3fa71a512a06ba5de98505`  
		Last Modified: Wed, 29 Mar 2023 22:12:42 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.8` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:ef1492e3d92dcf03c868b4266628c35bda33c3d78710121d3e7606c1fab1e669
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.5 MB (48521091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4bb5629cc85df77176510a0979e93e6392d0add4bf05deafc3ae5f7ef8e188c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:15:52 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 30 Mar 2023 04:15:53 GMT
ARG ASSET=ce
# Thu, 30 Mar 2023 04:15:53 GMT
ENV ASSET=ce
# Thu, 30 Mar 2023 04:15:53 GMT
ARG EE_PORTS
# Thu, 30 Mar 2023 04:15:53 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 30 Mar 2023 04:15:53 GMT
ARG KONG_VERSION=2.8.3
# Thu, 30 Mar 2023 04:15:53 GMT
ENV KONG_VERSION=2.8.3
# Thu, 30 Mar 2023 04:15:53 GMT
ARG KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa
# Thu, 30 Mar 2023 04:15:53 GMT
ARG KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
# Thu, 30 Mar 2023 04:15:59 GMT
# ARGS: KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 30 Mar 2023 04:16:00 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 30 Mar 2023 04:16:00 GMT
USER kong
# Thu, 30 Mar 2023 04:16:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Mar 2023 04:16:00 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 30 Mar 2023 04:16:00 GMT
STOPSIGNAL SIGQUIT
# Thu, 30 Mar 2023 04:16:00 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 30 Mar 2023 04:16:00 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:547446be3368f442c50ff95e2a2a9c85110b6b41bbb3c75b7e5ebb115f478b57`  
		Last Modified: Wed, 29 Mar 2023 17:39:56 GMT  
		Size: 2.7 MB (2709344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ff78970d3279285a92299fc4aca99872e9f7ad31a1dff143611df7b0b93a8c`  
		Last Modified: Thu, 30 Mar 2023 04:16:52 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b48e0173e1b427e16c7dbce6bc355cf2c26e68a51a444cb1782ae95506a7a893`  
		Last Modified: Thu, 30 Mar 2023 04:16:59 GMT  
		Size: 45.8 MB (45810736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb0a1ba1287b8da1a4810968cf7f49bad92b1340c00d942cae076865bb1737e1`  
		Last Modified: Thu, 30 Mar 2023 04:16:52 GMT  
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
$ docker pull kong@sha256:83b7264156246a942c1bc1c95d9409603d9fc71f578d13731bc77824388f0e21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.8.3` - linux; amd64

```console
$ docker pull kong@sha256:b767f991a30f9cac433865b63e465ccd0e485c104329391815372789b475f7a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49336669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f08d55de6605e1ff87d4bb5bf3bee1589e87b5390041fdeff55c501a60dbc5db`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:11:26 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 29 Mar 2023 22:11:26 GMT
ARG ASSET=ce
# Wed, 29 Mar 2023 22:11:26 GMT
ENV ASSET=ce
# Wed, 29 Mar 2023 22:11:26 GMT
ARG EE_PORTS
# Wed, 29 Mar 2023 22:11:26 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 29 Mar 2023 22:11:26 GMT
ARG KONG_VERSION=2.8.3
# Wed, 29 Mar 2023 22:11:27 GMT
ENV KONG_VERSION=2.8.3
# Wed, 29 Mar 2023 22:11:27 GMT
ARG KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa
# Wed, 29 Mar 2023 22:11:27 GMT
ARG KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
# Wed, 29 Mar 2023 22:11:33 GMT
# ARGS: KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Wed, 29 Mar 2023 22:11:33 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 29 Mar 2023 22:11:34 GMT
USER kong
# Wed, 29 Mar 2023 22:11:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 29 Mar 2023 22:11:34 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 29 Mar 2023 22:11:34 GMT
STOPSIGNAL SIGQUIT
# Wed, 29 Mar 2023 22:11:34 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 29 Mar 2023 22:11:34 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:91d30c5bc19582de1415b18f1ec5bcbf52a558b62cf6cc201c9669df9f748c22`  
		Last Modified: Wed, 29 Mar 2023 18:20:09 GMT  
		Size: 2.8 MB (2807803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c6c1798758d52be09614fa8ec90799ee184e137bc78da7792dcfd727d51c26`  
		Last Modified: Wed, 29 Mar 2023 22:12:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd40f0f27d03b3579307957241a10fe96137a75555eb4ceb5f0436ebcc48a735`  
		Last Modified: Wed, 29 Mar 2023 22:12:49 GMT  
		Size: 46.5 MB (46527857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae3de81c97825904984d09363568c9ac780869f6bc3fa71a512a06ba5de98505`  
		Last Modified: Wed, 29 Mar 2023 22:12:42 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.8.3` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:ef1492e3d92dcf03c868b4266628c35bda33c3d78710121d3e7606c1fab1e669
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.5 MB (48521091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4bb5629cc85df77176510a0979e93e6392d0add4bf05deafc3ae5f7ef8e188c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:15:52 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 30 Mar 2023 04:15:53 GMT
ARG ASSET=ce
# Thu, 30 Mar 2023 04:15:53 GMT
ENV ASSET=ce
# Thu, 30 Mar 2023 04:15:53 GMT
ARG EE_PORTS
# Thu, 30 Mar 2023 04:15:53 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 30 Mar 2023 04:15:53 GMT
ARG KONG_VERSION=2.8.3
# Thu, 30 Mar 2023 04:15:53 GMT
ENV KONG_VERSION=2.8.3
# Thu, 30 Mar 2023 04:15:53 GMT
ARG KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa
# Thu, 30 Mar 2023 04:15:53 GMT
ARG KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
# Thu, 30 Mar 2023 04:15:59 GMT
# ARGS: KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 30 Mar 2023 04:16:00 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 30 Mar 2023 04:16:00 GMT
USER kong
# Thu, 30 Mar 2023 04:16:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Mar 2023 04:16:00 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 30 Mar 2023 04:16:00 GMT
STOPSIGNAL SIGQUIT
# Thu, 30 Mar 2023 04:16:00 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 30 Mar 2023 04:16:00 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:547446be3368f442c50ff95e2a2a9c85110b6b41bbb3c75b7e5ebb115f478b57`  
		Last Modified: Wed, 29 Mar 2023 17:39:56 GMT  
		Size: 2.7 MB (2709344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ff78970d3279285a92299fc4aca99872e9f7ad31a1dff143611df7b0b93a8c`  
		Last Modified: Thu, 30 Mar 2023 04:16:52 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b48e0173e1b427e16c7dbce6bc355cf2c26e68a51a444cb1782ae95506a7a893`  
		Last Modified: Thu, 30 Mar 2023 04:16:59 GMT  
		Size: 45.8 MB (45810736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb0a1ba1287b8da1a4810968cf7f49bad92b1340c00d942cae076865bb1737e1`  
		Last Modified: Thu, 30 Mar 2023 04:16:52 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.8.3-alpine`

```console
$ docker pull kong@sha256:83b7264156246a942c1bc1c95d9409603d9fc71f578d13731bc77824388f0e21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.8.3-alpine` - linux; amd64

```console
$ docker pull kong@sha256:b767f991a30f9cac433865b63e465ccd0e485c104329391815372789b475f7a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49336669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f08d55de6605e1ff87d4bb5bf3bee1589e87b5390041fdeff55c501a60dbc5db`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:11:26 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 29 Mar 2023 22:11:26 GMT
ARG ASSET=ce
# Wed, 29 Mar 2023 22:11:26 GMT
ENV ASSET=ce
# Wed, 29 Mar 2023 22:11:26 GMT
ARG EE_PORTS
# Wed, 29 Mar 2023 22:11:26 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 29 Mar 2023 22:11:26 GMT
ARG KONG_VERSION=2.8.3
# Wed, 29 Mar 2023 22:11:27 GMT
ENV KONG_VERSION=2.8.3
# Wed, 29 Mar 2023 22:11:27 GMT
ARG KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa
# Wed, 29 Mar 2023 22:11:27 GMT
ARG KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
# Wed, 29 Mar 2023 22:11:33 GMT
# ARGS: KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Wed, 29 Mar 2023 22:11:33 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 29 Mar 2023 22:11:34 GMT
USER kong
# Wed, 29 Mar 2023 22:11:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 29 Mar 2023 22:11:34 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 29 Mar 2023 22:11:34 GMT
STOPSIGNAL SIGQUIT
# Wed, 29 Mar 2023 22:11:34 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 29 Mar 2023 22:11:34 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:91d30c5bc19582de1415b18f1ec5bcbf52a558b62cf6cc201c9669df9f748c22`  
		Last Modified: Wed, 29 Mar 2023 18:20:09 GMT  
		Size: 2.8 MB (2807803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c6c1798758d52be09614fa8ec90799ee184e137bc78da7792dcfd727d51c26`  
		Last Modified: Wed, 29 Mar 2023 22:12:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd40f0f27d03b3579307957241a10fe96137a75555eb4ceb5f0436ebcc48a735`  
		Last Modified: Wed, 29 Mar 2023 22:12:49 GMT  
		Size: 46.5 MB (46527857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae3de81c97825904984d09363568c9ac780869f6bc3fa71a512a06ba5de98505`  
		Last Modified: Wed, 29 Mar 2023 22:12:42 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.8.3-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:ef1492e3d92dcf03c868b4266628c35bda33c3d78710121d3e7606c1fab1e669
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.5 MB (48521091 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4bb5629cc85df77176510a0979e93e6392d0add4bf05deafc3ae5f7ef8e188c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:15:52 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 30 Mar 2023 04:15:53 GMT
ARG ASSET=ce
# Thu, 30 Mar 2023 04:15:53 GMT
ENV ASSET=ce
# Thu, 30 Mar 2023 04:15:53 GMT
ARG EE_PORTS
# Thu, 30 Mar 2023 04:15:53 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 30 Mar 2023 04:15:53 GMT
ARG KONG_VERSION=2.8.3
# Thu, 30 Mar 2023 04:15:53 GMT
ENV KONG_VERSION=2.8.3
# Thu, 30 Mar 2023 04:15:53 GMT
ARG KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa
# Thu, 30 Mar 2023 04:15:53 GMT
ARG KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
# Thu, 30 Mar 2023 04:15:59 GMT
# ARGS: KONG_AMD64_SHA=46e8ccd60fdcfb44a02b7ff9cfc79b701bf1275ec6ba88138d98317509c682fa KONG_ARM64_SHA=f6c90eb9b126e049859f037e81f070f4116ac701c4e4b9ad2d1ec574fbe44bb3
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     else       apk upgrade;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Thu, 30 Mar 2023 04:16:00 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 30 Mar 2023 04:16:00 GMT
USER kong
# Thu, 30 Mar 2023 04:16:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Mar 2023 04:16:00 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 30 Mar 2023 04:16:00 GMT
STOPSIGNAL SIGQUIT
# Thu, 30 Mar 2023 04:16:00 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 30 Mar 2023 04:16:00 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:547446be3368f442c50ff95e2a2a9c85110b6b41bbb3c75b7e5ebb115f478b57`  
		Last Modified: Wed, 29 Mar 2023 17:39:56 GMT  
		Size: 2.7 MB (2709344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ff78970d3279285a92299fc4aca99872e9f7ad31a1dff143611df7b0b93a8c`  
		Last Modified: Thu, 30 Mar 2023 04:16:52 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b48e0173e1b427e16c7dbce6bc355cf2c26e68a51a444cb1782ae95506a7a893`  
		Last Modified: Thu, 30 Mar 2023 04:16:59 GMT  
		Size: 45.8 MB (45810736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb0a1ba1287b8da1a4810968cf7f49bad92b1340c00d942cae076865bb1737e1`  
		Last Modified: Thu, 30 Mar 2023 04:16:52 GMT  
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
$ docker pull kong@sha256:73513cfe5921762fbb2a8fcf5436dfed69d207224c10a15115f67da3807b3ea9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3` - linux; amd64

```console
$ docker pull kong@sha256:71cdbcbcf156077528e0ebb698a44670ccb33f846d6927e27f0ea3e8ff31ba2c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.5 MB (74451841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fa2e7c7b0b42a300c9c9f3194f853c86749f987f7e7003d32bd0226889b0b88`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 07:49:24 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 04 May 2023 07:49:24 GMT
ARG ASSET=ce
# Thu, 04 May 2023 07:49:24 GMT
ENV ASSET=ce
# Thu, 04 May 2023 07:49:24 GMT
ARG EE_PORTS
# Thu, 04 May 2023 07:49:24 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Thu, 04 May 2023 07:49:24 GMT
ARG KONG_VERSION=3.2.2
# Thu, 04 May 2023 07:49:24 GMT
ENV KONG_VERSION=3.2.2
# Thu, 04 May 2023 07:49:24 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Thu, 04 May 2023 07:49:24 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Thu, 04 May 2023 07:49:53 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Thu, 04 May 2023 07:49:54 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Thu, 04 May 2023 07:49:54 GMT
USER kong
# Thu, 04 May 2023 07:49:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 04 May 2023 07:49:54 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 04 May 2023 07:49:54 GMT
STOPSIGNAL SIGQUIT
# Thu, 04 May 2023 07:49:54 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 04 May 2023 07:49:54 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4452e2a99e08079eada765eaec98220af45483cd8a0e7809ca19f969da460e32`  
		Last Modified: Thu, 04 May 2023 07:50:22 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d9a6e2b2b5f047a029e37c75236c24d4929d3b90f9f1540d69889bbabbe8d2`  
		Last Modified: Thu, 04 May 2023 07:50:29 GMT  
		Size: 44.0 MB (44020342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eccf8a96cc3972523193277dfcc6d7d0125e72e86cb9177b2479637c54be8f6e`  
		Last Modified: Thu, 04 May 2023 07:50:22 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:331455622bce663694cf274fa5acc68a84bea80ecbe4b4b7403ec54eab362d3f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.6 MB (78563017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53cb403e2e2a3e8ccb433f50a8ae3f79029e5ae441e50157c90bc9fca8c52cfc`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 03:44:59 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 04 May 2023 03:44:59 GMT
ARG ASSET=ce
# Thu, 04 May 2023 03:44:59 GMT
ENV ASSET=ce
# Thu, 04 May 2023 03:44:59 GMT
ARG EE_PORTS
# Thu, 04 May 2023 03:44:59 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Thu, 04 May 2023 03:44:59 GMT
ARG KONG_VERSION=3.2.2
# Thu, 04 May 2023 03:44:59 GMT
ENV KONG_VERSION=3.2.2
# Thu, 04 May 2023 03:44:59 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Thu, 04 May 2023 03:44:59 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Thu, 04 May 2023 03:45:16 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Thu, 04 May 2023 03:45:17 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Thu, 04 May 2023 03:45:17 GMT
USER kong
# Thu, 04 May 2023 03:45:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 04 May 2023 03:45:17 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 04 May 2023 03:45:17 GMT
STOPSIGNAL SIGQUIT
# Thu, 04 May 2023 03:45:17 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 04 May 2023 03:45:17 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aead6b4c2aa9f393a63e92067a6a16c0f1527ee558eda6b45181f820bcf1f61`  
		Last Modified: Thu, 04 May 2023 03:45:39 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e562bf9fba3e3ac55944fd6b19bac4ffac0d4bee31828b1d3cdca127298dca6`  
		Last Modified: Thu, 04 May 2023 03:45:45 GMT  
		Size: 50.2 MB (50172295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b47e7a18f6ca88337071e2830f034ea6b85f3b0a4d3d980a63b3c7d5309394`  
		Last Modified: Thu, 04 May 2023 03:45:39 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.0`

```console
$ docker pull kong@sha256:6ec945bbf2598d9c07d922f449ed76f68c43f2450091c9b38e7aac7102826ddd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.0` - linux; amd64

```console
$ docker pull kong@sha256:a1eab74296e15d62b224adb036f3a26e660a956c22823b5a0747ece8e81800f9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75643533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0c74ed2b904a2cfcb6073f76e42b1f36c0e4220514bc6273e7c33b3423eccb3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:11:00 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 29 Mar 2023 22:11:13 GMT
ARG KONG_VERSION=3.0.2
# Wed, 29 Mar 2023 22:11:13 GMT
ENV KONG_VERSION=3.0.2
# Wed, 29 Mar 2023 22:11:13 GMT
ARG KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e
# Wed, 29 Mar 2023 22:11:13 GMT
ARG KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
# Wed, 29 Mar 2023 22:11:13 GMT
ARG ASSET=remote
# Wed, 29 Mar 2023 22:11:13 GMT
ARG EE_PORTS
# Wed, 29 Mar 2023 22:11:13 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Wed, 29 Mar 2023 22:11:21 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Wed, 29 Mar 2023 22:11:21 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 29 Mar 2023 22:11:21 GMT
USER kong
# Wed, 29 Mar 2023 22:11:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 29 Mar 2023 22:11:22 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 29 Mar 2023 22:11:22 GMT
STOPSIGNAL SIGQUIT
# Wed, 29 Mar 2023 22:11:22 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 29 Mar 2023 22:11:22 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:91d30c5bc19582de1415b18f1ec5bcbf52a558b62cf6cc201c9669df9f748c22`  
		Last Modified: Wed, 29 Mar 2023 18:20:09 GMT  
		Size: 2.8 MB (2807803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b6d5af9a6b2c0f0247f96a311ae5dee1a5d4344b6cb3304adf47fd9ab3d7641`  
		Last Modified: Wed, 29 Mar 2023 22:12:22 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26edd0fc7e7b2a33bad841f24f8b6605d85c6c0fa75ec6f40677e98e56e7944`  
		Last Modified: Wed, 29 Mar 2023 22:12:30 GMT  
		Size: 72.8 MB (72834717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3ff3083ae5c235de11e009601fd437ea359ba779e077b3ac7fad09676d7a248`  
		Last Modified: Wed, 29 Mar 2023 22:12:22 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.0` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:69b6e1c46339ae4502000925473572c7d03427e6302a677ce8dbef83b950036d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73630832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43951a1b92592cb3dfe51442d60505e5dda21ec6e70a101e9bbc6ecbea6de818`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:15:30 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 30 Mar 2023 04:15:40 GMT
ARG KONG_VERSION=3.0.2
# Thu, 30 Mar 2023 04:15:41 GMT
ENV KONG_VERSION=3.0.2
# Thu, 30 Mar 2023 04:15:41 GMT
ARG KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e
# Thu, 30 Mar 2023 04:15:41 GMT
ARG KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
# Thu, 30 Mar 2023 04:15:41 GMT
ARG ASSET=remote
# Thu, 30 Mar 2023 04:15:41 GMT
ARG EE_PORTS
# Thu, 30 Mar 2023 04:15:41 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Thu, 30 Mar 2023 04:15:48 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Thu, 30 Mar 2023 04:15:48 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 30 Mar 2023 04:15:48 GMT
USER kong
# Thu, 30 Mar 2023 04:15:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Mar 2023 04:15:49 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 30 Mar 2023 04:15:49 GMT
STOPSIGNAL SIGQUIT
# Thu, 30 Mar 2023 04:15:49 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 30 Mar 2023 04:15:49 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:547446be3368f442c50ff95e2a2a9c85110b6b41bbb3c75b7e5ebb115f478b57`  
		Last Modified: Wed, 29 Mar 2023 17:39:56 GMT  
		Size: 2.7 MB (2709344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c090df497f98006d418bbf46a5a99c1c0dde3d77d7d48e53a634a9eb250de9`  
		Last Modified: Thu, 30 Mar 2023 04:16:33 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d29085e17f36af88970040b865e5238ebf340d6926363115d8d2de6e8ceb1f2`  
		Last Modified: Thu, 30 Mar 2023 04:16:41 GMT  
		Size: 70.9 MB (70920472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32421f87e119ba5582a53f513eb740d9d3a892b553ae3bb214f1bfbf82ad9309`  
		Last Modified: Thu, 30 Mar 2023 04:16:33 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.0-alpine`

```console
$ docker pull kong@sha256:6ec945bbf2598d9c07d922f449ed76f68c43f2450091c9b38e7aac7102826ddd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.0-alpine` - linux; amd64

```console
$ docker pull kong@sha256:a1eab74296e15d62b224adb036f3a26e660a956c22823b5a0747ece8e81800f9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75643533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0c74ed2b904a2cfcb6073f76e42b1f36c0e4220514bc6273e7c33b3423eccb3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:11:00 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 29 Mar 2023 22:11:13 GMT
ARG KONG_VERSION=3.0.2
# Wed, 29 Mar 2023 22:11:13 GMT
ENV KONG_VERSION=3.0.2
# Wed, 29 Mar 2023 22:11:13 GMT
ARG KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e
# Wed, 29 Mar 2023 22:11:13 GMT
ARG KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
# Wed, 29 Mar 2023 22:11:13 GMT
ARG ASSET=remote
# Wed, 29 Mar 2023 22:11:13 GMT
ARG EE_PORTS
# Wed, 29 Mar 2023 22:11:13 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Wed, 29 Mar 2023 22:11:21 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Wed, 29 Mar 2023 22:11:21 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 29 Mar 2023 22:11:21 GMT
USER kong
# Wed, 29 Mar 2023 22:11:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 29 Mar 2023 22:11:22 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 29 Mar 2023 22:11:22 GMT
STOPSIGNAL SIGQUIT
# Wed, 29 Mar 2023 22:11:22 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 29 Mar 2023 22:11:22 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:91d30c5bc19582de1415b18f1ec5bcbf52a558b62cf6cc201c9669df9f748c22`  
		Last Modified: Wed, 29 Mar 2023 18:20:09 GMT  
		Size: 2.8 MB (2807803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b6d5af9a6b2c0f0247f96a311ae5dee1a5d4344b6cb3304adf47fd9ab3d7641`  
		Last Modified: Wed, 29 Mar 2023 22:12:22 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26edd0fc7e7b2a33bad841f24f8b6605d85c6c0fa75ec6f40677e98e56e7944`  
		Last Modified: Wed, 29 Mar 2023 22:12:30 GMT  
		Size: 72.8 MB (72834717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3ff3083ae5c235de11e009601fd437ea359ba779e077b3ac7fad09676d7a248`  
		Last Modified: Wed, 29 Mar 2023 22:12:22 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.0-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:69b6e1c46339ae4502000925473572c7d03427e6302a677ce8dbef83b950036d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73630832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43951a1b92592cb3dfe51442d60505e5dda21ec6e70a101e9bbc6ecbea6de818`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:15:30 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 30 Mar 2023 04:15:40 GMT
ARG KONG_VERSION=3.0.2
# Thu, 30 Mar 2023 04:15:41 GMT
ENV KONG_VERSION=3.0.2
# Thu, 30 Mar 2023 04:15:41 GMT
ARG KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e
# Thu, 30 Mar 2023 04:15:41 GMT
ARG KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
# Thu, 30 Mar 2023 04:15:41 GMT
ARG ASSET=remote
# Thu, 30 Mar 2023 04:15:41 GMT
ARG EE_PORTS
# Thu, 30 Mar 2023 04:15:41 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Thu, 30 Mar 2023 04:15:48 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Thu, 30 Mar 2023 04:15:48 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 30 Mar 2023 04:15:48 GMT
USER kong
# Thu, 30 Mar 2023 04:15:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Mar 2023 04:15:49 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 30 Mar 2023 04:15:49 GMT
STOPSIGNAL SIGQUIT
# Thu, 30 Mar 2023 04:15:49 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 30 Mar 2023 04:15:49 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:547446be3368f442c50ff95e2a2a9c85110b6b41bbb3c75b7e5ebb115f478b57`  
		Last Modified: Wed, 29 Mar 2023 17:39:56 GMT  
		Size: 2.7 MB (2709344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c090df497f98006d418bbf46a5a99c1c0dde3d77d7d48e53a634a9eb250de9`  
		Last Modified: Thu, 30 Mar 2023 04:16:33 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d29085e17f36af88970040b865e5238ebf340d6926363115d8d2de6e8ceb1f2`  
		Last Modified: Thu, 30 Mar 2023 04:16:41 GMT  
		Size: 70.9 MB (70920472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32421f87e119ba5582a53f513eb740d9d3a892b553ae3bb214f1bfbf82ad9309`  
		Last Modified: Thu, 30 Mar 2023 04:16:33 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.0-ubuntu`

```console
$ docker pull kong@sha256:738bdbd123ee7b0bed1f9038fa0bbc1beddc53ae8980dab6b64df135f24b2d94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.0-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:e9d5dda1bd4f39e7fa0e6bcf12718bfd1e1f4057db65fa53fd48096e4aa0fbe6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.7 MB (101694617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36c7abb2de81c0557d2da44bf4acd75ec4ff518d832005295e87e3b132e0b032`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 00:48:57 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Tue, 18 Apr 2023 00:48:57 GMT
ARG ASSET=ce
# Tue, 18 Apr 2023 00:48:57 GMT
ENV ASSET=ce
# Tue, 18 Apr 2023 00:48:57 GMT
ARG EE_PORTS
# Tue, 18 Apr 2023 00:48:57 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Tue, 18 Apr 2023 00:49:32 GMT
ARG KONG_VERSION=3.0.2
# Tue, 18 Apr 2023 00:49:32 GMT
ENV KONG_VERSION=3.0.2
# Tue, 18 Apr 2023 00:49:32 GMT
ARG KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396
# Tue, 18 Apr 2023 00:49:32 GMT
ARG KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
# Tue, 18 Apr 2023 00:49:52 GMT
# ARGS: KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396 KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 18 Apr 2023 00:49:53 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 18 Apr 2023 00:49:53 GMT
USER kong
# Tue, 18 Apr 2023 00:49:53 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 18 Apr 2023 00:49:53 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 18 Apr 2023 00:49:53 GMT
STOPSIGNAL SIGQUIT
# Tue, 18 Apr 2023 00:49:53 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 18 Apr 2023 00:49:54 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1270117cfa3f1bf43891c96ffc5e3f48c9b1b960b8f1c17ad7d5cbb6971f0fbd`  
		Last Modified: Tue, 18 Apr 2023 00:50:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e3e94b7778f468bc9687113229b1550d32f2d19632c324489f5d87c564f2749`  
		Last Modified: Tue, 18 Apr 2023 00:50:49 GMT  
		Size: 73.1 MB (73115045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c3709def9dda22e3f52d5000041dd3ba80e64c58ca7e5ff6738b29dd2cedbf`  
		Last Modified: Tue, 18 Apr 2023 00:50:38 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.0-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:937d285da6fa08264c2c28e8e997ea4c87520d795f513d9966fe5d7f75a8fc32
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.9 MB (98937255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cfb522eb11ee3d925d76914207df69726d88542c8ce5afc775b3300ed32a7df`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:55:38 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Tue, 18 Apr 2023 01:55:38 GMT
ARG ASSET=ce
# Tue, 18 Apr 2023 01:55:38 GMT
ENV ASSET=ce
# Tue, 18 Apr 2023 01:55:38 GMT
ARG EE_PORTS
# Tue, 18 Apr 2023 01:55:38 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Tue, 18 Apr 2023 01:56:02 GMT
ARG KONG_VERSION=3.0.2
# Tue, 18 Apr 2023 01:56:02 GMT
ENV KONG_VERSION=3.0.2
# Tue, 18 Apr 2023 01:56:02 GMT
ARG KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396
# Tue, 18 Apr 2023 01:56:02 GMT
ARG KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
# Tue, 18 Apr 2023 01:56:22 GMT
# ARGS: KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396 KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 18 Apr 2023 01:56:23 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 18 Apr 2023 01:56:23 GMT
USER kong
# Tue, 18 Apr 2023 01:56:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 18 Apr 2023 01:56:23 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 18 Apr 2023 01:56:23 GMT
STOPSIGNAL SIGQUIT
# Tue, 18 Apr 2023 01:56:23 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 18 Apr 2023 01:56:23 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33117919705427cc2b91c73428239666db66c5521aad5bb7169b1d6fc9d0b5dc`  
		Last Modified: Tue, 18 Apr 2023 01:56:41 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b5d517b7ce411115a69d3a88946c56ca87258d1cd048d9a878b949d8a2abb5`  
		Last Modified: Tue, 18 Apr 2023 01:57:08 GMT  
		Size: 71.7 MB (71739854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19e1a10cf887d91c6182976d4bbbb1e0b2c85d8ed10c3e11373e94c35e6dbdc9`  
		Last Modified: Tue, 18 Apr 2023 01:56:59 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.0.2`

```console
$ docker pull kong@sha256:6ec945bbf2598d9c07d922f449ed76f68c43f2450091c9b38e7aac7102826ddd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.0.2` - linux; amd64

```console
$ docker pull kong@sha256:a1eab74296e15d62b224adb036f3a26e660a956c22823b5a0747ece8e81800f9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75643533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0c74ed2b904a2cfcb6073f76e42b1f36c0e4220514bc6273e7c33b3423eccb3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:11:00 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 29 Mar 2023 22:11:13 GMT
ARG KONG_VERSION=3.0.2
# Wed, 29 Mar 2023 22:11:13 GMT
ENV KONG_VERSION=3.0.2
# Wed, 29 Mar 2023 22:11:13 GMT
ARG KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e
# Wed, 29 Mar 2023 22:11:13 GMT
ARG KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
# Wed, 29 Mar 2023 22:11:13 GMT
ARG ASSET=remote
# Wed, 29 Mar 2023 22:11:13 GMT
ARG EE_PORTS
# Wed, 29 Mar 2023 22:11:13 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Wed, 29 Mar 2023 22:11:21 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Wed, 29 Mar 2023 22:11:21 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 29 Mar 2023 22:11:21 GMT
USER kong
# Wed, 29 Mar 2023 22:11:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 29 Mar 2023 22:11:22 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 29 Mar 2023 22:11:22 GMT
STOPSIGNAL SIGQUIT
# Wed, 29 Mar 2023 22:11:22 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 29 Mar 2023 22:11:22 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:91d30c5bc19582de1415b18f1ec5bcbf52a558b62cf6cc201c9669df9f748c22`  
		Last Modified: Wed, 29 Mar 2023 18:20:09 GMT  
		Size: 2.8 MB (2807803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b6d5af9a6b2c0f0247f96a311ae5dee1a5d4344b6cb3304adf47fd9ab3d7641`  
		Last Modified: Wed, 29 Mar 2023 22:12:22 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26edd0fc7e7b2a33bad841f24f8b6605d85c6c0fa75ec6f40677e98e56e7944`  
		Last Modified: Wed, 29 Mar 2023 22:12:30 GMT  
		Size: 72.8 MB (72834717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3ff3083ae5c235de11e009601fd437ea359ba779e077b3ac7fad09676d7a248`  
		Last Modified: Wed, 29 Mar 2023 22:12:22 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.0.2` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:69b6e1c46339ae4502000925473572c7d03427e6302a677ce8dbef83b950036d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73630832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43951a1b92592cb3dfe51442d60505e5dda21ec6e70a101e9bbc6ecbea6de818`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:15:30 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 30 Mar 2023 04:15:40 GMT
ARG KONG_VERSION=3.0.2
# Thu, 30 Mar 2023 04:15:41 GMT
ENV KONG_VERSION=3.0.2
# Thu, 30 Mar 2023 04:15:41 GMT
ARG KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e
# Thu, 30 Mar 2023 04:15:41 GMT
ARG KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
# Thu, 30 Mar 2023 04:15:41 GMT
ARG ASSET=remote
# Thu, 30 Mar 2023 04:15:41 GMT
ARG EE_PORTS
# Thu, 30 Mar 2023 04:15:41 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Thu, 30 Mar 2023 04:15:48 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Thu, 30 Mar 2023 04:15:48 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 30 Mar 2023 04:15:48 GMT
USER kong
# Thu, 30 Mar 2023 04:15:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Mar 2023 04:15:49 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 30 Mar 2023 04:15:49 GMT
STOPSIGNAL SIGQUIT
# Thu, 30 Mar 2023 04:15:49 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 30 Mar 2023 04:15:49 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:547446be3368f442c50ff95e2a2a9c85110b6b41bbb3c75b7e5ebb115f478b57`  
		Last Modified: Wed, 29 Mar 2023 17:39:56 GMT  
		Size: 2.7 MB (2709344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c090df497f98006d418bbf46a5a99c1c0dde3d77d7d48e53a634a9eb250de9`  
		Last Modified: Thu, 30 Mar 2023 04:16:33 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d29085e17f36af88970040b865e5238ebf340d6926363115d8d2de6e8ceb1f2`  
		Last Modified: Thu, 30 Mar 2023 04:16:41 GMT  
		Size: 70.9 MB (70920472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32421f87e119ba5582a53f513eb740d9d3a892b553ae3bb214f1bfbf82ad9309`  
		Last Modified: Thu, 30 Mar 2023 04:16:33 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.0.2-alpine`

```console
$ docker pull kong@sha256:6ec945bbf2598d9c07d922f449ed76f68c43f2450091c9b38e7aac7102826ddd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.0.2-alpine` - linux; amd64

```console
$ docker pull kong@sha256:a1eab74296e15d62b224adb036f3a26e660a956c22823b5a0747ece8e81800f9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75643533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0c74ed2b904a2cfcb6073f76e42b1f36c0e4220514bc6273e7c33b3423eccb3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:11:00 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 29 Mar 2023 22:11:13 GMT
ARG KONG_VERSION=3.0.2
# Wed, 29 Mar 2023 22:11:13 GMT
ENV KONG_VERSION=3.0.2
# Wed, 29 Mar 2023 22:11:13 GMT
ARG KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e
# Wed, 29 Mar 2023 22:11:13 GMT
ARG KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
# Wed, 29 Mar 2023 22:11:13 GMT
ARG ASSET=remote
# Wed, 29 Mar 2023 22:11:13 GMT
ARG EE_PORTS
# Wed, 29 Mar 2023 22:11:13 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Wed, 29 Mar 2023 22:11:21 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Wed, 29 Mar 2023 22:11:21 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 29 Mar 2023 22:11:21 GMT
USER kong
# Wed, 29 Mar 2023 22:11:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 29 Mar 2023 22:11:22 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 29 Mar 2023 22:11:22 GMT
STOPSIGNAL SIGQUIT
# Wed, 29 Mar 2023 22:11:22 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 29 Mar 2023 22:11:22 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:91d30c5bc19582de1415b18f1ec5bcbf52a558b62cf6cc201c9669df9f748c22`  
		Last Modified: Wed, 29 Mar 2023 18:20:09 GMT  
		Size: 2.8 MB (2807803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b6d5af9a6b2c0f0247f96a311ae5dee1a5d4344b6cb3304adf47fd9ab3d7641`  
		Last Modified: Wed, 29 Mar 2023 22:12:22 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f26edd0fc7e7b2a33bad841f24f8b6605d85c6c0fa75ec6f40677e98e56e7944`  
		Last Modified: Wed, 29 Mar 2023 22:12:30 GMT  
		Size: 72.8 MB (72834717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3ff3083ae5c235de11e009601fd437ea359ba779e077b3ac7fad09676d7a248`  
		Last Modified: Wed, 29 Mar 2023 22:12:22 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.0.2-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:69b6e1c46339ae4502000925473572c7d03427e6302a677ce8dbef83b950036d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73630832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43951a1b92592cb3dfe51442d60505e5dda21ec6e70a101e9bbc6ecbea6de818`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:15:30 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 30 Mar 2023 04:15:40 GMT
ARG KONG_VERSION=3.0.2
# Thu, 30 Mar 2023 04:15:41 GMT
ENV KONG_VERSION=3.0.2
# Thu, 30 Mar 2023 04:15:41 GMT
ARG KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e
# Thu, 30 Mar 2023 04:15:41 GMT
ARG KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
# Thu, 30 Mar 2023 04:15:41 GMT
ARG ASSET=remote
# Thu, 30 Mar 2023 04:15:41 GMT
ARG EE_PORTS
# Thu, 30 Mar 2023 04:15:41 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Thu, 30 Mar 2023 04:15:48 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=5f2f4c953cfc06c750614148b90f8216321b869ba44e1cf509f2dbbd9182516e KONG_ARM64_SHA=049efeb9f82898a0c4b0e3257c3389a2cb8fbf51339b497cff78c2687106718b
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Thu, 30 Mar 2023 04:15:48 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 30 Mar 2023 04:15:48 GMT
USER kong
# Thu, 30 Mar 2023 04:15:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Mar 2023 04:15:49 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 30 Mar 2023 04:15:49 GMT
STOPSIGNAL SIGQUIT
# Thu, 30 Mar 2023 04:15:49 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 30 Mar 2023 04:15:49 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:547446be3368f442c50ff95e2a2a9c85110b6b41bbb3c75b7e5ebb115f478b57`  
		Last Modified: Wed, 29 Mar 2023 17:39:56 GMT  
		Size: 2.7 MB (2709344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c090df497f98006d418bbf46a5a99c1c0dde3d77d7d48e53a634a9eb250de9`  
		Last Modified: Thu, 30 Mar 2023 04:16:33 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d29085e17f36af88970040b865e5238ebf340d6926363115d8d2de6e8ceb1f2`  
		Last Modified: Thu, 30 Mar 2023 04:16:41 GMT  
		Size: 70.9 MB (70920472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32421f87e119ba5582a53f513eb740d9d3a892b553ae3bb214f1bfbf82ad9309`  
		Last Modified: Thu, 30 Mar 2023 04:16:33 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.0.2-ubuntu`

```console
$ docker pull kong@sha256:738bdbd123ee7b0bed1f9038fa0bbc1beddc53ae8980dab6b64df135f24b2d94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.0.2-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:e9d5dda1bd4f39e7fa0e6bcf12718bfd1e1f4057db65fa53fd48096e4aa0fbe6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.7 MB (101694617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36c7abb2de81c0557d2da44bf4acd75ec4ff518d832005295e87e3b132e0b032`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 00:48:57 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Tue, 18 Apr 2023 00:48:57 GMT
ARG ASSET=ce
# Tue, 18 Apr 2023 00:48:57 GMT
ENV ASSET=ce
# Tue, 18 Apr 2023 00:48:57 GMT
ARG EE_PORTS
# Tue, 18 Apr 2023 00:48:57 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Tue, 18 Apr 2023 00:49:32 GMT
ARG KONG_VERSION=3.0.2
# Tue, 18 Apr 2023 00:49:32 GMT
ENV KONG_VERSION=3.0.2
# Tue, 18 Apr 2023 00:49:32 GMT
ARG KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396
# Tue, 18 Apr 2023 00:49:32 GMT
ARG KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
# Tue, 18 Apr 2023 00:49:52 GMT
# ARGS: KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396 KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 18 Apr 2023 00:49:53 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 18 Apr 2023 00:49:53 GMT
USER kong
# Tue, 18 Apr 2023 00:49:53 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 18 Apr 2023 00:49:53 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 18 Apr 2023 00:49:53 GMT
STOPSIGNAL SIGQUIT
# Tue, 18 Apr 2023 00:49:53 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 18 Apr 2023 00:49:54 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1270117cfa3f1bf43891c96ffc5e3f48c9b1b960b8f1c17ad7d5cbb6971f0fbd`  
		Last Modified: Tue, 18 Apr 2023 00:50:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e3e94b7778f468bc9687113229b1550d32f2d19632c324489f5d87c564f2749`  
		Last Modified: Tue, 18 Apr 2023 00:50:49 GMT  
		Size: 73.1 MB (73115045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35c3709def9dda22e3f52d5000041dd3ba80e64c58ca7e5ff6738b29dd2cedbf`  
		Last Modified: Tue, 18 Apr 2023 00:50:38 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.0.2-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:937d285da6fa08264c2c28e8e997ea4c87520d795f513d9966fe5d7f75a8fc32
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.9 MB (98937255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cfb522eb11ee3d925d76914207df69726d88542c8ce5afc775b3300ed32a7df`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:55:38 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Tue, 18 Apr 2023 01:55:38 GMT
ARG ASSET=ce
# Tue, 18 Apr 2023 01:55:38 GMT
ENV ASSET=ce
# Tue, 18 Apr 2023 01:55:38 GMT
ARG EE_PORTS
# Tue, 18 Apr 2023 01:55:38 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Tue, 18 Apr 2023 01:56:02 GMT
ARG KONG_VERSION=3.0.2
# Tue, 18 Apr 2023 01:56:02 GMT
ENV KONG_VERSION=3.0.2
# Tue, 18 Apr 2023 01:56:02 GMT
ARG KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396
# Tue, 18 Apr 2023 01:56:02 GMT
ARG KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
# Tue, 18 Apr 2023 01:56:22 GMT
# ARGS: KONG_AMD64_SHA=ad9b0b97b48e2a939d2aefa1ae2e4f2924a4cda5382e99524589ccbb90f7c396 KONG_ARM64_SHA=8e10e6693ece4166c9acf3eb0745c119468d6902e7c27b2841f900644b3e2c53
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 18 Apr 2023 01:56:23 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 18 Apr 2023 01:56:23 GMT
USER kong
# Tue, 18 Apr 2023 01:56:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 18 Apr 2023 01:56:23 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 18 Apr 2023 01:56:23 GMT
STOPSIGNAL SIGQUIT
# Tue, 18 Apr 2023 01:56:23 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 18 Apr 2023 01:56:23 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33117919705427cc2b91c73428239666db66c5521aad5bb7169b1d6fc9d0b5dc`  
		Last Modified: Tue, 18 Apr 2023 01:56:41 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b5d517b7ce411115a69d3a88946c56ca87258d1cd048d9a878b949d8a2abb5`  
		Last Modified: Tue, 18 Apr 2023 01:57:08 GMT  
		Size: 71.7 MB (71739854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19e1a10cf887d91c6182976d4bbbb1e0b2c85d8ed10c3e11373e94c35e6dbdc9`  
		Last Modified: Tue, 18 Apr 2023 01:56:59 GMT  
		Size: 880.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.1`

```console
$ docker pull kong@sha256:95de25fe58f6fe96e63b129a6963a3ce60e03d670100dc82103f2ce362a60db7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.1` - linux; amd64

```console
$ docker pull kong@sha256:fe077a1e32c364576237a33b1916e625416a60630cc20578f20d1e5a5df376f0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75688407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b815af25ca31f8d87d21059367ff86ef810fc8761eb1e73196ff92c438fc8dbe`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:11:00 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 29 Mar 2023 22:11:00 GMT
ARG KONG_VERSION=3.1.1
# Wed, 29 Mar 2023 22:11:00 GMT
ENV KONG_VERSION=3.1.1
# Wed, 29 Mar 2023 22:11:00 GMT
ARG KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c
# Wed, 29 Mar 2023 22:11:00 GMT
ARG KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
# Wed, 29 Mar 2023 22:11:00 GMT
ARG ASSET=remote
# Wed, 29 Mar 2023 22:11:00 GMT
ARG EE_PORTS
# Wed, 29 Mar 2023 22:11:00 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Wed, 29 Mar 2023 22:11:07 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Wed, 29 Mar 2023 22:11:08 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 29 Mar 2023 22:11:08 GMT
USER kong
# Wed, 29 Mar 2023 22:11:08 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 29 Mar 2023 22:11:08 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 29 Mar 2023 22:11:08 GMT
STOPSIGNAL SIGQUIT
# Wed, 29 Mar 2023 22:11:08 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 29 Mar 2023 22:11:08 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:91d30c5bc19582de1415b18f1ec5bcbf52a558b62cf6cc201c9669df9f748c22`  
		Last Modified: Wed, 29 Mar 2023 18:20:09 GMT  
		Size: 2.8 MB (2807803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d355939d3033d764ca6ac536976f4e0ef35234a8139659930ed75004b7ac3b`  
		Last Modified: Wed, 29 Mar 2023 22:12:04 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e2d991ca57d6678cd5b80335d6cd62bcda57cda9ad09f4356fc3f54974664a`  
		Last Modified: Wed, 29 Mar 2023 22:12:11 GMT  
		Size: 72.9 MB (72879589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40141fb6acdb9e60f527a720a3bee407e6cc53e6998f1055f9c98d52a2449bef`  
		Last Modified: Wed, 29 Mar 2023 22:12:04 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.1` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:d88708954f3766d18f2aa86efa96c599507d7ea47f82d524548fc8c35875b6c5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.7 MB (73704060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9479f123cf5449eed5a7ad7a3493ef51469e5a73179ab97fdc21294abb3d9f86`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:15:30 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 30 Mar 2023 04:15:30 GMT
ARG KONG_VERSION=3.1.1
# Thu, 30 Mar 2023 04:15:31 GMT
ENV KONG_VERSION=3.1.1
# Thu, 30 Mar 2023 04:15:31 GMT
ARG KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c
# Thu, 30 Mar 2023 04:15:31 GMT
ARG KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
# Thu, 30 Mar 2023 04:15:31 GMT
ARG ASSET=remote
# Thu, 30 Mar 2023 04:15:31 GMT
ARG EE_PORTS
# Thu, 30 Mar 2023 04:15:31 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Thu, 30 Mar 2023 04:15:36 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Thu, 30 Mar 2023 04:15:37 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 30 Mar 2023 04:15:37 GMT
USER kong
# Thu, 30 Mar 2023 04:15:37 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Mar 2023 04:15:38 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 30 Mar 2023 04:15:38 GMT
STOPSIGNAL SIGQUIT
# Thu, 30 Mar 2023 04:15:38 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 30 Mar 2023 04:15:38 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:547446be3368f442c50ff95e2a2a9c85110b6b41bbb3c75b7e5ebb115f478b57`  
		Last Modified: Wed, 29 Mar 2023 17:39:56 GMT  
		Size: 2.7 MB (2709344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f137c449ccbb530641e2cca76ab47da104148e987af90da334338ae8a75ee8d`  
		Last Modified: Thu, 30 Mar 2023 04:16:16 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa5ed9b55ad6f487ac77eb1ca65c204eaa1ff7c700229ffca32bf6d1e98e301`  
		Last Modified: Thu, 30 Mar 2023 04:16:23 GMT  
		Size: 71.0 MB (70993698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe163fe5badbb78866e8b29e88f7b2048cef5a67951386386625642b34e417f1`  
		Last Modified: Thu, 30 Mar 2023 04:16:16 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.1-ubuntu`

```console
$ docker pull kong@sha256:3bde6e63802d1c6799673d86602bc18a0ad7df02a928a980163360699b9283a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.1-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:fb7def9d63b24dc4c240b345e7e9355337786d632661945e06a15ef20e4779a1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.7 MB (101731018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5498f3ffdb5118b22860bb4093d18caa5b3149307152c58abc431e05d8685579`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 00:48:57 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Tue, 18 Apr 2023 00:48:57 GMT
ARG ASSET=ce
# Tue, 18 Apr 2023 00:48:57 GMT
ENV ASSET=ce
# Tue, 18 Apr 2023 00:48:57 GMT
ARG EE_PORTS
# Tue, 18 Apr 2023 00:48:57 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Tue, 18 Apr 2023 00:48:57 GMT
ARG KONG_VERSION=3.1.1
# Tue, 18 Apr 2023 00:48:57 GMT
ENV KONG_VERSION=3.1.1
# Tue, 18 Apr 2023 00:48:57 GMT
ARG KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b
# Tue, 18 Apr 2023 00:48:57 GMT
ARG KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
# Tue, 18 Apr 2023 00:49:26 GMT
# ARGS: KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 18 Apr 2023 00:49:26 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 18 Apr 2023 00:49:26 GMT
USER kong
# Tue, 18 Apr 2023 00:49:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 18 Apr 2023 00:49:26 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 18 Apr 2023 00:49:27 GMT
STOPSIGNAL SIGQUIT
# Tue, 18 Apr 2023 00:49:27 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 18 Apr 2023 00:49:27 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1270117cfa3f1bf43891c96ffc5e3f48c9b1b960b8f1c17ad7d5cbb6971f0fbd`  
		Last Modified: Tue, 18 Apr 2023 00:50:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bccee49244e3687399c9c24cc0ce516b0905e7442ed02f0fe26a5a84f5538a7b`  
		Last Modified: Tue, 18 Apr 2023 00:50:28 GMT  
		Size: 73.2 MB (73151444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53853e3583dd41f1e3da5406c276e344418ddaae1e4dbe056f2e4e205734273e`  
		Last Modified: Tue, 18 Apr 2023 00:50:16 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.1-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:c5b08a0c6e5170deba532287fe325be7b87ecb0c4710b857c519ae68507091ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.0 MB (98969390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85eab6242a1c3c38ed07152b648ebef2d657a39b9699ea9fb23dd60a94dc1a78`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:55:38 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Tue, 18 Apr 2023 01:55:38 GMT
ARG ASSET=ce
# Tue, 18 Apr 2023 01:55:38 GMT
ENV ASSET=ce
# Tue, 18 Apr 2023 01:55:38 GMT
ARG EE_PORTS
# Tue, 18 Apr 2023 01:55:38 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Tue, 18 Apr 2023 01:55:39 GMT
ARG KONG_VERSION=3.1.1
# Tue, 18 Apr 2023 01:55:39 GMT
ENV KONG_VERSION=3.1.1
# Tue, 18 Apr 2023 01:55:39 GMT
ARG KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b
# Tue, 18 Apr 2023 01:55:39 GMT
ARG KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
# Tue, 18 Apr 2023 01:55:55 GMT
# ARGS: KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 18 Apr 2023 01:55:56 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 18 Apr 2023 01:55:56 GMT
USER kong
# Tue, 18 Apr 2023 01:55:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 18 Apr 2023 01:55:57 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 18 Apr 2023 01:55:57 GMT
STOPSIGNAL SIGQUIT
# Tue, 18 Apr 2023 01:55:57 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 18 Apr 2023 01:55:57 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33117919705427cc2b91c73428239666db66c5521aad5bb7169b1d6fc9d0b5dc`  
		Last Modified: Tue, 18 Apr 2023 01:56:41 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dd8eef4dc95b72b5204ea83b481f2af54e5c5c4cf27232918bfcccd5cafd2c5`  
		Last Modified: Tue, 18 Apr 2023 01:56:50 GMT  
		Size: 71.8 MB (71771988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83592683ff2a59bc4dc1fb9e4c1df9fcd9e9cf7c783c57043f79f67657a7daab`  
		Last Modified: Tue, 18 Apr 2023 01:56:41 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.1.1`

```console
$ docker pull kong@sha256:95de25fe58f6fe96e63b129a6963a3ce60e03d670100dc82103f2ce362a60db7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.1.1` - linux; amd64

```console
$ docker pull kong@sha256:fe077a1e32c364576237a33b1916e625416a60630cc20578f20d1e5a5df376f0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75688407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b815af25ca31f8d87d21059367ff86ef810fc8761eb1e73196ff92c438fc8dbe`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:11:00 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 29 Mar 2023 22:11:00 GMT
ARG KONG_VERSION=3.1.1
# Wed, 29 Mar 2023 22:11:00 GMT
ENV KONG_VERSION=3.1.1
# Wed, 29 Mar 2023 22:11:00 GMT
ARG KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c
# Wed, 29 Mar 2023 22:11:00 GMT
ARG KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
# Wed, 29 Mar 2023 22:11:00 GMT
ARG ASSET=remote
# Wed, 29 Mar 2023 22:11:00 GMT
ARG EE_PORTS
# Wed, 29 Mar 2023 22:11:00 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Wed, 29 Mar 2023 22:11:07 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Wed, 29 Mar 2023 22:11:08 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 29 Mar 2023 22:11:08 GMT
USER kong
# Wed, 29 Mar 2023 22:11:08 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 29 Mar 2023 22:11:08 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 29 Mar 2023 22:11:08 GMT
STOPSIGNAL SIGQUIT
# Wed, 29 Mar 2023 22:11:08 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 29 Mar 2023 22:11:08 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:91d30c5bc19582de1415b18f1ec5bcbf52a558b62cf6cc201c9669df9f748c22`  
		Last Modified: Wed, 29 Mar 2023 18:20:09 GMT  
		Size: 2.8 MB (2807803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d355939d3033d764ca6ac536976f4e0ef35234a8139659930ed75004b7ac3b`  
		Last Modified: Wed, 29 Mar 2023 22:12:04 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e2d991ca57d6678cd5b80335d6cd62bcda57cda9ad09f4356fc3f54974664a`  
		Last Modified: Wed, 29 Mar 2023 22:12:11 GMT  
		Size: 72.9 MB (72879589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40141fb6acdb9e60f527a720a3bee407e6cc53e6998f1055f9c98d52a2449bef`  
		Last Modified: Wed, 29 Mar 2023 22:12:04 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.1.1` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:d88708954f3766d18f2aa86efa96c599507d7ea47f82d524548fc8c35875b6c5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.7 MB (73704060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9479f123cf5449eed5a7ad7a3493ef51469e5a73179ab97fdc21294abb3d9f86`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:15:30 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 30 Mar 2023 04:15:30 GMT
ARG KONG_VERSION=3.1.1
# Thu, 30 Mar 2023 04:15:31 GMT
ENV KONG_VERSION=3.1.1
# Thu, 30 Mar 2023 04:15:31 GMT
ARG KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c
# Thu, 30 Mar 2023 04:15:31 GMT
ARG KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
# Thu, 30 Mar 2023 04:15:31 GMT
ARG ASSET=remote
# Thu, 30 Mar 2023 04:15:31 GMT
ARG EE_PORTS
# Thu, 30 Mar 2023 04:15:31 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Thu, 30 Mar 2023 04:15:36 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Thu, 30 Mar 2023 04:15:37 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 30 Mar 2023 04:15:37 GMT
USER kong
# Thu, 30 Mar 2023 04:15:37 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Mar 2023 04:15:38 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 30 Mar 2023 04:15:38 GMT
STOPSIGNAL SIGQUIT
# Thu, 30 Mar 2023 04:15:38 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 30 Mar 2023 04:15:38 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:547446be3368f442c50ff95e2a2a9c85110b6b41bbb3c75b7e5ebb115f478b57`  
		Last Modified: Wed, 29 Mar 2023 17:39:56 GMT  
		Size: 2.7 MB (2709344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f137c449ccbb530641e2cca76ab47da104148e987af90da334338ae8a75ee8d`  
		Last Modified: Thu, 30 Mar 2023 04:16:16 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa5ed9b55ad6f487ac77eb1ca65c204eaa1ff7c700229ffca32bf6d1e98e301`  
		Last Modified: Thu, 30 Mar 2023 04:16:23 GMT  
		Size: 71.0 MB (70993698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe163fe5badbb78866e8b29e88f7b2048cef5a67951386386625642b34e417f1`  
		Last Modified: Thu, 30 Mar 2023 04:16:16 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.1.1-alpine`

```console
$ docker pull kong@sha256:95de25fe58f6fe96e63b129a6963a3ce60e03d670100dc82103f2ce362a60db7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.1.1-alpine` - linux; amd64

```console
$ docker pull kong@sha256:fe077a1e32c364576237a33b1916e625416a60630cc20578f20d1e5a5df376f0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75688407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b815af25ca31f8d87d21059367ff86ef810fc8761eb1e73196ff92c438fc8dbe`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:11:00 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 29 Mar 2023 22:11:00 GMT
ARG KONG_VERSION=3.1.1
# Wed, 29 Mar 2023 22:11:00 GMT
ENV KONG_VERSION=3.1.1
# Wed, 29 Mar 2023 22:11:00 GMT
ARG KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c
# Wed, 29 Mar 2023 22:11:00 GMT
ARG KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
# Wed, 29 Mar 2023 22:11:00 GMT
ARG ASSET=remote
# Wed, 29 Mar 2023 22:11:00 GMT
ARG EE_PORTS
# Wed, 29 Mar 2023 22:11:00 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Wed, 29 Mar 2023 22:11:07 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Wed, 29 Mar 2023 22:11:08 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Wed, 29 Mar 2023 22:11:08 GMT
USER kong
# Wed, 29 Mar 2023 22:11:08 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 29 Mar 2023 22:11:08 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 29 Mar 2023 22:11:08 GMT
STOPSIGNAL SIGQUIT
# Wed, 29 Mar 2023 22:11:08 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Wed, 29 Mar 2023 22:11:08 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:91d30c5bc19582de1415b18f1ec5bcbf52a558b62cf6cc201c9669df9f748c22`  
		Last Modified: Wed, 29 Mar 2023 18:20:09 GMT  
		Size: 2.8 MB (2807803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d355939d3033d764ca6ac536976f4e0ef35234a8139659930ed75004b7ac3b`  
		Last Modified: Wed, 29 Mar 2023 22:12:04 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e2d991ca57d6678cd5b80335d6cd62bcda57cda9ad09f4356fc3f54974664a`  
		Last Modified: Wed, 29 Mar 2023 22:12:11 GMT  
		Size: 72.9 MB (72879589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40141fb6acdb9e60f527a720a3bee407e6cc53e6998f1055f9c98d52a2449bef`  
		Last Modified: Wed, 29 Mar 2023 22:12:04 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.1.1-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:d88708954f3766d18f2aa86efa96c599507d7ea47f82d524548fc8c35875b6c5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.7 MB (73704060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9479f123cf5449eed5a7ad7a3493ef51469e5a73179ab97fdc21294abb3d9f86`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:15:30 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 30 Mar 2023 04:15:30 GMT
ARG KONG_VERSION=3.1.1
# Thu, 30 Mar 2023 04:15:31 GMT
ENV KONG_VERSION=3.1.1
# Thu, 30 Mar 2023 04:15:31 GMT
ARG KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c
# Thu, 30 Mar 2023 04:15:31 GMT
ARG KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
# Thu, 30 Mar 2023 04:15:31 GMT
ARG ASSET=remote
# Thu, 30 Mar 2023 04:15:31 GMT
ARG EE_PORTS
# Thu, 30 Mar 2023 04:15:31 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Thu, 30 Mar 2023 04:15:36 GMT
# ARGS: ASSET=remote KONG_AMD64_SHA=9194977814e91b6997ce4795957d9b4bcec9d220667e01a08ade7ac64704f57c KONG_ARM64_SHA=92d98307a3193602bbe4dbed2d099cde5404a8acd09d53f0b9a9f2bcf6038500
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) export ARCH='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) export ARCH='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc pcre perl tzdata libcap zlib zlib-dev bash     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Thu, 30 Mar 2023 04:15:37 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Thu, 30 Mar 2023 04:15:37 GMT
USER kong
# Thu, 30 Mar 2023 04:15:37 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Mar 2023 04:15:38 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 30 Mar 2023 04:15:38 GMT
STOPSIGNAL SIGQUIT
# Thu, 30 Mar 2023 04:15:38 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 30 Mar 2023 04:15:38 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:547446be3368f442c50ff95e2a2a9c85110b6b41bbb3c75b7e5ebb115f478b57`  
		Last Modified: Wed, 29 Mar 2023 17:39:56 GMT  
		Size: 2.7 MB (2709344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f137c449ccbb530641e2cca76ab47da104148e987af90da334338ae8a75ee8d`  
		Last Modified: Thu, 30 Mar 2023 04:16:16 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa5ed9b55ad6f487ac77eb1ca65c204eaa1ff7c700229ffca32bf6d1e98e301`  
		Last Modified: Thu, 30 Mar 2023 04:16:23 GMT  
		Size: 71.0 MB (70993698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe163fe5badbb78866e8b29e88f7b2048cef5a67951386386625642b34e417f1`  
		Last Modified: Thu, 30 Mar 2023 04:16:16 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.1.1-ubuntu`

```console
$ docker pull kong@sha256:3bde6e63802d1c6799673d86602bc18a0ad7df02a928a980163360699b9283a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.1.1-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:fb7def9d63b24dc4c240b345e7e9355337786d632661945e06a15ef20e4779a1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.7 MB (101731018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5498f3ffdb5118b22860bb4093d18caa5b3149307152c58abc431e05d8685579`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 13 Apr 2023 13:05:13 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:05:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:05:13 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:05:15 GMT
ADD file:d05d1c0936b046937bd5755876db2f8da3ed8ccbcf464bb56c312fbc7ed78589 in / 
# Thu, 13 Apr 2023 13:05:15 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 00:48:57 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Tue, 18 Apr 2023 00:48:57 GMT
ARG ASSET=ce
# Tue, 18 Apr 2023 00:48:57 GMT
ENV ASSET=ce
# Tue, 18 Apr 2023 00:48:57 GMT
ARG EE_PORTS
# Tue, 18 Apr 2023 00:48:57 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Tue, 18 Apr 2023 00:48:57 GMT
ARG KONG_VERSION=3.1.1
# Tue, 18 Apr 2023 00:48:57 GMT
ENV KONG_VERSION=3.1.1
# Tue, 18 Apr 2023 00:48:57 GMT
ARG KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b
# Tue, 18 Apr 2023 00:48:57 GMT
ARG KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
# Tue, 18 Apr 2023 00:49:26 GMT
# ARGS: KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 18 Apr 2023 00:49:26 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 18 Apr 2023 00:49:26 GMT
USER kong
# Tue, 18 Apr 2023 00:49:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 18 Apr 2023 00:49:26 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 18 Apr 2023 00:49:27 GMT
STOPSIGNAL SIGQUIT
# Tue, 18 Apr 2023 00:49:27 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 18 Apr 2023 00:49:27 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:99803d4b97f3db529ae9ca4174b0951afac6b309e7deaa8ec3214c584e02b3a8`  
		Last Modified: Thu, 13 Apr 2023 03:03:13 GMT  
		Size: 28.6 MB (28578563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1270117cfa3f1bf43891c96ffc5e3f48c9b1b960b8f1c17ad7d5cbb6971f0fbd`  
		Last Modified: Tue, 18 Apr 2023 00:50:16 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bccee49244e3687399c9c24cc0ce516b0905e7442ed02f0fe26a5a84f5538a7b`  
		Last Modified: Tue, 18 Apr 2023 00:50:28 GMT  
		Size: 73.2 MB (73151444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53853e3583dd41f1e3da5406c276e344418ddaae1e4dbe056f2e4e205734273e`  
		Last Modified: Tue, 18 Apr 2023 00:50:16 GMT  
		Size: 882.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.1.1-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:c5b08a0c6e5170deba532287fe325be7b87ecb0c4710b857c519ae68507091ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.0 MB (98969390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85eab6242a1c3c38ed07152b648ebef2d657a39b9699ea9fb23dd60a94dc1a78`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 13 Apr 2023 13:09:50 GMT
ARG RELEASE
# Thu, 13 Apr 2023 13:09:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 13 Apr 2023 13:09:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 13 Apr 2023 13:09:51 GMT
LABEL org.opencontainers.image.version=20.04
# Thu, 13 Apr 2023 13:09:59 GMT
ADD file:0150fa02321f8be160e90ff64583d263fe651b5d418ab65f05ba604449ab47c6 in / 
# Thu, 13 Apr 2023 13:10:00 GMT
CMD ["/bin/bash"]
# Tue, 18 Apr 2023 01:55:38 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Tue, 18 Apr 2023 01:55:38 GMT
ARG ASSET=ce
# Tue, 18 Apr 2023 01:55:38 GMT
ENV ASSET=ce
# Tue, 18 Apr 2023 01:55:38 GMT
ARG EE_PORTS
# Tue, 18 Apr 2023 01:55:38 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Tue, 18 Apr 2023 01:55:39 GMT
ARG KONG_VERSION=3.1.1
# Tue, 18 Apr 2023 01:55:39 GMT
ENV KONG_VERSION=3.1.1
# Tue, 18 Apr 2023 01:55:39 GMT
ARG KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b
# Tue, 18 Apr 2023 01:55:39 GMT
ARG KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
# Tue, 18 Apr 2023 01:55:55 GMT
# ARGS: KONG_AMD64_SHA=39bbefa14d348dedf7734c742da46acf7777ff0018f2cad7961799ba4663277b KONG_ARM64_SHA=66c88430fb641ace356af55db4377a697a5ee5a63fbb243bcc8a4a90e3874f9f
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Tue, 18 Apr 2023 01:55:56 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 18 Apr 2023 01:55:56 GMT
USER kong
# Tue, 18 Apr 2023 01:55:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 18 Apr 2023 01:55:57 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 18 Apr 2023 01:55:57 GMT
STOPSIGNAL SIGQUIT
# Tue, 18 Apr 2023 01:55:57 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 18 Apr 2023 01:55:57 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:2378679266ac5157323158b6e52e7a884e559db5217037e57992e47a1667d525`  
		Last Modified: Fri, 14 Apr 2023 07:39:20 GMT  
		Size: 27.2 MB (27196396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33117919705427cc2b91c73428239666db66c5521aad5bb7169b1d6fc9d0b5dc`  
		Last Modified: Tue, 18 Apr 2023 01:56:41 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dd8eef4dc95b72b5204ea83b481f2af54e5c5c4cf27232918bfcccd5cafd2c5`  
		Last Modified: Tue, 18 Apr 2023 01:56:50 GMT  
		Size: 71.8 MB (71771988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83592683ff2a59bc4dc1fb9e4c1df9fcd9e9cf7c783c57043f79f67657a7daab`  
		Last Modified: Tue, 18 Apr 2023 01:56:41 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.2`

```console
$ docker pull kong@sha256:73513cfe5921762fbb2a8fcf5436dfed69d207224c10a15115f67da3807b3ea9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.2` - linux; amd64

```console
$ docker pull kong@sha256:71cdbcbcf156077528e0ebb698a44670ccb33f846d6927e27f0ea3e8ff31ba2c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.5 MB (74451841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fa2e7c7b0b42a300c9c9f3194f853c86749f987f7e7003d32bd0226889b0b88`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 07:49:24 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 04 May 2023 07:49:24 GMT
ARG ASSET=ce
# Thu, 04 May 2023 07:49:24 GMT
ENV ASSET=ce
# Thu, 04 May 2023 07:49:24 GMT
ARG EE_PORTS
# Thu, 04 May 2023 07:49:24 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Thu, 04 May 2023 07:49:24 GMT
ARG KONG_VERSION=3.2.2
# Thu, 04 May 2023 07:49:24 GMT
ENV KONG_VERSION=3.2.2
# Thu, 04 May 2023 07:49:24 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Thu, 04 May 2023 07:49:24 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Thu, 04 May 2023 07:49:53 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Thu, 04 May 2023 07:49:54 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Thu, 04 May 2023 07:49:54 GMT
USER kong
# Thu, 04 May 2023 07:49:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 04 May 2023 07:49:54 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 04 May 2023 07:49:54 GMT
STOPSIGNAL SIGQUIT
# Thu, 04 May 2023 07:49:54 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 04 May 2023 07:49:54 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4452e2a99e08079eada765eaec98220af45483cd8a0e7809ca19f969da460e32`  
		Last Modified: Thu, 04 May 2023 07:50:22 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d9a6e2b2b5f047a029e37c75236c24d4929d3b90f9f1540d69889bbabbe8d2`  
		Last Modified: Thu, 04 May 2023 07:50:29 GMT  
		Size: 44.0 MB (44020342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eccf8a96cc3972523193277dfcc6d7d0125e72e86cb9177b2479637c54be8f6e`  
		Last Modified: Thu, 04 May 2023 07:50:22 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.2` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:331455622bce663694cf274fa5acc68a84bea80ecbe4b4b7403ec54eab362d3f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.6 MB (78563017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53cb403e2e2a3e8ccb433f50a8ae3f79029e5ae441e50157c90bc9fca8c52cfc`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 03:44:59 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 04 May 2023 03:44:59 GMT
ARG ASSET=ce
# Thu, 04 May 2023 03:44:59 GMT
ENV ASSET=ce
# Thu, 04 May 2023 03:44:59 GMT
ARG EE_PORTS
# Thu, 04 May 2023 03:44:59 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Thu, 04 May 2023 03:44:59 GMT
ARG KONG_VERSION=3.2.2
# Thu, 04 May 2023 03:44:59 GMT
ENV KONG_VERSION=3.2.2
# Thu, 04 May 2023 03:44:59 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Thu, 04 May 2023 03:44:59 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Thu, 04 May 2023 03:45:16 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Thu, 04 May 2023 03:45:17 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Thu, 04 May 2023 03:45:17 GMT
USER kong
# Thu, 04 May 2023 03:45:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 04 May 2023 03:45:17 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 04 May 2023 03:45:17 GMT
STOPSIGNAL SIGQUIT
# Thu, 04 May 2023 03:45:17 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 04 May 2023 03:45:17 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aead6b4c2aa9f393a63e92067a6a16c0f1527ee558eda6b45181f820bcf1f61`  
		Last Modified: Thu, 04 May 2023 03:45:39 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e562bf9fba3e3ac55944fd6b19bac4ffac0d4bee31828b1d3cdca127298dca6`  
		Last Modified: Thu, 04 May 2023 03:45:45 GMT  
		Size: 50.2 MB (50172295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b47e7a18f6ca88337071e2830f034ea6b85f3b0a4d3d980a63b3c7d5309394`  
		Last Modified: Thu, 04 May 2023 03:45:39 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.2-ubuntu`

```console
$ docker pull kong@sha256:73513cfe5921762fbb2a8fcf5436dfed69d207224c10a15115f67da3807b3ea9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.2-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:71cdbcbcf156077528e0ebb698a44670ccb33f846d6927e27f0ea3e8ff31ba2c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.5 MB (74451841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fa2e7c7b0b42a300c9c9f3194f853c86749f987f7e7003d32bd0226889b0b88`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 07:49:24 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 04 May 2023 07:49:24 GMT
ARG ASSET=ce
# Thu, 04 May 2023 07:49:24 GMT
ENV ASSET=ce
# Thu, 04 May 2023 07:49:24 GMT
ARG EE_PORTS
# Thu, 04 May 2023 07:49:24 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Thu, 04 May 2023 07:49:24 GMT
ARG KONG_VERSION=3.2.2
# Thu, 04 May 2023 07:49:24 GMT
ENV KONG_VERSION=3.2.2
# Thu, 04 May 2023 07:49:24 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Thu, 04 May 2023 07:49:24 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Thu, 04 May 2023 07:49:53 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Thu, 04 May 2023 07:49:54 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Thu, 04 May 2023 07:49:54 GMT
USER kong
# Thu, 04 May 2023 07:49:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 04 May 2023 07:49:54 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 04 May 2023 07:49:54 GMT
STOPSIGNAL SIGQUIT
# Thu, 04 May 2023 07:49:54 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 04 May 2023 07:49:54 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4452e2a99e08079eada765eaec98220af45483cd8a0e7809ca19f969da460e32`  
		Last Modified: Thu, 04 May 2023 07:50:22 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d9a6e2b2b5f047a029e37c75236c24d4929d3b90f9f1540d69889bbabbe8d2`  
		Last Modified: Thu, 04 May 2023 07:50:29 GMT  
		Size: 44.0 MB (44020342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eccf8a96cc3972523193277dfcc6d7d0125e72e86cb9177b2479637c54be8f6e`  
		Last Modified: Thu, 04 May 2023 07:50:22 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.2-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:331455622bce663694cf274fa5acc68a84bea80ecbe4b4b7403ec54eab362d3f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.6 MB (78563017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53cb403e2e2a3e8ccb433f50a8ae3f79029e5ae441e50157c90bc9fca8c52cfc`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 03:44:59 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 04 May 2023 03:44:59 GMT
ARG ASSET=ce
# Thu, 04 May 2023 03:44:59 GMT
ENV ASSET=ce
# Thu, 04 May 2023 03:44:59 GMT
ARG EE_PORTS
# Thu, 04 May 2023 03:44:59 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Thu, 04 May 2023 03:44:59 GMT
ARG KONG_VERSION=3.2.2
# Thu, 04 May 2023 03:44:59 GMT
ENV KONG_VERSION=3.2.2
# Thu, 04 May 2023 03:44:59 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Thu, 04 May 2023 03:44:59 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Thu, 04 May 2023 03:45:16 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Thu, 04 May 2023 03:45:17 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Thu, 04 May 2023 03:45:17 GMT
USER kong
# Thu, 04 May 2023 03:45:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 04 May 2023 03:45:17 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 04 May 2023 03:45:17 GMT
STOPSIGNAL SIGQUIT
# Thu, 04 May 2023 03:45:17 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 04 May 2023 03:45:17 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aead6b4c2aa9f393a63e92067a6a16c0f1527ee558eda6b45181f820bcf1f61`  
		Last Modified: Thu, 04 May 2023 03:45:39 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e562bf9fba3e3ac55944fd6b19bac4ffac0d4bee31828b1d3cdca127298dca6`  
		Last Modified: Thu, 04 May 2023 03:45:45 GMT  
		Size: 50.2 MB (50172295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b47e7a18f6ca88337071e2830f034ea6b85f3b0a4d3d980a63b3c7d5309394`  
		Last Modified: Thu, 04 May 2023 03:45:39 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.2.2`

```console
$ docker pull kong@sha256:73513cfe5921762fbb2a8fcf5436dfed69d207224c10a15115f67da3807b3ea9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.2.2` - linux; amd64

```console
$ docker pull kong@sha256:71cdbcbcf156077528e0ebb698a44670ccb33f846d6927e27f0ea3e8ff31ba2c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.5 MB (74451841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fa2e7c7b0b42a300c9c9f3194f853c86749f987f7e7003d32bd0226889b0b88`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 07:49:24 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 04 May 2023 07:49:24 GMT
ARG ASSET=ce
# Thu, 04 May 2023 07:49:24 GMT
ENV ASSET=ce
# Thu, 04 May 2023 07:49:24 GMT
ARG EE_PORTS
# Thu, 04 May 2023 07:49:24 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Thu, 04 May 2023 07:49:24 GMT
ARG KONG_VERSION=3.2.2
# Thu, 04 May 2023 07:49:24 GMT
ENV KONG_VERSION=3.2.2
# Thu, 04 May 2023 07:49:24 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Thu, 04 May 2023 07:49:24 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Thu, 04 May 2023 07:49:53 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Thu, 04 May 2023 07:49:54 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Thu, 04 May 2023 07:49:54 GMT
USER kong
# Thu, 04 May 2023 07:49:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 04 May 2023 07:49:54 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 04 May 2023 07:49:54 GMT
STOPSIGNAL SIGQUIT
# Thu, 04 May 2023 07:49:54 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 04 May 2023 07:49:54 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4452e2a99e08079eada765eaec98220af45483cd8a0e7809ca19f969da460e32`  
		Last Modified: Thu, 04 May 2023 07:50:22 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d9a6e2b2b5f047a029e37c75236c24d4929d3b90f9f1540d69889bbabbe8d2`  
		Last Modified: Thu, 04 May 2023 07:50:29 GMT  
		Size: 44.0 MB (44020342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eccf8a96cc3972523193277dfcc6d7d0125e72e86cb9177b2479637c54be8f6e`  
		Last Modified: Thu, 04 May 2023 07:50:22 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.2.2` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:331455622bce663694cf274fa5acc68a84bea80ecbe4b4b7403ec54eab362d3f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.6 MB (78563017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53cb403e2e2a3e8ccb433f50a8ae3f79029e5ae441e50157c90bc9fca8c52cfc`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 03:44:59 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 04 May 2023 03:44:59 GMT
ARG ASSET=ce
# Thu, 04 May 2023 03:44:59 GMT
ENV ASSET=ce
# Thu, 04 May 2023 03:44:59 GMT
ARG EE_PORTS
# Thu, 04 May 2023 03:44:59 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Thu, 04 May 2023 03:44:59 GMT
ARG KONG_VERSION=3.2.2
# Thu, 04 May 2023 03:44:59 GMT
ENV KONG_VERSION=3.2.2
# Thu, 04 May 2023 03:44:59 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Thu, 04 May 2023 03:44:59 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Thu, 04 May 2023 03:45:16 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Thu, 04 May 2023 03:45:17 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Thu, 04 May 2023 03:45:17 GMT
USER kong
# Thu, 04 May 2023 03:45:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 04 May 2023 03:45:17 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 04 May 2023 03:45:17 GMT
STOPSIGNAL SIGQUIT
# Thu, 04 May 2023 03:45:17 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 04 May 2023 03:45:17 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aead6b4c2aa9f393a63e92067a6a16c0f1527ee558eda6b45181f820bcf1f61`  
		Last Modified: Thu, 04 May 2023 03:45:39 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e562bf9fba3e3ac55944fd6b19bac4ffac0d4bee31828b1d3cdca127298dca6`  
		Last Modified: Thu, 04 May 2023 03:45:45 GMT  
		Size: 50.2 MB (50172295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b47e7a18f6ca88337071e2830f034ea6b85f3b0a4d3d980a63b3c7d5309394`  
		Last Modified: Thu, 04 May 2023 03:45:39 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.2.2-alpine`

```console
$ docker pull kong@sha256:11a7cf58a2cef55d1bf55bff33e5e307813f38f49ac0cee8360e3150770938a7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:3.2.2-alpine` - linux; amd64

```console
$ docker pull kong@sha256:610b26c277d63aa272b4348c2d645ba4573cd44210908eee3c85d0a7412b9778
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.9 MB (36925990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08bd9111271e321bd67d7ed15615b17c1a8494738470fa1dfe710a8a72ac539e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:10:49 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 29 Mar 2023 22:10:49 GMT
ARG KONG_VERSION=3.2.2
# Wed, 29 Mar 2023 22:10:49 GMT
ENV KONG_VERSION=3.2.2
# Wed, 29 Mar 2023 22:10:49 GMT
ARG KONG_SHA256=a07c3bc0307e2d8fe33acb8be5fe659f348279540eaa267bc6968005094835ef
# Wed, 29 Mar 2023 22:10:49 GMT
ARG KONG_PREFIX=/usr/local/kong
# Wed, 29 Mar 2023 22:10:49 GMT
ENV KONG_PREFIX=/usr/local/kong
# Wed, 29 Mar 2023 22:10:49 GMT
ARG ASSET=remote
# Wed, 29 Mar 2023 22:10:49 GMT
ARG EE_PORTS
# Wed, 29 Mar 2023 22:10:49 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Wed, 29 Mar 2023 22:10:55 GMT
# ARGS: ASSET=remote KONG_SHA256=a07c3bc0307e2d8fe33acb8be5fe659f348279540eaa267bc6968005094835ef
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     export ARCH='amd64';     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc perl tzdata libcap zlib zlib-dev bash yaml     && adduser -S kong     && addgroup -S kong     && mkdir -p "${KONG_PREFIX}"     && chown -R kong:0 ${KONG_PREFIX}     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u ${KONG_PREFIX}     && rm -rf /tmp/kong.apk.tar.gz     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Wed, 29 Mar 2023 22:10:55 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Wed, 29 Mar 2023 22:10:56 GMT
USER kong
# Wed, 29 Mar 2023 22:10:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 29 Mar 2023 22:10:56 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 29 Mar 2023 22:10:56 GMT
STOPSIGNAL SIGQUIT
# Wed, 29 Mar 2023 22:10:56 GMT
HEALTHCHECK &{["CMD-SHELL" "kong-health"] "1m0s" "10s" "0s" '\n'}
# Wed, 29 Mar 2023 22:10:56 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a18dd47ec6d14a9b3605e54f37ef954db1178374b29996f454b6dd8de91971e`  
		Last Modified: Wed, 29 Mar 2023 22:11:49 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988eb756b3dec47b267d400daaf4af0aecb7341be2520a7ef139be46a0265271`  
		Last Modified: Wed, 29 Mar 2023 22:11:54 GMT  
		Size: 33.6 MB (33550136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a00c5ea7f469c01cfba5cfb61429c6431267a4475a1798cca3cd838bde6b48`  
		Last Modified: Wed, 29 Mar 2023 22:11:49 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:3.2.2-ubuntu`

```console
$ docker pull kong@sha256:73513cfe5921762fbb2a8fcf5436dfed69d207224c10a15115f67da3807b3ea9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:3.2.2-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:71cdbcbcf156077528e0ebb698a44670ccb33f846d6927e27f0ea3e8ff31ba2c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.5 MB (74451841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fa2e7c7b0b42a300c9c9f3194f853c86749f987f7e7003d32bd0226889b0b88`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 07:49:24 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 04 May 2023 07:49:24 GMT
ARG ASSET=ce
# Thu, 04 May 2023 07:49:24 GMT
ENV ASSET=ce
# Thu, 04 May 2023 07:49:24 GMT
ARG EE_PORTS
# Thu, 04 May 2023 07:49:24 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Thu, 04 May 2023 07:49:24 GMT
ARG KONG_VERSION=3.2.2
# Thu, 04 May 2023 07:49:24 GMT
ENV KONG_VERSION=3.2.2
# Thu, 04 May 2023 07:49:24 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Thu, 04 May 2023 07:49:24 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Thu, 04 May 2023 07:49:53 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Thu, 04 May 2023 07:49:54 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Thu, 04 May 2023 07:49:54 GMT
USER kong
# Thu, 04 May 2023 07:49:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 04 May 2023 07:49:54 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 04 May 2023 07:49:54 GMT
STOPSIGNAL SIGQUIT
# Thu, 04 May 2023 07:49:54 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 04 May 2023 07:49:54 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4452e2a99e08079eada765eaec98220af45483cd8a0e7809ca19f969da460e32`  
		Last Modified: Thu, 04 May 2023 07:50:22 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d9a6e2b2b5f047a029e37c75236c24d4929d3b90f9f1540d69889bbabbe8d2`  
		Last Modified: Thu, 04 May 2023 07:50:29 GMT  
		Size: 44.0 MB (44020342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eccf8a96cc3972523193277dfcc6d7d0125e72e86cb9177b2479637c54be8f6e`  
		Last Modified: Thu, 04 May 2023 07:50:22 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:3.2.2-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:331455622bce663694cf274fa5acc68a84bea80ecbe4b4b7403ec54eab362d3f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.6 MB (78563017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53cb403e2e2a3e8ccb433f50a8ae3f79029e5ae441e50157c90bc9fca8c52cfc`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 03:44:59 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 04 May 2023 03:44:59 GMT
ARG ASSET=ce
# Thu, 04 May 2023 03:44:59 GMT
ENV ASSET=ce
# Thu, 04 May 2023 03:44:59 GMT
ARG EE_PORTS
# Thu, 04 May 2023 03:44:59 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Thu, 04 May 2023 03:44:59 GMT
ARG KONG_VERSION=3.2.2
# Thu, 04 May 2023 03:44:59 GMT
ENV KONG_VERSION=3.2.2
# Thu, 04 May 2023 03:44:59 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Thu, 04 May 2023 03:44:59 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Thu, 04 May 2023 03:45:16 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Thu, 04 May 2023 03:45:17 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Thu, 04 May 2023 03:45:17 GMT
USER kong
# Thu, 04 May 2023 03:45:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 04 May 2023 03:45:17 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 04 May 2023 03:45:17 GMT
STOPSIGNAL SIGQUIT
# Thu, 04 May 2023 03:45:17 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 04 May 2023 03:45:17 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aead6b4c2aa9f393a63e92067a6a16c0f1527ee558eda6b45181f820bcf1f61`  
		Last Modified: Thu, 04 May 2023 03:45:39 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e562bf9fba3e3ac55944fd6b19bac4ffac0d4bee31828b1d3cdca127298dca6`  
		Last Modified: Thu, 04 May 2023 03:45:45 GMT  
		Size: 50.2 MB (50172295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b47e7a18f6ca88337071e2830f034ea6b85f3b0a4d3d980a63b3c7d5309394`  
		Last Modified: Thu, 04 May 2023 03:45:39 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:alpine`

```console
$ docker pull kong@sha256:11a7cf58a2cef55d1bf55bff33e5e307813f38f49ac0cee8360e3150770938a7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:alpine` - linux; amd64

```console
$ docker pull kong@sha256:610b26c277d63aa272b4348c2d645ba4573cd44210908eee3c85d0a7412b9778
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.9 MB (36925990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08bd9111271e321bd67d7ed15615b17c1a8494738470fa1dfe710a8a72ac539e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:10:49 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Wed, 29 Mar 2023 22:10:49 GMT
ARG KONG_VERSION=3.2.2
# Wed, 29 Mar 2023 22:10:49 GMT
ENV KONG_VERSION=3.2.2
# Wed, 29 Mar 2023 22:10:49 GMT
ARG KONG_SHA256=a07c3bc0307e2d8fe33acb8be5fe659f348279540eaa267bc6968005094835ef
# Wed, 29 Mar 2023 22:10:49 GMT
ARG KONG_PREFIX=/usr/local/kong
# Wed, 29 Mar 2023 22:10:49 GMT
ENV KONG_PREFIX=/usr/local/kong
# Wed, 29 Mar 2023 22:10:49 GMT
ARG ASSET=remote
# Wed, 29 Mar 2023 22:10:49 GMT
ARG EE_PORTS
# Wed, 29 Mar 2023 22:10:49 GMT
COPY file:7815b5fca0a34ed4a30931ccd9d4786733aecc9e9b2d4c363dee07e4a5c9b32f in /tmp/kong.apk.tar.gz 
# Wed, 29 Mar 2023 22:10:55 GMT
# ARGS: ASSET=remote KONG_SHA256=a07c3bc0307e2d8fe33acb8be5fe659f348279540eaa267bc6968005094835ef
RUN set -ex;     apk add --virtual .build-deps curl tar gzip ca-certificates;     export ARCH='amd64';     if [ "$ASSET" = "remote" ] ; then       curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-${KONG_VERSION}.${ARCH}.apk.tar.gz" -o /tmp/kong.apk.tar.gz       && echo "$KONG_SHA256  /tmp/kong.apk.tar.gz" | sha256sum -c -;     fi     && tar -C / -xzf /tmp/kong.apk.tar.gz     && apk add --no-cache libstdc++ libgcc perl tzdata libcap zlib zlib-dev bash yaml     && adduser -S kong     && addgroup -S kong     && mkdir -p "${KONG_PREFIX}"     && chown -R kong:0 ${KONG_PREFIX}     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u ${KONG_PREFIX}     && rm -rf /tmp/kong.apk.tar.gz     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && apk del .build-deps     && kong version
# Wed, 29 Mar 2023 22:10:55 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Wed, 29 Mar 2023 22:10:56 GMT
USER kong
# Wed, 29 Mar 2023 22:10:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 29 Mar 2023 22:10:56 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 29 Mar 2023 22:10:56 GMT
STOPSIGNAL SIGQUIT
# Wed, 29 Mar 2023 22:10:56 GMT
HEALTHCHECK &{["CMD-SHELL" "kong-health"] "1m0s" "10s" "0s" '\n'}
# Wed, 29 Mar 2023 22:10:56 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a18dd47ec6d14a9b3605e54f37ef954db1178374b29996f454b6dd8de91971e`  
		Last Modified: Wed, 29 Mar 2023 22:11:49 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988eb756b3dec47b267d400daaf4af0aecb7341be2520a7ef139be46a0265271`  
		Last Modified: Wed, 29 Mar 2023 22:11:54 GMT  
		Size: 33.6 MB (33550136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a00c5ea7f469c01cfba5cfb61429c6431267a4475a1798cca3cd838bde6b48`  
		Last Modified: Wed, 29 Mar 2023 22:11:49 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:latest`

```console
$ docker pull kong@sha256:73513cfe5921762fbb2a8fcf5436dfed69d207224c10a15115f67da3807b3ea9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:latest` - linux; amd64

```console
$ docker pull kong@sha256:71cdbcbcf156077528e0ebb698a44670ccb33f846d6927e27f0ea3e8ff31ba2c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.5 MB (74451841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fa2e7c7b0b42a300c9c9f3194f853c86749f987f7e7003d32bd0226889b0b88`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 07:49:24 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 04 May 2023 07:49:24 GMT
ARG ASSET=ce
# Thu, 04 May 2023 07:49:24 GMT
ENV ASSET=ce
# Thu, 04 May 2023 07:49:24 GMT
ARG EE_PORTS
# Thu, 04 May 2023 07:49:24 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Thu, 04 May 2023 07:49:24 GMT
ARG KONG_VERSION=3.2.2
# Thu, 04 May 2023 07:49:24 GMT
ENV KONG_VERSION=3.2.2
# Thu, 04 May 2023 07:49:24 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Thu, 04 May 2023 07:49:24 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Thu, 04 May 2023 07:49:53 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Thu, 04 May 2023 07:49:54 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Thu, 04 May 2023 07:49:54 GMT
USER kong
# Thu, 04 May 2023 07:49:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 04 May 2023 07:49:54 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 04 May 2023 07:49:54 GMT
STOPSIGNAL SIGQUIT
# Thu, 04 May 2023 07:49:54 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 04 May 2023 07:49:54 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4452e2a99e08079eada765eaec98220af45483cd8a0e7809ca19f969da460e32`  
		Last Modified: Thu, 04 May 2023 07:50:22 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d9a6e2b2b5f047a029e37c75236c24d4929d3b90f9f1540d69889bbabbe8d2`  
		Last Modified: Thu, 04 May 2023 07:50:29 GMT  
		Size: 44.0 MB (44020342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eccf8a96cc3972523193277dfcc6d7d0125e72e86cb9177b2479637c54be8f6e`  
		Last Modified: Thu, 04 May 2023 07:50:22 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:latest` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:331455622bce663694cf274fa5acc68a84bea80ecbe4b4b7403ec54eab362d3f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.6 MB (78563017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53cb403e2e2a3e8ccb433f50a8ae3f79029e5ae441e50157c90bc9fca8c52cfc`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 03:44:59 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 04 May 2023 03:44:59 GMT
ARG ASSET=ce
# Thu, 04 May 2023 03:44:59 GMT
ENV ASSET=ce
# Thu, 04 May 2023 03:44:59 GMT
ARG EE_PORTS
# Thu, 04 May 2023 03:44:59 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Thu, 04 May 2023 03:44:59 GMT
ARG KONG_VERSION=3.2.2
# Thu, 04 May 2023 03:44:59 GMT
ENV KONG_VERSION=3.2.2
# Thu, 04 May 2023 03:44:59 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Thu, 04 May 2023 03:44:59 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Thu, 04 May 2023 03:45:16 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Thu, 04 May 2023 03:45:17 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Thu, 04 May 2023 03:45:17 GMT
USER kong
# Thu, 04 May 2023 03:45:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 04 May 2023 03:45:17 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 04 May 2023 03:45:17 GMT
STOPSIGNAL SIGQUIT
# Thu, 04 May 2023 03:45:17 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 04 May 2023 03:45:17 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aead6b4c2aa9f393a63e92067a6a16c0f1527ee558eda6b45181f820bcf1f61`  
		Last Modified: Thu, 04 May 2023 03:45:39 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e562bf9fba3e3ac55944fd6b19bac4ffac0d4bee31828b1d3cdca127298dca6`  
		Last Modified: Thu, 04 May 2023 03:45:45 GMT  
		Size: 50.2 MB (50172295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b47e7a18f6ca88337071e2830f034ea6b85f3b0a4d3d980a63b3c7d5309394`  
		Last Modified: Thu, 04 May 2023 03:45:39 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:ubuntu`

```console
$ docker pull kong@sha256:73513cfe5921762fbb2a8fcf5436dfed69d207224c10a15115f67da3807b3ea9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:71cdbcbcf156077528e0ebb698a44670ccb33f846d6927e27f0ea3e8ff31ba2c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.5 MB (74451841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fa2e7c7b0b42a300c9c9f3194f853c86749f987f7e7003d32bd0226889b0b88`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 25 Apr 2023 17:30:47 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:30:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:30:47 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:30:49 GMT
ADD file:2fc6364d149eccc7f94ead482a0dcf24b0e44cc0d00ac6a2c1797776153e9608 in / 
# Tue, 25 Apr 2023 17:30:49 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 07:49:24 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 04 May 2023 07:49:24 GMT
ARG ASSET=ce
# Thu, 04 May 2023 07:49:24 GMT
ENV ASSET=ce
# Thu, 04 May 2023 07:49:24 GMT
ARG EE_PORTS
# Thu, 04 May 2023 07:49:24 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Thu, 04 May 2023 07:49:24 GMT
ARG KONG_VERSION=3.2.2
# Thu, 04 May 2023 07:49:24 GMT
ENV KONG_VERSION=3.2.2
# Thu, 04 May 2023 07:49:24 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Thu, 04 May 2023 07:49:24 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Thu, 04 May 2023 07:49:53 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Thu, 04 May 2023 07:49:54 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Thu, 04 May 2023 07:49:54 GMT
USER kong
# Thu, 04 May 2023 07:49:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 04 May 2023 07:49:54 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 04 May 2023 07:49:54 GMT
STOPSIGNAL SIGQUIT
# Thu, 04 May 2023 07:49:54 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 04 May 2023 07:49:54 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:1bc677758ad7fa4503417ae5be18809c5a8679b5b36fcd1464d5a8e41cb13305`  
		Last Modified: Tue, 25 Apr 2023 22:54:44 GMT  
		Size: 30.4 MB (30430220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4452e2a99e08079eada765eaec98220af45483cd8a0e7809ca19f969da460e32`  
		Last Modified: Thu, 04 May 2023 07:50:22 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d9a6e2b2b5f047a029e37c75236c24d4929d3b90f9f1540d69889bbabbe8d2`  
		Last Modified: Thu, 04 May 2023 07:50:29 GMT  
		Size: 44.0 MB (44020342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eccf8a96cc3972523193277dfcc6d7d0125e72e86cb9177b2479637c54be8f6e`  
		Last Modified: Thu, 04 May 2023 07:50:22 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:331455622bce663694cf274fa5acc68a84bea80ecbe4b4b7403ec54eab362d3f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.6 MB (78563017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53cb403e2e2a3e8ccb433f50a8ae3f79029e5ae441e50157c90bc9fca8c52cfc`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 25 Apr 2023 17:31:58 GMT
ARG RELEASE
# Tue, 25 Apr 2023 17:31:58 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 25 Apr 2023 17:31:58 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 25 Apr 2023 17:31:59 GMT
LABEL org.opencontainers.image.version=22.04
# Tue, 25 Apr 2023 17:32:02 GMT
ADD file:aee0d7770ef2f24dc9697e86d391529d001a4013b6e30a3ac90a57932814a57e in / 
# Tue, 25 Apr 2023 17:32:02 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 03:44:59 GMT
LABEL maintainer=Kong Docker Maintainers <docker@konghq.com> (@team-gateway-bot)
# Thu, 04 May 2023 03:44:59 GMT
ARG ASSET=ce
# Thu, 04 May 2023 03:44:59 GMT
ENV ASSET=ce
# Thu, 04 May 2023 03:44:59 GMT
ARG EE_PORTS
# Thu, 04 May 2023 03:44:59 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Thu, 04 May 2023 03:44:59 GMT
ARG KONG_VERSION=3.2.2
# Thu, 04 May 2023 03:44:59 GMT
ENV KONG_VERSION=3.2.2
# Thu, 04 May 2023 03:44:59 GMT
ARG KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540
# Thu, 04 May 2023 03:44:59 GMT
ARG KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
# Thu, 04 May 2023 03:45:16 GMT
# ARGS: KONG_AMD64_SHA=bfb905c69950386397e8a975358324ec3e2c8fd6dd0425e4a5c2a4c80add4540 KONG_ARM64_SHA=676335fefeb77eff168b27161678615575f3d573a62b19a5a86a5c8bba2c492a
RUN set -ex;     arch=$(dpkg --print-architecture);     case "${arch}" in       amd64) KONG_SHA256=$KONG_AMD64_SHA ;;       arm64) KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     apt-get update     && if [ "$ASSET" = "ce" ] ; then       apt-get install -y curl       && UBUNTU_CODENAME=$(cat /etc/os-release | grep UBUNTU_CODENAME | cut -d = -f 2)       && curl -fL https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-ubuntu-${UBUNTU_CODENAME}/pool/all/k/kong/kong_${KONG_VERSION}_$arch.deb -o /tmp/kong.deb       && apt-get purge -y curl       && echo "$KONG_SHA256  /tmp/kong.deb" | sha256sum -c -       || exit 1;     else       apt-get upgrade -y ;     fi;     apt-get install -y --no-install-recommends unzip git     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && ln -sf /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -sf /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -sf /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version ;     fi
# Thu, 04 May 2023 03:45:17 GMT
COPY file:6bb80898c17e8239746044c0d891f54029077cb7b848c170e71b40f6e2243e33 in /docker-entrypoint.sh 
# Thu, 04 May 2023 03:45:17 GMT
USER kong
# Thu, 04 May 2023 03:45:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 04 May 2023 03:45:17 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 04 May 2023 03:45:17 GMT
STOPSIGNAL SIGQUIT
# Thu, 04 May 2023 03:45:17 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Thu, 04 May 2023 03:45:17 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:f3f60f415e9a03eed88bd5dd5268c841cde08dacf16911a3ef1e4e0fcdd76568`  
		Last Modified: Wed, 26 Apr 2023 02:08:37 GMT  
		Size: 28.4 MB (28389440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aead6b4c2aa9f393a63e92067a6a16c0f1527ee558eda6b45181f820bcf1f61`  
		Last Modified: Thu, 04 May 2023 03:45:39 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e562bf9fba3e3ac55944fd6b19bac4ffac0d4bee31828b1d3cdca127298dca6`  
		Last Modified: Thu, 04 May 2023 03:45:45 GMT  
		Size: 50.2 MB (50172295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41b47e7a18f6ca88337071e2830f034ea6b85f3b0a4d3d980a63b3c7d5309394`  
		Last Modified: Thu, 04 May 2023 03:45:39 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
