<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `kong`

-	[`kong:2`](#kong2)
-	[`kong:2.0`](#kong20)
-	[`kong:2.0.5`](#kong205)
-	[`kong:2.0.5-alpine`](#kong205-alpine)
-	[`kong:2.0.5-centos`](#kong205-centos)
-	[`kong:2.0.5-ubuntu`](#kong205-ubuntu)
-	[`kong:2.0-centos`](#kong20-centos)
-	[`kong:2.0-ubuntu`](#kong20-ubuntu)
-	[`kong:2.1`](#kong21)
-	[`kong:2.1.4`](#kong214)
-	[`kong:2.1.4-alpine`](#kong214-alpine)
-	[`kong:2.1.4-centos`](#kong214-centos)
-	[`kong:2.1.4-ubuntu`](#kong214-ubuntu)
-	[`kong:2.1-alpine`](#kong21-alpine)
-	[`kong:2.1-centos`](#kong21-centos)
-	[`kong:2.1-ubuntu`](#kong21-ubuntu)
-	[`kong:2.2`](#kong22)
-	[`kong:2.2.0`](#kong220)
-	[`kong:2.2.1-alpine`](#kong221-alpine)
-	[`kong:2.2.1-centos`](#kong221-centos)
-	[`kong:2.2.1-ubuntu`](#kong221-ubuntu)
-	[`kong:2.2-alpine`](#kong22-alpine)
-	[`kong:2.2-centos`](#kong22-centos)
-	[`kong:2.2-ubuntu`](#kong22-ubuntu)
-	[`kong:2.3`](#kong23)
-	[`kong:2.3.1`](#kong231)
-	[`kong:2.3.1-alpine`](#kong231-alpine)
-	[`kong:2.3.1-centos`](#kong231-centos)
-	[`kong:2.3.1-ubuntu`](#kong231-ubuntu)
-	[`kong:2.3-alpine`](#kong23-alpine)
-	[`kong:2.3-centos`](#kong23-centos)
-	[`kong:2.3-ubuntu`](#kong23-ubuntu)
-	[`kong:alpine`](#kongalpine)
-	[`kong:centos`](#kongcentos)
-	[`kong:latest`](#konglatest)
-	[`kong:ubuntu`](#kongubuntu)

## `kong:2`

```console
$ docker pull kong@sha256:38c82bcf40f627c1ed3edef3eb0ac9ab3d1fb29fe7eb8df69f5166b324a22153
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2` - linux; amd64

```console
$ docker pull kong@sha256:eaf0443b11346f6b7f4ac6c0979430462e5070b86a31f5cb2b16a0477773c715
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.9 MB (50938328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cd6edfe129b1c02465b0927dcfdc0d52765486279f5916a2c24d06f070dbd95`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 14:57:37 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 17 Dec 2020 14:57:37 GMT
ARG ASSET=ce
# Thu, 17 Dec 2020 14:57:37 GMT
ENV ASSET=ce
# Thu, 17 Dec 2020 14:57:37 GMT
ARG EE_PORTS
# Thu, 17 Dec 2020 14:57:38 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 27 Jan 2021 06:32:07 GMT
ARG KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 06:32:07 GMT
ENV KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 06:32:07 GMT
ARG KONG_AMD64_SHA=8a33a919f75bdb8bb708de23c0701def2aedfcd2679d27b7849040c3edf273f9
# Wed, 27 Jan 2021 06:32:07 GMT
ENV KONG_AMD64_SHA=8a33a919f75bdb8bb708de23c0701def2aedfcd2679d27b7849040c3edf273f9
# Wed, 27 Jan 2021 06:32:08 GMT
ARG KONG_ARM64_SHA=4ae43ecf9b1fcf11930d859efec475e216729b89b76de80a4c38e1fe58e3874f
# Wed, 27 Jan 2021 06:32:08 GMT
ENV KONG_ARM64_SHA=4ae43ecf9b1fcf11930d859efec475e216729b89b76de80a4c38e1fe58e3874f
# Wed, 27 Jan 2021 06:32:15 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;; 		aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Wed, 27 Jan 2021 06:32:16 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 27 Jan 2021 06:32:16 GMT
USER kong
# Wed, 27 Jan 2021 06:32:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 27 Jan 2021 06:32:16 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 27 Jan 2021 06:32:16 GMT
STOPSIGNAL SIGQUIT
# Wed, 27 Jan 2021 06:32:17 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274efec6805c2b13808c7bcb7932f07b136c0be74bf02bdbf77f79e89dc58725`  
		Last Modified: Thu, 17 Dec 2020 14:59:10 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b18e55f2934bb191d816e87b86e196e1c8d35d815f72f93f7e5f51c0f17319e`  
		Last Modified: Wed, 27 Jan 2021 06:35:34 GMT  
		Size: 48.1 MB (48122597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec1f7f35984e4dfe3874035c9af0e74955cc49424e7f4a0d50411d336f9228fa`  
		Last Modified: Wed, 27 Jan 2021 06:35:24 GMT  
		Size: 735.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:d87959fb87a61b8f9fba68a010a6e444317df9ca4bbba731d1374c9035077d0e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50462144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:065a1ea94079d9d30ef22ca0cbfffc961327ac4759c8ab96e9473a3daeb1b436`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:57:05 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 17 Dec 2020 04:57:06 GMT
ARG ASSET=ce
# Thu, 17 Dec 2020 04:57:07 GMT
ENV ASSET=ce
# Thu, 17 Dec 2020 04:57:08 GMT
ARG EE_PORTS
# Thu, 17 Dec 2020 04:57:09 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 27 Jan 2021 00:45:22 GMT
ARG KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 00:45:23 GMT
ENV KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 00:45:23 GMT
ARG KONG_AMD64_SHA=8a33a919f75bdb8bb708de23c0701def2aedfcd2679d27b7849040c3edf273f9
# Wed, 27 Jan 2021 00:45:24 GMT
ENV KONG_AMD64_SHA=8a33a919f75bdb8bb708de23c0701def2aedfcd2679d27b7849040c3edf273f9
# Wed, 27 Jan 2021 00:45:24 GMT
ARG KONG_ARM64_SHA=4ae43ecf9b1fcf11930d859efec475e216729b89b76de80a4c38e1fe58e3874f
# Wed, 27 Jan 2021 00:45:25 GMT
ENV KONG_ARM64_SHA=4ae43ecf9b1fcf11930d859efec475e216729b89b76de80a4c38e1fe58e3874f
# Wed, 27 Jan 2021 00:45:38 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;; 		aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Wed, 27 Jan 2021 00:45:40 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 27 Jan 2021 00:45:40 GMT
USER kong
# Wed, 27 Jan 2021 00:45:41 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 27 Jan 2021 00:45:42 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 27 Jan 2021 00:45:42 GMT
STOPSIGNAL SIGQUIT
# Wed, 27 Jan 2021 00:45:43 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:20d8a246443a66e74e17f2a0e81a51fe774876ca0c2676691c37ee1b0e4d3cd5`  
		Last Modified: Wed, 16 Dec 2020 23:41:20 GMT  
		Size: 2.7 MB (2725216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3181cc464c4af55ff9dd73d4603f67578cdc16237deb0e5e467594b40164ab6`  
		Last Modified: Thu, 17 Dec 2020 04:58:48 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:686913a20dd73c0bdaa7517e69803b84807b71b99b4ff55cc9764516b90461f7`  
		Last Modified: Wed, 27 Jan 2021 00:47:56 GMT  
		Size: 47.7 MB (47736063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5429c14c14d5050bce7546a62fa4539c4c325f122c109881ea4dc5f0b628ed6`  
		Last Modified: Wed, 27 Jan 2021 00:47:42 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.0`

```console
$ docker pull kong@sha256:2917f4d1cc826dff09641f8f5f2a61ee83b6ab81dd280d462a5412f2bff9a15d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.0` - linux; amd64

```console
$ docker pull kong@sha256:be89da2cf4c982993d88d3392a4ff0c9707e0038be5929e90c82339f0b01bad1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.8 MB (52766027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d735ec40ee38c6ee3e3864915340d87794317801665fb176e239697560c960af`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 14:57:37 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 17 Dec 2020 14:57:37 GMT
ARG ASSET=ce
# Thu, 17 Dec 2020 14:57:37 GMT
ENV ASSET=ce
# Thu, 17 Dec 2020 14:58:21 GMT
COPY file:987d0472e007e4e357d96fa432bce568836a2259b787227f9a9e1c369d9efc37 in /tmp/kong.tar.gz 
# Thu, 17 Dec 2020 14:58:21 GMT
ARG KONG_VERSION=2.0.5
# Thu, 17 Dec 2020 14:58:21 GMT
ENV KONG_VERSION=2.0.5
# Thu, 17 Dec 2020 14:58:21 GMT
ARG KONG_SHA256=2e78dee0e695c238cde7e607e85c2e62e44422b57c626ea12822d15ed898769b
# Thu, 17 Dec 2020 14:58:22 GMT
ENV KONG_SHA256=2e78dee0e695c238cde7e607e85c2e62e44422b57c626ea12822d15ed898769b
# Thu, 17 Dec 2020 14:58:29 GMT
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong; 	tar -C /kong -xzf /tmp/kong.tar.gz && 	mv /kong/usr/local/* /usr/local && 	mv /kong/etc/* /etc && 	rm -rf /kong && 	apk add --no-cache libgcc openssl pcre perl tzdata libcap zip bash zlib git ca-certificates && 	adduser -S kong && 	mkdir -p "/usr/local/kong" && 	chown -R kong:0 /usr/local/kong && 	chown kong:0 /usr/local/bin/kong && 	chmod -R g=u /usr/local/kong && 	rm -rf /tmp/kong.tar.gz && 	kong version
# Thu, 17 Dec 2020 14:58:29 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 17 Dec 2020 14:58:29 GMT
USER kong
# Thu, 17 Dec 2020 14:58:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 14:58:30 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 17 Dec 2020 14:58:30 GMT
STOPSIGNAL SIGQUIT
# Thu, 17 Dec 2020 14:58:30 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:710b3b50cceef66cd76ce1253baaf2ef8498d13efb8d07e175eb45cbdace8896`  
		Last Modified: Thu, 17 Dec 2020 14:59:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82935183debac230cc7e29f1504233e807537143f4ce086efd42e70cf44d307`  
		Last Modified: Thu, 17 Dec 2020 15:00:06 GMT  
		Size: 50.0 MB (49950299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b3cd38f7068a23d70dfb77b7d56ecdfcace230befe0b41fcf030ba6b2b3562`  
		Last Modified: Thu, 17 Dec 2020 14:59:54 GMT  
		Size: 735.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.0.5`

```console
$ docker pull kong@sha256:2917f4d1cc826dff09641f8f5f2a61ee83b6ab81dd280d462a5412f2bff9a15d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.0.5` - linux; amd64

```console
$ docker pull kong@sha256:be89da2cf4c982993d88d3392a4ff0c9707e0038be5929e90c82339f0b01bad1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.8 MB (52766027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d735ec40ee38c6ee3e3864915340d87794317801665fb176e239697560c960af`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 14:57:37 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 17 Dec 2020 14:57:37 GMT
ARG ASSET=ce
# Thu, 17 Dec 2020 14:57:37 GMT
ENV ASSET=ce
# Thu, 17 Dec 2020 14:58:21 GMT
COPY file:987d0472e007e4e357d96fa432bce568836a2259b787227f9a9e1c369d9efc37 in /tmp/kong.tar.gz 
# Thu, 17 Dec 2020 14:58:21 GMT
ARG KONG_VERSION=2.0.5
# Thu, 17 Dec 2020 14:58:21 GMT
ENV KONG_VERSION=2.0.5
# Thu, 17 Dec 2020 14:58:21 GMT
ARG KONG_SHA256=2e78dee0e695c238cde7e607e85c2e62e44422b57c626ea12822d15ed898769b
# Thu, 17 Dec 2020 14:58:22 GMT
ENV KONG_SHA256=2e78dee0e695c238cde7e607e85c2e62e44422b57c626ea12822d15ed898769b
# Thu, 17 Dec 2020 14:58:29 GMT
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong; 	tar -C /kong -xzf /tmp/kong.tar.gz && 	mv /kong/usr/local/* /usr/local && 	mv /kong/etc/* /etc && 	rm -rf /kong && 	apk add --no-cache libgcc openssl pcre perl tzdata libcap zip bash zlib git ca-certificates && 	adduser -S kong && 	mkdir -p "/usr/local/kong" && 	chown -R kong:0 /usr/local/kong && 	chown kong:0 /usr/local/bin/kong && 	chmod -R g=u /usr/local/kong && 	rm -rf /tmp/kong.tar.gz && 	kong version
# Thu, 17 Dec 2020 14:58:29 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 17 Dec 2020 14:58:29 GMT
USER kong
# Thu, 17 Dec 2020 14:58:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 14:58:30 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 17 Dec 2020 14:58:30 GMT
STOPSIGNAL SIGQUIT
# Thu, 17 Dec 2020 14:58:30 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:710b3b50cceef66cd76ce1253baaf2ef8498d13efb8d07e175eb45cbdace8896`  
		Last Modified: Thu, 17 Dec 2020 14:59:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82935183debac230cc7e29f1504233e807537143f4ce086efd42e70cf44d307`  
		Last Modified: Thu, 17 Dec 2020 15:00:06 GMT  
		Size: 50.0 MB (49950299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b3cd38f7068a23d70dfb77b7d56ecdfcace230befe0b41fcf030ba6b2b3562`  
		Last Modified: Thu, 17 Dec 2020 14:59:54 GMT  
		Size: 735.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.0.5-alpine`

```console
$ docker pull kong@sha256:2917f4d1cc826dff09641f8f5f2a61ee83b6ab81dd280d462a5412f2bff9a15d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.0.5-alpine` - linux; amd64

```console
$ docker pull kong@sha256:be89da2cf4c982993d88d3392a4ff0c9707e0038be5929e90c82339f0b01bad1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.8 MB (52766027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d735ec40ee38c6ee3e3864915340d87794317801665fb176e239697560c960af`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 14:57:37 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 17 Dec 2020 14:57:37 GMT
ARG ASSET=ce
# Thu, 17 Dec 2020 14:57:37 GMT
ENV ASSET=ce
# Thu, 17 Dec 2020 14:58:21 GMT
COPY file:987d0472e007e4e357d96fa432bce568836a2259b787227f9a9e1c369d9efc37 in /tmp/kong.tar.gz 
# Thu, 17 Dec 2020 14:58:21 GMT
ARG KONG_VERSION=2.0.5
# Thu, 17 Dec 2020 14:58:21 GMT
ENV KONG_VERSION=2.0.5
# Thu, 17 Dec 2020 14:58:21 GMT
ARG KONG_SHA256=2e78dee0e695c238cde7e607e85c2e62e44422b57c626ea12822d15ed898769b
# Thu, 17 Dec 2020 14:58:22 GMT
ENV KONG_SHA256=2e78dee0e695c238cde7e607e85c2e62e44422b57c626ea12822d15ed898769b
# Thu, 17 Dec 2020 14:58:29 GMT
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong; 	tar -C /kong -xzf /tmp/kong.tar.gz && 	mv /kong/usr/local/* /usr/local && 	mv /kong/etc/* /etc && 	rm -rf /kong && 	apk add --no-cache libgcc openssl pcre perl tzdata libcap zip bash zlib git ca-certificates && 	adduser -S kong && 	mkdir -p "/usr/local/kong" && 	chown -R kong:0 /usr/local/kong && 	chown kong:0 /usr/local/bin/kong && 	chmod -R g=u /usr/local/kong && 	rm -rf /tmp/kong.tar.gz && 	kong version
# Thu, 17 Dec 2020 14:58:29 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 17 Dec 2020 14:58:29 GMT
USER kong
# Thu, 17 Dec 2020 14:58:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 14:58:30 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 17 Dec 2020 14:58:30 GMT
STOPSIGNAL SIGQUIT
# Thu, 17 Dec 2020 14:58:30 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:710b3b50cceef66cd76ce1253baaf2ef8498d13efb8d07e175eb45cbdace8896`  
		Last Modified: Thu, 17 Dec 2020 14:59:55 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82935183debac230cc7e29f1504233e807537143f4ce086efd42e70cf44d307`  
		Last Modified: Thu, 17 Dec 2020 15:00:06 GMT  
		Size: 50.0 MB (49950299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b3cd38f7068a23d70dfb77b7d56ecdfcace230befe0b41fcf030ba6b2b3562`  
		Last Modified: Thu, 17 Dec 2020 14:59:54 GMT  
		Size: 735.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.0.5-centos`

```console
$ docker pull kong@sha256:079abab579c65a5b8d16be6cee38003ba4a57fd7e94b7de9168bb5c5d4d15ca4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.0.5-centos` - linux; amd64

```console
$ docker pull kong@sha256:554d9579ae5ccc7da6cfd7a742010c445cca0294e446abd55c10903c395e902b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127491262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12b9f5083661211369645dcdeb6b3f5338fd57bf7316dcde5c1258cad2f951eb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 14 Nov 2020 00:20:04 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Sat, 14 Nov 2020 00:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Sat, 14 Nov 2020 00:20:04 GMT
CMD ["/bin/bash"]
# Sat, 14 Nov 2020 01:01:33 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 14 Nov 2020 01:01:33 GMT
ARG ASSET=ce
# Sat, 14 Nov 2020 01:01:34 GMT
ENV ASSET=ce
# Sat, 14 Nov 2020 01:02:56 GMT
COPY file:73044b225363e2703a176f55b132687ead4bab30398788756be18d2965fac2cd in /tmp/kong.rpm 
# Sat, 14 Nov 2020 01:02:57 GMT
ARG KONG_VERSION=2.0.5
# Sat, 14 Nov 2020 01:02:57 GMT
ENV KONG_VERSION=2.0.5
# Sat, 14 Nov 2020 01:02:57 GMT
ARG KONG_SHA256=e05340680de3541c4c940f54e64f00c90fb5137f6a8c71e413b815a411d74fc6
# Sat, 14 Nov 2020 01:02:57 GMT
ENV KONG_SHA256=e05340680de3541c4c940f54e64f00c90fb5137f6a8c71e413b815a411d74fc6
# Sat, 14 Nov 2020 01:03:20 GMT
RUN set -ex; 	if [ "$ASSET" = "ce" ] ; then 		curl -fL "https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm" -o /tmp/kong.rpm 		&& echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -; 	fi; 	yum install -y -q unzip shadow-utils git zlib 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki 	&& useradd kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y /tmp/kong.rpm 	&& yum clean all 	&& rm /tmp/kong.rpm 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong 	&& kong version
# Sat, 14 Nov 2020 01:03:20 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Sat, 14 Nov 2020 01:03:21 GMT
USER kong
# Sat, 14 Nov 2020 01:03:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 14 Nov 2020 01:03:21 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 14 Nov 2020 01:03:21 GMT
STOPSIGNAL SIGQUIT
# Sat, 14 Nov 2020 01:03:21 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692b26149754880bb26d043fb2a9bba7fe1fb5406a67028d073895681609b4df`  
		Last Modified: Sat, 14 Nov 2020 01:04:21 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5f3c5952d48cacf33b16df4f8fac200bbecacd4350fd0629a4815eec28ff1cb`  
		Last Modified: Sat, 14 Nov 2020 01:04:31 GMT  
		Size: 51.4 MB (51393250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86ddac787b13b6ae84c90e260caa89eeb915b690116162d279d9fa5197477dc`  
		Last Modified: Sat, 14 Nov 2020 01:04:20 GMT  
		Size: 732.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.0.5-ubuntu`

```console
$ docker pull kong@sha256:a253f04133d6d0148add4df08c7e1af76a1d4f725d7105bf4085a1938ede66d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.0.5-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:d4a0adc64047bf3d0068bba75919963496dac9e4e3ecee7154bf6fba0fd53ca6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.1 MB (101061262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c632b0b299f9193785f70b918f73b2b4292b8b9836aa5cce54a2fe9418fa7186`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 21 Jan 2021 03:39:31 GMT
ADD file:925571658dd8453e5c80d862f5791d6b26b3c2a8688937b11741f2f2c5cdbfd7 in / 
# Thu, 21 Jan 2021 03:39:32 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:39:34 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:39:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:39:36 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 10:27:05 GMT
ARG ASSET=ce
# Thu, 21 Jan 2021 10:27:05 GMT
ENV ASSET=ce
# Thu, 21 Jan 2021 10:29:10 GMT
COPY file:5307743dbc5e81034b8adaf56f281bcb13b0da2d468cb6450d72fa5b77543ccf in /tmp/kong.deb 
# Thu, 21 Jan 2021 10:29:10 GMT
ARG KONG_VERSION=2.0.5
# Thu, 21 Jan 2021 10:29:10 GMT
ENV KONG_VERSION=2.0.5
# Thu, 21 Jan 2021 10:29:31 GMT
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apt-get update &&         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get update     && apt-get install -y --no-install-recommends perl unzip git zlib1g     && rm -rf /var/lib/apt/lists/* 	&& dpkg -i /tmp/kong.deb 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong 	&& kong version
# Thu, 21 Jan 2021 10:29:32 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Thu, 21 Jan 2021 10:29:32 GMT
USER kong
# Thu, 21 Jan 2021 10:29:33 GMT
RUN kong version
# Thu, 21 Jan 2021 10:29:33 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 21 Jan 2021 10:29:33 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 21 Jan 2021 10:29:34 GMT
STOPSIGNAL SIGQUIT
# Thu, 21 Jan 2021 10:29:34 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4007a89234b4f56c03e6831dc220550d2e5fba935d9f5f5bcea64857ac4f4888`  
		Last Modified: Mon, 18 Jan 2021 19:38:08 GMT  
		Size: 46.0 MB (45962352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfa26c6b9c9d1ccbcb1eaa65befa376805d9324174ac580ca76fdedc3575f54`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba7bf18aa406cb7dc372ac732de222b04d1c824ff1705d8900831c3d1361ff5`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6ec688ebe374ea7d89ce967576d221a177ebd2c02ca9f053197f954102e30b`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59df306867f48f345aeecb87f998c383dab57de7368896bab3a4fc9aabf2928`  
		Last Modified: Thu, 21 Jan 2021 10:31:48 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbaf794695116fea4fb60d592e4743d8cf5fd58375981c44b4d55c3673503be2`  
		Last Modified: Thu, 21 Jan 2021 10:32:00 GMT  
		Size: 55.1 MB (55096456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6609ef38227fc6f093b2cb90924604b7d65ef7190c21aa12f77633cce60923d`  
		Last Modified: Thu, 21 Jan 2021 10:31:48 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb7e5879b9302ce552acc5e0491da8154bd2db0c24cffe78e1866ccb191ceac`  
		Last Modified: Thu, 21 Jan 2021 10:31:48 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.0.5-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:2705e7dd0518af4a9c38edfd1092c04dbfbca05e3266383095e2e207ddfc1709
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 MB (93072709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47010f98eaabc4154f806c853cc83f2e95bb370fdfbe068b7e5e7cc58cfd7459`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 21 Jan 2021 03:51:12 GMT
ADD file:e2f37be259f081b70bc884e3b7f652e5d9a0ad4ae443f2258b79a1b14377cc20 in / 
# Thu, 21 Jan 2021 03:51:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:51:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:51:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:51:22 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:32:05 GMT
ARG ASSET=ce
# Thu, 21 Jan 2021 05:32:06 GMT
ENV ASSET=ce
# Thu, 21 Jan 2021 05:35:48 GMT
COPY file:5307743dbc5e81034b8adaf56f281bcb13b0da2d468cb6450d72fa5b77543ccf in /tmp/kong.deb 
# Thu, 21 Jan 2021 05:35:49 GMT
ARG KONG_VERSION=2.0.5
# Thu, 21 Jan 2021 05:35:50 GMT
ENV KONG_VERSION=2.0.5
# Thu, 21 Jan 2021 05:36:31 GMT
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apt-get update &&         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get update     && apt-get install -y --no-install-recommends perl unzip git zlib1g     && rm -rf /var/lib/apt/lists/* 	&& dpkg -i /tmp/kong.deb 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong 	&& kong version
# Thu, 21 Jan 2021 05:36:33 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Thu, 21 Jan 2021 05:36:34 GMT
USER kong
# Thu, 21 Jan 2021 05:36:36 GMT
RUN kong version
# Thu, 21 Jan 2021 05:36:36 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:36:37 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 21 Jan 2021 05:36:38 GMT
STOPSIGNAL SIGQUIT
# Thu, 21 Jan 2021 05:36:38 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:79186a4c5361c6b018fe75c9bba66c9bf717db8d7d4a6ddb18fb86171f277b61`  
		Last Modified: Thu, 14 Jan 2021 16:25:21 GMT  
		Size: 40.9 MB (40885219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96f901e8ebcf64a42ec369549f6269ec96cd97b424389ca99a8ebb722c59c12`  
		Last Modified: Thu, 21 Jan 2021 03:53:10 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36fd1545244608cb9ef92efa528b6e8c3229f1b01ca414ee8717219145cdff7d`  
		Last Modified: Thu, 21 Jan 2021 03:53:10 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d978c0f55122642ba1a22cc67abf7af2e898bfb42933b1879c2dd91fd987147d`  
		Last Modified: Thu, 21 Jan 2021 03:53:11 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e364343239094535f14c35ef5e131471b966188de44b93aeede0e05b1846721e`  
		Last Modified: Thu, 21 Jan 2021 05:38:48 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e0eac08498e298b622e08a7f87cd69a82817a5ace2acebed22998cd9e1b4fce`  
		Last Modified: Thu, 21 Jan 2021 05:39:00 GMT  
		Size: 52.2 MB (52185091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff3d4450827002eb8ce5cfc3c6b803a2b4c617fb6dd4c9394aefd07a3c80ed0`  
		Last Modified: Thu, 21 Jan 2021 05:38:47 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b858413272bc97018762df0a5c950702d25874f24c3830eb17215363a0e826b7`  
		Last Modified: Thu, 21 Jan 2021 05:38:48 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.0-centos`

```console
$ docker pull kong@sha256:079abab579c65a5b8d16be6cee38003ba4a57fd7e94b7de9168bb5c5d4d15ca4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.0-centos` - linux; amd64

```console
$ docker pull kong@sha256:554d9579ae5ccc7da6cfd7a742010c445cca0294e446abd55c10903c395e902b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127491262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12b9f5083661211369645dcdeb6b3f5338fd57bf7316dcde5c1258cad2f951eb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 14 Nov 2020 00:20:04 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Sat, 14 Nov 2020 00:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Sat, 14 Nov 2020 00:20:04 GMT
CMD ["/bin/bash"]
# Sat, 14 Nov 2020 01:01:33 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 14 Nov 2020 01:01:33 GMT
ARG ASSET=ce
# Sat, 14 Nov 2020 01:01:34 GMT
ENV ASSET=ce
# Sat, 14 Nov 2020 01:02:56 GMT
COPY file:73044b225363e2703a176f55b132687ead4bab30398788756be18d2965fac2cd in /tmp/kong.rpm 
# Sat, 14 Nov 2020 01:02:57 GMT
ARG KONG_VERSION=2.0.5
# Sat, 14 Nov 2020 01:02:57 GMT
ENV KONG_VERSION=2.0.5
# Sat, 14 Nov 2020 01:02:57 GMT
ARG KONG_SHA256=e05340680de3541c4c940f54e64f00c90fb5137f6a8c71e413b815a411d74fc6
# Sat, 14 Nov 2020 01:02:57 GMT
ENV KONG_SHA256=e05340680de3541c4c940f54e64f00c90fb5137f6a8c71e413b815a411d74fc6
# Sat, 14 Nov 2020 01:03:20 GMT
RUN set -ex; 	if [ "$ASSET" = "ce" ] ; then 		curl -fL "https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm" -o /tmp/kong.rpm 		&& echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -; 	fi; 	yum install -y -q unzip shadow-utils git zlib 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki 	&& useradd kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y /tmp/kong.rpm 	&& yum clean all 	&& rm /tmp/kong.rpm 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong 	&& kong version
# Sat, 14 Nov 2020 01:03:20 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Sat, 14 Nov 2020 01:03:21 GMT
USER kong
# Sat, 14 Nov 2020 01:03:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 14 Nov 2020 01:03:21 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 14 Nov 2020 01:03:21 GMT
STOPSIGNAL SIGQUIT
# Sat, 14 Nov 2020 01:03:21 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692b26149754880bb26d043fb2a9bba7fe1fb5406a67028d073895681609b4df`  
		Last Modified: Sat, 14 Nov 2020 01:04:21 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5f3c5952d48cacf33b16df4f8fac200bbecacd4350fd0629a4815eec28ff1cb`  
		Last Modified: Sat, 14 Nov 2020 01:04:31 GMT  
		Size: 51.4 MB (51393250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86ddac787b13b6ae84c90e260caa89eeb915b690116162d279d9fa5197477dc`  
		Last Modified: Sat, 14 Nov 2020 01:04:20 GMT  
		Size: 732.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.0-ubuntu`

```console
$ docker pull kong@sha256:a253f04133d6d0148add4df08c7e1af76a1d4f725d7105bf4085a1938ede66d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.0-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:d4a0adc64047bf3d0068bba75919963496dac9e4e3ecee7154bf6fba0fd53ca6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.1 MB (101061262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c632b0b299f9193785f70b918f73b2b4292b8b9836aa5cce54a2fe9418fa7186`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 21 Jan 2021 03:39:31 GMT
ADD file:925571658dd8453e5c80d862f5791d6b26b3c2a8688937b11741f2f2c5cdbfd7 in / 
# Thu, 21 Jan 2021 03:39:32 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:39:34 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:39:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:39:36 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 10:27:05 GMT
ARG ASSET=ce
# Thu, 21 Jan 2021 10:27:05 GMT
ENV ASSET=ce
# Thu, 21 Jan 2021 10:29:10 GMT
COPY file:5307743dbc5e81034b8adaf56f281bcb13b0da2d468cb6450d72fa5b77543ccf in /tmp/kong.deb 
# Thu, 21 Jan 2021 10:29:10 GMT
ARG KONG_VERSION=2.0.5
# Thu, 21 Jan 2021 10:29:10 GMT
ENV KONG_VERSION=2.0.5
# Thu, 21 Jan 2021 10:29:31 GMT
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apt-get update &&         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get update     && apt-get install -y --no-install-recommends perl unzip git zlib1g     && rm -rf /var/lib/apt/lists/* 	&& dpkg -i /tmp/kong.deb 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong 	&& kong version
# Thu, 21 Jan 2021 10:29:32 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Thu, 21 Jan 2021 10:29:32 GMT
USER kong
# Thu, 21 Jan 2021 10:29:33 GMT
RUN kong version
# Thu, 21 Jan 2021 10:29:33 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 21 Jan 2021 10:29:33 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 21 Jan 2021 10:29:34 GMT
STOPSIGNAL SIGQUIT
# Thu, 21 Jan 2021 10:29:34 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4007a89234b4f56c03e6831dc220550d2e5fba935d9f5f5bcea64857ac4f4888`  
		Last Modified: Mon, 18 Jan 2021 19:38:08 GMT  
		Size: 46.0 MB (45962352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfa26c6b9c9d1ccbcb1eaa65befa376805d9324174ac580ca76fdedc3575f54`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba7bf18aa406cb7dc372ac732de222b04d1c824ff1705d8900831c3d1361ff5`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6ec688ebe374ea7d89ce967576d221a177ebd2c02ca9f053197f954102e30b`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59df306867f48f345aeecb87f998c383dab57de7368896bab3a4fc9aabf2928`  
		Last Modified: Thu, 21 Jan 2021 10:31:48 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbaf794695116fea4fb60d592e4743d8cf5fd58375981c44b4d55c3673503be2`  
		Last Modified: Thu, 21 Jan 2021 10:32:00 GMT  
		Size: 55.1 MB (55096456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6609ef38227fc6f093b2cb90924604b7d65ef7190c21aa12f77633cce60923d`  
		Last Modified: Thu, 21 Jan 2021 10:31:48 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb7e5879b9302ce552acc5e0491da8154bd2db0c24cffe78e1866ccb191ceac`  
		Last Modified: Thu, 21 Jan 2021 10:31:48 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.0-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:2705e7dd0518af4a9c38edfd1092c04dbfbca05e3266383095e2e207ddfc1709
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 MB (93072709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47010f98eaabc4154f806c853cc83f2e95bb370fdfbe068b7e5e7cc58cfd7459`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 21 Jan 2021 03:51:12 GMT
ADD file:e2f37be259f081b70bc884e3b7f652e5d9a0ad4ae443f2258b79a1b14377cc20 in / 
# Thu, 21 Jan 2021 03:51:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:51:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:51:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:51:22 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:32:05 GMT
ARG ASSET=ce
# Thu, 21 Jan 2021 05:32:06 GMT
ENV ASSET=ce
# Thu, 21 Jan 2021 05:35:48 GMT
COPY file:5307743dbc5e81034b8adaf56f281bcb13b0da2d468cb6450d72fa5b77543ccf in /tmp/kong.deb 
# Thu, 21 Jan 2021 05:35:49 GMT
ARG KONG_VERSION=2.0.5
# Thu, 21 Jan 2021 05:35:50 GMT
ENV KONG_VERSION=2.0.5
# Thu, 21 Jan 2021 05:36:31 GMT
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apt-get update &&         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get update     && apt-get install -y --no-install-recommends perl unzip git zlib1g     && rm -rf /var/lib/apt/lists/* 	&& dpkg -i /tmp/kong.deb 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong 	&& kong version
# Thu, 21 Jan 2021 05:36:33 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Thu, 21 Jan 2021 05:36:34 GMT
USER kong
# Thu, 21 Jan 2021 05:36:36 GMT
RUN kong version
# Thu, 21 Jan 2021 05:36:36 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:36:37 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 21 Jan 2021 05:36:38 GMT
STOPSIGNAL SIGQUIT
# Thu, 21 Jan 2021 05:36:38 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:79186a4c5361c6b018fe75c9bba66c9bf717db8d7d4a6ddb18fb86171f277b61`  
		Last Modified: Thu, 14 Jan 2021 16:25:21 GMT  
		Size: 40.9 MB (40885219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96f901e8ebcf64a42ec369549f6269ec96cd97b424389ca99a8ebb722c59c12`  
		Last Modified: Thu, 21 Jan 2021 03:53:10 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36fd1545244608cb9ef92efa528b6e8c3229f1b01ca414ee8717219145cdff7d`  
		Last Modified: Thu, 21 Jan 2021 03:53:10 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d978c0f55122642ba1a22cc67abf7af2e898bfb42933b1879c2dd91fd987147d`  
		Last Modified: Thu, 21 Jan 2021 03:53:11 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e364343239094535f14c35ef5e131471b966188de44b93aeede0e05b1846721e`  
		Last Modified: Thu, 21 Jan 2021 05:38:48 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e0eac08498e298b622e08a7f87cd69a82817a5ace2acebed22998cd9e1b4fce`  
		Last Modified: Thu, 21 Jan 2021 05:39:00 GMT  
		Size: 52.2 MB (52185091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff3d4450827002eb8ce5cfc3c6b803a2b4c617fb6dd4c9394aefd07a3c80ed0`  
		Last Modified: Thu, 21 Jan 2021 05:38:47 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b858413272bc97018762df0a5c950702d25874f24c3830eb17215363a0e826b7`  
		Last Modified: Thu, 21 Jan 2021 05:38:48 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.1`

```console
$ docker pull kong@sha256:fd785a4fb730f27723ee2012871a4649cc8efedeed2e07b933221371eeb6bfaf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.1` - linux; amd64

```console
$ docker pull kong@sha256:66638610c5199438e899b6f97ea5aa615bc5ecfda9e940595f4456252736fefd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53151918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bda17790f5d47993bb5da2b47ced574cd11d090e263b49ac8eab6a95d0a4388`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 14:57:37 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 17 Dec 2020 14:57:37 GMT
ARG ASSET=ce
# Thu, 17 Dec 2020 14:57:37 GMT
ENV ASSET=ce
# Thu, 17 Dec 2020 14:57:37 GMT
ARG EE_PORTS
# Thu, 17 Dec 2020 14:57:38 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 17 Dec 2020 14:57:59 GMT
ARG KONG_VERSION=2.1.4
# Thu, 17 Dec 2020 14:57:59 GMT
ENV KONG_VERSION=2.1.4
# Thu, 17 Dec 2020 14:58:07 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256='760cea1f7a058be6000e14dfecfeb73cc79245f696f18e0fcf0825935b944ab3' ;; 		aarch64) arch='arm64'; KONG_SHA256='08038f49f162ab5edc357d7712e90241f6571027cb8741b15ba0c951653764c2' ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong; 	tar -C /kong -xzf /tmp/kong.tar.gz && 	mv /kong/usr/local/* /usr/local && 	mv /kong/etc/* /etc && 	rm -rf /kong && 	apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates && 	adduser -S kong && 	mkdir -p "/usr/local/kong" && 	chown -R kong:0 /usr/local/kong && 	chown kong:0 /usr/local/bin/kong && 	chmod -R g=u /usr/local/kong && 	rm -rf /tmp/kong.tar.gz &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Thu, 17 Dec 2020 14:58:07 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 17 Dec 2020 14:58:07 GMT
USER kong
# Thu, 17 Dec 2020 14:58:07 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 14:58:08 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 17 Dec 2020 14:58:08 GMT
STOPSIGNAL SIGQUIT
# Thu, 17 Dec 2020 14:58:08 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274efec6805c2b13808c7bcb7932f07b136c0be74bf02bdbf77f79e89dc58725`  
		Last Modified: Thu, 17 Dec 2020 14:59:10 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225b0abb30a19fff4fd85428b236bca3911068e5a902d535da6ab539e8d4e319`  
		Last Modified: Thu, 17 Dec 2020 14:59:45 GMT  
		Size: 50.3 MB (50336188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8997b6b5c0e212034dac86dd776b393c56687021b90a68bfd5164dbd482afd9`  
		Last Modified: Thu, 17 Dec 2020 14:59:36 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.1` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:2ada4f5522df9afdcc8230d55d29842c321585b16258c46616a6d1e7ef8dc7a8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.7 MB (52665031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d349242092b941662b5f7463ac4a33d865746d92ca9dfbf5ace92391d5cb0b5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:57:05 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 17 Dec 2020 04:57:06 GMT
ARG ASSET=ce
# Thu, 17 Dec 2020 04:57:07 GMT
ENV ASSET=ce
# Thu, 17 Dec 2020 04:57:08 GMT
ARG EE_PORTS
# Thu, 17 Dec 2020 04:57:09 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 17 Dec 2020 04:57:51 GMT
ARG KONG_VERSION=2.1.4
# Thu, 17 Dec 2020 04:57:53 GMT
ENV KONG_VERSION=2.1.4
# Thu, 17 Dec 2020 04:58:04 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256='760cea1f7a058be6000e14dfecfeb73cc79245f696f18e0fcf0825935b944ab3' ;; 		aarch64) arch='arm64'; KONG_SHA256='08038f49f162ab5edc357d7712e90241f6571027cb8741b15ba0c951653764c2' ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong; 	tar -C /kong -xzf /tmp/kong.tar.gz && 	mv /kong/usr/local/* /usr/local && 	mv /kong/etc/* /etc && 	rm -rf /kong && 	apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates && 	adduser -S kong && 	mkdir -p "/usr/local/kong" && 	chown -R kong:0 /usr/local/kong && 	chown kong:0 /usr/local/bin/kong && 	chmod -R g=u /usr/local/kong && 	rm -rf /tmp/kong.tar.gz &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Thu, 17 Dec 2020 04:58:06 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 17 Dec 2020 04:58:08 GMT
USER kong
# Thu, 17 Dec 2020 04:58:09 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 04:58:09 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 17 Dec 2020 04:58:10 GMT
STOPSIGNAL SIGQUIT
# Thu, 17 Dec 2020 04:58:11 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:20d8a246443a66e74e17f2a0e81a51fe774876ca0c2676691c37ee1b0e4d3cd5`  
		Last Modified: Wed, 16 Dec 2020 23:41:20 GMT  
		Size: 2.7 MB (2725216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3181cc464c4af55ff9dd73d4603f67578cdc16237deb0e5e467594b40164ab6`  
		Last Modified: Thu, 17 Dec 2020 04:58:48 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e8c4352649944a52a45f73f8267085e3e8f5f8c42cd7916f17e194af442ccdd`  
		Last Modified: Thu, 17 Dec 2020 04:59:39 GMT  
		Size: 49.9 MB (49938950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c2b84fa76be82f6d536a0c0a486863650800cfad97b972c7753461f8f4e3bc`  
		Last Modified: Thu, 17 Dec 2020 04:59:23 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.1.4`

```console
$ docker pull kong@sha256:fd785a4fb730f27723ee2012871a4649cc8efedeed2e07b933221371eeb6bfaf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.1.4` - linux; amd64

```console
$ docker pull kong@sha256:66638610c5199438e899b6f97ea5aa615bc5ecfda9e940595f4456252736fefd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53151918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bda17790f5d47993bb5da2b47ced574cd11d090e263b49ac8eab6a95d0a4388`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 14:57:37 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 17 Dec 2020 14:57:37 GMT
ARG ASSET=ce
# Thu, 17 Dec 2020 14:57:37 GMT
ENV ASSET=ce
# Thu, 17 Dec 2020 14:57:37 GMT
ARG EE_PORTS
# Thu, 17 Dec 2020 14:57:38 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 17 Dec 2020 14:57:59 GMT
ARG KONG_VERSION=2.1.4
# Thu, 17 Dec 2020 14:57:59 GMT
ENV KONG_VERSION=2.1.4
# Thu, 17 Dec 2020 14:58:07 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256='760cea1f7a058be6000e14dfecfeb73cc79245f696f18e0fcf0825935b944ab3' ;; 		aarch64) arch='arm64'; KONG_SHA256='08038f49f162ab5edc357d7712e90241f6571027cb8741b15ba0c951653764c2' ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong; 	tar -C /kong -xzf /tmp/kong.tar.gz && 	mv /kong/usr/local/* /usr/local && 	mv /kong/etc/* /etc && 	rm -rf /kong && 	apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates && 	adduser -S kong && 	mkdir -p "/usr/local/kong" && 	chown -R kong:0 /usr/local/kong && 	chown kong:0 /usr/local/bin/kong && 	chmod -R g=u /usr/local/kong && 	rm -rf /tmp/kong.tar.gz &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Thu, 17 Dec 2020 14:58:07 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 17 Dec 2020 14:58:07 GMT
USER kong
# Thu, 17 Dec 2020 14:58:07 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 14:58:08 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 17 Dec 2020 14:58:08 GMT
STOPSIGNAL SIGQUIT
# Thu, 17 Dec 2020 14:58:08 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274efec6805c2b13808c7bcb7932f07b136c0be74bf02bdbf77f79e89dc58725`  
		Last Modified: Thu, 17 Dec 2020 14:59:10 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225b0abb30a19fff4fd85428b236bca3911068e5a902d535da6ab539e8d4e319`  
		Last Modified: Thu, 17 Dec 2020 14:59:45 GMT  
		Size: 50.3 MB (50336188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8997b6b5c0e212034dac86dd776b393c56687021b90a68bfd5164dbd482afd9`  
		Last Modified: Thu, 17 Dec 2020 14:59:36 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.1.4` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:2ada4f5522df9afdcc8230d55d29842c321585b16258c46616a6d1e7ef8dc7a8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.7 MB (52665031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d349242092b941662b5f7463ac4a33d865746d92ca9dfbf5ace92391d5cb0b5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:57:05 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 17 Dec 2020 04:57:06 GMT
ARG ASSET=ce
# Thu, 17 Dec 2020 04:57:07 GMT
ENV ASSET=ce
# Thu, 17 Dec 2020 04:57:08 GMT
ARG EE_PORTS
# Thu, 17 Dec 2020 04:57:09 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 17 Dec 2020 04:57:51 GMT
ARG KONG_VERSION=2.1.4
# Thu, 17 Dec 2020 04:57:53 GMT
ENV KONG_VERSION=2.1.4
# Thu, 17 Dec 2020 04:58:04 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256='760cea1f7a058be6000e14dfecfeb73cc79245f696f18e0fcf0825935b944ab3' ;; 		aarch64) arch='arm64'; KONG_SHA256='08038f49f162ab5edc357d7712e90241f6571027cb8741b15ba0c951653764c2' ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong; 	tar -C /kong -xzf /tmp/kong.tar.gz && 	mv /kong/usr/local/* /usr/local && 	mv /kong/etc/* /etc && 	rm -rf /kong && 	apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates && 	adduser -S kong && 	mkdir -p "/usr/local/kong" && 	chown -R kong:0 /usr/local/kong && 	chown kong:0 /usr/local/bin/kong && 	chmod -R g=u /usr/local/kong && 	rm -rf /tmp/kong.tar.gz &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Thu, 17 Dec 2020 04:58:06 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 17 Dec 2020 04:58:08 GMT
USER kong
# Thu, 17 Dec 2020 04:58:09 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 04:58:09 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 17 Dec 2020 04:58:10 GMT
STOPSIGNAL SIGQUIT
# Thu, 17 Dec 2020 04:58:11 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:20d8a246443a66e74e17f2a0e81a51fe774876ca0c2676691c37ee1b0e4d3cd5`  
		Last Modified: Wed, 16 Dec 2020 23:41:20 GMT  
		Size: 2.7 MB (2725216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3181cc464c4af55ff9dd73d4603f67578cdc16237deb0e5e467594b40164ab6`  
		Last Modified: Thu, 17 Dec 2020 04:58:48 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e8c4352649944a52a45f73f8267085e3e8f5f8c42cd7916f17e194af442ccdd`  
		Last Modified: Thu, 17 Dec 2020 04:59:39 GMT  
		Size: 49.9 MB (49938950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c2b84fa76be82f6d536a0c0a486863650800cfad97b972c7753461f8f4e3bc`  
		Last Modified: Thu, 17 Dec 2020 04:59:23 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.1.4-alpine`

```console
$ docker pull kong@sha256:fd785a4fb730f27723ee2012871a4649cc8efedeed2e07b933221371eeb6bfaf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.1.4-alpine` - linux; amd64

```console
$ docker pull kong@sha256:66638610c5199438e899b6f97ea5aa615bc5ecfda9e940595f4456252736fefd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53151918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bda17790f5d47993bb5da2b47ced574cd11d090e263b49ac8eab6a95d0a4388`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 14:57:37 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 17 Dec 2020 14:57:37 GMT
ARG ASSET=ce
# Thu, 17 Dec 2020 14:57:37 GMT
ENV ASSET=ce
# Thu, 17 Dec 2020 14:57:37 GMT
ARG EE_PORTS
# Thu, 17 Dec 2020 14:57:38 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 17 Dec 2020 14:57:59 GMT
ARG KONG_VERSION=2.1.4
# Thu, 17 Dec 2020 14:57:59 GMT
ENV KONG_VERSION=2.1.4
# Thu, 17 Dec 2020 14:58:07 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256='760cea1f7a058be6000e14dfecfeb73cc79245f696f18e0fcf0825935b944ab3' ;; 		aarch64) arch='arm64'; KONG_SHA256='08038f49f162ab5edc357d7712e90241f6571027cb8741b15ba0c951653764c2' ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong; 	tar -C /kong -xzf /tmp/kong.tar.gz && 	mv /kong/usr/local/* /usr/local && 	mv /kong/etc/* /etc && 	rm -rf /kong && 	apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates && 	adduser -S kong && 	mkdir -p "/usr/local/kong" && 	chown -R kong:0 /usr/local/kong && 	chown kong:0 /usr/local/bin/kong && 	chmod -R g=u /usr/local/kong && 	rm -rf /tmp/kong.tar.gz &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Thu, 17 Dec 2020 14:58:07 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 17 Dec 2020 14:58:07 GMT
USER kong
# Thu, 17 Dec 2020 14:58:07 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 14:58:08 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 17 Dec 2020 14:58:08 GMT
STOPSIGNAL SIGQUIT
# Thu, 17 Dec 2020 14:58:08 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274efec6805c2b13808c7bcb7932f07b136c0be74bf02bdbf77f79e89dc58725`  
		Last Modified: Thu, 17 Dec 2020 14:59:10 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225b0abb30a19fff4fd85428b236bca3911068e5a902d535da6ab539e8d4e319`  
		Last Modified: Thu, 17 Dec 2020 14:59:45 GMT  
		Size: 50.3 MB (50336188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8997b6b5c0e212034dac86dd776b393c56687021b90a68bfd5164dbd482afd9`  
		Last Modified: Thu, 17 Dec 2020 14:59:36 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.1.4-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:2ada4f5522df9afdcc8230d55d29842c321585b16258c46616a6d1e7ef8dc7a8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.7 MB (52665031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d349242092b941662b5f7463ac4a33d865746d92ca9dfbf5ace92391d5cb0b5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:57:05 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 17 Dec 2020 04:57:06 GMT
ARG ASSET=ce
# Thu, 17 Dec 2020 04:57:07 GMT
ENV ASSET=ce
# Thu, 17 Dec 2020 04:57:08 GMT
ARG EE_PORTS
# Thu, 17 Dec 2020 04:57:09 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 17 Dec 2020 04:57:51 GMT
ARG KONG_VERSION=2.1.4
# Thu, 17 Dec 2020 04:57:53 GMT
ENV KONG_VERSION=2.1.4
# Thu, 17 Dec 2020 04:58:04 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256='760cea1f7a058be6000e14dfecfeb73cc79245f696f18e0fcf0825935b944ab3' ;; 		aarch64) arch='arm64'; KONG_SHA256='08038f49f162ab5edc357d7712e90241f6571027cb8741b15ba0c951653764c2' ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong; 	tar -C /kong -xzf /tmp/kong.tar.gz && 	mv /kong/usr/local/* /usr/local && 	mv /kong/etc/* /etc && 	rm -rf /kong && 	apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates && 	adduser -S kong && 	mkdir -p "/usr/local/kong" && 	chown -R kong:0 /usr/local/kong && 	chown kong:0 /usr/local/bin/kong && 	chmod -R g=u /usr/local/kong && 	rm -rf /tmp/kong.tar.gz &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Thu, 17 Dec 2020 04:58:06 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 17 Dec 2020 04:58:08 GMT
USER kong
# Thu, 17 Dec 2020 04:58:09 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 04:58:09 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 17 Dec 2020 04:58:10 GMT
STOPSIGNAL SIGQUIT
# Thu, 17 Dec 2020 04:58:11 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:20d8a246443a66e74e17f2a0e81a51fe774876ca0c2676691c37ee1b0e4d3cd5`  
		Last Modified: Wed, 16 Dec 2020 23:41:20 GMT  
		Size: 2.7 MB (2725216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3181cc464c4af55ff9dd73d4603f67578cdc16237deb0e5e467594b40164ab6`  
		Last Modified: Thu, 17 Dec 2020 04:58:48 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e8c4352649944a52a45f73f8267085e3e8f5f8c42cd7916f17e194af442ccdd`  
		Last Modified: Thu, 17 Dec 2020 04:59:39 GMT  
		Size: 49.9 MB (49938950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c2b84fa76be82f6d536a0c0a486863650800cfad97b972c7753461f8f4e3bc`  
		Last Modified: Thu, 17 Dec 2020 04:59:23 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.1.4-centos`

```console
$ docker pull kong@sha256:2074a8dbc332a2d158a41f480915d2cca721cd24449a36a956d673b992551da0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.1.4-centos` - linux; amd64

```console
$ docker pull kong@sha256:9abae830a109a6c87cf973fab99656a87fe37c1a53c195d79fa8b2448d85a75d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.3 MB (127260020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05a08e453725f88199609cc19d52cc849a8b829755d8ea61b90d497a84e9c4b3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 14 Nov 2020 00:20:04 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Sat, 14 Nov 2020 00:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Sat, 14 Nov 2020 00:20:04 GMT
CMD ["/bin/bash"]
# Sat, 14 Nov 2020 01:01:33 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 14 Nov 2020 01:01:33 GMT
ARG ASSET=ce
# Sat, 14 Nov 2020 01:01:34 GMT
ENV ASSET=ce
# Sat, 14 Nov 2020 01:01:34 GMT
ARG EE_PORTS
# Sat, 14 Nov 2020 01:01:34 GMT
COPY file:ff02c070e4c89f043b176279a7e41464b5fab8cb98cfcd6332fad2d2741fc41d in /tmp/kong.rpm 
# Sat, 14 Nov 2020 01:02:16 GMT
ARG KONG_VERSION=2.1.4
# Sat, 14 Nov 2020 01:02:16 GMT
ENV KONG_VERSION=2.1.4
# Sat, 14 Nov 2020 01:02:16 GMT
ARG KONG_SHA256=5f44985dcf79e0ad59463b3e3eb9d6623dc9234793bd9c108c0eac8d65b62ab0
# Sat, 14 Nov 2020 01:02:42 GMT
# ARGS: KONG_SHA256=5f44985dcf79e0ad59463b3e3eb9d6623dc9234793bd9c108c0eac8d65b62ab0
RUN set -ex; 	if [ "$ASSET" = "ce" ] ; then 		curl -fL "https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm" -o /tmp/kong.rpm 		&& echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -; 	fi; 	yum install -y -q unzip shadow-utils git 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki 	&& useradd kong 	&& mkdir -p "/usr/local/kong" 	&& yum --nogpgcheck localinstall -y /tmp/kong.rpm 	&& yum clean all 	&& rm /tmp/kong.rpm 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Sat, 14 Nov 2020 01:02:42 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Sat, 14 Nov 2020 01:02:43 GMT
USER kong
# Sat, 14 Nov 2020 01:02:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 14 Nov 2020 01:02:43 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 14 Nov 2020 01:02:43 GMT
STOPSIGNAL SIGQUIT
# Sat, 14 Nov 2020 01:02:43 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4dc7c6a187fe570e563de224bd35775b78d3ff78f05cf73c4e08319b2dc232`  
		Last Modified: Sat, 14 Nov 2020 01:03:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a690a7e5955b5f53b5859ac1391b51d1584818a0bbc504061e654b26d4d71f`  
		Last Modified: Sat, 14 Nov 2020 01:04:13 GMT  
		Size: 51.2 MB (51162000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4dd8889546b4ae415188145fb1dde0b9c303884420d3874d1673772dd91321`  
		Last Modified: Sat, 14 Nov 2020 01:04:01 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.1.4-ubuntu`

```console
$ docker pull kong@sha256:fbb43a92e427a8c475ca9aeab6da893dcbe664c2f5fe8662a4d9097ac8dc5a04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.1.4-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:c217a71f4c1b03322b0cb0cdaf0ef0f43cad8c383bbe7965df2c321769baafb9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.9 MB (133892825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6b939a024df189cd0c5d8d1b18bab5c712caae887c9b0f1952f0dd501cb55ee`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 21 Jan 2021 03:39:31 GMT
ADD file:925571658dd8453e5c80d862f5791d6b26b3c2a8688937b11741f2f2c5cdbfd7 in / 
# Thu, 21 Jan 2021 03:39:32 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:39:34 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:39:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:39:36 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 10:27:05 GMT
ARG ASSET=ce
# Thu, 21 Jan 2021 10:27:05 GMT
ENV ASSET=ce
# Thu, 21 Jan 2021 10:27:05 GMT
ARG EE_PORTS
# Thu, 21 Jan 2021 10:27:06 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Thu, 21 Jan 2021 10:28:29 GMT
ARG KONG_VERSION=2.1.4
# Thu, 21 Jan 2021 10:28:29 GMT
ENV KONG_VERSION=2.1.4
# Thu, 21 Jan 2021 10:28:53 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt update 	&& apt install --yes /tmp/kong.deb 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Thu, 21 Jan 2021 10:28:54 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Thu, 21 Jan 2021 10:28:54 GMT
USER kong
# Thu, 21 Jan 2021 10:28:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 21 Jan 2021 10:28:54 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 21 Jan 2021 10:28:55 GMT
STOPSIGNAL SIGQUIT
# Thu, 21 Jan 2021 10:28:55 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4007a89234b4f56c03e6831dc220550d2e5fba935d9f5f5bcea64857ac4f4888`  
		Last Modified: Mon, 18 Jan 2021 19:38:08 GMT  
		Size: 46.0 MB (45962352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfa26c6b9c9d1ccbcb1eaa65befa376805d9324174ac580ca76fdedc3575f54`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba7bf18aa406cb7dc372ac732de222b04d1c824ff1705d8900831c3d1361ff5`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6ec688ebe374ea7d89ce967576d221a177ebd2c02ca9f053197f954102e30b`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7491b48e51562c145461304393cbc54944e319e09a7714bf0e4264da38b8a8f0`  
		Last Modified: Thu, 21 Jan 2021 10:30:38 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478fb2c434a20e74e5b8e75ac9bee465de878d648ea39cd63d103f13094e148c`  
		Last Modified: Thu, 21 Jan 2021 10:31:36 GMT  
		Size: 62.8 MB (62846282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72b38df337740461e6803aeffe82a6b1667ea01b7ad839bebd14044c0b47ec4c`  
		Last Modified: Thu, 21 Jan 2021 10:31:24 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.1.4-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:49baf2f4e15be6f983e1c64447cac8320374e4febeecdb236d31baf651756995
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125199807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff1fde0c7a655bd82a5ce2e18ae7ffa4d9ed68905b1182906263de7418295374`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 21 Jan 2021 03:51:12 GMT
ADD file:e2f37be259f081b70bc884e3b7f652e5d9a0ad4ae443f2258b79a1b14377cc20 in / 
# Thu, 21 Jan 2021 03:51:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:51:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:51:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:51:22 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:32:05 GMT
ARG ASSET=ce
# Thu, 21 Jan 2021 05:32:06 GMT
ENV ASSET=ce
# Thu, 21 Jan 2021 05:32:06 GMT
ARG EE_PORTS
# Thu, 21 Jan 2021 05:32:07 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Thu, 21 Jan 2021 05:34:29 GMT
ARG KONG_VERSION=2.1.4
# Thu, 21 Jan 2021 05:34:30 GMT
ENV KONG_VERSION=2.1.4
# Thu, 21 Jan 2021 05:35:34 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt update 	&& apt install --yes /tmp/kong.deb 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Thu, 21 Jan 2021 05:35:37 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Thu, 21 Jan 2021 05:35:38 GMT
USER kong
# Thu, 21 Jan 2021 05:35:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:35:39 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 21 Jan 2021 05:35:40 GMT
STOPSIGNAL SIGQUIT
# Thu, 21 Jan 2021 05:35:40 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:79186a4c5361c6b018fe75c9bba66c9bf717db8d7d4a6ddb18fb86171f277b61`  
		Last Modified: Thu, 14 Jan 2021 16:25:21 GMT  
		Size: 40.9 MB (40885219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96f901e8ebcf64a42ec369549f6269ec96cd97b424389ca99a8ebb722c59c12`  
		Last Modified: Thu, 21 Jan 2021 03:53:10 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36fd1545244608cb9ef92efa528b6e8c3229f1b01ca414ee8717219145cdff7d`  
		Last Modified: Thu, 21 Jan 2021 03:53:10 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d978c0f55122642ba1a22cc67abf7af2e898bfb42933b1879c2dd91fd987147d`  
		Last Modified: Thu, 21 Jan 2021 03:53:11 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e81e83cdfa4fc6fce4a28de27bb31753456d14bad0dcc25aabceaa0a03a3345`  
		Last Modified: Thu, 21 Jan 2021 05:37:21 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ac4802aab8eabcd73e4641d6fe9c881be6b1d4564d4e3908ac28ae82444846f`  
		Last Modified: Thu, 21 Jan 2021 05:38:36 GMT  
		Size: 59.2 MB (59230458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6220a51772734a4fe75e8179450595e1682af3caec53ce05dd7891e8accb5811`  
		Last Modified: Thu, 21 Jan 2021 05:38:20 GMT  
		Size: 688.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.1-alpine`

```console
$ docker pull kong@sha256:fd785a4fb730f27723ee2012871a4649cc8efedeed2e07b933221371eeb6bfaf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.1-alpine` - linux; amd64

```console
$ docker pull kong@sha256:66638610c5199438e899b6f97ea5aa615bc5ecfda9e940595f4456252736fefd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53151918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bda17790f5d47993bb5da2b47ced574cd11d090e263b49ac8eab6a95d0a4388`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 14:57:37 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 17 Dec 2020 14:57:37 GMT
ARG ASSET=ce
# Thu, 17 Dec 2020 14:57:37 GMT
ENV ASSET=ce
# Thu, 17 Dec 2020 14:57:37 GMT
ARG EE_PORTS
# Thu, 17 Dec 2020 14:57:38 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 17 Dec 2020 14:57:59 GMT
ARG KONG_VERSION=2.1.4
# Thu, 17 Dec 2020 14:57:59 GMT
ENV KONG_VERSION=2.1.4
# Thu, 17 Dec 2020 14:58:07 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256='760cea1f7a058be6000e14dfecfeb73cc79245f696f18e0fcf0825935b944ab3' ;; 		aarch64) arch='arm64'; KONG_SHA256='08038f49f162ab5edc357d7712e90241f6571027cb8741b15ba0c951653764c2' ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong; 	tar -C /kong -xzf /tmp/kong.tar.gz && 	mv /kong/usr/local/* /usr/local && 	mv /kong/etc/* /etc && 	rm -rf /kong && 	apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates && 	adduser -S kong && 	mkdir -p "/usr/local/kong" && 	chown -R kong:0 /usr/local/kong && 	chown kong:0 /usr/local/bin/kong && 	chmod -R g=u /usr/local/kong && 	rm -rf /tmp/kong.tar.gz &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Thu, 17 Dec 2020 14:58:07 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 17 Dec 2020 14:58:07 GMT
USER kong
# Thu, 17 Dec 2020 14:58:07 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 14:58:08 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 17 Dec 2020 14:58:08 GMT
STOPSIGNAL SIGQUIT
# Thu, 17 Dec 2020 14:58:08 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274efec6805c2b13808c7bcb7932f07b136c0be74bf02bdbf77f79e89dc58725`  
		Last Modified: Thu, 17 Dec 2020 14:59:10 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225b0abb30a19fff4fd85428b236bca3911068e5a902d535da6ab539e8d4e319`  
		Last Modified: Thu, 17 Dec 2020 14:59:45 GMT  
		Size: 50.3 MB (50336188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8997b6b5c0e212034dac86dd776b393c56687021b90a68bfd5164dbd482afd9`  
		Last Modified: Thu, 17 Dec 2020 14:59:36 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.1-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:2ada4f5522df9afdcc8230d55d29842c321585b16258c46616a6d1e7ef8dc7a8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.7 MB (52665031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d349242092b941662b5f7463ac4a33d865746d92ca9dfbf5ace92391d5cb0b5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:57:05 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 17 Dec 2020 04:57:06 GMT
ARG ASSET=ce
# Thu, 17 Dec 2020 04:57:07 GMT
ENV ASSET=ce
# Thu, 17 Dec 2020 04:57:08 GMT
ARG EE_PORTS
# Thu, 17 Dec 2020 04:57:09 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 17 Dec 2020 04:57:51 GMT
ARG KONG_VERSION=2.1.4
# Thu, 17 Dec 2020 04:57:53 GMT
ENV KONG_VERSION=2.1.4
# Thu, 17 Dec 2020 04:58:04 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256='760cea1f7a058be6000e14dfecfeb73cc79245f696f18e0fcf0825935b944ab3' ;; 		aarch64) arch='arm64'; KONG_SHA256='08038f49f162ab5edc357d7712e90241f6571027cb8741b15ba0c951653764c2' ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong; 	tar -C /kong -xzf /tmp/kong.tar.gz && 	mv /kong/usr/local/* /usr/local && 	mv /kong/etc/* /etc && 	rm -rf /kong && 	apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates && 	adduser -S kong && 	mkdir -p "/usr/local/kong" && 	chown -R kong:0 /usr/local/kong && 	chown kong:0 /usr/local/bin/kong && 	chmod -R g=u /usr/local/kong && 	rm -rf /tmp/kong.tar.gz &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Thu, 17 Dec 2020 04:58:06 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 17 Dec 2020 04:58:08 GMT
USER kong
# Thu, 17 Dec 2020 04:58:09 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 04:58:09 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 17 Dec 2020 04:58:10 GMT
STOPSIGNAL SIGQUIT
# Thu, 17 Dec 2020 04:58:11 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:20d8a246443a66e74e17f2a0e81a51fe774876ca0c2676691c37ee1b0e4d3cd5`  
		Last Modified: Wed, 16 Dec 2020 23:41:20 GMT  
		Size: 2.7 MB (2725216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3181cc464c4af55ff9dd73d4603f67578cdc16237deb0e5e467594b40164ab6`  
		Last Modified: Thu, 17 Dec 2020 04:58:48 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e8c4352649944a52a45f73f8267085e3e8f5f8c42cd7916f17e194af442ccdd`  
		Last Modified: Thu, 17 Dec 2020 04:59:39 GMT  
		Size: 49.9 MB (49938950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c2b84fa76be82f6d536a0c0a486863650800cfad97b972c7753461f8f4e3bc`  
		Last Modified: Thu, 17 Dec 2020 04:59:23 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.1-centos`

```console
$ docker pull kong@sha256:2074a8dbc332a2d158a41f480915d2cca721cd24449a36a956d673b992551da0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.1-centos` - linux; amd64

```console
$ docker pull kong@sha256:9abae830a109a6c87cf973fab99656a87fe37c1a53c195d79fa8b2448d85a75d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.3 MB (127260020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05a08e453725f88199609cc19d52cc849a8b829755d8ea61b90d497a84e9c4b3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 14 Nov 2020 00:20:04 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Sat, 14 Nov 2020 00:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Sat, 14 Nov 2020 00:20:04 GMT
CMD ["/bin/bash"]
# Sat, 14 Nov 2020 01:01:33 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 14 Nov 2020 01:01:33 GMT
ARG ASSET=ce
# Sat, 14 Nov 2020 01:01:34 GMT
ENV ASSET=ce
# Sat, 14 Nov 2020 01:01:34 GMT
ARG EE_PORTS
# Sat, 14 Nov 2020 01:01:34 GMT
COPY file:ff02c070e4c89f043b176279a7e41464b5fab8cb98cfcd6332fad2d2741fc41d in /tmp/kong.rpm 
# Sat, 14 Nov 2020 01:02:16 GMT
ARG KONG_VERSION=2.1.4
# Sat, 14 Nov 2020 01:02:16 GMT
ENV KONG_VERSION=2.1.4
# Sat, 14 Nov 2020 01:02:16 GMT
ARG KONG_SHA256=5f44985dcf79e0ad59463b3e3eb9d6623dc9234793bd9c108c0eac8d65b62ab0
# Sat, 14 Nov 2020 01:02:42 GMT
# ARGS: KONG_SHA256=5f44985dcf79e0ad59463b3e3eb9d6623dc9234793bd9c108c0eac8d65b62ab0
RUN set -ex; 	if [ "$ASSET" = "ce" ] ; then 		curl -fL "https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm" -o /tmp/kong.rpm 		&& echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -; 	fi; 	yum install -y -q unzip shadow-utils git 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki 	&& useradd kong 	&& mkdir -p "/usr/local/kong" 	&& yum --nogpgcheck localinstall -y /tmp/kong.rpm 	&& yum clean all 	&& rm /tmp/kong.rpm 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Sat, 14 Nov 2020 01:02:42 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Sat, 14 Nov 2020 01:02:43 GMT
USER kong
# Sat, 14 Nov 2020 01:02:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 14 Nov 2020 01:02:43 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 14 Nov 2020 01:02:43 GMT
STOPSIGNAL SIGQUIT
# Sat, 14 Nov 2020 01:02:43 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4dc7c6a187fe570e563de224bd35775b78d3ff78f05cf73c4e08319b2dc232`  
		Last Modified: Sat, 14 Nov 2020 01:03:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a690a7e5955b5f53b5859ac1391b51d1584818a0bbc504061e654b26d4d71f`  
		Last Modified: Sat, 14 Nov 2020 01:04:13 GMT  
		Size: 51.2 MB (51162000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4dd8889546b4ae415188145fb1dde0b9c303884420d3874d1673772dd91321`  
		Last Modified: Sat, 14 Nov 2020 01:04:01 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.1-ubuntu`

```console
$ docker pull kong@sha256:fbb43a92e427a8c475ca9aeab6da893dcbe664c2f5fe8662a4d9097ac8dc5a04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.1-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:c217a71f4c1b03322b0cb0cdaf0ef0f43cad8c383bbe7965df2c321769baafb9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.9 MB (133892825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6b939a024df189cd0c5d8d1b18bab5c712caae887c9b0f1952f0dd501cb55ee`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 21 Jan 2021 03:39:31 GMT
ADD file:925571658dd8453e5c80d862f5791d6b26b3c2a8688937b11741f2f2c5cdbfd7 in / 
# Thu, 21 Jan 2021 03:39:32 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:39:34 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:39:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:39:36 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 10:27:05 GMT
ARG ASSET=ce
# Thu, 21 Jan 2021 10:27:05 GMT
ENV ASSET=ce
# Thu, 21 Jan 2021 10:27:05 GMT
ARG EE_PORTS
# Thu, 21 Jan 2021 10:27:06 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Thu, 21 Jan 2021 10:28:29 GMT
ARG KONG_VERSION=2.1.4
# Thu, 21 Jan 2021 10:28:29 GMT
ENV KONG_VERSION=2.1.4
# Thu, 21 Jan 2021 10:28:53 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt update 	&& apt install --yes /tmp/kong.deb 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Thu, 21 Jan 2021 10:28:54 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Thu, 21 Jan 2021 10:28:54 GMT
USER kong
# Thu, 21 Jan 2021 10:28:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 21 Jan 2021 10:28:54 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 21 Jan 2021 10:28:55 GMT
STOPSIGNAL SIGQUIT
# Thu, 21 Jan 2021 10:28:55 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4007a89234b4f56c03e6831dc220550d2e5fba935d9f5f5bcea64857ac4f4888`  
		Last Modified: Mon, 18 Jan 2021 19:38:08 GMT  
		Size: 46.0 MB (45962352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfa26c6b9c9d1ccbcb1eaa65befa376805d9324174ac580ca76fdedc3575f54`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba7bf18aa406cb7dc372ac732de222b04d1c824ff1705d8900831c3d1361ff5`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6ec688ebe374ea7d89ce967576d221a177ebd2c02ca9f053197f954102e30b`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7491b48e51562c145461304393cbc54944e319e09a7714bf0e4264da38b8a8f0`  
		Last Modified: Thu, 21 Jan 2021 10:30:38 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478fb2c434a20e74e5b8e75ac9bee465de878d648ea39cd63d103f13094e148c`  
		Last Modified: Thu, 21 Jan 2021 10:31:36 GMT  
		Size: 62.8 MB (62846282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72b38df337740461e6803aeffe82a6b1667ea01b7ad839bebd14044c0b47ec4c`  
		Last Modified: Thu, 21 Jan 2021 10:31:24 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.1-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:49baf2f4e15be6f983e1c64447cac8320374e4febeecdb236d31baf651756995
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.2 MB (125199807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff1fde0c7a655bd82a5ce2e18ae7ffa4d9ed68905b1182906263de7418295374`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 21 Jan 2021 03:51:12 GMT
ADD file:e2f37be259f081b70bc884e3b7f652e5d9a0ad4ae443f2258b79a1b14377cc20 in / 
# Thu, 21 Jan 2021 03:51:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:51:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:51:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:51:22 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:32:05 GMT
ARG ASSET=ce
# Thu, 21 Jan 2021 05:32:06 GMT
ENV ASSET=ce
# Thu, 21 Jan 2021 05:32:06 GMT
ARG EE_PORTS
# Thu, 21 Jan 2021 05:32:07 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Thu, 21 Jan 2021 05:34:29 GMT
ARG KONG_VERSION=2.1.4
# Thu, 21 Jan 2021 05:34:30 GMT
ENV KONG_VERSION=2.1.4
# Thu, 21 Jan 2021 05:35:34 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt update 	&& apt install --yes /tmp/kong.deb 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Thu, 21 Jan 2021 05:35:37 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Thu, 21 Jan 2021 05:35:38 GMT
USER kong
# Thu, 21 Jan 2021 05:35:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:35:39 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 21 Jan 2021 05:35:40 GMT
STOPSIGNAL SIGQUIT
# Thu, 21 Jan 2021 05:35:40 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:79186a4c5361c6b018fe75c9bba66c9bf717db8d7d4a6ddb18fb86171f277b61`  
		Last Modified: Thu, 14 Jan 2021 16:25:21 GMT  
		Size: 40.9 MB (40885219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96f901e8ebcf64a42ec369549f6269ec96cd97b424389ca99a8ebb722c59c12`  
		Last Modified: Thu, 21 Jan 2021 03:53:10 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36fd1545244608cb9ef92efa528b6e8c3229f1b01ca414ee8717219145cdff7d`  
		Last Modified: Thu, 21 Jan 2021 03:53:10 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d978c0f55122642ba1a22cc67abf7af2e898bfb42933b1879c2dd91fd987147d`  
		Last Modified: Thu, 21 Jan 2021 03:53:11 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e81e83cdfa4fc6fce4a28de27bb31753456d14bad0dcc25aabceaa0a03a3345`  
		Last Modified: Thu, 21 Jan 2021 05:37:21 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ac4802aab8eabcd73e4641d6fe9c881be6b1d4564d4e3908ac28ae82444846f`  
		Last Modified: Thu, 21 Jan 2021 05:38:36 GMT  
		Size: 59.2 MB (59230458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6220a51772734a4fe75e8179450595e1682af3caec53ce05dd7891e8accb5811`  
		Last Modified: Thu, 21 Jan 2021 05:38:20 GMT  
		Size: 688.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.2`

```console
$ docker pull kong@sha256:ca07a0baf23ae4c7591c3ba1905ac048f5701512f026fdf3e037dfa82e8256db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.2` - linux; amd64

```console
$ docker pull kong@sha256:a7d926085080e8d5c225bc9b28475c3b9f355c724140f54b3846337efc4c021a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53279171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a97d41b7e3eb7f30365dadf31733b6aad4854195b47bc80f877249b7d3cf22a7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 14:57:37 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 17 Dec 2020 14:57:37 GMT
ARG ASSET=ce
# Thu, 17 Dec 2020 14:57:37 GMT
ENV ASSET=ce
# Thu, 17 Dec 2020 14:57:37 GMT
ARG EE_PORTS
# Thu, 17 Dec 2020 14:57:38 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 17 Dec 2020 14:57:38 GMT
ARG KONG_VERSION=2.2.1
# Thu, 17 Dec 2020 14:57:38 GMT
ENV KONG_VERSION=2.2.1
# Thu, 17 Dec 2020 14:57:46 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256='e05c7075ae263bb7ef84b0370bf4e31f5246a41d910e5d4336216ae95b654af1' ;; 		aarch64) arch='arm64'; KONG_SHA256='c7b2c0e1f47e3009e55b492344bd1ff689a41eca91c21f2c3f57f9172932c96d' ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Thu, 17 Dec 2020 14:57:46 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 17 Dec 2020 14:57:46 GMT
USER kong
# Thu, 17 Dec 2020 14:57:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 14:57:46 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 17 Dec 2020 14:57:47 GMT
STOPSIGNAL SIGQUIT
# Thu, 17 Dec 2020 14:57:47 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274efec6805c2b13808c7bcb7932f07b136c0be74bf02bdbf77f79e89dc58725`  
		Last Modified: Thu, 17 Dec 2020 14:59:10 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8794d72b045907b1a101e2d81d75b9c9a49656d698300a28812b5bd819fdbcbc`  
		Last Modified: Thu, 17 Dec 2020 14:59:21 GMT  
		Size: 50.5 MB (50463440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2135d06e1a774c8a794cdf438cd9bcf78a1efe921acc3fb477575e9022942ce6`  
		Last Modified: Thu, 17 Dec 2020 14:59:11 GMT  
		Size: 735.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.2` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:d1c2daab221d9e5054c5cd6a7df3e855c056bd8a79cf679833fe069f74ebceaf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.8 MB (52801740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0813154a7843d44b47a393a769eedcf892d4c234e21226c7e3b03e9d496d652`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:57:05 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 17 Dec 2020 04:57:06 GMT
ARG ASSET=ce
# Thu, 17 Dec 2020 04:57:07 GMT
ENV ASSET=ce
# Thu, 17 Dec 2020 04:57:08 GMT
ARG EE_PORTS
# Thu, 17 Dec 2020 04:57:09 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 17 Dec 2020 04:57:11 GMT
ARG KONG_VERSION=2.2.1
# Thu, 17 Dec 2020 04:57:12 GMT
ENV KONG_VERSION=2.2.1
# Thu, 17 Dec 2020 04:57:30 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256='e05c7075ae263bb7ef84b0370bf4e31f5246a41d910e5d4336216ae95b654af1' ;; 		aarch64) arch='arm64'; KONG_SHA256='c7b2c0e1f47e3009e55b492344bd1ff689a41eca91c21f2c3f57f9172932c96d' ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Thu, 17 Dec 2020 04:57:33 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 17 Dec 2020 04:57:35 GMT
USER kong
# Thu, 17 Dec 2020 04:57:37 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 04:57:37 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 17 Dec 2020 04:57:38 GMT
STOPSIGNAL SIGQUIT
# Thu, 17 Dec 2020 04:57:39 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:20d8a246443a66e74e17f2a0e81a51fe774876ca0c2676691c37ee1b0e4d3cd5`  
		Last Modified: Wed, 16 Dec 2020 23:41:20 GMT  
		Size: 2.7 MB (2725216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3181cc464c4af55ff9dd73d4603f67578cdc16237deb0e5e467594b40164ab6`  
		Last Modified: Thu, 17 Dec 2020 04:58:48 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73439c4e6c349f3f7edf0a15636c8b402f48bc351c48dfd010aa03c8a980a0ff`  
		Last Modified: Thu, 17 Dec 2020 04:59:05 GMT  
		Size: 50.1 MB (50075659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ae76d2ad481a47953973f988b2abfb80a24ff497eb267680d4a0b68f2da543`  
		Last Modified: Thu, 17 Dec 2020 04:58:48 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.2.0`

```console
$ docker pull kong@sha256:ca07a0baf23ae4c7591c3ba1905ac048f5701512f026fdf3e037dfa82e8256db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.2.0` - linux; amd64

```console
$ docker pull kong@sha256:a7d926085080e8d5c225bc9b28475c3b9f355c724140f54b3846337efc4c021a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53279171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a97d41b7e3eb7f30365dadf31733b6aad4854195b47bc80f877249b7d3cf22a7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 14:57:37 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 17 Dec 2020 14:57:37 GMT
ARG ASSET=ce
# Thu, 17 Dec 2020 14:57:37 GMT
ENV ASSET=ce
# Thu, 17 Dec 2020 14:57:37 GMT
ARG EE_PORTS
# Thu, 17 Dec 2020 14:57:38 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 17 Dec 2020 14:57:38 GMT
ARG KONG_VERSION=2.2.1
# Thu, 17 Dec 2020 14:57:38 GMT
ENV KONG_VERSION=2.2.1
# Thu, 17 Dec 2020 14:57:46 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256='e05c7075ae263bb7ef84b0370bf4e31f5246a41d910e5d4336216ae95b654af1' ;; 		aarch64) arch='arm64'; KONG_SHA256='c7b2c0e1f47e3009e55b492344bd1ff689a41eca91c21f2c3f57f9172932c96d' ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Thu, 17 Dec 2020 14:57:46 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 17 Dec 2020 14:57:46 GMT
USER kong
# Thu, 17 Dec 2020 14:57:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 14:57:46 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 17 Dec 2020 14:57:47 GMT
STOPSIGNAL SIGQUIT
# Thu, 17 Dec 2020 14:57:47 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274efec6805c2b13808c7bcb7932f07b136c0be74bf02bdbf77f79e89dc58725`  
		Last Modified: Thu, 17 Dec 2020 14:59:10 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8794d72b045907b1a101e2d81d75b9c9a49656d698300a28812b5bd819fdbcbc`  
		Last Modified: Thu, 17 Dec 2020 14:59:21 GMT  
		Size: 50.5 MB (50463440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2135d06e1a774c8a794cdf438cd9bcf78a1efe921acc3fb477575e9022942ce6`  
		Last Modified: Thu, 17 Dec 2020 14:59:11 GMT  
		Size: 735.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.2.0` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:d1c2daab221d9e5054c5cd6a7df3e855c056bd8a79cf679833fe069f74ebceaf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.8 MB (52801740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0813154a7843d44b47a393a769eedcf892d4c234e21226c7e3b03e9d496d652`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:57:05 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 17 Dec 2020 04:57:06 GMT
ARG ASSET=ce
# Thu, 17 Dec 2020 04:57:07 GMT
ENV ASSET=ce
# Thu, 17 Dec 2020 04:57:08 GMT
ARG EE_PORTS
# Thu, 17 Dec 2020 04:57:09 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 17 Dec 2020 04:57:11 GMT
ARG KONG_VERSION=2.2.1
# Thu, 17 Dec 2020 04:57:12 GMT
ENV KONG_VERSION=2.2.1
# Thu, 17 Dec 2020 04:57:30 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256='e05c7075ae263bb7ef84b0370bf4e31f5246a41d910e5d4336216ae95b654af1' ;; 		aarch64) arch='arm64'; KONG_SHA256='c7b2c0e1f47e3009e55b492344bd1ff689a41eca91c21f2c3f57f9172932c96d' ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Thu, 17 Dec 2020 04:57:33 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 17 Dec 2020 04:57:35 GMT
USER kong
# Thu, 17 Dec 2020 04:57:37 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 04:57:37 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 17 Dec 2020 04:57:38 GMT
STOPSIGNAL SIGQUIT
# Thu, 17 Dec 2020 04:57:39 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:20d8a246443a66e74e17f2a0e81a51fe774876ca0c2676691c37ee1b0e4d3cd5`  
		Last Modified: Wed, 16 Dec 2020 23:41:20 GMT  
		Size: 2.7 MB (2725216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3181cc464c4af55ff9dd73d4603f67578cdc16237deb0e5e467594b40164ab6`  
		Last Modified: Thu, 17 Dec 2020 04:58:48 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73439c4e6c349f3f7edf0a15636c8b402f48bc351c48dfd010aa03c8a980a0ff`  
		Last Modified: Thu, 17 Dec 2020 04:59:05 GMT  
		Size: 50.1 MB (50075659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ae76d2ad481a47953973f988b2abfb80a24ff497eb267680d4a0b68f2da543`  
		Last Modified: Thu, 17 Dec 2020 04:58:48 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.2.1-alpine`

```console
$ docker pull kong@sha256:ca07a0baf23ae4c7591c3ba1905ac048f5701512f026fdf3e037dfa82e8256db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.2.1-alpine` - linux; amd64

```console
$ docker pull kong@sha256:a7d926085080e8d5c225bc9b28475c3b9f355c724140f54b3846337efc4c021a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53279171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a97d41b7e3eb7f30365dadf31733b6aad4854195b47bc80f877249b7d3cf22a7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 14:57:37 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 17 Dec 2020 14:57:37 GMT
ARG ASSET=ce
# Thu, 17 Dec 2020 14:57:37 GMT
ENV ASSET=ce
# Thu, 17 Dec 2020 14:57:37 GMT
ARG EE_PORTS
# Thu, 17 Dec 2020 14:57:38 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 17 Dec 2020 14:57:38 GMT
ARG KONG_VERSION=2.2.1
# Thu, 17 Dec 2020 14:57:38 GMT
ENV KONG_VERSION=2.2.1
# Thu, 17 Dec 2020 14:57:46 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256='e05c7075ae263bb7ef84b0370bf4e31f5246a41d910e5d4336216ae95b654af1' ;; 		aarch64) arch='arm64'; KONG_SHA256='c7b2c0e1f47e3009e55b492344bd1ff689a41eca91c21f2c3f57f9172932c96d' ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Thu, 17 Dec 2020 14:57:46 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 17 Dec 2020 14:57:46 GMT
USER kong
# Thu, 17 Dec 2020 14:57:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 14:57:46 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 17 Dec 2020 14:57:47 GMT
STOPSIGNAL SIGQUIT
# Thu, 17 Dec 2020 14:57:47 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274efec6805c2b13808c7bcb7932f07b136c0be74bf02bdbf77f79e89dc58725`  
		Last Modified: Thu, 17 Dec 2020 14:59:10 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8794d72b045907b1a101e2d81d75b9c9a49656d698300a28812b5bd819fdbcbc`  
		Last Modified: Thu, 17 Dec 2020 14:59:21 GMT  
		Size: 50.5 MB (50463440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2135d06e1a774c8a794cdf438cd9bcf78a1efe921acc3fb477575e9022942ce6`  
		Last Modified: Thu, 17 Dec 2020 14:59:11 GMT  
		Size: 735.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.2.1-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:d1c2daab221d9e5054c5cd6a7df3e855c056bd8a79cf679833fe069f74ebceaf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.8 MB (52801740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0813154a7843d44b47a393a769eedcf892d4c234e21226c7e3b03e9d496d652`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:57:05 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 17 Dec 2020 04:57:06 GMT
ARG ASSET=ce
# Thu, 17 Dec 2020 04:57:07 GMT
ENV ASSET=ce
# Thu, 17 Dec 2020 04:57:08 GMT
ARG EE_PORTS
# Thu, 17 Dec 2020 04:57:09 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 17 Dec 2020 04:57:11 GMT
ARG KONG_VERSION=2.2.1
# Thu, 17 Dec 2020 04:57:12 GMT
ENV KONG_VERSION=2.2.1
# Thu, 17 Dec 2020 04:57:30 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256='e05c7075ae263bb7ef84b0370bf4e31f5246a41d910e5d4336216ae95b654af1' ;; 		aarch64) arch='arm64'; KONG_SHA256='c7b2c0e1f47e3009e55b492344bd1ff689a41eca91c21f2c3f57f9172932c96d' ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Thu, 17 Dec 2020 04:57:33 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 17 Dec 2020 04:57:35 GMT
USER kong
# Thu, 17 Dec 2020 04:57:37 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 04:57:37 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 17 Dec 2020 04:57:38 GMT
STOPSIGNAL SIGQUIT
# Thu, 17 Dec 2020 04:57:39 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:20d8a246443a66e74e17f2a0e81a51fe774876ca0c2676691c37ee1b0e4d3cd5`  
		Last Modified: Wed, 16 Dec 2020 23:41:20 GMT  
		Size: 2.7 MB (2725216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3181cc464c4af55ff9dd73d4603f67578cdc16237deb0e5e467594b40164ab6`  
		Last Modified: Thu, 17 Dec 2020 04:58:48 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73439c4e6c349f3f7edf0a15636c8b402f48bc351c48dfd010aa03c8a980a0ff`  
		Last Modified: Thu, 17 Dec 2020 04:59:05 GMT  
		Size: 50.1 MB (50075659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ae76d2ad481a47953973f988b2abfb80a24ff497eb267680d4a0b68f2da543`  
		Last Modified: Thu, 17 Dec 2020 04:58:48 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.2.1-centos`

```console
$ docker pull kong@sha256:ad8632341f4a81d75058c45dff279fa8938f20b2a18d7eae41b843fb2d94f4ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.2.1-centos` - linux; amd64

```console
$ docker pull kong@sha256:6a710cd063951cfe5e89bca7b1f64e68ad1b5ea33f7268fb9ba13c530dcb9307
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127352007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43a665d19b27df8e7b9b66445eeae0c72957bde11c041ee73094b778406c6d86`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 14 Nov 2020 00:20:04 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Sat, 14 Nov 2020 00:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Sat, 14 Nov 2020 00:20:04 GMT
CMD ["/bin/bash"]
# Sat, 14 Nov 2020 01:01:33 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 14 Nov 2020 01:01:33 GMT
ARG ASSET=ce
# Sat, 14 Nov 2020 01:01:34 GMT
ENV ASSET=ce
# Sat, 14 Nov 2020 01:01:34 GMT
ARG EE_PORTS
# Sat, 14 Nov 2020 01:01:34 GMT
COPY file:ff02c070e4c89f043b176279a7e41464b5fab8cb98cfcd6332fad2d2741fc41d in /tmp/kong.rpm 
# Wed, 02 Dec 2020 01:05:53 GMT
ARG KONG_VERSION=2.2.1
# Wed, 02 Dec 2020 01:05:53 GMT
ENV KONG_VERSION=2.2.1
# Wed, 02 Dec 2020 01:05:53 GMT
ARG KONG_SHA256=aed53fd4779559d9ff618c634e4c3c3281cca550d9b1bcdae8e7359602bd6771
# Wed, 02 Dec 2020 01:06:25 GMT
# ARGS: KONG_SHA256=aed53fd4779559d9ff618c634e4c3c3281cca550d9b1bcdae8e7359602bd6771
RUN set -ex;   if [ "$ASSET" = "ce" ] ; then     curl -fL "https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm" -o /tmp/kong.rpm     && echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -;   fi;   yum install -y -q unzip shadow-utils git   && yum clean all -q   && rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki   && yum install -y /tmp/kong.rpm   && yum clean all   && rm /tmp/kong.rpm   && chown kong:0 /usr/local/bin/kong   && chown -R kong:0 /usr/local/kong &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Wed, 02 Dec 2020 01:06:25 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 02 Dec 2020 01:06:25 GMT
USER kong
# Wed, 02 Dec 2020 01:06:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Dec 2020 01:06:26 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 02 Dec 2020 01:06:26 GMT
STOPSIGNAL SIGQUIT
# Wed, 02 Dec 2020 01:06:26 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4dc7c6a187fe570e563de224bd35775b78d3ff78f05cf73c4e08319b2dc232`  
		Last Modified: Sat, 14 Nov 2020 01:03:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ef344440583f6238cd4ca52ab5606f1580aa083301cde2fc96a8a774b86132`  
		Last Modified: Wed, 02 Dec 2020 01:07:59 GMT  
		Size: 51.3 MB (51253987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4f52bbd47f126044058af2b82176e13c002b85536baa59a34e64c9b3f78e70`  
		Last Modified: Wed, 02 Dec 2020 01:07:48 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.2.1-ubuntu`

```console
$ docker pull kong@sha256:06ac94140ba2decd2ef435f85b639f7a2ed7e9727e02637a2a594917897a0aa8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.2.1-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:b9e0f47fc5cd1de5b7b4a66de656beb70a80f14682d05ed1a544b0aedf56bcf9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.0 MB (133971365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6571bd1a9beea71ef9e8413ff7ac5035cf9f508766cdaa9142dcba12432a3b0c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 21 Jan 2021 03:39:31 GMT
ADD file:925571658dd8453e5c80d862f5791d6b26b3c2a8688937b11741f2f2c5cdbfd7 in / 
# Thu, 21 Jan 2021 03:39:32 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:39:34 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:39:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:39:36 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 10:27:05 GMT
ARG ASSET=ce
# Thu, 21 Jan 2021 10:27:05 GMT
ENV ASSET=ce
# Thu, 21 Jan 2021 10:27:05 GMT
ARG EE_PORTS
# Thu, 21 Jan 2021 10:27:06 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Thu, 21 Jan 2021 10:27:46 GMT
ARG KONG_VERSION=2.2.1
# Thu, 21 Jan 2021 10:27:47 GMT
ENV KONG_VERSION=2.2.1
# Thu, 21 Jan 2021 10:28:11 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt update     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Thu, 21 Jan 2021 10:28:12 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Thu, 21 Jan 2021 10:28:12 GMT
USER kong
# Thu, 21 Jan 2021 10:28:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 21 Jan 2021 10:28:12 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 21 Jan 2021 10:28:13 GMT
STOPSIGNAL SIGQUIT
# Thu, 21 Jan 2021 10:28:13 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4007a89234b4f56c03e6831dc220550d2e5fba935d9f5f5bcea64857ac4f4888`  
		Last Modified: Mon, 18 Jan 2021 19:38:08 GMT  
		Size: 46.0 MB (45962352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfa26c6b9c9d1ccbcb1eaa65befa376805d9324174ac580ca76fdedc3575f54`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba7bf18aa406cb7dc372ac732de222b04d1c824ff1705d8900831c3d1361ff5`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6ec688ebe374ea7d89ce967576d221a177ebd2c02ca9f053197f954102e30b`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7491b48e51562c145461304393cbc54944e319e09a7714bf0e4264da38b8a8f0`  
		Last Modified: Thu, 21 Jan 2021 10:30:38 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c723eda59c9aaf83a7cfabf052c52524f972d8b7e7143311cba0c901f9d3fba`  
		Last Modified: Thu, 21 Jan 2021 10:31:12 GMT  
		Size: 62.9 MB (62924822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a06631380cf61805879ae1c3ba484ca939c7e1ead8649519907b9326657599`  
		Last Modified: Thu, 21 Jan 2021 10:31:00 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.2.1-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:1f260bffdb3ba66996ff0dfefb4752c826a10fe2f86671d7680de040b117dc98
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125310381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c06364eb859878bd561e717336897154eb340edd64b397a641760a25bce9b5f6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 21 Jan 2021 03:51:12 GMT
ADD file:e2f37be259f081b70bc884e3b7f652e5d9a0ad4ae443f2258b79a1b14377cc20 in / 
# Thu, 21 Jan 2021 03:51:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:51:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:51:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:51:22 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:32:05 GMT
ARG ASSET=ce
# Thu, 21 Jan 2021 05:32:06 GMT
ENV ASSET=ce
# Thu, 21 Jan 2021 05:32:06 GMT
ARG EE_PORTS
# Thu, 21 Jan 2021 05:32:07 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Thu, 21 Jan 2021 05:33:17 GMT
ARG KONG_VERSION=2.2.1
# Thu, 21 Jan 2021 05:33:18 GMT
ENV KONG_VERSION=2.2.1
# Thu, 21 Jan 2021 05:34:09 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt update     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Thu, 21 Jan 2021 05:34:11 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Thu, 21 Jan 2021 05:34:11 GMT
USER kong
# Thu, 21 Jan 2021 05:34:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:34:13 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 21 Jan 2021 05:34:13 GMT
STOPSIGNAL SIGQUIT
# Thu, 21 Jan 2021 05:34:14 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:79186a4c5361c6b018fe75c9bba66c9bf717db8d7d4a6ddb18fb86171f277b61`  
		Last Modified: Thu, 14 Jan 2021 16:25:21 GMT  
		Size: 40.9 MB (40885219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96f901e8ebcf64a42ec369549f6269ec96cd97b424389ca99a8ebb722c59c12`  
		Last Modified: Thu, 21 Jan 2021 03:53:10 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36fd1545244608cb9ef92efa528b6e8c3229f1b01ca414ee8717219145cdff7d`  
		Last Modified: Thu, 21 Jan 2021 03:53:10 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d978c0f55122642ba1a22cc67abf7af2e898bfb42933b1879c2dd91fd987147d`  
		Last Modified: Thu, 21 Jan 2021 03:53:11 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e81e83cdfa4fc6fce4a28de27bb31753456d14bad0dcc25aabceaa0a03a3345`  
		Last Modified: Thu, 21 Jan 2021 05:37:21 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c07b5f37536d981d099266e8c8e6378a5db1ef1f1fc4eb7237506959e2e467b`  
		Last Modified: Thu, 21 Jan 2021 05:38:06 GMT  
		Size: 59.3 MB (59341032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:325527c598003a1519b9e3b5ae36346af0aacfcf97c4b60f77653fa6c7d821ba`  
		Last Modified: Thu, 21 Jan 2021 05:37:52 GMT  
		Size: 688.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.2-alpine`

```console
$ docker pull kong@sha256:ca07a0baf23ae4c7591c3ba1905ac048f5701512f026fdf3e037dfa82e8256db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.2-alpine` - linux; amd64

```console
$ docker pull kong@sha256:a7d926085080e8d5c225bc9b28475c3b9f355c724140f54b3846337efc4c021a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53279171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a97d41b7e3eb7f30365dadf31733b6aad4854195b47bc80f877249b7d3cf22a7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 14:57:37 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 17 Dec 2020 14:57:37 GMT
ARG ASSET=ce
# Thu, 17 Dec 2020 14:57:37 GMT
ENV ASSET=ce
# Thu, 17 Dec 2020 14:57:37 GMT
ARG EE_PORTS
# Thu, 17 Dec 2020 14:57:38 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 17 Dec 2020 14:57:38 GMT
ARG KONG_VERSION=2.2.1
# Thu, 17 Dec 2020 14:57:38 GMT
ENV KONG_VERSION=2.2.1
# Thu, 17 Dec 2020 14:57:46 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256='e05c7075ae263bb7ef84b0370bf4e31f5246a41d910e5d4336216ae95b654af1' ;; 		aarch64) arch='arm64'; KONG_SHA256='c7b2c0e1f47e3009e55b492344bd1ff689a41eca91c21f2c3f57f9172932c96d' ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Thu, 17 Dec 2020 14:57:46 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 17 Dec 2020 14:57:46 GMT
USER kong
# Thu, 17 Dec 2020 14:57:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 14:57:46 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 17 Dec 2020 14:57:47 GMT
STOPSIGNAL SIGQUIT
# Thu, 17 Dec 2020 14:57:47 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274efec6805c2b13808c7bcb7932f07b136c0be74bf02bdbf77f79e89dc58725`  
		Last Modified: Thu, 17 Dec 2020 14:59:10 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8794d72b045907b1a101e2d81d75b9c9a49656d698300a28812b5bd819fdbcbc`  
		Last Modified: Thu, 17 Dec 2020 14:59:21 GMT  
		Size: 50.5 MB (50463440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2135d06e1a774c8a794cdf438cd9bcf78a1efe921acc3fb477575e9022942ce6`  
		Last Modified: Thu, 17 Dec 2020 14:59:11 GMT  
		Size: 735.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.2-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:d1c2daab221d9e5054c5cd6a7df3e855c056bd8a79cf679833fe069f74ebceaf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.8 MB (52801740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0813154a7843d44b47a393a769eedcf892d4c234e21226c7e3b03e9d496d652`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:57:05 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 17 Dec 2020 04:57:06 GMT
ARG ASSET=ce
# Thu, 17 Dec 2020 04:57:07 GMT
ENV ASSET=ce
# Thu, 17 Dec 2020 04:57:08 GMT
ARG EE_PORTS
# Thu, 17 Dec 2020 04:57:09 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 17 Dec 2020 04:57:11 GMT
ARG KONG_VERSION=2.2.1
# Thu, 17 Dec 2020 04:57:12 GMT
ENV KONG_VERSION=2.2.1
# Thu, 17 Dec 2020 04:57:30 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256='e05c7075ae263bb7ef84b0370bf4e31f5246a41d910e5d4336216ae95b654af1' ;; 		aarch64) arch='arm64'; KONG_SHA256='c7b2c0e1f47e3009e55b492344bd1ff689a41eca91c21f2c3f57f9172932c96d' ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Thu, 17 Dec 2020 04:57:33 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 17 Dec 2020 04:57:35 GMT
USER kong
# Thu, 17 Dec 2020 04:57:37 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Dec 2020 04:57:37 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 17 Dec 2020 04:57:38 GMT
STOPSIGNAL SIGQUIT
# Thu, 17 Dec 2020 04:57:39 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:20d8a246443a66e74e17f2a0e81a51fe774876ca0c2676691c37ee1b0e4d3cd5`  
		Last Modified: Wed, 16 Dec 2020 23:41:20 GMT  
		Size: 2.7 MB (2725216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3181cc464c4af55ff9dd73d4603f67578cdc16237deb0e5e467594b40164ab6`  
		Last Modified: Thu, 17 Dec 2020 04:58:48 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73439c4e6c349f3f7edf0a15636c8b402f48bc351c48dfd010aa03c8a980a0ff`  
		Last Modified: Thu, 17 Dec 2020 04:59:05 GMT  
		Size: 50.1 MB (50075659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ae76d2ad481a47953973f988b2abfb80a24ff497eb267680d4a0b68f2da543`  
		Last Modified: Thu, 17 Dec 2020 04:58:48 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.2-centos`

```console
$ docker pull kong@sha256:ad8632341f4a81d75058c45dff279fa8938f20b2a18d7eae41b843fb2d94f4ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.2-centos` - linux; amd64

```console
$ docker pull kong@sha256:6a710cd063951cfe5e89bca7b1f64e68ad1b5ea33f7268fb9ba13c530dcb9307
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127352007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43a665d19b27df8e7b9b66445eeae0c72957bde11c041ee73094b778406c6d86`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 14 Nov 2020 00:20:04 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Sat, 14 Nov 2020 00:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Sat, 14 Nov 2020 00:20:04 GMT
CMD ["/bin/bash"]
# Sat, 14 Nov 2020 01:01:33 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 14 Nov 2020 01:01:33 GMT
ARG ASSET=ce
# Sat, 14 Nov 2020 01:01:34 GMT
ENV ASSET=ce
# Sat, 14 Nov 2020 01:01:34 GMT
ARG EE_PORTS
# Sat, 14 Nov 2020 01:01:34 GMT
COPY file:ff02c070e4c89f043b176279a7e41464b5fab8cb98cfcd6332fad2d2741fc41d in /tmp/kong.rpm 
# Wed, 02 Dec 2020 01:05:53 GMT
ARG KONG_VERSION=2.2.1
# Wed, 02 Dec 2020 01:05:53 GMT
ENV KONG_VERSION=2.2.1
# Wed, 02 Dec 2020 01:05:53 GMT
ARG KONG_SHA256=aed53fd4779559d9ff618c634e4c3c3281cca550d9b1bcdae8e7359602bd6771
# Wed, 02 Dec 2020 01:06:25 GMT
# ARGS: KONG_SHA256=aed53fd4779559d9ff618c634e4c3c3281cca550d9b1bcdae8e7359602bd6771
RUN set -ex;   if [ "$ASSET" = "ce" ] ; then     curl -fL "https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm" -o /tmp/kong.rpm     && echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -;   fi;   yum install -y -q unzip shadow-utils git   && yum clean all -q   && rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki   && yum install -y /tmp/kong.rpm   && yum clean all   && rm /tmp/kong.rpm   && chown kong:0 /usr/local/bin/kong   && chown -R kong:0 /usr/local/kong &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Wed, 02 Dec 2020 01:06:25 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 02 Dec 2020 01:06:25 GMT
USER kong
# Wed, 02 Dec 2020 01:06:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 02 Dec 2020 01:06:26 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 02 Dec 2020 01:06:26 GMT
STOPSIGNAL SIGQUIT
# Wed, 02 Dec 2020 01:06:26 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4dc7c6a187fe570e563de224bd35775b78d3ff78f05cf73c4e08319b2dc232`  
		Last Modified: Sat, 14 Nov 2020 01:03:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ef344440583f6238cd4ca52ab5606f1580aa083301cde2fc96a8a774b86132`  
		Last Modified: Wed, 02 Dec 2020 01:07:59 GMT  
		Size: 51.3 MB (51253987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4f52bbd47f126044058af2b82176e13c002b85536baa59a34e64c9b3f78e70`  
		Last Modified: Wed, 02 Dec 2020 01:07:48 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.2-ubuntu`

```console
$ docker pull kong@sha256:06ac94140ba2decd2ef435f85b639f7a2ed7e9727e02637a2a594917897a0aa8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.2-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:b9e0f47fc5cd1de5b7b4a66de656beb70a80f14682d05ed1a544b0aedf56bcf9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.0 MB (133971365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6571bd1a9beea71ef9e8413ff7ac5035cf9f508766cdaa9142dcba12432a3b0c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 21 Jan 2021 03:39:31 GMT
ADD file:925571658dd8453e5c80d862f5791d6b26b3c2a8688937b11741f2f2c5cdbfd7 in / 
# Thu, 21 Jan 2021 03:39:32 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:39:34 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:39:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:39:36 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 10:27:05 GMT
ARG ASSET=ce
# Thu, 21 Jan 2021 10:27:05 GMT
ENV ASSET=ce
# Thu, 21 Jan 2021 10:27:05 GMT
ARG EE_PORTS
# Thu, 21 Jan 2021 10:27:06 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Thu, 21 Jan 2021 10:27:46 GMT
ARG KONG_VERSION=2.2.1
# Thu, 21 Jan 2021 10:27:47 GMT
ENV KONG_VERSION=2.2.1
# Thu, 21 Jan 2021 10:28:11 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt update     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Thu, 21 Jan 2021 10:28:12 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Thu, 21 Jan 2021 10:28:12 GMT
USER kong
# Thu, 21 Jan 2021 10:28:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 21 Jan 2021 10:28:12 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 21 Jan 2021 10:28:13 GMT
STOPSIGNAL SIGQUIT
# Thu, 21 Jan 2021 10:28:13 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4007a89234b4f56c03e6831dc220550d2e5fba935d9f5f5bcea64857ac4f4888`  
		Last Modified: Mon, 18 Jan 2021 19:38:08 GMT  
		Size: 46.0 MB (45962352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfa26c6b9c9d1ccbcb1eaa65befa376805d9324174ac580ca76fdedc3575f54`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba7bf18aa406cb7dc372ac732de222b04d1c824ff1705d8900831c3d1361ff5`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6ec688ebe374ea7d89ce967576d221a177ebd2c02ca9f053197f954102e30b`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7491b48e51562c145461304393cbc54944e319e09a7714bf0e4264da38b8a8f0`  
		Last Modified: Thu, 21 Jan 2021 10:30:38 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c723eda59c9aaf83a7cfabf052c52524f972d8b7e7143311cba0c901f9d3fba`  
		Last Modified: Thu, 21 Jan 2021 10:31:12 GMT  
		Size: 62.9 MB (62924822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a06631380cf61805879ae1c3ba484ca939c7e1ead8649519907b9326657599`  
		Last Modified: Thu, 21 Jan 2021 10:31:00 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.2-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:1f260bffdb3ba66996ff0dfefb4752c826a10fe2f86671d7680de040b117dc98
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125310381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c06364eb859878bd561e717336897154eb340edd64b397a641760a25bce9b5f6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 21 Jan 2021 03:51:12 GMT
ADD file:e2f37be259f081b70bc884e3b7f652e5d9a0ad4ae443f2258b79a1b14377cc20 in / 
# Thu, 21 Jan 2021 03:51:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:51:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:51:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:51:22 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:32:05 GMT
ARG ASSET=ce
# Thu, 21 Jan 2021 05:32:06 GMT
ENV ASSET=ce
# Thu, 21 Jan 2021 05:32:06 GMT
ARG EE_PORTS
# Thu, 21 Jan 2021 05:32:07 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Thu, 21 Jan 2021 05:33:17 GMT
ARG KONG_VERSION=2.2.1
# Thu, 21 Jan 2021 05:33:18 GMT
ENV KONG_VERSION=2.2.1
# Thu, 21 Jan 2021 05:34:09 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt update     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Thu, 21 Jan 2021 05:34:11 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Thu, 21 Jan 2021 05:34:11 GMT
USER kong
# Thu, 21 Jan 2021 05:34:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 21 Jan 2021 05:34:13 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 21 Jan 2021 05:34:13 GMT
STOPSIGNAL SIGQUIT
# Thu, 21 Jan 2021 05:34:14 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:79186a4c5361c6b018fe75c9bba66c9bf717db8d7d4a6ddb18fb86171f277b61`  
		Last Modified: Thu, 14 Jan 2021 16:25:21 GMT  
		Size: 40.9 MB (40885219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96f901e8ebcf64a42ec369549f6269ec96cd97b424389ca99a8ebb722c59c12`  
		Last Modified: Thu, 21 Jan 2021 03:53:10 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36fd1545244608cb9ef92efa528b6e8c3229f1b01ca414ee8717219145cdff7d`  
		Last Modified: Thu, 21 Jan 2021 03:53:10 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d978c0f55122642ba1a22cc67abf7af2e898bfb42933b1879c2dd91fd987147d`  
		Last Modified: Thu, 21 Jan 2021 03:53:11 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e81e83cdfa4fc6fce4a28de27bb31753456d14bad0dcc25aabceaa0a03a3345`  
		Last Modified: Thu, 21 Jan 2021 05:37:21 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c07b5f37536d981d099266e8c8e6378a5db1ef1f1fc4eb7237506959e2e467b`  
		Last Modified: Thu, 21 Jan 2021 05:38:06 GMT  
		Size: 59.3 MB (59341032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:325527c598003a1519b9e3b5ae36346af0aacfcf97c4b60f77653fa6c7d821ba`  
		Last Modified: Thu, 21 Jan 2021 05:37:52 GMT  
		Size: 688.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.3`

```console
$ docker pull kong@sha256:38c82bcf40f627c1ed3edef3eb0ac9ab3d1fb29fe7eb8df69f5166b324a22153
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.3` - linux; amd64

```console
$ docker pull kong@sha256:eaf0443b11346f6b7f4ac6c0979430462e5070b86a31f5cb2b16a0477773c715
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.9 MB (50938328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cd6edfe129b1c02465b0927dcfdc0d52765486279f5916a2c24d06f070dbd95`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 14:57:37 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 17 Dec 2020 14:57:37 GMT
ARG ASSET=ce
# Thu, 17 Dec 2020 14:57:37 GMT
ENV ASSET=ce
# Thu, 17 Dec 2020 14:57:37 GMT
ARG EE_PORTS
# Thu, 17 Dec 2020 14:57:38 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 27 Jan 2021 06:32:07 GMT
ARG KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 06:32:07 GMT
ENV KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 06:32:07 GMT
ARG KONG_AMD64_SHA=8a33a919f75bdb8bb708de23c0701def2aedfcd2679d27b7849040c3edf273f9
# Wed, 27 Jan 2021 06:32:07 GMT
ENV KONG_AMD64_SHA=8a33a919f75bdb8bb708de23c0701def2aedfcd2679d27b7849040c3edf273f9
# Wed, 27 Jan 2021 06:32:08 GMT
ARG KONG_ARM64_SHA=4ae43ecf9b1fcf11930d859efec475e216729b89b76de80a4c38e1fe58e3874f
# Wed, 27 Jan 2021 06:32:08 GMT
ENV KONG_ARM64_SHA=4ae43ecf9b1fcf11930d859efec475e216729b89b76de80a4c38e1fe58e3874f
# Wed, 27 Jan 2021 06:32:15 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;; 		aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Wed, 27 Jan 2021 06:32:16 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 27 Jan 2021 06:32:16 GMT
USER kong
# Wed, 27 Jan 2021 06:32:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 27 Jan 2021 06:32:16 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 27 Jan 2021 06:32:16 GMT
STOPSIGNAL SIGQUIT
# Wed, 27 Jan 2021 06:32:17 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274efec6805c2b13808c7bcb7932f07b136c0be74bf02bdbf77f79e89dc58725`  
		Last Modified: Thu, 17 Dec 2020 14:59:10 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b18e55f2934bb191d816e87b86e196e1c8d35d815f72f93f7e5f51c0f17319e`  
		Last Modified: Wed, 27 Jan 2021 06:35:34 GMT  
		Size: 48.1 MB (48122597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec1f7f35984e4dfe3874035c9af0e74955cc49424e7f4a0d50411d336f9228fa`  
		Last Modified: Wed, 27 Jan 2021 06:35:24 GMT  
		Size: 735.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.3` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:d87959fb87a61b8f9fba68a010a6e444317df9ca4bbba731d1374c9035077d0e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50462144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:065a1ea94079d9d30ef22ca0cbfffc961327ac4759c8ab96e9473a3daeb1b436`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:57:05 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 17 Dec 2020 04:57:06 GMT
ARG ASSET=ce
# Thu, 17 Dec 2020 04:57:07 GMT
ENV ASSET=ce
# Thu, 17 Dec 2020 04:57:08 GMT
ARG EE_PORTS
# Thu, 17 Dec 2020 04:57:09 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 27 Jan 2021 00:45:22 GMT
ARG KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 00:45:23 GMT
ENV KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 00:45:23 GMT
ARG KONG_AMD64_SHA=8a33a919f75bdb8bb708de23c0701def2aedfcd2679d27b7849040c3edf273f9
# Wed, 27 Jan 2021 00:45:24 GMT
ENV KONG_AMD64_SHA=8a33a919f75bdb8bb708de23c0701def2aedfcd2679d27b7849040c3edf273f9
# Wed, 27 Jan 2021 00:45:24 GMT
ARG KONG_ARM64_SHA=4ae43ecf9b1fcf11930d859efec475e216729b89b76de80a4c38e1fe58e3874f
# Wed, 27 Jan 2021 00:45:25 GMT
ENV KONG_ARM64_SHA=4ae43ecf9b1fcf11930d859efec475e216729b89b76de80a4c38e1fe58e3874f
# Wed, 27 Jan 2021 00:45:38 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;; 		aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Wed, 27 Jan 2021 00:45:40 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 27 Jan 2021 00:45:40 GMT
USER kong
# Wed, 27 Jan 2021 00:45:41 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 27 Jan 2021 00:45:42 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 27 Jan 2021 00:45:42 GMT
STOPSIGNAL SIGQUIT
# Wed, 27 Jan 2021 00:45:43 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:20d8a246443a66e74e17f2a0e81a51fe774876ca0c2676691c37ee1b0e4d3cd5`  
		Last Modified: Wed, 16 Dec 2020 23:41:20 GMT  
		Size: 2.7 MB (2725216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3181cc464c4af55ff9dd73d4603f67578cdc16237deb0e5e467594b40164ab6`  
		Last Modified: Thu, 17 Dec 2020 04:58:48 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:686913a20dd73c0bdaa7517e69803b84807b71b99b4ff55cc9764516b90461f7`  
		Last Modified: Wed, 27 Jan 2021 00:47:56 GMT  
		Size: 47.7 MB (47736063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5429c14c14d5050bce7546a62fa4539c4c325f122c109881ea4dc5f0b628ed6`  
		Last Modified: Wed, 27 Jan 2021 00:47:42 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.3.1`

```console
$ docker pull kong@sha256:38c82bcf40f627c1ed3edef3eb0ac9ab3d1fb29fe7eb8df69f5166b324a22153
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.3.1` - linux; amd64

```console
$ docker pull kong@sha256:eaf0443b11346f6b7f4ac6c0979430462e5070b86a31f5cb2b16a0477773c715
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.9 MB (50938328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cd6edfe129b1c02465b0927dcfdc0d52765486279f5916a2c24d06f070dbd95`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 14:57:37 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 17 Dec 2020 14:57:37 GMT
ARG ASSET=ce
# Thu, 17 Dec 2020 14:57:37 GMT
ENV ASSET=ce
# Thu, 17 Dec 2020 14:57:37 GMT
ARG EE_PORTS
# Thu, 17 Dec 2020 14:57:38 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 27 Jan 2021 06:32:07 GMT
ARG KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 06:32:07 GMT
ENV KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 06:32:07 GMT
ARG KONG_AMD64_SHA=8a33a919f75bdb8bb708de23c0701def2aedfcd2679d27b7849040c3edf273f9
# Wed, 27 Jan 2021 06:32:07 GMT
ENV KONG_AMD64_SHA=8a33a919f75bdb8bb708de23c0701def2aedfcd2679d27b7849040c3edf273f9
# Wed, 27 Jan 2021 06:32:08 GMT
ARG KONG_ARM64_SHA=4ae43ecf9b1fcf11930d859efec475e216729b89b76de80a4c38e1fe58e3874f
# Wed, 27 Jan 2021 06:32:08 GMT
ENV KONG_ARM64_SHA=4ae43ecf9b1fcf11930d859efec475e216729b89b76de80a4c38e1fe58e3874f
# Wed, 27 Jan 2021 06:32:15 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;; 		aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Wed, 27 Jan 2021 06:32:16 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 27 Jan 2021 06:32:16 GMT
USER kong
# Wed, 27 Jan 2021 06:32:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 27 Jan 2021 06:32:16 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 27 Jan 2021 06:32:16 GMT
STOPSIGNAL SIGQUIT
# Wed, 27 Jan 2021 06:32:17 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274efec6805c2b13808c7bcb7932f07b136c0be74bf02bdbf77f79e89dc58725`  
		Last Modified: Thu, 17 Dec 2020 14:59:10 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b18e55f2934bb191d816e87b86e196e1c8d35d815f72f93f7e5f51c0f17319e`  
		Last Modified: Wed, 27 Jan 2021 06:35:34 GMT  
		Size: 48.1 MB (48122597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec1f7f35984e4dfe3874035c9af0e74955cc49424e7f4a0d50411d336f9228fa`  
		Last Modified: Wed, 27 Jan 2021 06:35:24 GMT  
		Size: 735.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.3.1` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:d87959fb87a61b8f9fba68a010a6e444317df9ca4bbba731d1374c9035077d0e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50462144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:065a1ea94079d9d30ef22ca0cbfffc961327ac4759c8ab96e9473a3daeb1b436`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:57:05 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 17 Dec 2020 04:57:06 GMT
ARG ASSET=ce
# Thu, 17 Dec 2020 04:57:07 GMT
ENV ASSET=ce
# Thu, 17 Dec 2020 04:57:08 GMT
ARG EE_PORTS
# Thu, 17 Dec 2020 04:57:09 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 27 Jan 2021 00:45:22 GMT
ARG KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 00:45:23 GMT
ENV KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 00:45:23 GMT
ARG KONG_AMD64_SHA=8a33a919f75bdb8bb708de23c0701def2aedfcd2679d27b7849040c3edf273f9
# Wed, 27 Jan 2021 00:45:24 GMT
ENV KONG_AMD64_SHA=8a33a919f75bdb8bb708de23c0701def2aedfcd2679d27b7849040c3edf273f9
# Wed, 27 Jan 2021 00:45:24 GMT
ARG KONG_ARM64_SHA=4ae43ecf9b1fcf11930d859efec475e216729b89b76de80a4c38e1fe58e3874f
# Wed, 27 Jan 2021 00:45:25 GMT
ENV KONG_ARM64_SHA=4ae43ecf9b1fcf11930d859efec475e216729b89b76de80a4c38e1fe58e3874f
# Wed, 27 Jan 2021 00:45:38 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;; 		aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Wed, 27 Jan 2021 00:45:40 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 27 Jan 2021 00:45:40 GMT
USER kong
# Wed, 27 Jan 2021 00:45:41 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 27 Jan 2021 00:45:42 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 27 Jan 2021 00:45:42 GMT
STOPSIGNAL SIGQUIT
# Wed, 27 Jan 2021 00:45:43 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:20d8a246443a66e74e17f2a0e81a51fe774876ca0c2676691c37ee1b0e4d3cd5`  
		Last Modified: Wed, 16 Dec 2020 23:41:20 GMT  
		Size: 2.7 MB (2725216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3181cc464c4af55ff9dd73d4603f67578cdc16237deb0e5e467594b40164ab6`  
		Last Modified: Thu, 17 Dec 2020 04:58:48 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:686913a20dd73c0bdaa7517e69803b84807b71b99b4ff55cc9764516b90461f7`  
		Last Modified: Wed, 27 Jan 2021 00:47:56 GMT  
		Size: 47.7 MB (47736063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5429c14c14d5050bce7546a62fa4539c4c325f122c109881ea4dc5f0b628ed6`  
		Last Modified: Wed, 27 Jan 2021 00:47:42 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.3.1-alpine`

```console
$ docker pull kong@sha256:38c82bcf40f627c1ed3edef3eb0ac9ab3d1fb29fe7eb8df69f5166b324a22153
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.3.1-alpine` - linux; amd64

```console
$ docker pull kong@sha256:eaf0443b11346f6b7f4ac6c0979430462e5070b86a31f5cb2b16a0477773c715
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.9 MB (50938328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cd6edfe129b1c02465b0927dcfdc0d52765486279f5916a2c24d06f070dbd95`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 14:57:37 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 17 Dec 2020 14:57:37 GMT
ARG ASSET=ce
# Thu, 17 Dec 2020 14:57:37 GMT
ENV ASSET=ce
# Thu, 17 Dec 2020 14:57:37 GMT
ARG EE_PORTS
# Thu, 17 Dec 2020 14:57:38 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 27 Jan 2021 06:32:07 GMT
ARG KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 06:32:07 GMT
ENV KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 06:32:07 GMT
ARG KONG_AMD64_SHA=8a33a919f75bdb8bb708de23c0701def2aedfcd2679d27b7849040c3edf273f9
# Wed, 27 Jan 2021 06:32:07 GMT
ENV KONG_AMD64_SHA=8a33a919f75bdb8bb708de23c0701def2aedfcd2679d27b7849040c3edf273f9
# Wed, 27 Jan 2021 06:32:08 GMT
ARG KONG_ARM64_SHA=4ae43ecf9b1fcf11930d859efec475e216729b89b76de80a4c38e1fe58e3874f
# Wed, 27 Jan 2021 06:32:08 GMT
ENV KONG_ARM64_SHA=4ae43ecf9b1fcf11930d859efec475e216729b89b76de80a4c38e1fe58e3874f
# Wed, 27 Jan 2021 06:32:15 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;; 		aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Wed, 27 Jan 2021 06:32:16 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 27 Jan 2021 06:32:16 GMT
USER kong
# Wed, 27 Jan 2021 06:32:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 27 Jan 2021 06:32:16 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 27 Jan 2021 06:32:16 GMT
STOPSIGNAL SIGQUIT
# Wed, 27 Jan 2021 06:32:17 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274efec6805c2b13808c7bcb7932f07b136c0be74bf02bdbf77f79e89dc58725`  
		Last Modified: Thu, 17 Dec 2020 14:59:10 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b18e55f2934bb191d816e87b86e196e1c8d35d815f72f93f7e5f51c0f17319e`  
		Last Modified: Wed, 27 Jan 2021 06:35:34 GMT  
		Size: 48.1 MB (48122597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec1f7f35984e4dfe3874035c9af0e74955cc49424e7f4a0d50411d336f9228fa`  
		Last Modified: Wed, 27 Jan 2021 06:35:24 GMT  
		Size: 735.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.3.1-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:d87959fb87a61b8f9fba68a010a6e444317df9ca4bbba731d1374c9035077d0e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50462144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:065a1ea94079d9d30ef22ca0cbfffc961327ac4759c8ab96e9473a3daeb1b436`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:57:05 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 17 Dec 2020 04:57:06 GMT
ARG ASSET=ce
# Thu, 17 Dec 2020 04:57:07 GMT
ENV ASSET=ce
# Thu, 17 Dec 2020 04:57:08 GMT
ARG EE_PORTS
# Thu, 17 Dec 2020 04:57:09 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 27 Jan 2021 00:45:22 GMT
ARG KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 00:45:23 GMT
ENV KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 00:45:23 GMT
ARG KONG_AMD64_SHA=8a33a919f75bdb8bb708de23c0701def2aedfcd2679d27b7849040c3edf273f9
# Wed, 27 Jan 2021 00:45:24 GMT
ENV KONG_AMD64_SHA=8a33a919f75bdb8bb708de23c0701def2aedfcd2679d27b7849040c3edf273f9
# Wed, 27 Jan 2021 00:45:24 GMT
ARG KONG_ARM64_SHA=4ae43ecf9b1fcf11930d859efec475e216729b89b76de80a4c38e1fe58e3874f
# Wed, 27 Jan 2021 00:45:25 GMT
ENV KONG_ARM64_SHA=4ae43ecf9b1fcf11930d859efec475e216729b89b76de80a4c38e1fe58e3874f
# Wed, 27 Jan 2021 00:45:38 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;; 		aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Wed, 27 Jan 2021 00:45:40 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 27 Jan 2021 00:45:40 GMT
USER kong
# Wed, 27 Jan 2021 00:45:41 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 27 Jan 2021 00:45:42 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 27 Jan 2021 00:45:42 GMT
STOPSIGNAL SIGQUIT
# Wed, 27 Jan 2021 00:45:43 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:20d8a246443a66e74e17f2a0e81a51fe774876ca0c2676691c37ee1b0e4d3cd5`  
		Last Modified: Wed, 16 Dec 2020 23:41:20 GMT  
		Size: 2.7 MB (2725216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3181cc464c4af55ff9dd73d4603f67578cdc16237deb0e5e467594b40164ab6`  
		Last Modified: Thu, 17 Dec 2020 04:58:48 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:686913a20dd73c0bdaa7517e69803b84807b71b99b4ff55cc9764516b90461f7`  
		Last Modified: Wed, 27 Jan 2021 00:47:56 GMT  
		Size: 47.7 MB (47736063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5429c14c14d5050bce7546a62fa4539c4c325f122c109881ea4dc5f0b628ed6`  
		Last Modified: Wed, 27 Jan 2021 00:47:42 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.3.1-centos`

```console
$ docker pull kong@sha256:176363657cdf7dc411f1d738aae37ff5016542170c9a2696607361cb5cfb9b91
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.3.1-centos` - linux; amd64

```console
$ docker pull kong@sha256:c59b96b4d57a32a72e9b8be4b6e1c14c6a1e3bb3340d80266fae91460769ef40
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127400802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6ddf4deeb4ee04ebf0f68f79a2ee0486fd26465754de034da59bd93c53d6b5b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 14 Nov 2020 00:20:04 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Sat, 14 Nov 2020 00:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Sat, 14 Nov 2020 00:20:04 GMT
CMD ["/bin/bash"]
# Sat, 14 Nov 2020 01:01:33 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 14 Nov 2020 01:01:33 GMT
ARG ASSET=ce
# Sat, 14 Nov 2020 01:01:34 GMT
ENV ASSET=ce
# Sat, 14 Nov 2020 01:01:34 GMT
ARG EE_PORTS
# Sat, 14 Nov 2020 01:01:34 GMT
COPY file:ff02c070e4c89f043b176279a7e41464b5fab8cb98cfcd6332fad2d2741fc41d in /tmp/kong.rpm 
# Wed, 27 Jan 2021 06:33:26 GMT
ARG KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 06:33:27 GMT
ENV KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 06:33:27 GMT
ARG KONG_SHA256=c95c8306f31eb9bb3fce6d3436d3782eb352dfb17dca10edad8a0f0d982b1219
# Wed, 27 Jan 2021 06:33:56 GMT
# ARGS: KONG_SHA256=c95c8306f31eb9bb3fce6d3436d3782eb352dfb17dca10edad8a0f0d982b1219
RUN set -ex;   if [ "$ASSET" = "ce" ] ; then     curl -fL "https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm" -o /tmp/kong.rpm     && echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -;   fi;   yum install -y -q unzip shadow-utils git   && yum clean all -q   && rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki   && yum install -y /tmp/kong.rpm   && yum clean all   && rm /tmp/kong.rpm   && chown kong:0 /usr/local/bin/kong   && chown -R kong:0 /usr/local/kong &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Wed, 27 Jan 2021 06:33:56 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 27 Jan 2021 06:33:56 GMT
USER kong
# Wed, 27 Jan 2021 06:33:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 27 Jan 2021 06:33:57 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 27 Jan 2021 06:33:57 GMT
STOPSIGNAL SIGQUIT
# Wed, 27 Jan 2021 06:33:57 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4dc7c6a187fe570e563de224bd35775b78d3ff78f05cf73c4e08319b2dc232`  
		Last Modified: Sat, 14 Nov 2020 01:03:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db8e71dccdabe2284554e8e30b0937710417a94f009b08bbbc6c7f88bac451a`  
		Last Modified: Wed, 27 Jan 2021 06:36:22 GMT  
		Size: 51.3 MB (51302781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2de3757aca98a38a9abef3cdbfd3ac04a92c479502e5ae467734ecc9c60fdcc`  
		Last Modified: Wed, 27 Jan 2021 06:36:11 GMT  
		Size: 735.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.3.1-ubuntu`

```console
$ docker pull kong@sha256:b46fb4a0cfeedb5a99723b50e3c4d8e251eba950bb95d996f546108469e520d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.3.1-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:597d3f899451bab38b28bc472c6af7ce10a79d4a7f72b242b9dba5a5b80dae9c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.0 MB (134011512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecdda63d33dee4365e82d62414c95e28dac508e4f96086475f17d7411fe7ef11`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 21 Jan 2021 03:39:31 GMT
ADD file:925571658dd8453e5c80d862f5791d6b26b3c2a8688937b11741f2f2c5cdbfd7 in / 
# Thu, 21 Jan 2021 03:39:32 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:39:34 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:39:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:39:36 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 10:27:05 GMT
ARG ASSET=ce
# Thu, 21 Jan 2021 10:27:05 GMT
ENV ASSET=ce
# Thu, 21 Jan 2021 10:27:05 GMT
ARG EE_PORTS
# Thu, 21 Jan 2021 10:27:06 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 27 Jan 2021 06:32:22 GMT
ARG KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 06:32:22 GMT
ENV KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 06:33:11 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt update     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Wed, 27 Jan 2021 06:33:12 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Wed, 27 Jan 2021 06:33:12 GMT
USER kong
# Wed, 27 Jan 2021 06:33:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 27 Jan 2021 06:33:12 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 27 Jan 2021 06:33:13 GMT
STOPSIGNAL SIGQUIT
# Wed, 27 Jan 2021 06:33:13 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4007a89234b4f56c03e6831dc220550d2e5fba935d9f5f5bcea64857ac4f4888`  
		Last Modified: Mon, 18 Jan 2021 19:38:08 GMT  
		Size: 46.0 MB (45962352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfa26c6b9c9d1ccbcb1eaa65befa376805d9324174ac580ca76fdedc3575f54`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba7bf18aa406cb7dc372ac732de222b04d1c824ff1705d8900831c3d1361ff5`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6ec688ebe374ea7d89ce967576d221a177ebd2c02ca9f053197f954102e30b`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7491b48e51562c145461304393cbc54944e319e09a7714bf0e4264da38b8a8f0`  
		Last Modified: Thu, 21 Jan 2021 10:30:38 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c37a4a4ce379b4b55c1ee57df48a2c7f66ef0480f4217df19284fb0ac887147`  
		Last Modified: Wed, 27 Jan 2021 06:36:06 GMT  
		Size: 63.0 MB (62964969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff52cba088e18ceb7be8ffce04fd152b6a4df798b5bad5a296d22fd49538e01`  
		Last Modified: Wed, 27 Jan 2021 06:35:43 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.3.1-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:f16de38cd2620af9554e1a3a8e55c22d36cb4640d73bea97c7cdcbed88cff9e2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.4 MB (125352533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f74865582600b00fdd71d91664fb06575999525d67115492f4cc56371a8daeee`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 21 Jan 2021 03:51:12 GMT
ADD file:e2f37be259f081b70bc884e3b7f652e5d9a0ad4ae443f2258b79a1b14377cc20 in / 
# Thu, 21 Jan 2021 03:51:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:51:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:51:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:51:22 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:32:05 GMT
ARG ASSET=ce
# Thu, 21 Jan 2021 05:32:06 GMT
ENV ASSET=ce
# Thu, 21 Jan 2021 05:32:06 GMT
ARG EE_PORTS
# Thu, 21 Jan 2021 05:32:07 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 27 Jan 2021 00:45:49 GMT
ARG KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 00:45:50 GMT
ENV KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 00:46:39 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt update     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Wed, 27 Jan 2021 00:46:41 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Wed, 27 Jan 2021 00:46:42 GMT
USER kong
# Wed, 27 Jan 2021 00:46:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 27 Jan 2021 00:46:43 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 27 Jan 2021 00:46:44 GMT
STOPSIGNAL SIGQUIT
# Wed, 27 Jan 2021 00:46:44 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:79186a4c5361c6b018fe75c9bba66c9bf717db8d7d4a6ddb18fb86171f277b61`  
		Last Modified: Thu, 14 Jan 2021 16:25:21 GMT  
		Size: 40.9 MB (40885219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96f901e8ebcf64a42ec369549f6269ec96cd97b424389ca99a8ebb722c59c12`  
		Last Modified: Thu, 21 Jan 2021 03:53:10 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36fd1545244608cb9ef92efa528b6e8c3229f1b01ca414ee8717219145cdff7d`  
		Last Modified: Thu, 21 Jan 2021 03:53:10 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d978c0f55122642ba1a22cc67abf7af2e898bfb42933b1879c2dd91fd987147d`  
		Last Modified: Thu, 21 Jan 2021 03:53:11 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e81e83cdfa4fc6fce4a28de27bb31753456d14bad0dcc25aabceaa0a03a3345`  
		Last Modified: Thu, 21 Jan 2021 05:37:21 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e92def6c86f1cd19fef7864bb7f4b62cbb86f8d16f6845ecec91126b1f9c7d`  
		Last Modified: Wed, 27 Jan 2021 00:48:28 GMT  
		Size: 59.4 MB (59383183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa36af64dff18650ff7c3948d67dab978c2fa075442c01a124f7cb86ba51ff5`  
		Last Modified: Wed, 27 Jan 2021 00:48:09 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.3-alpine`

```console
$ docker pull kong@sha256:38c82bcf40f627c1ed3edef3eb0ac9ab3d1fb29fe7eb8df69f5166b324a22153
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.3-alpine` - linux; amd64

```console
$ docker pull kong@sha256:eaf0443b11346f6b7f4ac6c0979430462e5070b86a31f5cb2b16a0477773c715
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.9 MB (50938328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cd6edfe129b1c02465b0927dcfdc0d52765486279f5916a2c24d06f070dbd95`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 14:57:37 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 17 Dec 2020 14:57:37 GMT
ARG ASSET=ce
# Thu, 17 Dec 2020 14:57:37 GMT
ENV ASSET=ce
# Thu, 17 Dec 2020 14:57:37 GMT
ARG EE_PORTS
# Thu, 17 Dec 2020 14:57:38 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 27 Jan 2021 06:32:07 GMT
ARG KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 06:32:07 GMT
ENV KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 06:32:07 GMT
ARG KONG_AMD64_SHA=8a33a919f75bdb8bb708de23c0701def2aedfcd2679d27b7849040c3edf273f9
# Wed, 27 Jan 2021 06:32:07 GMT
ENV KONG_AMD64_SHA=8a33a919f75bdb8bb708de23c0701def2aedfcd2679d27b7849040c3edf273f9
# Wed, 27 Jan 2021 06:32:08 GMT
ARG KONG_ARM64_SHA=4ae43ecf9b1fcf11930d859efec475e216729b89b76de80a4c38e1fe58e3874f
# Wed, 27 Jan 2021 06:32:08 GMT
ENV KONG_ARM64_SHA=4ae43ecf9b1fcf11930d859efec475e216729b89b76de80a4c38e1fe58e3874f
# Wed, 27 Jan 2021 06:32:15 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;; 		aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Wed, 27 Jan 2021 06:32:16 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 27 Jan 2021 06:32:16 GMT
USER kong
# Wed, 27 Jan 2021 06:32:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 27 Jan 2021 06:32:16 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 27 Jan 2021 06:32:16 GMT
STOPSIGNAL SIGQUIT
# Wed, 27 Jan 2021 06:32:17 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274efec6805c2b13808c7bcb7932f07b136c0be74bf02bdbf77f79e89dc58725`  
		Last Modified: Thu, 17 Dec 2020 14:59:10 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b18e55f2934bb191d816e87b86e196e1c8d35d815f72f93f7e5f51c0f17319e`  
		Last Modified: Wed, 27 Jan 2021 06:35:34 GMT  
		Size: 48.1 MB (48122597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec1f7f35984e4dfe3874035c9af0e74955cc49424e7f4a0d50411d336f9228fa`  
		Last Modified: Wed, 27 Jan 2021 06:35:24 GMT  
		Size: 735.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.3-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:d87959fb87a61b8f9fba68a010a6e444317df9ca4bbba731d1374c9035077d0e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50462144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:065a1ea94079d9d30ef22ca0cbfffc961327ac4759c8ab96e9473a3daeb1b436`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:57:05 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 17 Dec 2020 04:57:06 GMT
ARG ASSET=ce
# Thu, 17 Dec 2020 04:57:07 GMT
ENV ASSET=ce
# Thu, 17 Dec 2020 04:57:08 GMT
ARG EE_PORTS
# Thu, 17 Dec 2020 04:57:09 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 27 Jan 2021 00:45:22 GMT
ARG KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 00:45:23 GMT
ENV KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 00:45:23 GMT
ARG KONG_AMD64_SHA=8a33a919f75bdb8bb708de23c0701def2aedfcd2679d27b7849040c3edf273f9
# Wed, 27 Jan 2021 00:45:24 GMT
ENV KONG_AMD64_SHA=8a33a919f75bdb8bb708de23c0701def2aedfcd2679d27b7849040c3edf273f9
# Wed, 27 Jan 2021 00:45:24 GMT
ARG KONG_ARM64_SHA=4ae43ecf9b1fcf11930d859efec475e216729b89b76de80a4c38e1fe58e3874f
# Wed, 27 Jan 2021 00:45:25 GMT
ENV KONG_ARM64_SHA=4ae43ecf9b1fcf11930d859efec475e216729b89b76de80a4c38e1fe58e3874f
# Wed, 27 Jan 2021 00:45:38 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;; 		aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Wed, 27 Jan 2021 00:45:40 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 27 Jan 2021 00:45:40 GMT
USER kong
# Wed, 27 Jan 2021 00:45:41 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 27 Jan 2021 00:45:42 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 27 Jan 2021 00:45:42 GMT
STOPSIGNAL SIGQUIT
# Wed, 27 Jan 2021 00:45:43 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:20d8a246443a66e74e17f2a0e81a51fe774876ca0c2676691c37ee1b0e4d3cd5`  
		Last Modified: Wed, 16 Dec 2020 23:41:20 GMT  
		Size: 2.7 MB (2725216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3181cc464c4af55ff9dd73d4603f67578cdc16237deb0e5e467594b40164ab6`  
		Last Modified: Thu, 17 Dec 2020 04:58:48 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:686913a20dd73c0bdaa7517e69803b84807b71b99b4ff55cc9764516b90461f7`  
		Last Modified: Wed, 27 Jan 2021 00:47:56 GMT  
		Size: 47.7 MB (47736063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5429c14c14d5050bce7546a62fa4539c4c325f122c109881ea4dc5f0b628ed6`  
		Last Modified: Wed, 27 Jan 2021 00:47:42 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.3-centos`

```console
$ docker pull kong@sha256:176363657cdf7dc411f1d738aae37ff5016542170c9a2696607361cb5cfb9b91
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.3-centos` - linux; amd64

```console
$ docker pull kong@sha256:c59b96b4d57a32a72e9b8be4b6e1c14c6a1e3bb3340d80266fae91460769ef40
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127400802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6ddf4deeb4ee04ebf0f68f79a2ee0486fd26465754de034da59bd93c53d6b5b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 14 Nov 2020 00:20:04 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Sat, 14 Nov 2020 00:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Sat, 14 Nov 2020 00:20:04 GMT
CMD ["/bin/bash"]
# Sat, 14 Nov 2020 01:01:33 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 14 Nov 2020 01:01:33 GMT
ARG ASSET=ce
# Sat, 14 Nov 2020 01:01:34 GMT
ENV ASSET=ce
# Sat, 14 Nov 2020 01:01:34 GMT
ARG EE_PORTS
# Sat, 14 Nov 2020 01:01:34 GMT
COPY file:ff02c070e4c89f043b176279a7e41464b5fab8cb98cfcd6332fad2d2741fc41d in /tmp/kong.rpm 
# Wed, 27 Jan 2021 06:33:26 GMT
ARG KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 06:33:27 GMT
ENV KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 06:33:27 GMT
ARG KONG_SHA256=c95c8306f31eb9bb3fce6d3436d3782eb352dfb17dca10edad8a0f0d982b1219
# Wed, 27 Jan 2021 06:33:56 GMT
# ARGS: KONG_SHA256=c95c8306f31eb9bb3fce6d3436d3782eb352dfb17dca10edad8a0f0d982b1219
RUN set -ex;   if [ "$ASSET" = "ce" ] ; then     curl -fL "https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm" -o /tmp/kong.rpm     && echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -;   fi;   yum install -y -q unzip shadow-utils git   && yum clean all -q   && rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki   && yum install -y /tmp/kong.rpm   && yum clean all   && rm /tmp/kong.rpm   && chown kong:0 /usr/local/bin/kong   && chown -R kong:0 /usr/local/kong &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Wed, 27 Jan 2021 06:33:56 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 27 Jan 2021 06:33:56 GMT
USER kong
# Wed, 27 Jan 2021 06:33:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 27 Jan 2021 06:33:57 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 27 Jan 2021 06:33:57 GMT
STOPSIGNAL SIGQUIT
# Wed, 27 Jan 2021 06:33:57 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4dc7c6a187fe570e563de224bd35775b78d3ff78f05cf73c4e08319b2dc232`  
		Last Modified: Sat, 14 Nov 2020 01:03:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db8e71dccdabe2284554e8e30b0937710417a94f009b08bbbc6c7f88bac451a`  
		Last Modified: Wed, 27 Jan 2021 06:36:22 GMT  
		Size: 51.3 MB (51302781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2de3757aca98a38a9abef3cdbfd3ac04a92c479502e5ae467734ecc9c60fdcc`  
		Last Modified: Wed, 27 Jan 2021 06:36:11 GMT  
		Size: 735.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.3-ubuntu`

```console
$ docker pull kong@sha256:b46fb4a0cfeedb5a99723b50e3c4d8e251eba950bb95d996f546108469e520d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.3-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:597d3f899451bab38b28bc472c6af7ce10a79d4a7f72b242b9dba5a5b80dae9c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.0 MB (134011512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecdda63d33dee4365e82d62414c95e28dac508e4f96086475f17d7411fe7ef11`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 21 Jan 2021 03:39:31 GMT
ADD file:925571658dd8453e5c80d862f5791d6b26b3c2a8688937b11741f2f2c5cdbfd7 in / 
# Thu, 21 Jan 2021 03:39:32 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:39:34 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:39:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:39:36 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 10:27:05 GMT
ARG ASSET=ce
# Thu, 21 Jan 2021 10:27:05 GMT
ENV ASSET=ce
# Thu, 21 Jan 2021 10:27:05 GMT
ARG EE_PORTS
# Thu, 21 Jan 2021 10:27:06 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 27 Jan 2021 06:32:22 GMT
ARG KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 06:32:22 GMT
ENV KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 06:33:11 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt update     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Wed, 27 Jan 2021 06:33:12 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Wed, 27 Jan 2021 06:33:12 GMT
USER kong
# Wed, 27 Jan 2021 06:33:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 27 Jan 2021 06:33:12 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 27 Jan 2021 06:33:13 GMT
STOPSIGNAL SIGQUIT
# Wed, 27 Jan 2021 06:33:13 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4007a89234b4f56c03e6831dc220550d2e5fba935d9f5f5bcea64857ac4f4888`  
		Last Modified: Mon, 18 Jan 2021 19:38:08 GMT  
		Size: 46.0 MB (45962352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfa26c6b9c9d1ccbcb1eaa65befa376805d9324174ac580ca76fdedc3575f54`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba7bf18aa406cb7dc372ac732de222b04d1c824ff1705d8900831c3d1361ff5`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6ec688ebe374ea7d89ce967576d221a177ebd2c02ca9f053197f954102e30b`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7491b48e51562c145461304393cbc54944e319e09a7714bf0e4264da38b8a8f0`  
		Last Modified: Thu, 21 Jan 2021 10:30:38 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c37a4a4ce379b4b55c1ee57df48a2c7f66ef0480f4217df19284fb0ac887147`  
		Last Modified: Wed, 27 Jan 2021 06:36:06 GMT  
		Size: 63.0 MB (62964969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff52cba088e18ceb7be8ffce04fd152b6a4df798b5bad5a296d22fd49538e01`  
		Last Modified: Wed, 27 Jan 2021 06:35:43 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.3-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:f16de38cd2620af9554e1a3a8e55c22d36cb4640d73bea97c7cdcbed88cff9e2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.4 MB (125352533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f74865582600b00fdd71d91664fb06575999525d67115492f4cc56371a8daeee`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 21 Jan 2021 03:51:12 GMT
ADD file:e2f37be259f081b70bc884e3b7f652e5d9a0ad4ae443f2258b79a1b14377cc20 in / 
# Thu, 21 Jan 2021 03:51:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:51:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:51:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:51:22 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:32:05 GMT
ARG ASSET=ce
# Thu, 21 Jan 2021 05:32:06 GMT
ENV ASSET=ce
# Thu, 21 Jan 2021 05:32:06 GMT
ARG EE_PORTS
# Thu, 21 Jan 2021 05:32:07 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 27 Jan 2021 00:45:49 GMT
ARG KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 00:45:50 GMT
ENV KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 00:46:39 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt update     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Wed, 27 Jan 2021 00:46:41 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Wed, 27 Jan 2021 00:46:42 GMT
USER kong
# Wed, 27 Jan 2021 00:46:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 27 Jan 2021 00:46:43 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 27 Jan 2021 00:46:44 GMT
STOPSIGNAL SIGQUIT
# Wed, 27 Jan 2021 00:46:44 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:79186a4c5361c6b018fe75c9bba66c9bf717db8d7d4a6ddb18fb86171f277b61`  
		Last Modified: Thu, 14 Jan 2021 16:25:21 GMT  
		Size: 40.9 MB (40885219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96f901e8ebcf64a42ec369549f6269ec96cd97b424389ca99a8ebb722c59c12`  
		Last Modified: Thu, 21 Jan 2021 03:53:10 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36fd1545244608cb9ef92efa528b6e8c3229f1b01ca414ee8717219145cdff7d`  
		Last Modified: Thu, 21 Jan 2021 03:53:10 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d978c0f55122642ba1a22cc67abf7af2e898bfb42933b1879c2dd91fd987147d`  
		Last Modified: Thu, 21 Jan 2021 03:53:11 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e81e83cdfa4fc6fce4a28de27bb31753456d14bad0dcc25aabceaa0a03a3345`  
		Last Modified: Thu, 21 Jan 2021 05:37:21 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e92def6c86f1cd19fef7864bb7f4b62cbb86f8d16f6845ecec91126b1f9c7d`  
		Last Modified: Wed, 27 Jan 2021 00:48:28 GMT  
		Size: 59.4 MB (59383183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa36af64dff18650ff7c3948d67dab978c2fa075442c01a124f7cb86ba51ff5`  
		Last Modified: Wed, 27 Jan 2021 00:48:09 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:alpine`

```console
$ docker pull kong@sha256:38c82bcf40f627c1ed3edef3eb0ac9ab3d1fb29fe7eb8df69f5166b324a22153
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:alpine` - linux; amd64

```console
$ docker pull kong@sha256:eaf0443b11346f6b7f4ac6c0979430462e5070b86a31f5cb2b16a0477773c715
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.9 MB (50938328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cd6edfe129b1c02465b0927dcfdc0d52765486279f5916a2c24d06f070dbd95`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 14:57:37 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 17 Dec 2020 14:57:37 GMT
ARG ASSET=ce
# Thu, 17 Dec 2020 14:57:37 GMT
ENV ASSET=ce
# Thu, 17 Dec 2020 14:57:37 GMT
ARG EE_PORTS
# Thu, 17 Dec 2020 14:57:38 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 27 Jan 2021 06:32:07 GMT
ARG KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 06:32:07 GMT
ENV KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 06:32:07 GMT
ARG KONG_AMD64_SHA=8a33a919f75bdb8bb708de23c0701def2aedfcd2679d27b7849040c3edf273f9
# Wed, 27 Jan 2021 06:32:07 GMT
ENV KONG_AMD64_SHA=8a33a919f75bdb8bb708de23c0701def2aedfcd2679d27b7849040c3edf273f9
# Wed, 27 Jan 2021 06:32:08 GMT
ARG KONG_ARM64_SHA=4ae43ecf9b1fcf11930d859efec475e216729b89b76de80a4c38e1fe58e3874f
# Wed, 27 Jan 2021 06:32:08 GMT
ENV KONG_ARM64_SHA=4ae43ecf9b1fcf11930d859efec475e216729b89b76de80a4c38e1fe58e3874f
# Wed, 27 Jan 2021 06:32:15 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;; 		aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Wed, 27 Jan 2021 06:32:16 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 27 Jan 2021 06:32:16 GMT
USER kong
# Wed, 27 Jan 2021 06:32:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 27 Jan 2021 06:32:16 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 27 Jan 2021 06:32:16 GMT
STOPSIGNAL SIGQUIT
# Wed, 27 Jan 2021 06:32:17 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274efec6805c2b13808c7bcb7932f07b136c0be74bf02bdbf77f79e89dc58725`  
		Last Modified: Thu, 17 Dec 2020 14:59:10 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b18e55f2934bb191d816e87b86e196e1c8d35d815f72f93f7e5f51c0f17319e`  
		Last Modified: Wed, 27 Jan 2021 06:35:34 GMT  
		Size: 48.1 MB (48122597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec1f7f35984e4dfe3874035c9af0e74955cc49424e7f4a0d50411d336f9228fa`  
		Last Modified: Wed, 27 Jan 2021 06:35:24 GMT  
		Size: 735.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:d87959fb87a61b8f9fba68a010a6e444317df9ca4bbba731d1374c9035077d0e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50462144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:065a1ea94079d9d30ef22ca0cbfffc961327ac4759c8ab96e9473a3daeb1b436`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:57:05 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 17 Dec 2020 04:57:06 GMT
ARG ASSET=ce
# Thu, 17 Dec 2020 04:57:07 GMT
ENV ASSET=ce
# Thu, 17 Dec 2020 04:57:08 GMT
ARG EE_PORTS
# Thu, 17 Dec 2020 04:57:09 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 27 Jan 2021 00:45:22 GMT
ARG KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 00:45:23 GMT
ENV KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 00:45:23 GMT
ARG KONG_AMD64_SHA=8a33a919f75bdb8bb708de23c0701def2aedfcd2679d27b7849040c3edf273f9
# Wed, 27 Jan 2021 00:45:24 GMT
ENV KONG_AMD64_SHA=8a33a919f75bdb8bb708de23c0701def2aedfcd2679d27b7849040c3edf273f9
# Wed, 27 Jan 2021 00:45:24 GMT
ARG KONG_ARM64_SHA=4ae43ecf9b1fcf11930d859efec475e216729b89b76de80a4c38e1fe58e3874f
# Wed, 27 Jan 2021 00:45:25 GMT
ENV KONG_ARM64_SHA=4ae43ecf9b1fcf11930d859efec475e216729b89b76de80a4c38e1fe58e3874f
# Wed, 27 Jan 2021 00:45:38 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;; 		aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Wed, 27 Jan 2021 00:45:40 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 27 Jan 2021 00:45:40 GMT
USER kong
# Wed, 27 Jan 2021 00:45:41 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 27 Jan 2021 00:45:42 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 27 Jan 2021 00:45:42 GMT
STOPSIGNAL SIGQUIT
# Wed, 27 Jan 2021 00:45:43 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:20d8a246443a66e74e17f2a0e81a51fe774876ca0c2676691c37ee1b0e4d3cd5`  
		Last Modified: Wed, 16 Dec 2020 23:41:20 GMT  
		Size: 2.7 MB (2725216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3181cc464c4af55ff9dd73d4603f67578cdc16237deb0e5e467594b40164ab6`  
		Last Modified: Thu, 17 Dec 2020 04:58:48 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:686913a20dd73c0bdaa7517e69803b84807b71b99b4ff55cc9764516b90461f7`  
		Last Modified: Wed, 27 Jan 2021 00:47:56 GMT  
		Size: 47.7 MB (47736063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5429c14c14d5050bce7546a62fa4539c4c325f122c109881ea4dc5f0b628ed6`  
		Last Modified: Wed, 27 Jan 2021 00:47:42 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:centos`

```console
$ docker pull kong@sha256:176363657cdf7dc411f1d738aae37ff5016542170c9a2696607361cb5cfb9b91
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:centos` - linux; amd64

```console
$ docker pull kong@sha256:c59b96b4d57a32a72e9b8be4b6e1c14c6a1e3bb3340d80266fae91460769ef40
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127400802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6ddf4deeb4ee04ebf0f68f79a2ee0486fd26465754de034da59bd93c53d6b5b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Sat, 14 Nov 2020 00:20:04 GMT
ADD file:b3ebbe8bd304723d43b7b44a6d990cd657b63d93d6a2a9293983a30bfc1dfa53 in / 
# Sat, 14 Nov 2020 00:20:04 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20201113 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-11-13 00:00:00+00:00
# Sat, 14 Nov 2020 00:20:04 GMT
CMD ["/bin/bash"]
# Sat, 14 Nov 2020 01:01:33 GMT
LABEL maintainer=Kong <support@konghq.com>
# Sat, 14 Nov 2020 01:01:33 GMT
ARG ASSET=ce
# Sat, 14 Nov 2020 01:01:34 GMT
ENV ASSET=ce
# Sat, 14 Nov 2020 01:01:34 GMT
ARG EE_PORTS
# Sat, 14 Nov 2020 01:01:34 GMT
COPY file:ff02c070e4c89f043b176279a7e41464b5fab8cb98cfcd6332fad2d2741fc41d in /tmp/kong.rpm 
# Wed, 27 Jan 2021 06:33:26 GMT
ARG KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 06:33:27 GMT
ENV KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 06:33:27 GMT
ARG KONG_SHA256=c95c8306f31eb9bb3fce6d3436d3782eb352dfb17dca10edad8a0f0d982b1219
# Wed, 27 Jan 2021 06:33:56 GMT
# ARGS: KONG_SHA256=c95c8306f31eb9bb3fce6d3436d3782eb352dfb17dca10edad8a0f0d982b1219
RUN set -ex;   if [ "$ASSET" = "ce" ] ; then     curl -fL "https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm" -o /tmp/kong.rpm     && echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -;   fi;   yum install -y -q unzip shadow-utils git   && yum clean all -q   && rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki   && yum install -y /tmp/kong.rpm   && yum clean all   && rm /tmp/kong.rpm   && chown kong:0 /usr/local/bin/kong   && chown -R kong:0 /usr/local/kong &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Wed, 27 Jan 2021 06:33:56 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 27 Jan 2021 06:33:56 GMT
USER kong
# Wed, 27 Jan 2021 06:33:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 27 Jan 2021 06:33:57 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 27 Jan 2021 06:33:57 GMT
STOPSIGNAL SIGQUIT
# Wed, 27 Jan 2021 06:33:57 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:2d473b07cdd5f0912cd6f1a703352c82b512407db6b05b43f2553732b55df3bc`  
		Last Modified: Sat, 14 Nov 2020 00:21:39 GMT  
		Size: 76.1 MB (76097157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4dc7c6a187fe570e563de224bd35775b78d3ff78f05cf73c4e08319b2dc232`  
		Last Modified: Sat, 14 Nov 2020 01:03:42 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db8e71dccdabe2284554e8e30b0937710417a94f009b08bbbc6c7f88bac451a`  
		Last Modified: Wed, 27 Jan 2021 06:36:22 GMT  
		Size: 51.3 MB (51302781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2de3757aca98a38a9abef3cdbfd3ac04a92c479502e5ae467734ecc9c60fdcc`  
		Last Modified: Wed, 27 Jan 2021 06:36:11 GMT  
		Size: 735.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:latest`

```console
$ docker pull kong@sha256:38c82bcf40f627c1ed3edef3eb0ac9ab3d1fb29fe7eb8df69f5166b324a22153
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:latest` - linux; amd64

```console
$ docker pull kong@sha256:eaf0443b11346f6b7f4ac6c0979430462e5070b86a31f5cb2b16a0477773c715
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.9 MB (50938328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cd6edfe129b1c02465b0927dcfdc0d52765486279f5916a2c24d06f070dbd95`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:49 GMT
ADD file:8ed80010e443da19d72546bcee9a35e0a8d244c72052b1994610bf5939d479c2 in / 
# Thu, 17 Dec 2020 00:19:49 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 14:57:37 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 17 Dec 2020 14:57:37 GMT
ARG ASSET=ce
# Thu, 17 Dec 2020 14:57:37 GMT
ENV ASSET=ce
# Thu, 17 Dec 2020 14:57:37 GMT
ARG EE_PORTS
# Thu, 17 Dec 2020 14:57:38 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 27 Jan 2021 06:32:07 GMT
ARG KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 06:32:07 GMT
ENV KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 06:32:07 GMT
ARG KONG_AMD64_SHA=8a33a919f75bdb8bb708de23c0701def2aedfcd2679d27b7849040c3edf273f9
# Wed, 27 Jan 2021 06:32:07 GMT
ENV KONG_AMD64_SHA=8a33a919f75bdb8bb708de23c0701def2aedfcd2679d27b7849040c3edf273f9
# Wed, 27 Jan 2021 06:32:08 GMT
ARG KONG_ARM64_SHA=4ae43ecf9b1fcf11930d859efec475e216729b89b76de80a4c38e1fe58e3874f
# Wed, 27 Jan 2021 06:32:08 GMT
ENV KONG_ARM64_SHA=4ae43ecf9b1fcf11930d859efec475e216729b89b76de80a4c38e1fe58e3874f
# Wed, 27 Jan 2021 06:32:15 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;; 		aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Wed, 27 Jan 2021 06:32:16 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 27 Jan 2021 06:32:16 GMT
USER kong
# Wed, 27 Jan 2021 06:32:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 27 Jan 2021 06:32:16 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 27 Jan 2021 06:32:16 GMT
STOPSIGNAL SIGQUIT
# Wed, 27 Jan 2021 06:32:17 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:0a6724ff3fcd51338afdfdc2b1d4ffd04569818e31efad957213d67c29b45101`  
		Last Modified: Thu, 17 Dec 2020 00:20:26 GMT  
		Size: 2.8 MB (2814864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274efec6805c2b13808c7bcb7932f07b136c0be74bf02bdbf77f79e89dc58725`  
		Last Modified: Thu, 17 Dec 2020 14:59:10 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b18e55f2934bb191d816e87b86e196e1c8d35d815f72f93f7e5f51c0f17319e`  
		Last Modified: Wed, 27 Jan 2021 06:35:34 GMT  
		Size: 48.1 MB (48122597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec1f7f35984e4dfe3874035c9af0e74955cc49424e7f4a0d50411d336f9228fa`  
		Last Modified: Wed, 27 Jan 2021 06:35:24 GMT  
		Size: 735.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:latest` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:d87959fb87a61b8f9fba68a010a6e444317df9ca4bbba731d1374c9035077d0e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50462144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:065a1ea94079d9d30ef22ca0cbfffc961327ac4759c8ab96e9473a3daeb1b436`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:37 GMT
ADD file:47bb1b85a4eb4d0b355ae89ec5c71c09e2c2b7e21e1851a2896365eb17134f57 in / 
# Wed, 16 Dec 2020 23:40:39 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:57:05 GMT
LABEL maintainer=Kong <support@konghq.com>
# Thu, 17 Dec 2020 04:57:06 GMT
ARG ASSET=ce
# Thu, 17 Dec 2020 04:57:07 GMT
ENV ASSET=ce
# Thu, 17 Dec 2020 04:57:08 GMT
ARG EE_PORTS
# Thu, 17 Dec 2020 04:57:09 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 27 Jan 2021 00:45:22 GMT
ARG KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 00:45:23 GMT
ENV KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 00:45:23 GMT
ARG KONG_AMD64_SHA=8a33a919f75bdb8bb708de23c0701def2aedfcd2679d27b7849040c3edf273f9
# Wed, 27 Jan 2021 00:45:24 GMT
ENV KONG_AMD64_SHA=8a33a919f75bdb8bb708de23c0701def2aedfcd2679d27b7849040c3edf273f9
# Wed, 27 Jan 2021 00:45:24 GMT
ARG KONG_ARM64_SHA=4ae43ecf9b1fcf11930d859efec475e216729b89b76de80a4c38e1fe58e3874f
# Wed, 27 Jan 2021 00:45:25 GMT
ENV KONG_ARM64_SHA=4ae43ecf9b1fcf11930d859efec475e216729b89b76de80a4c38e1fe58e3874f
# Wed, 27 Jan 2021 00:45:38 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256=$KONG_AMD64_SHA ;; 		aarch64) arch='arm64'; KONG_SHA256=$KONG_ARM64_SHA ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Wed, 27 Jan 2021 00:45:40 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 27 Jan 2021 00:45:40 GMT
USER kong
# Wed, 27 Jan 2021 00:45:41 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 27 Jan 2021 00:45:42 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 27 Jan 2021 00:45:42 GMT
STOPSIGNAL SIGQUIT
# Wed, 27 Jan 2021 00:45:43 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:20d8a246443a66e74e17f2a0e81a51fe774876ca0c2676691c37ee1b0e4d3cd5`  
		Last Modified: Wed, 16 Dec 2020 23:41:20 GMT  
		Size: 2.7 MB (2725216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3181cc464c4af55ff9dd73d4603f67578cdc16237deb0e5e467594b40164ab6`  
		Last Modified: Thu, 17 Dec 2020 04:58:48 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:686913a20dd73c0bdaa7517e69803b84807b71b99b4ff55cc9764516b90461f7`  
		Last Modified: Wed, 27 Jan 2021 00:47:56 GMT  
		Size: 47.7 MB (47736063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5429c14c14d5050bce7546a62fa4539c4c325f122c109881ea4dc5f0b628ed6`  
		Last Modified: Wed, 27 Jan 2021 00:47:42 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:ubuntu`

```console
$ docker pull kong@sha256:b46fb4a0cfeedb5a99723b50e3c4d8e251eba950bb95d996f546108469e520d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:597d3f899451bab38b28bc472c6af7ce10a79d4a7f72b242b9dba5a5b80dae9c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.0 MB (134011512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecdda63d33dee4365e82d62414c95e28dac508e4f96086475f17d7411fe7ef11`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 21 Jan 2021 03:39:31 GMT
ADD file:925571658dd8453e5c80d862f5791d6b26b3c2a8688937b11741f2f2c5cdbfd7 in / 
# Thu, 21 Jan 2021 03:39:32 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:39:34 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:39:35 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:39:36 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 10:27:05 GMT
ARG ASSET=ce
# Thu, 21 Jan 2021 10:27:05 GMT
ENV ASSET=ce
# Thu, 21 Jan 2021 10:27:05 GMT
ARG EE_PORTS
# Thu, 21 Jan 2021 10:27:06 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 27 Jan 2021 06:32:22 GMT
ARG KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 06:32:22 GMT
ENV KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 06:33:11 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt update     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Wed, 27 Jan 2021 06:33:12 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Wed, 27 Jan 2021 06:33:12 GMT
USER kong
# Wed, 27 Jan 2021 06:33:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 27 Jan 2021 06:33:12 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 27 Jan 2021 06:33:13 GMT
STOPSIGNAL SIGQUIT
# Wed, 27 Jan 2021 06:33:13 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4007a89234b4f56c03e6831dc220550d2e5fba935d9f5f5bcea64857ac4f4888`  
		Last Modified: Mon, 18 Jan 2021 19:38:08 GMT  
		Size: 46.0 MB (45962352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfa26c6b9c9d1ccbcb1eaa65befa376805d9324174ac580ca76fdedc3575f54`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba7bf18aa406cb7dc372ac732de222b04d1c824ff1705d8900831c3d1361ff5`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 527.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6ec688ebe374ea7d89ce967576d221a177ebd2c02ca9f053197f954102e30b`  
		Last Modified: Thu, 21 Jan 2021 03:41:24 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7491b48e51562c145461304393cbc54944e319e09a7714bf0e4264da38b8a8f0`  
		Last Modified: Thu, 21 Jan 2021 10:30:38 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c37a4a4ce379b4b55c1ee57df48a2c7f66ef0480f4217df19284fb0ac887147`  
		Last Modified: Wed, 27 Jan 2021 06:36:06 GMT  
		Size: 63.0 MB (62964969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ff52cba088e18ceb7be8ffce04fd152b6a4df798b5bad5a296d22fd49538e01`  
		Last Modified: Wed, 27 Jan 2021 06:35:43 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:f16de38cd2620af9554e1a3a8e55c22d36cb4640d73bea97c7cdcbed88cff9e2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.4 MB (125352533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f74865582600b00fdd71d91664fb06575999525d67115492f4cc56371a8daeee`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Thu, 21 Jan 2021 03:51:12 GMT
ADD file:e2f37be259f081b70bc884e3b7f652e5d9a0ad4ae443f2258b79a1b14377cc20 in / 
# Thu, 21 Jan 2021 03:51:17 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 21 Jan 2021 03:51:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 21 Jan 2021 03:51:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 21 Jan 2021 03:51:22 GMT
CMD ["/bin/bash"]
# Thu, 21 Jan 2021 05:32:05 GMT
ARG ASSET=ce
# Thu, 21 Jan 2021 05:32:06 GMT
ENV ASSET=ce
# Thu, 21 Jan 2021 05:32:06 GMT
ARG EE_PORTS
# Thu, 21 Jan 2021 05:32:07 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 27 Jan 2021 00:45:49 GMT
ARG KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 00:45:50 GMT
ENV KONG_VERSION=2.3.1
# Wed, 27 Jan 2021 00:46:39 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt update     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && chown kong:0 /usr/local/bin/kong     && chown -R kong:0 /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Wed, 27 Jan 2021 00:46:41 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Wed, 27 Jan 2021 00:46:42 GMT
USER kong
# Wed, 27 Jan 2021 00:46:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 27 Jan 2021 00:46:43 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 27 Jan 2021 00:46:44 GMT
STOPSIGNAL SIGQUIT
# Wed, 27 Jan 2021 00:46:44 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:79186a4c5361c6b018fe75c9bba66c9bf717db8d7d4a6ddb18fb86171f277b61`  
		Last Modified: Thu, 14 Jan 2021 16:25:21 GMT  
		Size: 40.9 MB (40885219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96f901e8ebcf64a42ec369549f6269ec96cd97b424389ca99a8ebb722c59c12`  
		Last Modified: Thu, 21 Jan 2021 03:53:10 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36fd1545244608cb9ef92efa528b6e8c3229f1b01ca414ee8717219145cdff7d`  
		Last Modified: Thu, 21 Jan 2021 03:53:10 GMT  
		Size: 468.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d978c0f55122642ba1a22cc67abf7af2e898bfb42933b1879c2dd91fd987147d`  
		Last Modified: Thu, 21 Jan 2021 03:53:11 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e81e83cdfa4fc6fce4a28de27bb31753456d14bad0dcc25aabceaa0a03a3345`  
		Last Modified: Thu, 21 Jan 2021 05:37:21 GMT  
		Size: 25.1 MB (25081954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e92def6c86f1cd19fef7864bb7f4b62cbb86f8d16f6845ecec91126b1f9c7d`  
		Last Modified: Wed, 27 Jan 2021 00:48:28 GMT  
		Size: 59.4 MB (59383183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fa36af64dff18650ff7c3948d67dab978c2fa075442c01a124f7cb86ba51ff5`  
		Last Modified: Wed, 27 Jan 2021 00:48:09 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
