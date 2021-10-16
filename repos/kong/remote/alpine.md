## `kong:alpine`

```console
$ docker pull kong@sha256:57d1cc553bce0f0602f6dc4200d979aeddc1807d1fb4e7a04c2ba0c179e25ae6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:alpine` - linux; amd64

```console
$ docker pull kong@sha256:bd1064f3e76c5315f46d5361bdbc8fa62c57d45a24664402ec0071e0bd174245
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 MB (49855158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5ef5ae48a052818b2567e65ab0e2e45332dea662fd20af66a49a04c6a5ab54e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Wed, 15 Sep 2021 23:20:07 GMT
LABEL maintainer=Kong <support@konghq.com>
# Wed, 15 Sep 2021 23:20:08 GMT
ARG ASSET=ce
# Wed, 15 Sep 2021 23:20:08 GMT
ENV ASSET=ce
# Wed, 15 Sep 2021 23:20:08 GMT
ARG EE_PORTS
# Wed, 15 Sep 2021 23:20:08 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 05 Oct 2021 17:41:44 GMT
ARG KONG_VERSION=2.6.0
# Tue, 05 Oct 2021 17:41:44 GMT
ENV KONG_VERSION=2.6.0
# Tue, 05 Oct 2021 17:41:45 GMT
ARG KONG_AMD64_SHA=43fb5f27185e274e22b4a36b93b1b7e27afe94b9fd2efbe4ec69b8ed8a9e5902
# Tue, 05 Oct 2021 17:41:45 GMT
ENV KONG_AMD64_SHA=43fb5f27185e274e22b4a36b93b1b7e27afe94b9fd2efbe4ec69b8ed8a9e5902
# Tue, 05 Oct 2021 17:41:45 GMT
ARG KONG_ARM64_SHA=a057eaa6d10ecf49443ec0cac6e1b70a62ee357a777e0e169c780e18fd5c5544
# Tue, 05 Oct 2021 17:41:45 GMT
ENV KONG_ARM64_SHA=a057eaa6d10ecf49443ec0cac6e1b70a62ee357a777e0e169c780e18fd5c5544
# Tue, 05 Oct 2021 17:41:53 GMT
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Tue, 05 Oct 2021 17:41:54 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Tue, 05 Oct 2021 17:41:54 GMT
USER kong
# Tue, 05 Oct 2021 17:41:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 05 Oct 2021 17:41:55 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 05 Oct 2021 17:41:55 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 Oct 2021 17:41:55 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Tue, 05 Oct 2021 17:41:55 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f7e2c0ec31857d2cfb927962749512b048ffbf7701e394fc43f994413896b93`  
		Last Modified: Wed, 15 Sep 2021 23:22:34 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f74d93e491913e9b473ee77987093b695d7476fa64f2fea47c88a9751a1bf5`  
		Last Modified: Tue, 05 Oct 2021 17:44:42 GMT  
		Size: 47.0 MB (47039699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dadfea022cd0a1fc9dca58ad8d8fdf8729ee623d6cd03505690b9ab7665817e`  
		Last Modified: Tue, 05 Oct 2021 17:44:33 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:eb57fd149e5fe95d073e7a36c082c9bd47c7a9853df05aa03238226ff7866903
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49265990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cec6b4428e14e75cb168840828b4cc4f32a835e74bd82d2e56e1dda7c2c1fb7d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Sat, 16 Oct 2021 03:37:25 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 16 Oct 2021 03:37:26 GMT
ARG ASSET=ce
# Sat, 16 Oct 2021 03:37:27 GMT
ENV ASSET=ce
# Sat, 16 Oct 2021 03:37:28 GMT
ARG EE_PORTS
# Sat, 16 Oct 2021 03:37:30 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Sat, 16 Oct 2021 03:37:30 GMT
ARG KONG_VERSION=2.6.0
# Sat, 16 Oct 2021 03:37:31 GMT
ENV KONG_VERSION=2.6.0
# Sat, 16 Oct 2021 03:37:32 GMT
ARG KONG_AMD64_SHA=43fb5f27185e274e22b4a36b93b1b7e27afe94b9fd2efbe4ec69b8ed8a9e5902
# Sat, 16 Oct 2021 03:37:33 GMT
ENV KONG_AMD64_SHA=43fb5f27185e274e22b4a36b93b1b7e27afe94b9fd2efbe4ec69b8ed8a9e5902
# Sat, 16 Oct 2021 03:37:34 GMT
ARG KONG_ARM64_SHA=a057eaa6d10ecf49443ec0cac6e1b70a62ee357a777e0e169c780e18fd5c5544
# Sat, 16 Oct 2021 03:37:35 GMT
ENV KONG_ARM64_SHA=a057eaa6d10ecf49443ec0cac6e1b70a62ee357a777e0e169c780e18fd5c5544
# Sat, 16 Oct 2021 03:37:48 GMT
RUN set -eux;     arch="$(apk --print-arch)";     case "${arch}" in       x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;;       aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;;     esac;     if [ "$ASSET" = "ce" ] ; then       apk add --no-cache --virtual .build-deps curl wget tar ca-certificates       && curl -fL "https://download.konghq.com/gateway-${KONG_VERSION%%.*}.x-alpine/kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz       && echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -       && apk del .build-deps;     fi;     mkdir /kong     && tar -C /kong -xzf /tmp/kong.tar.gz     && mv /kong/usr/local/* /usr/local     && mv /kong/etc/* /etc     && rm -rf /kong     && apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates     && adduser -S kong     && addgroup -S kong     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && rm -rf /tmp/kong.tar.gz     && ln -s /usr/local/openresty/bin/resty /usr/local/bin/resty     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/luajit     && ln -s /usr/local/openresty/luajit/bin/luajit /usr/local/bin/lua     && ln -s /usr/local/openresty/nginx/sbin/nginx /usr/local/bin/nginx     && if [ "$ASSET" = "ce" ] ; then       kong version;     fi
# Sat, 16 Oct 2021 03:37:49 GMT
COPY file:df7f26941e26fd034e43646906785ecba3877cf078fa891fd1d304925f70408e in /docker-entrypoint.sh 
# Sat, 16 Oct 2021 03:37:49 GMT
USER kong
# Sat, 16 Oct 2021 03:37:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 16 Oct 2021 03:37:51 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 16 Oct 2021 03:37:52 GMT
STOPSIGNAL SIGQUIT
# Sat, 16 Oct 2021 03:37:53 GMT
HEALTHCHECK &{["CMD-SHELL" "kong health"] "10s" "10s" "0s" '\n'}
# Sat, 16 Oct 2021 03:37:54 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaf524f62eb906cf9274183d48b257701a07f0795d229fd3138874d18a3ba14a`  
		Last Modified: Sat, 16 Oct 2021 03:43:14 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a01bfca048d1ceeaa05e27bb8ebed0b9eab2e4bb78b53c85c15370508cc58c3`  
		Last Modified: Sat, 16 Oct 2021 03:43:23 GMT  
		Size: 46.6 MB (46553151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d780c4722fe7929b92ba27bb68aaa27f4e53da70f2c057d7d63750bf99258c97`  
		Last Modified: Sat, 16 Oct 2021 03:43:14 GMT  
		Size: 881.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
