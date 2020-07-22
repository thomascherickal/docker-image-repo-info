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
-	[`kong:2.1.0`](#kong210)
-	[`kong:2.1.0-alpine`](#kong210-alpine)
-	[`kong:2.1.0-centos`](#kong210-centos)
-	[`kong:2.1.0-ubuntu`](#kong210-ubuntu)
-	[`kong:2.1-alpine`](#kong21-alpine)
-	[`kong:2.1-centos`](#kong21-centos)
-	[`kong:2.1-ubuntu`](#kong21-ubuntu)
-	[`kong:alpine`](#kongalpine)
-	[`kong:centos`](#kongcentos)
-	[`kong:latest`](#konglatest)
-	[`kong:ubuntu`](#kongubuntu)

## `kong:2`

```console
$ docker pull kong@sha256:f2b002534e28d44d70ae19e8dc30acb47ee3c14503a661d6cc16526d9b212d49
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2` - linux; amd64

```console
$ docker pull kong@sha256:aa6d39989058a27439807d9fc09becdcef04ca9d5c3a87fd2390f3e4fe210cf2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53140755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d91e9ff0399c788d760a0dc5f7416ef1d02a910dbf02b9a23d49dc0d0d7666f2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Tue, 05 May 2020 00:19:56 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 05 May 2020 00:19:56 GMT
ARG ASSET=ce
# Tue, 05 May 2020 00:19:56 GMT
ENV ASSET=ce
# Mon, 13 Jul 2020 17:19:53 GMT
ARG EE_PORTS
# Mon, 13 Jul 2020 17:19:53 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 22 Jul 2020 00:34:09 GMT
ARG KONG_VERSION=2.1.0
# Wed, 22 Jul 2020 00:34:09 GMT
ENV KONG_VERSION=2.1.0
# Wed, 22 Jul 2020 00:34:10 GMT
ARG KONG_SHA256=8e5322ba57591e75e6c0d2cfe602cc104467be2336a4075c80831fb53cbb1f78
# Wed, 22 Jul 2020 00:34:22 GMT
# ARGS: KONG_SHA256=8e5322ba57591e75e6c0d2cfe602cc104467be2336a4075c80831fb53cbb1f78
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong; 	tar -C /kong -xzf /tmp/kong.tar.gz && 	mv /kong/usr/local/* /usr/local && 	mv /kong/etc/* /etc && 	rm -rf /kong && 	apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates && 	adduser -S kong && 	mkdir -p "/usr/local/kong" && 	chown -R kong:0 /usr/local/kong && 	chown kong:0 /usr/local/bin/kong && 	chmod -R g=u /usr/local/kong && 	rm -rf /tmp/kong.tar.gz &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Wed, 22 Jul 2020 00:34:23 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 22 Jul 2020 00:34:24 GMT
USER kong
# Wed, 22 Jul 2020 00:34:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jul 2020 00:34:24 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 22 Jul 2020 00:34:25 GMT
STOPSIGNAL SIGQUIT
# Wed, 22 Jul 2020 00:34:25 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e0de2dc0e7e86d092bbee85a6c1ef2769273bd1a78d87bc9a745745fe2d3b9`  
		Last Modified: Mon, 13 Jul 2020 17:21:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d7dc22eefcb6b9c7d444afb334e5cf62640b57f3d58a8a1d608b258bd30f90`  
		Last Modified: Wed, 22 Jul 2020 00:36:57 GMT  
		Size: 50.3 MB (50326578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b904e61d124ac9189b2e76c7f81a19d1b66899fe651573b702594f557ecc34d`  
		Last Modified: Wed, 22 Jul 2020 00:36:42 GMT  
		Size: 732.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.0`

```console
$ docker pull kong@sha256:694e8a2b046a28a846029e0e6b00f9087d644fab94435c872514c0673053087c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.0` - linux; amd64

```console
$ docker pull kong@sha256:dcbcf61b6577441fd7d9b0b3729f4ae08a5d1bf7f277bcc79fd60fe3e110a15b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.8 MB (52761708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cd6bc3dc6120ac04c63d99c82a2d117798dc4663ada08099c314d45bb49c9d2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Tue, 05 May 2020 00:19:56 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 05 May 2020 00:19:56 GMT
ARG ASSET=ce
# Tue, 05 May 2020 00:19:56 GMT
ENV ASSET=ce
# Tue, 05 May 2020 00:19:57 GMT
COPY file:987d0472e007e4e357d96fa432bce568836a2259b787227f9a9e1c369d9efc37 in /tmp/kong.tar.gz 
# Fri, 10 Jul 2020 20:22:10 GMT
ARG KONG_VERSION=2.0.5
# Fri, 10 Jul 2020 20:22:10 GMT
ENV KONG_VERSION=2.0.5
# Fri, 10 Jul 2020 20:22:10 GMT
ARG KONG_SHA256=2e78dee0e695c238cde7e607e85c2e62e44422b57c626ea12822d15ed898769b
# Fri, 10 Jul 2020 20:22:11 GMT
ENV KONG_SHA256=2e78dee0e695c238cde7e607e85c2e62e44422b57c626ea12822d15ed898769b
# Fri, 10 Jul 2020 20:22:17 GMT
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong; 	tar -C /kong -xzf /tmp/kong.tar.gz && 	mv /kong/usr/local/* /usr/local && 	mv /kong/etc/* /etc && 	rm -rf /kong && 	apk add --no-cache libgcc openssl pcre perl tzdata libcap zip bash zlib git ca-certificates && 	adduser -S kong && 	mkdir -p "/usr/local/kong" && 	chown -R kong:0 /usr/local/kong && 	chown kong:0 /usr/local/bin/kong && 	chmod -R g=u /usr/local/kong && 	rm -rf /tmp/kong.tar.gz && 	kong version
# Tue, 14 Jul 2020 20:21:10 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Tue, 14 Jul 2020 20:21:10 GMT
USER kong
# Tue, 14 Jul 2020 20:21:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 14 Jul 2020 20:21:10 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 14 Jul 2020 20:21:11 GMT
STOPSIGNAL SIGQUIT
# Tue, 14 Jul 2020 20:21:11 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79162f4c09617b6148c79941fef29989fd4efaf75afb688429147db76f1c1937`  
		Last Modified: Tue, 05 May 2020 00:22:34 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9927a578c07417ddbd09bec114df84f8a70d2dc31ed211de27e60350865702`  
		Last Modified: Fri, 10 Jul 2020 20:24:59 GMT  
		Size: 49.9 MB (49947527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d1ef16fef2b440996e796673a1b4cf393245998265d908753d82e07c122512`  
		Last Modified: Tue, 14 Jul 2020 20:22:19 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.0.5`

```console
$ docker pull kong@sha256:694e8a2b046a28a846029e0e6b00f9087d644fab94435c872514c0673053087c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.0.5` - linux; amd64

```console
$ docker pull kong@sha256:dcbcf61b6577441fd7d9b0b3729f4ae08a5d1bf7f277bcc79fd60fe3e110a15b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.8 MB (52761708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cd6bc3dc6120ac04c63d99c82a2d117798dc4663ada08099c314d45bb49c9d2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Tue, 05 May 2020 00:19:56 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 05 May 2020 00:19:56 GMT
ARG ASSET=ce
# Tue, 05 May 2020 00:19:56 GMT
ENV ASSET=ce
# Tue, 05 May 2020 00:19:57 GMT
COPY file:987d0472e007e4e357d96fa432bce568836a2259b787227f9a9e1c369d9efc37 in /tmp/kong.tar.gz 
# Fri, 10 Jul 2020 20:22:10 GMT
ARG KONG_VERSION=2.0.5
# Fri, 10 Jul 2020 20:22:10 GMT
ENV KONG_VERSION=2.0.5
# Fri, 10 Jul 2020 20:22:10 GMT
ARG KONG_SHA256=2e78dee0e695c238cde7e607e85c2e62e44422b57c626ea12822d15ed898769b
# Fri, 10 Jul 2020 20:22:11 GMT
ENV KONG_SHA256=2e78dee0e695c238cde7e607e85c2e62e44422b57c626ea12822d15ed898769b
# Fri, 10 Jul 2020 20:22:17 GMT
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong; 	tar -C /kong -xzf /tmp/kong.tar.gz && 	mv /kong/usr/local/* /usr/local && 	mv /kong/etc/* /etc && 	rm -rf /kong && 	apk add --no-cache libgcc openssl pcre perl tzdata libcap zip bash zlib git ca-certificates && 	adduser -S kong && 	mkdir -p "/usr/local/kong" && 	chown -R kong:0 /usr/local/kong && 	chown kong:0 /usr/local/bin/kong && 	chmod -R g=u /usr/local/kong && 	rm -rf /tmp/kong.tar.gz && 	kong version
# Tue, 14 Jul 2020 20:21:10 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Tue, 14 Jul 2020 20:21:10 GMT
USER kong
# Tue, 14 Jul 2020 20:21:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 14 Jul 2020 20:21:10 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 14 Jul 2020 20:21:11 GMT
STOPSIGNAL SIGQUIT
# Tue, 14 Jul 2020 20:21:11 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79162f4c09617b6148c79941fef29989fd4efaf75afb688429147db76f1c1937`  
		Last Modified: Tue, 05 May 2020 00:22:34 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9927a578c07417ddbd09bec114df84f8a70d2dc31ed211de27e60350865702`  
		Last Modified: Fri, 10 Jul 2020 20:24:59 GMT  
		Size: 49.9 MB (49947527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d1ef16fef2b440996e796673a1b4cf393245998265d908753d82e07c122512`  
		Last Modified: Tue, 14 Jul 2020 20:22:19 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.0.5-alpine`

```console
$ docker pull kong@sha256:694e8a2b046a28a846029e0e6b00f9087d644fab94435c872514c0673053087c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.0.5-alpine` - linux; amd64

```console
$ docker pull kong@sha256:dcbcf61b6577441fd7d9b0b3729f4ae08a5d1bf7f277bcc79fd60fe3e110a15b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.8 MB (52761708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cd6bc3dc6120ac04c63d99c82a2d117798dc4663ada08099c314d45bb49c9d2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Tue, 05 May 2020 00:19:56 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 05 May 2020 00:19:56 GMT
ARG ASSET=ce
# Tue, 05 May 2020 00:19:56 GMT
ENV ASSET=ce
# Tue, 05 May 2020 00:19:57 GMT
COPY file:987d0472e007e4e357d96fa432bce568836a2259b787227f9a9e1c369d9efc37 in /tmp/kong.tar.gz 
# Fri, 10 Jul 2020 20:22:10 GMT
ARG KONG_VERSION=2.0.5
# Fri, 10 Jul 2020 20:22:10 GMT
ENV KONG_VERSION=2.0.5
# Fri, 10 Jul 2020 20:22:10 GMT
ARG KONG_SHA256=2e78dee0e695c238cde7e607e85c2e62e44422b57c626ea12822d15ed898769b
# Fri, 10 Jul 2020 20:22:11 GMT
ENV KONG_SHA256=2e78dee0e695c238cde7e607e85c2e62e44422b57c626ea12822d15ed898769b
# Fri, 10 Jul 2020 20:22:17 GMT
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong; 	tar -C /kong -xzf /tmp/kong.tar.gz && 	mv /kong/usr/local/* /usr/local && 	mv /kong/etc/* /etc && 	rm -rf /kong && 	apk add --no-cache libgcc openssl pcre perl tzdata libcap zip bash zlib git ca-certificates && 	adduser -S kong && 	mkdir -p "/usr/local/kong" && 	chown -R kong:0 /usr/local/kong && 	chown kong:0 /usr/local/bin/kong && 	chmod -R g=u /usr/local/kong && 	rm -rf /tmp/kong.tar.gz && 	kong version
# Tue, 14 Jul 2020 20:21:10 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Tue, 14 Jul 2020 20:21:10 GMT
USER kong
# Tue, 14 Jul 2020 20:21:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 14 Jul 2020 20:21:10 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 14 Jul 2020 20:21:11 GMT
STOPSIGNAL SIGQUIT
# Tue, 14 Jul 2020 20:21:11 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79162f4c09617b6148c79941fef29989fd4efaf75afb688429147db76f1c1937`  
		Last Modified: Tue, 05 May 2020 00:22:34 GMT  
		Size: 132.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9927a578c07417ddbd09bec114df84f8a70d2dc31ed211de27e60350865702`  
		Last Modified: Fri, 10 Jul 2020 20:24:59 GMT  
		Size: 49.9 MB (49947527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d1ef16fef2b440996e796673a1b4cf393245998265d908753d82e07c122512`  
		Last Modified: Tue, 14 Jul 2020 20:22:19 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.0.5-centos`

```console
$ docker pull kong@sha256:796bde8b61581c315bbfdf3c85e9002599dc630c6fbb456c8bbf9ec5aa2c12cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.0.5-centos` - linux; amd64

```console
$ docker pull kong@sha256:5e129dca95cbb055cdaaa9806966569be196446d3b38122a01991a1245e1c1fa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127222587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6ff1d4be6c902aabe1ad9a93e37eac121f1781af332682e2826cb27087f357d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:54:26 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 05 May 2020 21:54:26 GMT
ARG ASSET=ce
# Tue, 05 May 2020 21:54:27 GMT
ENV ASSET=ce
# Tue, 05 May 2020 21:54:27 GMT
COPY file:73044b225363e2703a176f55b132687ead4bab30398788756be18d2965fac2cd in /tmp/kong.rpm 
# Fri, 10 Jul 2020 20:23:32 GMT
ARG KONG_VERSION=2.0.5
# Fri, 10 Jul 2020 20:23:32 GMT
ENV KONG_VERSION=2.0.5
# Fri, 10 Jul 2020 20:23:33 GMT
ARG KONG_SHA256=e05340680de3541c4c940f54e64f00c90fb5137f6a8c71e413b815a411d74fc6
# Fri, 10 Jul 2020 20:23:33 GMT
ENV KONG_SHA256=e05340680de3541c4c940f54e64f00c90fb5137f6a8c71e413b815a411d74fc6
# Fri, 10 Jul 2020 20:24:05 GMT
RUN set -ex; 	if [ "$ASSET" = "ce" ] ; then 		curl -fL "https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm" -o /tmp/kong.rpm 		&& echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -; 	fi; 	yum install -y -q unzip shadow-utils git zlib 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki 	&& useradd kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y /tmp/kong.rpm 	&& yum clean all 	&& rm /tmp/kong.rpm 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong 	&& kong version
# Tue, 14 Jul 2020 20:21:20 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Tue, 14 Jul 2020 20:21:20 GMT
USER kong
# Tue, 14 Jul 2020 20:21:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 14 Jul 2020 20:21:21 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 14 Jul 2020 20:21:21 GMT
STOPSIGNAL SIGQUIT
# Tue, 14 Jul 2020 20:21:21 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce7701dd3817fcacdc04d8abfd7cd6ea61fe7f4d909903260a2ebe43fce007f`  
		Last Modified: Tue, 05 May 2020 22:02:15 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e839438e3b2588088e4bb0885546faeba1afe1d70b47fd88048e9d0c70ae370`  
		Last Modified: Fri, 10 Jul 2020 20:25:43 GMT  
		Size: 51.3 MB (51341586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9126f205ac0dfa5d13b956c46b11ff4a8f1b45f444a6d30d7d070dbbc3f882`  
		Last Modified: Tue, 14 Jul 2020 20:22:29 GMT  
		Size: 731.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.0.5-ubuntu`

```console
$ docker pull kong@sha256:c3eb87c75880fe0f23add5953e09fe57f9d00d5760a110879d285dbf594c32fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.0.5-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:6b4e8a1a9a62a630681c7756712cc750fabfe497fc3fb5fb10fb74be48d40ab8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.5 MB (99451284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df667bda5f7cfff805a379a18b00d1c0ee6b3b914d38aa5491af43e68b299779`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 06 Jul 2020 21:57:02 GMT
ADD file:47805a69cb7dd669e357d291ce27735c2d514348468b2d3e69c66161a4f80abd in / 
# Mon, 06 Jul 2020 21:57:03 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 21:57:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:57:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:57:05 GMT
CMD ["/bin/bash"]
# Tue, 07 Jul 2020 00:16:32 GMT
ARG ASSET=ce
# Tue, 07 Jul 2020 00:16:32 GMT
ENV ASSET=ce
# Tue, 07 Jul 2020 00:16:32 GMT
COPY file:5307743dbc5e81034b8adaf56f281bcb13b0da2d468cb6450d72fa5b77543ccf in /tmp/kong.deb 
# Fri, 10 Jul 2020 20:22:26 GMT
ARG KONG_VERSION=2.0.5
# Fri, 10 Jul 2020 20:22:27 GMT
ENV KONG_VERSION=2.0.5
# Fri, 10 Jul 2020 20:23:19 GMT
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apt-get update &&         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get update     && apt-get install -y --no-install-recommends perl unzip git zlib1g     && rm -rf /var/lib/apt/lists/* 	&& dpkg -i /tmp/kong.deb 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong 	&& kong version
# Tue, 14 Jul 2020 20:21:15 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Tue, 14 Jul 2020 20:21:15 GMT
USER kong
# Tue, 14 Jul 2020 20:21:16 GMT
RUN kong version
# Tue, 14 Jul 2020 20:21:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 14 Jul 2020 20:21:16 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 14 Jul 2020 20:21:16 GMT
STOPSIGNAL SIGQUIT
# Tue, 14 Jul 2020 20:21:16 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:6aa38bd67045d3ed7e7a73ca42e06fadbfd139a26693bf2dc8b9ccc318d87c3c`  
		Last Modified: Sat, 20 Jun 2020 13:20:13 GMT  
		Size: 44.4 MB (44374155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981ae4862c056451e69578c614f07a5b552995d3fc1cf17d5dc78a26e8455d5a`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bad8949dcb16a7693551042e056cef1e767ac0a23625a2eb9ae33ac44ac80f9`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9461589e708efab1c30577ec50f06db05714523e2976c7da421b0b418312e0`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:143c32b458621fe6c4f8e03075d63acff14f384d32857620905001d581d3c71c`  
		Last Modified: Tue, 07 Jul 2020 00:18:48 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45172d359af51baaf3dc0a9e537bc71fac320cf453f5b369f70fba3418223e7`  
		Last Modified: Fri, 10 Jul 2020 20:25:24 GMT  
		Size: 55.1 MB (55074676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e564bc0d8300439c3273f39bc63005787298e59f06bbfab6e87199d3ba52d5b`  
		Last Modified: Tue, 14 Jul 2020 20:22:25 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b59fe2ff34e8eaa3294fc6f9da73182f47cc2b7f93b922d3d7f94d46475240`  
		Last Modified: Tue, 14 Jul 2020 20:22:24 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.0.5-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:edf13a5e37df421ac8019f8074d6c5cdadc11267485e2f1e3adb42a3b2b24058
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.2 MB (92210065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b17f54197a5b2fca719b002bc8c26363d1e816fbb479e62038e41eed156b35ec`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 06 Jul 2020 22:06:25 GMT
ADD file:eacc4e3c71dca085a01eb1b781c8312350bcb2288a1f6ceeefb68d660b3215b5 in / 
# Mon, 06 Jul 2020 22:06:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 22:06:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 22:06:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 22:06:39 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:11:52 GMT
ARG ASSET=ce
# Mon, 06 Jul 2020 23:11:52 GMT
ENV ASSET=ce
# Mon, 06 Jul 2020 23:11:53 GMT
COPY file:5307743dbc5e81034b8adaf56f281bcb13b0da2d468cb6450d72fa5b77543ccf in /tmp/kong.deb 
# Fri, 10 Jul 2020 18:54:55 GMT
ARG KONG_VERSION=2.0.5
# Fri, 10 Jul 2020 18:54:56 GMT
ENV KONG_VERSION=2.0.5
# Fri, 10 Jul 2020 18:55:47 GMT
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apt-get update &&         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get update     && apt-get install -y --no-install-recommends perl unzip git zlib1g     && rm -rf /var/lib/apt/lists/* 	&& dpkg -i /tmp/kong.deb 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong 	&& kong version
# Tue, 14 Jul 2020 19:46:30 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Tue, 14 Jul 2020 19:46:50 GMT
USER kong
# Tue, 14 Jul 2020 19:48:02 GMT
RUN kong version
# Tue, 14 Jul 2020 19:48:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 14 Jul 2020 19:48:33 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 14 Jul 2020 19:48:51 GMT
STOPSIGNAL SIGQUIT
# Tue, 14 Jul 2020 19:49:07 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4ab489c2a6275c4f4b0c3ccbc0c397c7b4d1e3278136f158f0345707b88775ce`  
		Last Modified: Sat, 20 Jun 2020 00:25:22 GMT  
		Size: 40.0 MB (40035468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd7a7bb5cc1bf1dc02973eb563c00d2491059923f17bdcc83b37d65a6015b74`  
		Last Modified: Mon, 06 Jul 2020 22:07:41 GMT  
		Size: 471.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3150055c00370319e479ec8c335cd23b2564e0546e6e50593f651a6311be5a83`  
		Last Modified: Mon, 06 Jul 2020 22:07:41 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee51ca48c53d0f23ff69410d387087d1f50be8472db56cb051f280b80038ac7`  
		Last Modified: Mon, 06 Jul 2020 22:07:41 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3e9d9ca3d496619cb7d9dd321c5e1b12f499e234a4bfff523ed3169665df8b`  
		Last Modified: Mon, 06 Jul 2020 23:15:03 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2b84f9b564c8b8ef4fd6cdb868810c92459d745ea478b543b2503fc566f3ea`  
		Last Modified: Fri, 10 Jul 2020 18:56:29 GMT  
		Size: 52.2 MB (52172193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e17eeb803c5a09b4917500aeffac3fdee8dfa37b2f1d3ce3b42886b86dde907c`  
		Last Modified: Tue, 14 Jul 2020 19:49:57 GMT  
		Size: 687.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a7ab924b8f955fba2c16769a45de94449dcfca1b998551c1bb4aef09d13a81e`  
		Last Modified: Tue, 14 Jul 2020 19:49:57 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.0-centos`

```console
$ docker pull kong@sha256:796bde8b61581c315bbfdf3c85e9002599dc630c6fbb456c8bbf9ec5aa2c12cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.0-centos` - linux; amd64

```console
$ docker pull kong@sha256:5e129dca95cbb055cdaaa9806966569be196446d3b38122a01991a1245e1c1fa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127222587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6ff1d4be6c902aabe1ad9a93e37eac121f1781af332682e2826cb27087f357d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:54:26 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 05 May 2020 21:54:26 GMT
ARG ASSET=ce
# Tue, 05 May 2020 21:54:27 GMT
ENV ASSET=ce
# Tue, 05 May 2020 21:54:27 GMT
COPY file:73044b225363e2703a176f55b132687ead4bab30398788756be18d2965fac2cd in /tmp/kong.rpm 
# Fri, 10 Jul 2020 20:23:32 GMT
ARG KONG_VERSION=2.0.5
# Fri, 10 Jul 2020 20:23:32 GMT
ENV KONG_VERSION=2.0.5
# Fri, 10 Jul 2020 20:23:33 GMT
ARG KONG_SHA256=e05340680de3541c4c940f54e64f00c90fb5137f6a8c71e413b815a411d74fc6
# Fri, 10 Jul 2020 20:23:33 GMT
ENV KONG_SHA256=e05340680de3541c4c940f54e64f00c90fb5137f6a8c71e413b815a411d74fc6
# Fri, 10 Jul 2020 20:24:05 GMT
RUN set -ex; 	if [ "$ASSET" = "ce" ] ; then 		curl -fL "https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm" -o /tmp/kong.rpm 		&& echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -; 	fi; 	yum install -y -q unzip shadow-utils git zlib 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki 	&& useradd kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y /tmp/kong.rpm 	&& yum clean all 	&& rm /tmp/kong.rpm 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong 	&& kong version
# Tue, 14 Jul 2020 20:21:20 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Tue, 14 Jul 2020 20:21:20 GMT
USER kong
# Tue, 14 Jul 2020 20:21:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 14 Jul 2020 20:21:21 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 14 Jul 2020 20:21:21 GMT
STOPSIGNAL SIGQUIT
# Tue, 14 Jul 2020 20:21:21 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce7701dd3817fcacdc04d8abfd7cd6ea61fe7f4d909903260a2ebe43fce007f`  
		Last Modified: Tue, 05 May 2020 22:02:15 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e839438e3b2588088e4bb0885546faeba1afe1d70b47fd88048e9d0c70ae370`  
		Last Modified: Fri, 10 Jul 2020 20:25:43 GMT  
		Size: 51.3 MB (51341586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9126f205ac0dfa5d13b956c46b11ff4a8f1b45f444a6d30d7d070dbbc3f882`  
		Last Modified: Tue, 14 Jul 2020 20:22:29 GMT  
		Size: 731.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.0-ubuntu`

```console
$ docker pull kong@sha256:c3eb87c75880fe0f23add5953e09fe57f9d00d5760a110879d285dbf594c32fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.0-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:6b4e8a1a9a62a630681c7756712cc750fabfe497fc3fb5fb10fb74be48d40ab8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.5 MB (99451284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df667bda5f7cfff805a379a18b00d1c0ee6b3b914d38aa5491af43e68b299779`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 06 Jul 2020 21:57:02 GMT
ADD file:47805a69cb7dd669e357d291ce27735c2d514348468b2d3e69c66161a4f80abd in / 
# Mon, 06 Jul 2020 21:57:03 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 21:57:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:57:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:57:05 GMT
CMD ["/bin/bash"]
# Tue, 07 Jul 2020 00:16:32 GMT
ARG ASSET=ce
# Tue, 07 Jul 2020 00:16:32 GMT
ENV ASSET=ce
# Tue, 07 Jul 2020 00:16:32 GMT
COPY file:5307743dbc5e81034b8adaf56f281bcb13b0da2d468cb6450d72fa5b77543ccf in /tmp/kong.deb 
# Fri, 10 Jul 2020 20:22:26 GMT
ARG KONG_VERSION=2.0.5
# Fri, 10 Jul 2020 20:22:27 GMT
ENV KONG_VERSION=2.0.5
# Fri, 10 Jul 2020 20:23:19 GMT
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apt-get update &&         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get update     && apt-get install -y --no-install-recommends perl unzip git zlib1g     && rm -rf /var/lib/apt/lists/* 	&& dpkg -i /tmp/kong.deb 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong 	&& kong version
# Tue, 14 Jul 2020 20:21:15 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Tue, 14 Jul 2020 20:21:15 GMT
USER kong
# Tue, 14 Jul 2020 20:21:16 GMT
RUN kong version
# Tue, 14 Jul 2020 20:21:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 14 Jul 2020 20:21:16 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 14 Jul 2020 20:21:16 GMT
STOPSIGNAL SIGQUIT
# Tue, 14 Jul 2020 20:21:16 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:6aa38bd67045d3ed7e7a73ca42e06fadbfd139a26693bf2dc8b9ccc318d87c3c`  
		Last Modified: Sat, 20 Jun 2020 13:20:13 GMT  
		Size: 44.4 MB (44374155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981ae4862c056451e69578c614f07a5b552995d3fc1cf17d5dc78a26e8455d5a`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bad8949dcb16a7693551042e056cef1e767ac0a23625a2eb9ae33ac44ac80f9`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9461589e708efab1c30577ec50f06db05714523e2976c7da421b0b418312e0`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:143c32b458621fe6c4f8e03075d63acff14f384d32857620905001d581d3c71c`  
		Last Modified: Tue, 07 Jul 2020 00:18:48 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45172d359af51baaf3dc0a9e537bc71fac320cf453f5b369f70fba3418223e7`  
		Last Modified: Fri, 10 Jul 2020 20:25:24 GMT  
		Size: 55.1 MB (55074676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e564bc0d8300439c3273f39bc63005787298e59f06bbfab6e87199d3ba52d5b`  
		Last Modified: Tue, 14 Jul 2020 20:22:25 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b59fe2ff34e8eaa3294fc6f9da73182f47cc2b7f93b922d3d7f94d46475240`  
		Last Modified: Tue, 14 Jul 2020 20:22:24 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.0-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:edf13a5e37df421ac8019f8074d6c5cdadc11267485e2f1e3adb42a3b2b24058
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.2 MB (92210065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b17f54197a5b2fca719b002bc8c26363d1e816fbb479e62038e41eed156b35ec`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 06 Jul 2020 22:06:25 GMT
ADD file:eacc4e3c71dca085a01eb1b781c8312350bcb2288a1f6ceeefb68d660b3215b5 in / 
# Mon, 06 Jul 2020 22:06:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 22:06:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 22:06:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 22:06:39 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:11:52 GMT
ARG ASSET=ce
# Mon, 06 Jul 2020 23:11:52 GMT
ENV ASSET=ce
# Mon, 06 Jul 2020 23:11:53 GMT
COPY file:5307743dbc5e81034b8adaf56f281bcb13b0da2d468cb6450d72fa5b77543ccf in /tmp/kong.deb 
# Fri, 10 Jul 2020 18:54:55 GMT
ARG KONG_VERSION=2.0.5
# Fri, 10 Jul 2020 18:54:56 GMT
ENV KONG_VERSION=2.0.5
# Fri, 10 Jul 2020 18:55:47 GMT
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apt-get update &&         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get update     && apt-get install -y --no-install-recommends perl unzip git zlib1g     && rm -rf /var/lib/apt/lists/* 	&& dpkg -i /tmp/kong.deb 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong 	&& kong version
# Tue, 14 Jul 2020 19:46:30 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Tue, 14 Jul 2020 19:46:50 GMT
USER kong
# Tue, 14 Jul 2020 19:48:02 GMT
RUN kong version
# Tue, 14 Jul 2020 19:48:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 14 Jul 2020 19:48:33 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 14 Jul 2020 19:48:51 GMT
STOPSIGNAL SIGQUIT
# Tue, 14 Jul 2020 19:49:07 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4ab489c2a6275c4f4b0c3ccbc0c397c7b4d1e3278136f158f0345707b88775ce`  
		Last Modified: Sat, 20 Jun 2020 00:25:22 GMT  
		Size: 40.0 MB (40035468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd7a7bb5cc1bf1dc02973eb563c00d2491059923f17bdcc83b37d65a6015b74`  
		Last Modified: Mon, 06 Jul 2020 22:07:41 GMT  
		Size: 471.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3150055c00370319e479ec8c335cd23b2564e0546e6e50593f651a6311be5a83`  
		Last Modified: Mon, 06 Jul 2020 22:07:41 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee51ca48c53d0f23ff69410d387087d1f50be8472db56cb051f280b80038ac7`  
		Last Modified: Mon, 06 Jul 2020 22:07:41 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3e9d9ca3d496619cb7d9dd321c5e1b12f499e234a4bfff523ed3169665df8b`  
		Last Modified: Mon, 06 Jul 2020 23:15:03 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c2b84f9b564c8b8ef4fd6cdb868810c92459d745ea478b543b2503fc566f3ea`  
		Last Modified: Fri, 10 Jul 2020 18:56:29 GMT  
		Size: 52.2 MB (52172193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e17eeb803c5a09b4917500aeffac3fdee8dfa37b2f1d3ce3b42886b86dde907c`  
		Last Modified: Tue, 14 Jul 2020 19:49:57 GMT  
		Size: 687.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a7ab924b8f955fba2c16769a45de94449dcfca1b998551c1bb4aef09d13a81e`  
		Last Modified: Tue, 14 Jul 2020 19:49:57 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.1`

```console
$ docker pull kong@sha256:f2b002534e28d44d70ae19e8dc30acb47ee3c14503a661d6cc16526d9b212d49
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.1` - linux; amd64

```console
$ docker pull kong@sha256:aa6d39989058a27439807d9fc09becdcef04ca9d5c3a87fd2390f3e4fe210cf2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53140755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d91e9ff0399c788d760a0dc5f7416ef1d02a910dbf02b9a23d49dc0d0d7666f2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Tue, 05 May 2020 00:19:56 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 05 May 2020 00:19:56 GMT
ARG ASSET=ce
# Tue, 05 May 2020 00:19:56 GMT
ENV ASSET=ce
# Mon, 13 Jul 2020 17:19:53 GMT
ARG EE_PORTS
# Mon, 13 Jul 2020 17:19:53 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 22 Jul 2020 00:34:09 GMT
ARG KONG_VERSION=2.1.0
# Wed, 22 Jul 2020 00:34:09 GMT
ENV KONG_VERSION=2.1.0
# Wed, 22 Jul 2020 00:34:10 GMT
ARG KONG_SHA256=8e5322ba57591e75e6c0d2cfe602cc104467be2336a4075c80831fb53cbb1f78
# Wed, 22 Jul 2020 00:34:22 GMT
# ARGS: KONG_SHA256=8e5322ba57591e75e6c0d2cfe602cc104467be2336a4075c80831fb53cbb1f78
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong; 	tar -C /kong -xzf /tmp/kong.tar.gz && 	mv /kong/usr/local/* /usr/local && 	mv /kong/etc/* /etc && 	rm -rf /kong && 	apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates && 	adduser -S kong && 	mkdir -p "/usr/local/kong" && 	chown -R kong:0 /usr/local/kong && 	chown kong:0 /usr/local/bin/kong && 	chmod -R g=u /usr/local/kong && 	rm -rf /tmp/kong.tar.gz &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Wed, 22 Jul 2020 00:34:23 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 22 Jul 2020 00:34:24 GMT
USER kong
# Wed, 22 Jul 2020 00:34:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jul 2020 00:34:24 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 22 Jul 2020 00:34:25 GMT
STOPSIGNAL SIGQUIT
# Wed, 22 Jul 2020 00:34:25 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e0de2dc0e7e86d092bbee85a6c1ef2769273bd1a78d87bc9a745745fe2d3b9`  
		Last Modified: Mon, 13 Jul 2020 17:21:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d7dc22eefcb6b9c7d444afb334e5cf62640b57f3d58a8a1d608b258bd30f90`  
		Last Modified: Wed, 22 Jul 2020 00:36:57 GMT  
		Size: 50.3 MB (50326578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b904e61d124ac9189b2e76c7f81a19d1b66899fe651573b702594f557ecc34d`  
		Last Modified: Wed, 22 Jul 2020 00:36:42 GMT  
		Size: 732.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.1.0`

```console
$ docker pull kong@sha256:f2b002534e28d44d70ae19e8dc30acb47ee3c14503a661d6cc16526d9b212d49
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.1.0` - linux; amd64

```console
$ docker pull kong@sha256:aa6d39989058a27439807d9fc09becdcef04ca9d5c3a87fd2390f3e4fe210cf2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53140755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d91e9ff0399c788d760a0dc5f7416ef1d02a910dbf02b9a23d49dc0d0d7666f2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Tue, 05 May 2020 00:19:56 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 05 May 2020 00:19:56 GMT
ARG ASSET=ce
# Tue, 05 May 2020 00:19:56 GMT
ENV ASSET=ce
# Mon, 13 Jul 2020 17:19:53 GMT
ARG EE_PORTS
# Mon, 13 Jul 2020 17:19:53 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 22 Jul 2020 00:34:09 GMT
ARG KONG_VERSION=2.1.0
# Wed, 22 Jul 2020 00:34:09 GMT
ENV KONG_VERSION=2.1.0
# Wed, 22 Jul 2020 00:34:10 GMT
ARG KONG_SHA256=8e5322ba57591e75e6c0d2cfe602cc104467be2336a4075c80831fb53cbb1f78
# Wed, 22 Jul 2020 00:34:22 GMT
# ARGS: KONG_SHA256=8e5322ba57591e75e6c0d2cfe602cc104467be2336a4075c80831fb53cbb1f78
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong; 	tar -C /kong -xzf /tmp/kong.tar.gz && 	mv /kong/usr/local/* /usr/local && 	mv /kong/etc/* /etc && 	rm -rf /kong && 	apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates && 	adduser -S kong && 	mkdir -p "/usr/local/kong" && 	chown -R kong:0 /usr/local/kong && 	chown kong:0 /usr/local/bin/kong && 	chmod -R g=u /usr/local/kong && 	rm -rf /tmp/kong.tar.gz &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Wed, 22 Jul 2020 00:34:23 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 22 Jul 2020 00:34:24 GMT
USER kong
# Wed, 22 Jul 2020 00:34:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jul 2020 00:34:24 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 22 Jul 2020 00:34:25 GMT
STOPSIGNAL SIGQUIT
# Wed, 22 Jul 2020 00:34:25 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e0de2dc0e7e86d092bbee85a6c1ef2769273bd1a78d87bc9a745745fe2d3b9`  
		Last Modified: Mon, 13 Jul 2020 17:21:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d7dc22eefcb6b9c7d444afb334e5cf62640b57f3d58a8a1d608b258bd30f90`  
		Last Modified: Wed, 22 Jul 2020 00:36:57 GMT  
		Size: 50.3 MB (50326578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b904e61d124ac9189b2e76c7f81a19d1b66899fe651573b702594f557ecc34d`  
		Last Modified: Wed, 22 Jul 2020 00:36:42 GMT  
		Size: 732.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.1.0-alpine`

```console
$ docker pull kong@sha256:f2b002534e28d44d70ae19e8dc30acb47ee3c14503a661d6cc16526d9b212d49
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.1.0-alpine` - linux; amd64

```console
$ docker pull kong@sha256:aa6d39989058a27439807d9fc09becdcef04ca9d5c3a87fd2390f3e4fe210cf2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53140755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d91e9ff0399c788d760a0dc5f7416ef1d02a910dbf02b9a23d49dc0d0d7666f2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Tue, 05 May 2020 00:19:56 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 05 May 2020 00:19:56 GMT
ARG ASSET=ce
# Tue, 05 May 2020 00:19:56 GMT
ENV ASSET=ce
# Mon, 13 Jul 2020 17:19:53 GMT
ARG EE_PORTS
# Mon, 13 Jul 2020 17:19:53 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 22 Jul 2020 00:34:09 GMT
ARG KONG_VERSION=2.1.0
# Wed, 22 Jul 2020 00:34:09 GMT
ENV KONG_VERSION=2.1.0
# Wed, 22 Jul 2020 00:34:10 GMT
ARG KONG_SHA256=8e5322ba57591e75e6c0d2cfe602cc104467be2336a4075c80831fb53cbb1f78
# Wed, 22 Jul 2020 00:34:22 GMT
# ARGS: KONG_SHA256=8e5322ba57591e75e6c0d2cfe602cc104467be2336a4075c80831fb53cbb1f78
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong; 	tar -C /kong -xzf /tmp/kong.tar.gz && 	mv /kong/usr/local/* /usr/local && 	mv /kong/etc/* /etc && 	rm -rf /kong && 	apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates && 	adduser -S kong && 	mkdir -p "/usr/local/kong" && 	chown -R kong:0 /usr/local/kong && 	chown kong:0 /usr/local/bin/kong && 	chmod -R g=u /usr/local/kong && 	rm -rf /tmp/kong.tar.gz &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Wed, 22 Jul 2020 00:34:23 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 22 Jul 2020 00:34:24 GMT
USER kong
# Wed, 22 Jul 2020 00:34:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jul 2020 00:34:24 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 22 Jul 2020 00:34:25 GMT
STOPSIGNAL SIGQUIT
# Wed, 22 Jul 2020 00:34:25 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e0de2dc0e7e86d092bbee85a6c1ef2769273bd1a78d87bc9a745745fe2d3b9`  
		Last Modified: Mon, 13 Jul 2020 17:21:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d7dc22eefcb6b9c7d444afb334e5cf62640b57f3d58a8a1d608b258bd30f90`  
		Last Modified: Wed, 22 Jul 2020 00:36:57 GMT  
		Size: 50.3 MB (50326578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b904e61d124ac9189b2e76c7f81a19d1b66899fe651573b702594f557ecc34d`  
		Last Modified: Wed, 22 Jul 2020 00:36:42 GMT  
		Size: 732.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.1.0-centos`

```console
$ docker pull kong@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `kong:2.1.0-ubuntu`

```console
$ docker pull kong@sha256:cfa17f065e22eb525b133427804cac2a279e7dffc3474f5ba1b9b6b49c6bc1c5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.1.0-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:4257052170ff58c26aca38d50bce8830844b1194abaf8ae1ebe57d20f75bb188
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.0 MB (109048772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5593e58b150d111a56c25898d068a0053cd214f3df4232dcccef6aab203985b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 06 Jul 2020 21:57:02 GMT
ADD file:47805a69cb7dd669e357d291ce27735c2d514348468b2d3e69c66161a4f80abd in / 
# Mon, 06 Jul 2020 21:57:03 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 21:57:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:57:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:57:05 GMT
CMD ["/bin/bash"]
# Tue, 07 Jul 2020 00:16:32 GMT
ARG ASSET=ce
# Tue, 07 Jul 2020 00:16:32 GMT
ENV ASSET=ce
# Mon, 13 Jul 2020 17:20:07 GMT
ARG EE_PORTS
# Mon, 13 Jul 2020 17:20:07 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Wed, 22 Jul 2020 00:34:32 GMT
ARG KONG_VERSION=2.1.0
# Wed, 22 Jul 2020 00:34:33 GMT
ENV KONG_VERSION=2.1.0
# Wed, 22 Jul 2020 00:35:40 GMT
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apt-get update &&         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get update     && apt-get install -y --no-install-recommends perl unzip git     && { apt-get install -y --no-install-recommends zlibc || true; }     && { apt-get install -y --no-install-recommends zlib1g-dev || true; }     && rm -rf /var/lib/apt/lists/* 	&& dpkg -i /tmp/kong.deb 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Wed, 22 Jul 2020 00:35:41 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Wed, 22 Jul 2020 00:35:41 GMT
USER kong
# Wed, 22 Jul 2020 00:35:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jul 2020 00:35:42 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 22 Jul 2020 00:35:42 GMT
STOPSIGNAL SIGQUIT
# Wed, 22 Jul 2020 00:35:43 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:6aa38bd67045d3ed7e7a73ca42e06fadbfd139a26693bf2dc8b9ccc318d87c3c`  
		Last Modified: Sat, 20 Jun 2020 13:20:13 GMT  
		Size: 44.4 MB (44374155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981ae4862c056451e69578c614f07a5b552995d3fc1cf17d5dc78a26e8455d5a`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bad8949dcb16a7693551042e056cef1e767ac0a23625a2eb9ae33ac44ac80f9`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9461589e708efab1c30577ec50f06db05714523e2976c7da421b0b418312e0`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5985390f23b5b2d9731baa84ebb3b12bde638fb0c5c24bf1ac0e46b192b6309c`  
		Last Modified: Mon, 13 Jul 2020 17:22:13 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0b785ac0cc62606e0654292b880c0c56372390450bff35f0a077a7bb2247b0`  
		Last Modified: Wed, 22 Jul 2020 00:37:33 GMT  
		Size: 64.7 MB (64672261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22dd25f36dd41de85b9fe53b1ed81385179443b042de6d54b2e6bddb77f424d`  
		Last Modified: Wed, 22 Jul 2020 00:37:12 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.1.0-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:a5f98754d29c6476a9ca2866f17b02e444f24aaf3a0afb01719ca224028ba3e4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.3 MB (100327898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f6950dfa4c5e1cfbaded0226aa1d5ac234d7dff426ede13b06194e0745f3b39`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 06 Jul 2020 22:06:25 GMT
ADD file:eacc4e3c71dca085a01eb1b781c8312350bcb2288a1f6ceeefb68d660b3215b5 in / 
# Mon, 06 Jul 2020 22:06:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 22:06:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 22:06:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 22:06:39 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:11:52 GMT
ARG ASSET=ce
# Mon, 06 Jul 2020 23:11:52 GMT
ENV ASSET=ce
# Mon, 13 Jul 2020 17:39:46 GMT
ARG EE_PORTS
# Mon, 13 Jul 2020 17:39:47 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Tue, 21 Jul 2020 23:21:12 GMT
ARG KONG_VERSION=2.1.0
# Tue, 21 Jul 2020 23:21:15 GMT
ENV KONG_VERSION=2.1.0
# Tue, 21 Jul 2020 23:22:39 GMT
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apt-get update &&         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get update     && apt-get install -y --no-install-recommends perl unzip git     && { apt-get install -y --no-install-recommends zlibc || true; }     && { apt-get install -y --no-install-recommends zlib1g-dev || true; }     && rm -rf /var/lib/apt/lists/* 	&& dpkg -i /tmp/kong.deb 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Tue, 21 Jul 2020 23:22:42 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Tue, 21 Jul 2020 23:22:42 GMT
USER kong
# Tue, 21 Jul 2020 23:22:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 21 Jul 2020 23:22:44 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 21 Jul 2020 23:22:46 GMT
STOPSIGNAL SIGQUIT
# Tue, 21 Jul 2020 23:22:47 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4ab489c2a6275c4f4b0c3ccbc0c397c7b4d1e3278136f158f0345707b88775ce`  
		Last Modified: Sat, 20 Jun 2020 00:25:22 GMT  
		Size: 40.0 MB (40035468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd7a7bb5cc1bf1dc02973eb563c00d2491059923f17bdcc83b37d65a6015b74`  
		Last Modified: Mon, 06 Jul 2020 22:07:41 GMT  
		Size: 471.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3150055c00370319e479ec8c335cd23b2564e0546e6e50593f651a6311be5a83`  
		Last Modified: Mon, 06 Jul 2020 22:07:41 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee51ca48c53d0f23ff69410d387087d1f50be8472db56cb051f280b80038ac7`  
		Last Modified: Mon, 06 Jul 2020 22:07:41 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:067ab254ee421c1c91ef88db879def7f3df9bfcd4b10f002fb3f8920fc23e03b`  
		Last Modified: Mon, 13 Jul 2020 17:41:20 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9dd945b2d004ec28bb8850965d691a4b893abce5cee9b1f6df3615c3ba31f73`  
		Last Modified: Tue, 21 Jul 2020 23:23:38 GMT  
		Size: 60.3 MB (60290116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f36be9002a7d8de6f071d275afb31302dbacb7f66f6b5f546f092fb48e8f7ba7`  
		Last Modified: Tue, 21 Jul 2020 23:23:12 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.1-alpine`

```console
$ docker pull kong@sha256:f2b002534e28d44d70ae19e8dc30acb47ee3c14503a661d6cc16526d9b212d49
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.1-alpine` - linux; amd64

```console
$ docker pull kong@sha256:aa6d39989058a27439807d9fc09becdcef04ca9d5c3a87fd2390f3e4fe210cf2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53140755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d91e9ff0399c788d760a0dc5f7416ef1d02a910dbf02b9a23d49dc0d0d7666f2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Tue, 05 May 2020 00:19:56 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 05 May 2020 00:19:56 GMT
ARG ASSET=ce
# Tue, 05 May 2020 00:19:56 GMT
ENV ASSET=ce
# Mon, 13 Jul 2020 17:19:53 GMT
ARG EE_PORTS
# Mon, 13 Jul 2020 17:19:53 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 22 Jul 2020 00:34:09 GMT
ARG KONG_VERSION=2.1.0
# Wed, 22 Jul 2020 00:34:09 GMT
ENV KONG_VERSION=2.1.0
# Wed, 22 Jul 2020 00:34:10 GMT
ARG KONG_SHA256=8e5322ba57591e75e6c0d2cfe602cc104467be2336a4075c80831fb53cbb1f78
# Wed, 22 Jul 2020 00:34:22 GMT
# ARGS: KONG_SHA256=8e5322ba57591e75e6c0d2cfe602cc104467be2336a4075c80831fb53cbb1f78
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong; 	tar -C /kong -xzf /tmp/kong.tar.gz && 	mv /kong/usr/local/* /usr/local && 	mv /kong/etc/* /etc && 	rm -rf /kong && 	apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates && 	adduser -S kong && 	mkdir -p "/usr/local/kong" && 	chown -R kong:0 /usr/local/kong && 	chown kong:0 /usr/local/bin/kong && 	chmod -R g=u /usr/local/kong && 	rm -rf /tmp/kong.tar.gz &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Wed, 22 Jul 2020 00:34:23 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 22 Jul 2020 00:34:24 GMT
USER kong
# Wed, 22 Jul 2020 00:34:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jul 2020 00:34:24 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 22 Jul 2020 00:34:25 GMT
STOPSIGNAL SIGQUIT
# Wed, 22 Jul 2020 00:34:25 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e0de2dc0e7e86d092bbee85a6c1ef2769273bd1a78d87bc9a745745fe2d3b9`  
		Last Modified: Mon, 13 Jul 2020 17:21:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d7dc22eefcb6b9c7d444afb334e5cf62640b57f3d58a8a1d608b258bd30f90`  
		Last Modified: Wed, 22 Jul 2020 00:36:57 GMT  
		Size: 50.3 MB (50326578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b904e61d124ac9189b2e76c7f81a19d1b66899fe651573b702594f557ecc34d`  
		Last Modified: Wed, 22 Jul 2020 00:36:42 GMT  
		Size: 732.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.1-centos`

```console
$ docker pull kong@sha256:bd75530c4ea8e706e2a48d82473a421ce0029ca2adfef123b50773eacf0bcb1e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.1-centos` - linux; amd64

```console
$ docker pull kong@sha256:36ba91d200e99c25c108814398474b98220f7eca0641da33b4ef721861a9c2e1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.1 MB (127068768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8baa0a020eda5e0a5776fcb5241579a95e037fdaca56c311f20a93110ee8cc20`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:54:26 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 05 May 2020 21:54:26 GMT
ARG ASSET=ce
# Tue, 05 May 2020 21:54:27 GMT
ENV ASSET=ce
# Mon, 13 Jul 2020 17:20:53 GMT
ARG EE_PORTS
# Mon, 13 Jul 2020 17:20:54 GMT
COPY file:ff02c070e4c89f043b176279a7e41464b5fab8cb98cfcd6332fad2d2741fc41d in /tmp/kong.rpm 
# Mon, 13 Jul 2020 17:20:54 GMT
ARG KONG_VERSION=2.1.0rc.1
# Mon, 13 Jul 2020 17:20:54 GMT
ENV KONG_VERSION=2.1.0rc.1
# Mon, 13 Jul 2020 17:20:54 GMT
ARG KONG_SHA256=8ea531b374d48fc125f19f68190a420f5870c267940d4fb701968c13950b6872
# Mon, 13 Jul 2020 17:21:19 GMT
# ARGS: KONG_SHA256=8ea531b374d48fc125f19f68190a420f5870c267940d4fb701968c13950b6872
RUN set -ex; 	if [ "$ASSET" = "ce" ] ; then 		curl -fL "https://bintray.com/kong/kong-prerelease/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm" -o /tmp/kong.rpm 		&& echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -; 	fi; 	yum install -y -q unzip shadow-utils git zlib zlib-devel 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki 	&& useradd kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y /tmp/kong.rpm 	&& yum clean all 	&& rm /tmp/kong.rpm 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Tue, 14 Jul 2020 20:21:05 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Tue, 14 Jul 2020 20:21:05 GMT
USER kong
# Tue, 14 Jul 2020 20:21:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 14 Jul 2020 20:21:06 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 14 Jul 2020 20:21:06 GMT
STOPSIGNAL SIGQUIT
# Tue, 14 Jul 2020 20:21:06 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:704a3409f16a6a57c8a784478d138fc2416316afff34de47d993548467e36b47`  
		Last Modified: Mon, 13 Jul 2020 17:22:33 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:405f44fcf53df0044476d810e9cc23e9654a2097aa3b898fe9ef2f76281d3174`  
		Last Modified: Mon, 13 Jul 2020 17:22:43 GMT  
		Size: 51.2 MB (51187766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ccf12c1b91dfdefcc602cbfdb26dd918d0226a6007f2f0a1a84b59da686cf4`  
		Last Modified: Tue, 14 Jul 2020 20:22:14 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.1-ubuntu`

```console
$ docker pull kong@sha256:cfa17f065e22eb525b133427804cac2a279e7dffc3474f5ba1b9b6b49c6bc1c5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.1-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:4257052170ff58c26aca38d50bce8830844b1194abaf8ae1ebe57d20f75bb188
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.0 MB (109048772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5593e58b150d111a56c25898d068a0053cd214f3df4232dcccef6aab203985b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 06 Jul 2020 21:57:02 GMT
ADD file:47805a69cb7dd669e357d291ce27735c2d514348468b2d3e69c66161a4f80abd in / 
# Mon, 06 Jul 2020 21:57:03 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 21:57:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:57:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:57:05 GMT
CMD ["/bin/bash"]
# Tue, 07 Jul 2020 00:16:32 GMT
ARG ASSET=ce
# Tue, 07 Jul 2020 00:16:32 GMT
ENV ASSET=ce
# Mon, 13 Jul 2020 17:20:07 GMT
ARG EE_PORTS
# Mon, 13 Jul 2020 17:20:07 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Wed, 22 Jul 2020 00:34:32 GMT
ARG KONG_VERSION=2.1.0
# Wed, 22 Jul 2020 00:34:33 GMT
ENV KONG_VERSION=2.1.0
# Wed, 22 Jul 2020 00:35:40 GMT
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apt-get update &&         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get update     && apt-get install -y --no-install-recommends perl unzip git     && { apt-get install -y --no-install-recommends zlibc || true; }     && { apt-get install -y --no-install-recommends zlib1g-dev || true; }     && rm -rf /var/lib/apt/lists/* 	&& dpkg -i /tmp/kong.deb 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Wed, 22 Jul 2020 00:35:41 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Wed, 22 Jul 2020 00:35:41 GMT
USER kong
# Wed, 22 Jul 2020 00:35:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jul 2020 00:35:42 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 22 Jul 2020 00:35:42 GMT
STOPSIGNAL SIGQUIT
# Wed, 22 Jul 2020 00:35:43 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:6aa38bd67045d3ed7e7a73ca42e06fadbfd139a26693bf2dc8b9ccc318d87c3c`  
		Last Modified: Sat, 20 Jun 2020 13:20:13 GMT  
		Size: 44.4 MB (44374155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981ae4862c056451e69578c614f07a5b552995d3fc1cf17d5dc78a26e8455d5a`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bad8949dcb16a7693551042e056cef1e767ac0a23625a2eb9ae33ac44ac80f9`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9461589e708efab1c30577ec50f06db05714523e2976c7da421b0b418312e0`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5985390f23b5b2d9731baa84ebb3b12bde638fb0c5c24bf1ac0e46b192b6309c`  
		Last Modified: Mon, 13 Jul 2020 17:22:13 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0b785ac0cc62606e0654292b880c0c56372390450bff35f0a077a7bb2247b0`  
		Last Modified: Wed, 22 Jul 2020 00:37:33 GMT  
		Size: 64.7 MB (64672261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22dd25f36dd41de85b9fe53b1ed81385179443b042de6d54b2e6bddb77f424d`  
		Last Modified: Wed, 22 Jul 2020 00:37:12 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.1-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:a5f98754d29c6476a9ca2866f17b02e444f24aaf3a0afb01719ca224028ba3e4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.3 MB (100327898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f6950dfa4c5e1cfbaded0226aa1d5ac234d7dff426ede13b06194e0745f3b39`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 06 Jul 2020 22:06:25 GMT
ADD file:eacc4e3c71dca085a01eb1b781c8312350bcb2288a1f6ceeefb68d660b3215b5 in / 
# Mon, 06 Jul 2020 22:06:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 22:06:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 22:06:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 22:06:39 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:11:52 GMT
ARG ASSET=ce
# Mon, 06 Jul 2020 23:11:52 GMT
ENV ASSET=ce
# Mon, 13 Jul 2020 17:39:46 GMT
ARG EE_PORTS
# Mon, 13 Jul 2020 17:39:47 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Tue, 21 Jul 2020 23:21:12 GMT
ARG KONG_VERSION=2.1.0
# Tue, 21 Jul 2020 23:21:15 GMT
ENV KONG_VERSION=2.1.0
# Tue, 21 Jul 2020 23:22:39 GMT
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apt-get update &&         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get update     && apt-get install -y --no-install-recommends perl unzip git     && { apt-get install -y --no-install-recommends zlibc || true; }     && { apt-get install -y --no-install-recommends zlib1g-dev || true; }     && rm -rf /var/lib/apt/lists/* 	&& dpkg -i /tmp/kong.deb 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Tue, 21 Jul 2020 23:22:42 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Tue, 21 Jul 2020 23:22:42 GMT
USER kong
# Tue, 21 Jul 2020 23:22:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 21 Jul 2020 23:22:44 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 21 Jul 2020 23:22:46 GMT
STOPSIGNAL SIGQUIT
# Tue, 21 Jul 2020 23:22:47 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4ab489c2a6275c4f4b0c3ccbc0c397c7b4d1e3278136f158f0345707b88775ce`  
		Last Modified: Sat, 20 Jun 2020 00:25:22 GMT  
		Size: 40.0 MB (40035468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd7a7bb5cc1bf1dc02973eb563c00d2491059923f17bdcc83b37d65a6015b74`  
		Last Modified: Mon, 06 Jul 2020 22:07:41 GMT  
		Size: 471.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3150055c00370319e479ec8c335cd23b2564e0546e6e50593f651a6311be5a83`  
		Last Modified: Mon, 06 Jul 2020 22:07:41 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee51ca48c53d0f23ff69410d387087d1f50be8472db56cb051f280b80038ac7`  
		Last Modified: Mon, 06 Jul 2020 22:07:41 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:067ab254ee421c1c91ef88db879def7f3df9bfcd4b10f002fb3f8920fc23e03b`  
		Last Modified: Mon, 13 Jul 2020 17:41:20 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9dd945b2d004ec28bb8850965d691a4b893abce5cee9b1f6df3615c3ba31f73`  
		Last Modified: Tue, 21 Jul 2020 23:23:38 GMT  
		Size: 60.3 MB (60290116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f36be9002a7d8de6f071d275afb31302dbacb7f66f6b5f546f092fb48e8f7ba7`  
		Last Modified: Tue, 21 Jul 2020 23:23:12 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:alpine`

```console
$ docker pull kong@sha256:f2b002534e28d44d70ae19e8dc30acb47ee3c14503a661d6cc16526d9b212d49
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:alpine` - linux; amd64

```console
$ docker pull kong@sha256:aa6d39989058a27439807d9fc09becdcef04ca9d5c3a87fd2390f3e4fe210cf2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53140755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d91e9ff0399c788d760a0dc5f7416ef1d02a910dbf02b9a23d49dc0d0d7666f2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Tue, 05 May 2020 00:19:56 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 05 May 2020 00:19:56 GMT
ARG ASSET=ce
# Tue, 05 May 2020 00:19:56 GMT
ENV ASSET=ce
# Mon, 13 Jul 2020 17:19:53 GMT
ARG EE_PORTS
# Mon, 13 Jul 2020 17:19:53 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 22 Jul 2020 00:34:09 GMT
ARG KONG_VERSION=2.1.0
# Wed, 22 Jul 2020 00:34:09 GMT
ENV KONG_VERSION=2.1.0
# Wed, 22 Jul 2020 00:34:10 GMT
ARG KONG_SHA256=8e5322ba57591e75e6c0d2cfe602cc104467be2336a4075c80831fb53cbb1f78
# Wed, 22 Jul 2020 00:34:22 GMT
# ARGS: KONG_SHA256=8e5322ba57591e75e6c0d2cfe602cc104467be2336a4075c80831fb53cbb1f78
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong; 	tar -C /kong -xzf /tmp/kong.tar.gz && 	mv /kong/usr/local/* /usr/local && 	mv /kong/etc/* /etc && 	rm -rf /kong && 	apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates && 	adduser -S kong && 	mkdir -p "/usr/local/kong" && 	chown -R kong:0 /usr/local/kong && 	chown kong:0 /usr/local/bin/kong && 	chmod -R g=u /usr/local/kong && 	rm -rf /tmp/kong.tar.gz &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Wed, 22 Jul 2020 00:34:23 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 22 Jul 2020 00:34:24 GMT
USER kong
# Wed, 22 Jul 2020 00:34:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jul 2020 00:34:24 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 22 Jul 2020 00:34:25 GMT
STOPSIGNAL SIGQUIT
# Wed, 22 Jul 2020 00:34:25 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e0de2dc0e7e86d092bbee85a6c1ef2769273bd1a78d87bc9a745745fe2d3b9`  
		Last Modified: Mon, 13 Jul 2020 17:21:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d7dc22eefcb6b9c7d444afb334e5cf62640b57f3d58a8a1d608b258bd30f90`  
		Last Modified: Wed, 22 Jul 2020 00:36:57 GMT  
		Size: 50.3 MB (50326578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b904e61d124ac9189b2e76c7f81a19d1b66899fe651573b702594f557ecc34d`  
		Last Modified: Wed, 22 Jul 2020 00:36:42 GMT  
		Size: 732.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:centos`

```console
$ docker pull kong@sha256:796bde8b61581c315bbfdf3c85e9002599dc630c6fbb456c8bbf9ec5aa2c12cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:centos` - linux; amd64

```console
$ docker pull kong@sha256:5e129dca95cbb055cdaaa9806966569be196446d3b38122a01991a1245e1c1fa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127222587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6ff1d4be6c902aabe1ad9a93e37eac121f1781af332682e2826cb27087f357d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Tue, 05 May 2020 21:20:06 GMT
ADD file:38e2d2a1a0cd8694bd5086f257fdf7504f0c2481bf4f746c9bd1c8d9f3f6430d in / 
# Tue, 05 May 2020 21:20:06 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200504 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-05-04 00:00:00+01:00
# Tue, 05 May 2020 21:20:07 GMT
CMD ["/bin/bash"]
# Tue, 05 May 2020 21:54:26 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 05 May 2020 21:54:26 GMT
ARG ASSET=ce
# Tue, 05 May 2020 21:54:27 GMT
ENV ASSET=ce
# Tue, 05 May 2020 21:54:27 GMT
COPY file:73044b225363e2703a176f55b132687ead4bab30398788756be18d2965fac2cd in /tmp/kong.rpm 
# Fri, 10 Jul 2020 20:23:32 GMT
ARG KONG_VERSION=2.0.5
# Fri, 10 Jul 2020 20:23:32 GMT
ENV KONG_VERSION=2.0.5
# Fri, 10 Jul 2020 20:23:33 GMT
ARG KONG_SHA256=e05340680de3541c4c940f54e64f00c90fb5137f6a8c71e413b815a411d74fc6
# Fri, 10 Jul 2020 20:23:33 GMT
ENV KONG_SHA256=e05340680de3541c4c940f54e64f00c90fb5137f6a8c71e413b815a411d74fc6
# Fri, 10 Jul 2020 20:24:05 GMT
RUN set -ex; 	if [ "$ASSET" = "ce" ] ; then 		curl -fL "https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm" -o /tmp/kong.rpm 		&& echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -; 	fi; 	yum install -y -q unzip shadow-utils git zlib 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki 	&& useradd kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y /tmp/kong.rpm 	&& yum clean all 	&& rm /tmp/kong.rpm 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong 	&& kong version
# Tue, 14 Jul 2020 20:21:20 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Tue, 14 Jul 2020 20:21:20 GMT
USER kong
# Tue, 14 Jul 2020 20:21:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 14 Jul 2020 20:21:21 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 14 Jul 2020 20:21:21 GMT
STOPSIGNAL SIGQUIT
# Tue, 14 Jul 2020 20:21:21 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:524b0c1e57f8ee5fee01a1decba2f301c324a6513ca3551021264e3aa7341ebc`  
		Last Modified: Tue, 05 May 2020 21:23:14 GMT  
		Size: 75.9 MB (75880141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce7701dd3817fcacdc04d8abfd7cd6ea61fe7f4d909903260a2ebe43fce007f`  
		Last Modified: Tue, 05 May 2020 22:02:15 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e839438e3b2588088e4bb0885546faeba1afe1d70b47fd88048e9d0c70ae370`  
		Last Modified: Fri, 10 Jul 2020 20:25:43 GMT  
		Size: 51.3 MB (51341586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9126f205ac0dfa5d13b956c46b11ff4a8f1b45f444a6d30d7d070dbbc3f882`  
		Last Modified: Tue, 14 Jul 2020 20:22:29 GMT  
		Size: 731.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:latest`

```console
$ docker pull kong@sha256:f2b002534e28d44d70ae19e8dc30acb47ee3c14503a661d6cc16526d9b212d49
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:latest` - linux; amd64

```console
$ docker pull kong@sha256:aa6d39989058a27439807d9fc09becdcef04ca9d5c3a87fd2390f3e4fe210cf2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53140755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d91e9ff0399c788d760a0dc5f7416ef1d02a910dbf02b9a23d49dc0d0d7666f2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Tue, 05 May 2020 00:19:56 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 05 May 2020 00:19:56 GMT
ARG ASSET=ce
# Tue, 05 May 2020 00:19:56 GMT
ENV ASSET=ce
# Mon, 13 Jul 2020 17:19:53 GMT
ARG EE_PORTS
# Mon, 13 Jul 2020 17:19:53 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Wed, 22 Jul 2020 00:34:09 GMT
ARG KONG_VERSION=2.1.0
# Wed, 22 Jul 2020 00:34:09 GMT
ENV KONG_VERSION=2.1.0
# Wed, 22 Jul 2020 00:34:10 GMT
ARG KONG_SHA256=8e5322ba57591e75e6c0d2cfe602cc104467be2336a4075c80831fb53cbb1f78
# Wed, 22 Jul 2020 00:34:22 GMT
# ARGS: KONG_SHA256=8e5322ba57591e75e6c0d2cfe602cc104467be2336a4075c80831fb53cbb1f78
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong; 	tar -C /kong -xzf /tmp/kong.tar.gz && 	mv /kong/usr/local/* /usr/local && 	mv /kong/etc/* /etc && 	rm -rf /kong && 	apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates && 	adduser -S kong && 	mkdir -p "/usr/local/kong" && 	chown -R kong:0 /usr/local/kong && 	chown kong:0 /usr/local/bin/kong && 	chmod -R g=u /usr/local/kong && 	rm -rf /tmp/kong.tar.gz &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Wed, 22 Jul 2020 00:34:23 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Wed, 22 Jul 2020 00:34:24 GMT
USER kong
# Wed, 22 Jul 2020 00:34:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jul 2020 00:34:24 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 22 Jul 2020 00:34:25 GMT
STOPSIGNAL SIGQUIT
# Wed, 22 Jul 2020 00:34:25 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e0de2dc0e7e86d092bbee85a6c1ef2769273bd1a78d87bc9a745745fe2d3b9`  
		Last Modified: Mon, 13 Jul 2020 17:21:58 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d7dc22eefcb6b9c7d444afb334e5cf62640b57f3d58a8a1d608b258bd30f90`  
		Last Modified: Wed, 22 Jul 2020 00:36:57 GMT  
		Size: 50.3 MB (50326578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b904e61d124ac9189b2e76c7f81a19d1b66899fe651573b702594f557ecc34d`  
		Last Modified: Wed, 22 Jul 2020 00:36:42 GMT  
		Size: 732.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:ubuntu`

```console
$ docker pull kong@sha256:cfa17f065e22eb525b133427804cac2a279e7dffc3474f5ba1b9b6b49c6bc1c5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:4257052170ff58c26aca38d50bce8830844b1194abaf8ae1ebe57d20f75bb188
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.0 MB (109048772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5593e58b150d111a56c25898d068a0053cd214f3df4232dcccef6aab203985b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 06 Jul 2020 21:57:02 GMT
ADD file:47805a69cb7dd669e357d291ce27735c2d514348468b2d3e69c66161a4f80abd in / 
# Mon, 06 Jul 2020 21:57:03 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 21:57:04 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 21:57:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 21:57:05 GMT
CMD ["/bin/bash"]
# Tue, 07 Jul 2020 00:16:32 GMT
ARG ASSET=ce
# Tue, 07 Jul 2020 00:16:32 GMT
ENV ASSET=ce
# Mon, 13 Jul 2020 17:20:07 GMT
ARG EE_PORTS
# Mon, 13 Jul 2020 17:20:07 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Wed, 22 Jul 2020 00:34:32 GMT
ARG KONG_VERSION=2.1.0
# Wed, 22 Jul 2020 00:34:33 GMT
ENV KONG_VERSION=2.1.0
# Wed, 22 Jul 2020 00:35:40 GMT
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apt-get update &&         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get update     && apt-get install -y --no-install-recommends perl unzip git     && { apt-get install -y --no-install-recommends zlibc || true; }     && { apt-get install -y --no-install-recommends zlib1g-dev || true; }     && rm -rf /var/lib/apt/lists/* 	&& dpkg -i /tmp/kong.deb 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Wed, 22 Jul 2020 00:35:41 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Wed, 22 Jul 2020 00:35:41 GMT
USER kong
# Wed, 22 Jul 2020 00:35:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jul 2020 00:35:42 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 22 Jul 2020 00:35:42 GMT
STOPSIGNAL SIGQUIT
# Wed, 22 Jul 2020 00:35:43 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:6aa38bd67045d3ed7e7a73ca42e06fadbfd139a26693bf2dc8b9ccc318d87c3c`  
		Last Modified: Sat, 20 Jun 2020 13:20:13 GMT  
		Size: 44.4 MB (44374155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981ae4862c056451e69578c614f07a5b552995d3fc1cf17d5dc78a26e8455d5a`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bad8949dcb16a7693551042e056cef1e767ac0a23625a2eb9ae33ac44ac80f9`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9461589e708efab1c30577ec50f06db05714523e2976c7da421b0b418312e0`  
		Last Modified: Mon, 06 Jul 2020 21:57:46 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5985390f23b5b2d9731baa84ebb3b12bde638fb0c5c24bf1ac0e46b192b6309c`  
		Last Modified: Mon, 13 Jul 2020 17:22:13 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0b785ac0cc62606e0654292b880c0c56372390450bff35f0a077a7bb2247b0`  
		Last Modified: Wed, 22 Jul 2020 00:37:33 GMT  
		Size: 64.7 MB (64672261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22dd25f36dd41de85b9fe53b1ed81385179443b042de6d54b2e6bddb77f424d`  
		Last Modified: Wed, 22 Jul 2020 00:37:12 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:a5f98754d29c6476a9ca2866f17b02e444f24aaf3a0afb01719ca224028ba3e4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.3 MB (100327898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f6950dfa4c5e1cfbaded0226aa1d5ac234d7dff426ede13b06194e0745f3b39`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 06 Jul 2020 22:06:25 GMT
ADD file:eacc4e3c71dca085a01eb1b781c8312350bcb2288a1f6ceeefb68d660b3215b5 in / 
# Mon, 06 Jul 2020 22:06:31 GMT
RUN rm -rf /var/lib/apt/lists/*
# Mon, 06 Jul 2020 22:06:35 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Mon, 06 Jul 2020 22:06:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Mon, 06 Jul 2020 22:06:39 GMT
CMD ["/bin/bash"]
# Mon, 06 Jul 2020 23:11:52 GMT
ARG ASSET=ce
# Mon, 06 Jul 2020 23:11:52 GMT
ENV ASSET=ce
# Mon, 13 Jul 2020 17:39:46 GMT
ARG EE_PORTS
# Mon, 13 Jul 2020 17:39:47 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Tue, 21 Jul 2020 23:21:12 GMT
ARG KONG_VERSION=2.1.0
# Tue, 21 Jul 2020 23:21:15 GMT
ENV KONG_VERSION=2.1.0
# Tue, 21 Jul 2020 23:22:39 GMT
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apt-get update &&         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get update     && apt-get install -y --no-install-recommends perl unzip git     && { apt-get install -y --no-install-recommends zlibc || true; }     && { apt-get install -y --no-install-recommends zlib1g-dev || true; }     && rm -rf /var/lib/apt/lists/* 	&& dpkg -i /tmp/kong.deb 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Tue, 21 Jul 2020 23:22:42 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Tue, 21 Jul 2020 23:22:42 GMT
USER kong
# Tue, 21 Jul 2020 23:22:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 21 Jul 2020 23:22:44 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 21 Jul 2020 23:22:46 GMT
STOPSIGNAL SIGQUIT
# Tue, 21 Jul 2020 23:22:47 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:4ab489c2a6275c4f4b0c3ccbc0c397c7b4d1e3278136f158f0345707b88775ce`  
		Last Modified: Sat, 20 Jun 2020 00:25:22 GMT  
		Size: 40.0 MB (40035468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd7a7bb5cc1bf1dc02973eb563c00d2491059923f17bdcc83b37d65a6015b74`  
		Last Modified: Mon, 06 Jul 2020 22:07:41 GMT  
		Size: 471.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3150055c00370319e479ec8c335cd23b2564e0546e6e50593f651a6311be5a83`  
		Last Modified: Mon, 06 Jul 2020 22:07:41 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee51ca48c53d0f23ff69410d387087d1f50be8472db56cb051f280b80038ac7`  
		Last Modified: Mon, 06 Jul 2020 22:07:41 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:067ab254ee421c1c91ef88db879def7f3df9bfcd4b10f002fb3f8920fc23e03b`  
		Last Modified: Mon, 13 Jul 2020 17:41:20 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9dd945b2d004ec28bb8850965d691a4b893abce5cee9b1f6df3615c3ba31f73`  
		Last Modified: Tue, 21 Jul 2020 23:23:38 GMT  
		Size: 60.3 MB (60290116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f36be9002a7d8de6f071d275afb31302dbacb7f66f6b5f546f092fb48e8f7ba7`  
		Last Modified: Tue, 21 Jul 2020 23:23:12 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
