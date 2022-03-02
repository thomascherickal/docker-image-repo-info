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
