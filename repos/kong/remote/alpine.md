## `kong:alpine`

```console
$ docker pull kong@sha256:7a33695e8c817dbc8776d5c8d0167457893d151b6c66f10ef52650d06db2334d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `kong:alpine` - linux; amd64

```console
$ docker pull kong@sha256:40d7a2eac255f47e1af9c30a5525230573aa9e120cf25cc6dcb7d6eb61cff38b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49536515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6ccc21c00cef6852bbf840402c7c92cd19d23882e66880b3c4b74fa7c48c6a7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Tue, 13 Jul 2021 21:20:05 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 13 Jul 2021 21:20:06 GMT
ARG ASSET=ce
# Tue, 13 Jul 2021 21:20:06 GMT
ENV ASSET=ce
# Tue, 13 Jul 2021 21:20:06 GMT
ARG EE_PORTS
# Tue, 13 Jul 2021 21:20:06 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 13 Jul 2021 21:20:06 GMT
ARG KONG_VERSION=2.5.0
# Tue, 13 Jul 2021 21:20:07 GMT
ENV KONG_VERSION=2.5.0
# Tue, 13 Jul 2021 21:20:07 GMT
ARG KONG_AMD64_SHA=ebe0cf3a3e71d202774ede5083c98e2ae39fae0459d11140f53401a66527e1b7
# Tue, 13 Jul 2021 21:20:07 GMT
ENV KONG_AMD64_SHA=ebe0cf3a3e71d202774ede5083c98e2ae39fae0459d11140f53401a66527e1b7
# Tue, 13 Jul 2021 21:20:07 GMT
ARG KONG_ARM64_SHA=131964ce443f2d08dc98191fcc442867f2dee2f741ccee9cc519bb99c765f3cf
# Tue, 13 Jul 2021 21:20:07 GMT
ENV KONG_ARM64_SHA=131964ce443f2d08dc98191fcc442867f2dee2f741ccee9cc519bb99c765f3cf
# Tue, 13 Jul 2021 21:20:15 GMT
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Tue, 13 Jul 2021 21:20:15 GMT
COPY file:a9828df20ead648b4c991bfb67a40d0065e248e50a2ae98fad0104e78f32d234 in /docker-entrypoint.sh 
# Tue, 13 Jul 2021 21:20:16 GMT
USER kong
# Tue, 13 Jul 2021 21:20:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 13 Jul 2021 21:20:16 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 13 Jul 2021 21:20:16 GMT
STOPSIGNAL SIGQUIT
# Tue, 13 Jul 2021 21:20:16 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 13 Jul 2021 21:20:17 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dcb869933b18a40e5829078fafe0a2045da1deafddf08550c6346d15353e9b`  
		Last Modified: Tue, 13 Jul 2021 21:22:43 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae5d676504a7ba5bcd7a66c7882841aa52368badcb077e8e97d40bb184cc27f`  
		Last Modified: Tue, 13 Jul 2021 21:22:51 GMT  
		Size: 46.7 MB (46723678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ab8837b0f778269986d4d09b2595189cd801706ebade92f33ca9260d77bffc`  
		Last Modified: Tue, 13 Jul 2021 21:22:44 GMT  
		Size: 736.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
