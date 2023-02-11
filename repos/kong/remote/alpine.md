## `kong:alpine`

```console
$ docker pull kong@sha256:a786dee47155a6c3ed793cdb038c35888884e05d1682736858a073e736ee0dc2
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
