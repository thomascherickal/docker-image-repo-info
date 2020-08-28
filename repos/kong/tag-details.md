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
-	[`kong:2.1.3`](#kong213)
-	[`kong:2.1.3-alpine`](#kong213-alpine)
-	[`kong:2.1.3-centos`](#kong213-centos)
-	[`kong:2.1.3-ubuntu`](#kong213-ubuntu)
-	[`kong:2.1-alpine`](#kong21-alpine)
-	[`kong:2.1-centos`](#kong21-centos)
-	[`kong:2.1-ubuntu`](#kong21-ubuntu)
-	[`kong:alpine`](#kongalpine)
-	[`kong:centos`](#kongcentos)
-	[`kong:latest`](#konglatest)
-	[`kong:ubuntu`](#kongubuntu)

## `kong:2`

```console
$ docker pull kong@sha256:da6a051abc306094600d9aeee1acf68361966450f516de38255125469b2d8f5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2` - linux; amd64

```console
$ docker pull kong@sha256:723bf97cfdeaa1a406935e1759c2f592d327566d659b30202f80da02c78ffc62
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53144837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a62a8307bf7fd7fe6031f9b0ff3763a461143e6da341da33ea955ee31877ba02`
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
# Thu, 20 Aug 2020 23:19:49 GMT
ARG KONG_VERSION=2.1.3
# Thu, 20 Aug 2020 23:19:49 GMT
ENV KONG_VERSION=2.1.3
# Thu, 20 Aug 2020 23:19:49 GMT
ARG KONG_SHA256=2f2a73d468d95f3ded495aa4199b55d2148d1ad5cb5050372621a1768b34ba8a
# Thu, 20 Aug 2020 23:19:55 GMT
# ARGS: KONG_SHA256=2f2a73d468d95f3ded495aa4199b55d2148d1ad5cb5050372621a1768b34ba8a
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong; 	tar -C /kong -xzf /tmp/kong.tar.gz && 	mv /kong/usr/local/* /usr/local && 	mv /kong/etc/* /etc && 	rm -rf /kong && 	apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates && 	adduser -S kong && 	mkdir -p "/usr/local/kong" && 	chown -R kong:0 /usr/local/kong && 	chown kong:0 /usr/local/bin/kong && 	chmod -R g=u /usr/local/kong && 	rm -rf /tmp/kong.tar.gz &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Thu, 20 Aug 2020 23:19:55 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 20 Aug 2020 23:19:55 GMT
USER kong
# Thu, 20 Aug 2020 23:19:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 20 Aug 2020 23:19:56 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 20 Aug 2020 23:19:56 GMT
STOPSIGNAL SIGQUIT
# Thu, 20 Aug 2020 23:19:56 GMT
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
	-	`sha256:59f67e15df63b8d20592937e5d3cc7d55d5c2e0e3d5cf38f8cdc640bdc919394`  
		Last Modified: Thu, 20 Aug 2020 23:21:38 GMT  
		Size: 50.3 MB (50330658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985f1bf5706fb044dc193de9b6d0007ac3a07720ac24a5d500937e8dcabe1acf`  
		Last Modified: Thu, 20 Aug 2020 23:21:29 GMT  
		Size: 734.0 B  
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
$ docker pull kong@sha256:e7d0bb138aaab2a0b48c168c0cb406a44584d64faf73d333254cccb9ab3e218e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.0.5-centos` - linux; amd64

```console
$ docker pull kong@sha256:e1828c43034e91df55f0aa1a32ea967b84520f226ee25e3e8d5c2ff907b859f6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127201659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5eccb2f98f5256209df2d30d3093ff94de3a5bd02c91c35466fb149296dbc1ed`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:37:24 GMT
LABEL maintainer=Kong <support@konghq.com>
# Mon, 10 Aug 2020 18:37:24 GMT
ARG ASSET=ce
# Mon, 10 Aug 2020 18:37:25 GMT
ENV ASSET=ce
# Mon, 10 Aug 2020 18:38:05 GMT
COPY file:73044b225363e2703a176f55b132687ead4bab30398788756be18d2965fac2cd in /tmp/kong.rpm 
# Mon, 10 Aug 2020 18:38:06 GMT
ARG KONG_VERSION=2.0.5
# Mon, 10 Aug 2020 18:38:06 GMT
ENV KONG_VERSION=2.0.5
# Mon, 10 Aug 2020 18:38:06 GMT
ARG KONG_SHA256=e05340680de3541c4c940f54e64f00c90fb5137f6a8c71e413b815a411d74fc6
# Mon, 10 Aug 2020 18:38:06 GMT
ENV KONG_SHA256=e05340680de3541c4c940f54e64f00c90fb5137f6a8c71e413b815a411d74fc6
# Mon, 10 Aug 2020 18:38:32 GMT
RUN set -ex; 	if [ "$ASSET" = "ce" ] ; then 		curl -fL "https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm" -o /tmp/kong.rpm 		&& echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -; 	fi; 	yum install -y -q unzip shadow-utils git zlib 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki 	&& useradd kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y /tmp/kong.rpm 	&& yum clean all 	&& rm /tmp/kong.rpm 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong 	&& kong version
# Mon, 10 Aug 2020 18:38:32 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Mon, 10 Aug 2020 18:38:32 GMT
USER kong
# Mon, 10 Aug 2020 18:38:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 10 Aug 2020 18:38:33 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 10 Aug 2020 18:38:33 GMT
STOPSIGNAL SIGQUIT
# Mon, 10 Aug 2020 18:38:33 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f3b62d32c3ab06f347d7567be4d156da784b07551ad32e0a6f565f74e58524e`  
		Last Modified: Mon, 10 Aug 2020 18:39:18 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a67a34788f80c318ce6435f02b7ecf00a427c76d5faedee06fa8f85c275a802`  
		Last Modified: Mon, 10 Aug 2020 18:39:30 GMT  
		Size: 51.3 MB (51337613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1fe6963c7e1249558c8e9725ed8a57f6c1c54e35436eea259a72bc69bfd27d`  
		Last Modified: Mon, 10 Aug 2020 18:39:18 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.0.5-ubuntu`

```console
$ docker pull kong@sha256:cc996e6fce9573a8a73bfd4fdda7611f4a62aaf14d981b367cfbe4564ee9072e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.0.5-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:acbdb86c32156cfb6dcc5362fb05163ad74235001d06de964404f2a61e853aa8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.5 MB (99524394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fcadd93de406a33158eeca0900a9975eba10b42aa2fec90602573cf848aee73`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 19 Aug 2020 21:16:18 GMT
ADD file:144835a276ed2d8eaf6e893d5560444fe0d6a6f9b9bdadec1eb56e7bd9814427 in / 
# Wed, 19 Aug 2020 21:16:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:16:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:16:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:16:22 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 23:17:58 GMT
ARG ASSET=ce
# Wed, 19 Aug 2020 23:17:58 GMT
ENV ASSET=ce
# Wed, 19 Aug 2020 23:19:11 GMT
COPY file:5307743dbc5e81034b8adaf56f281bcb13b0da2d468cb6450d72fa5b77543ccf in /tmp/kong.deb 
# Wed, 19 Aug 2020 23:19:11 GMT
ARG KONG_VERSION=2.0.5
# Wed, 19 Aug 2020 23:19:11 GMT
ENV KONG_VERSION=2.0.5
# Wed, 19 Aug 2020 23:19:31 GMT
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apt-get update &&         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get update     && apt-get install -y --no-install-recommends perl unzip git zlib1g     && rm -rf /var/lib/apt/lists/* 	&& dpkg -i /tmp/kong.deb 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong 	&& kong version
# Wed, 19 Aug 2020 23:19:31 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Wed, 19 Aug 2020 23:19:31 GMT
USER kong
# Wed, 19 Aug 2020 23:19:32 GMT
RUN kong version
# Wed, 19 Aug 2020 23:19:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 19 Aug 2020 23:19:32 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 19 Aug 2020 23:19:33 GMT
STOPSIGNAL SIGQUIT
# Wed, 19 Aug 2020 23:19:33 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:8e097b52bfb8e743e52ccd2dfbd5a0363e48a00b06cdd3728a6fd4d1f3a34280`  
		Last Modified: Sat, 08 Aug 2020 13:20:06 GMT  
		Size: 44.4 MB (44447543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a613a9b4553ca86fac22546f2f79e2ff3d17d8d6aeea8b97d67862a5a40ad8ec`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc000f015361df35e770a910ce03d30691e35aa10d52f4a4f432f183a6c03db`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73eef93b7466c41f22f32d28aae5eb87e1ebc0c4d232c5f5e68c955d0e798dca`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3dcaaf0f6c97a4755caf3ecf36b0594655f5e8621a94400a628cea8862728c6`  
		Last Modified: Wed, 19 Aug 2020 23:20:16 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52932ec30bd1cf0a4092b674f2fa8341712a7cea7f82fa990fd6b49fe5c3685a`  
		Last Modified: Wed, 19 Aug 2020 23:20:26 GMT  
		Size: 55.1 MB (55074393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9772dd3fe2513d9b5aead5aafc80fbab584ab2e1ddfc9831c27b0ebae33d97f5`  
		Last Modified: Wed, 19 Aug 2020 23:20:16 GMT  
		Size: 688.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0181b8d544d98f7988a3804336da4f99273d7b085115347c17abb1cc745e700d`  
		Last Modified: Wed, 19 Aug 2020 23:20:16 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.0.5-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:0819fc5e5c68a156e20aafc9f8dd44080451dbc6cc7d7228771a6565f2b9360f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.2 MB (92248969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b8f0b0980825bc46e4d69c4d4d866d36c06dd2b4316f7f6d0f9dbadc1babae7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 19 Aug 2020 21:31:42 GMT
ADD file:20ffb81d6b7edd3826c028369ed1774914394328d1ccef79ecee109f5cfbcc5f in / 
# Wed, 19 Aug 2020 21:31:45 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:31:49 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:31:51 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:31:52 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:17:19 GMT
ARG ASSET=ce
# Wed, 19 Aug 2020 22:17:19 GMT
ENV ASSET=ce
# Wed, 19 Aug 2020 22:18:38 GMT
COPY file:5307743dbc5e81034b8adaf56f281bcb13b0da2d468cb6450d72fa5b77543ccf in /tmp/kong.deb 
# Wed, 19 Aug 2020 22:18:39 GMT
ARG KONG_VERSION=2.0.5
# Wed, 19 Aug 2020 22:18:40 GMT
ENV KONG_VERSION=2.0.5
# Wed, 19 Aug 2020 22:19:20 GMT
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apt-get update &&         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get update     && apt-get install -y --no-install-recommends perl unzip git zlib1g     && rm -rf /var/lib/apt/lists/* 	&& dpkg -i /tmp/kong.deb 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong 	&& kong version
# Wed, 19 Aug 2020 22:19:22 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Wed, 19 Aug 2020 22:19:23 GMT
USER kong
# Wed, 19 Aug 2020 22:19:25 GMT
RUN kong version
# Wed, 19 Aug 2020 22:19:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 19 Aug 2020 22:19:26 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 19 Aug 2020 22:19:27 GMT
STOPSIGNAL SIGQUIT
# Wed, 19 Aug 2020 22:19:27 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:3266c9b0302777bdc8ccdffab895ef058fb0777dc7600b0fe0b6c80dd3e71f9b`  
		Last Modified: Sat, 08 Aug 2020 00:25:28 GMT  
		Size: 40.1 MB (40073893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5240d1a89e17ed7dda51e3b38d3749e4ab3fb2fc2433de69ea23a838bb00c7`  
		Last Modified: Wed, 19 Aug 2020 21:33:04 GMT  
		Size: 469.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be065fa7bcd4d9f2540e1fec00c455a04755974444b17fb108b73cd4b15963a1`  
		Last Modified: Wed, 19 Aug 2020 21:33:04 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75305dc60d93c15276fd1b3dc21a09ef1ce9c248393c85eb1a5caf2be6e02671`  
		Last Modified: Wed, 19 Aug 2020 21:33:04 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa46bfa329110f43562ee6e8827c14ba35ca854832546866433eb48c646a4834`  
		Last Modified: Wed, 19 Aug 2020 22:20:08 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e687126cc3fdc8430861719ffae8ef5301c37308cbf8d33dad4de3e35d76ce07`  
		Last Modified: Wed, 19 Aug 2020 22:20:25 GMT  
		Size: 52.2 MB (52172683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09cc9ce67878ccf32c6510c937e47680d6e42b8acef2d1d607171b66e5373dc7`  
		Last Modified: Wed, 19 Aug 2020 22:20:07 GMT  
		Size: 687.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461d95bafc1614a36a1baebe5679ad2636bbba96a795a1d380871913936e7244`  
		Last Modified: Wed, 19 Aug 2020 22:20:08 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.0-centos`

```console
$ docker pull kong@sha256:e7d0bb138aaab2a0b48c168c0cb406a44584d64faf73d333254cccb9ab3e218e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.0-centos` - linux; amd64

```console
$ docker pull kong@sha256:e1828c43034e91df55f0aa1a32ea967b84520f226ee25e3e8d5c2ff907b859f6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.2 MB (127201659 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5eccb2f98f5256209df2d30d3093ff94de3a5bd02c91c35466fb149296dbc1ed`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:37:24 GMT
LABEL maintainer=Kong <support@konghq.com>
# Mon, 10 Aug 2020 18:37:24 GMT
ARG ASSET=ce
# Mon, 10 Aug 2020 18:37:25 GMT
ENV ASSET=ce
# Mon, 10 Aug 2020 18:38:05 GMT
COPY file:73044b225363e2703a176f55b132687ead4bab30398788756be18d2965fac2cd in /tmp/kong.rpm 
# Mon, 10 Aug 2020 18:38:06 GMT
ARG KONG_VERSION=2.0.5
# Mon, 10 Aug 2020 18:38:06 GMT
ENV KONG_VERSION=2.0.5
# Mon, 10 Aug 2020 18:38:06 GMT
ARG KONG_SHA256=e05340680de3541c4c940f54e64f00c90fb5137f6a8c71e413b815a411d74fc6
# Mon, 10 Aug 2020 18:38:06 GMT
ENV KONG_SHA256=e05340680de3541c4c940f54e64f00c90fb5137f6a8c71e413b815a411d74fc6
# Mon, 10 Aug 2020 18:38:32 GMT
RUN set -ex; 	if [ "$ASSET" = "ce" ] ; then 		curl -fL "https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm" -o /tmp/kong.rpm 		&& echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -; 	fi; 	yum install -y -q unzip shadow-utils git zlib 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki 	&& useradd kong 	&& mkdir -p "/usr/local/kong" 	&& yum install -y /tmp/kong.rpm 	&& yum clean all 	&& rm /tmp/kong.rpm 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong 	&& kong version
# Mon, 10 Aug 2020 18:38:32 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Mon, 10 Aug 2020 18:38:32 GMT
USER kong
# Mon, 10 Aug 2020 18:38:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 10 Aug 2020 18:38:33 GMT
EXPOSE 8000 8001 8443 8444
# Mon, 10 Aug 2020 18:38:33 GMT
STOPSIGNAL SIGQUIT
# Mon, 10 Aug 2020 18:38:33 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f3b62d32c3ab06f347d7567be4d156da784b07551ad32e0a6f565f74e58524e`  
		Last Modified: Mon, 10 Aug 2020 18:39:18 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a67a34788f80c318ce6435f02b7ecf00a427c76d5faedee06fa8f85c275a802`  
		Last Modified: Mon, 10 Aug 2020 18:39:30 GMT  
		Size: 51.3 MB (51337613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1fe6963c7e1249558c8e9725ed8a57f6c1c54e35436eea259a72bc69bfd27d`  
		Last Modified: Mon, 10 Aug 2020 18:39:18 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.0-ubuntu`

```console
$ docker pull kong@sha256:cc996e6fce9573a8a73bfd4fdda7611f4a62aaf14d981b367cfbe4564ee9072e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.0-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:acbdb86c32156cfb6dcc5362fb05163ad74235001d06de964404f2a61e853aa8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.5 MB (99524394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fcadd93de406a33158eeca0900a9975eba10b42aa2fec90602573cf848aee73`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 19 Aug 2020 21:16:18 GMT
ADD file:144835a276ed2d8eaf6e893d5560444fe0d6a6f9b9bdadec1eb56e7bd9814427 in / 
# Wed, 19 Aug 2020 21:16:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:16:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:16:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:16:22 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 23:17:58 GMT
ARG ASSET=ce
# Wed, 19 Aug 2020 23:17:58 GMT
ENV ASSET=ce
# Wed, 19 Aug 2020 23:19:11 GMT
COPY file:5307743dbc5e81034b8adaf56f281bcb13b0da2d468cb6450d72fa5b77543ccf in /tmp/kong.deb 
# Wed, 19 Aug 2020 23:19:11 GMT
ARG KONG_VERSION=2.0.5
# Wed, 19 Aug 2020 23:19:11 GMT
ENV KONG_VERSION=2.0.5
# Wed, 19 Aug 2020 23:19:31 GMT
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apt-get update &&         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get update     && apt-get install -y --no-install-recommends perl unzip git zlib1g     && rm -rf /var/lib/apt/lists/* 	&& dpkg -i /tmp/kong.deb 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong 	&& kong version
# Wed, 19 Aug 2020 23:19:31 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Wed, 19 Aug 2020 23:19:31 GMT
USER kong
# Wed, 19 Aug 2020 23:19:32 GMT
RUN kong version
# Wed, 19 Aug 2020 23:19:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 19 Aug 2020 23:19:32 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 19 Aug 2020 23:19:33 GMT
STOPSIGNAL SIGQUIT
# Wed, 19 Aug 2020 23:19:33 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:8e097b52bfb8e743e52ccd2dfbd5a0363e48a00b06cdd3728a6fd4d1f3a34280`  
		Last Modified: Sat, 08 Aug 2020 13:20:06 GMT  
		Size: 44.4 MB (44447543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a613a9b4553ca86fac22546f2f79e2ff3d17d8d6aeea8b97d67862a5a40ad8ec`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc000f015361df35e770a910ce03d30691e35aa10d52f4a4f432f183a6c03db`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73eef93b7466c41f22f32d28aae5eb87e1ebc0c4d232c5f5e68c955d0e798dca`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3dcaaf0f6c97a4755caf3ecf36b0594655f5e8621a94400a628cea8862728c6`  
		Last Modified: Wed, 19 Aug 2020 23:20:16 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52932ec30bd1cf0a4092b674f2fa8341712a7cea7f82fa990fd6b49fe5c3685a`  
		Last Modified: Wed, 19 Aug 2020 23:20:26 GMT  
		Size: 55.1 MB (55074393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9772dd3fe2513d9b5aead5aafc80fbab584ab2e1ddfc9831c27b0ebae33d97f5`  
		Last Modified: Wed, 19 Aug 2020 23:20:16 GMT  
		Size: 688.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0181b8d544d98f7988a3804336da4f99273d7b085115347c17abb1cc745e700d`  
		Last Modified: Wed, 19 Aug 2020 23:20:16 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.0-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:0819fc5e5c68a156e20aafc9f8dd44080451dbc6cc7d7228771a6565f2b9360f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.2 MB (92248969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b8f0b0980825bc46e4d69c4d4d866d36c06dd2b4316f7f6d0f9dbadc1babae7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 19 Aug 2020 21:31:42 GMT
ADD file:20ffb81d6b7edd3826c028369ed1774914394328d1ccef79ecee109f5cfbcc5f in / 
# Wed, 19 Aug 2020 21:31:45 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:31:49 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:31:51 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:31:52 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:17:19 GMT
ARG ASSET=ce
# Wed, 19 Aug 2020 22:17:19 GMT
ENV ASSET=ce
# Wed, 19 Aug 2020 22:18:38 GMT
COPY file:5307743dbc5e81034b8adaf56f281bcb13b0da2d468cb6450d72fa5b77543ccf in /tmp/kong.deb 
# Wed, 19 Aug 2020 22:18:39 GMT
ARG KONG_VERSION=2.0.5
# Wed, 19 Aug 2020 22:18:40 GMT
ENV KONG_VERSION=2.0.5
# Wed, 19 Aug 2020 22:19:20 GMT
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apt-get update &&         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get update     && apt-get install -y --no-install-recommends perl unzip git zlib1g     && rm -rf /var/lib/apt/lists/* 	&& dpkg -i /tmp/kong.deb 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong 	&& kong version
# Wed, 19 Aug 2020 22:19:22 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Wed, 19 Aug 2020 22:19:23 GMT
USER kong
# Wed, 19 Aug 2020 22:19:25 GMT
RUN kong version
# Wed, 19 Aug 2020 22:19:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 19 Aug 2020 22:19:26 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 19 Aug 2020 22:19:27 GMT
STOPSIGNAL SIGQUIT
# Wed, 19 Aug 2020 22:19:27 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:3266c9b0302777bdc8ccdffab895ef058fb0777dc7600b0fe0b6c80dd3e71f9b`  
		Last Modified: Sat, 08 Aug 2020 00:25:28 GMT  
		Size: 40.1 MB (40073893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5240d1a89e17ed7dda51e3b38d3749e4ab3fb2fc2433de69ea23a838bb00c7`  
		Last Modified: Wed, 19 Aug 2020 21:33:04 GMT  
		Size: 469.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be065fa7bcd4d9f2540e1fec00c455a04755974444b17fb108b73cd4b15963a1`  
		Last Modified: Wed, 19 Aug 2020 21:33:04 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75305dc60d93c15276fd1b3dc21a09ef1ce9c248393c85eb1a5caf2be6e02671`  
		Last Modified: Wed, 19 Aug 2020 21:33:04 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa46bfa329110f43562ee6e8827c14ba35ca854832546866433eb48c646a4834`  
		Last Modified: Wed, 19 Aug 2020 22:20:08 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e687126cc3fdc8430861719ffae8ef5301c37308cbf8d33dad4de3e35d76ce07`  
		Last Modified: Wed, 19 Aug 2020 22:20:25 GMT  
		Size: 52.2 MB (52172683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09cc9ce67878ccf32c6510c937e47680d6e42b8acef2d1d607171b66e5373dc7`  
		Last Modified: Wed, 19 Aug 2020 22:20:07 GMT  
		Size: 687.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:461d95bafc1614a36a1baebe5679ad2636bbba96a795a1d380871913936e7244`  
		Last Modified: Wed, 19 Aug 2020 22:20:08 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.1`

```console
$ docker pull kong@sha256:da6a051abc306094600d9aeee1acf68361966450f516de38255125469b2d8f5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.1` - linux; amd64

```console
$ docker pull kong@sha256:723bf97cfdeaa1a406935e1759c2f592d327566d659b30202f80da02c78ffc62
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53144837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a62a8307bf7fd7fe6031f9b0ff3763a461143e6da341da33ea955ee31877ba02`
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
# Thu, 20 Aug 2020 23:19:49 GMT
ARG KONG_VERSION=2.1.3
# Thu, 20 Aug 2020 23:19:49 GMT
ENV KONG_VERSION=2.1.3
# Thu, 20 Aug 2020 23:19:49 GMT
ARG KONG_SHA256=2f2a73d468d95f3ded495aa4199b55d2148d1ad5cb5050372621a1768b34ba8a
# Thu, 20 Aug 2020 23:19:55 GMT
# ARGS: KONG_SHA256=2f2a73d468d95f3ded495aa4199b55d2148d1ad5cb5050372621a1768b34ba8a
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong; 	tar -C /kong -xzf /tmp/kong.tar.gz && 	mv /kong/usr/local/* /usr/local && 	mv /kong/etc/* /etc && 	rm -rf /kong && 	apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates && 	adduser -S kong && 	mkdir -p "/usr/local/kong" && 	chown -R kong:0 /usr/local/kong && 	chown kong:0 /usr/local/bin/kong && 	chmod -R g=u /usr/local/kong && 	rm -rf /tmp/kong.tar.gz &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Thu, 20 Aug 2020 23:19:55 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 20 Aug 2020 23:19:55 GMT
USER kong
# Thu, 20 Aug 2020 23:19:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 20 Aug 2020 23:19:56 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 20 Aug 2020 23:19:56 GMT
STOPSIGNAL SIGQUIT
# Thu, 20 Aug 2020 23:19:56 GMT
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
	-	`sha256:59f67e15df63b8d20592937e5d3cc7d55d5c2e0e3d5cf38f8cdc640bdc919394`  
		Last Modified: Thu, 20 Aug 2020 23:21:38 GMT  
		Size: 50.3 MB (50330658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985f1bf5706fb044dc193de9b6d0007ac3a07720ac24a5d500937e8dcabe1acf`  
		Last Modified: Thu, 20 Aug 2020 23:21:29 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.1.3`

```console
$ docker pull kong@sha256:da6a051abc306094600d9aeee1acf68361966450f516de38255125469b2d8f5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.1.3` - linux; amd64

```console
$ docker pull kong@sha256:723bf97cfdeaa1a406935e1759c2f592d327566d659b30202f80da02c78ffc62
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53144837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a62a8307bf7fd7fe6031f9b0ff3763a461143e6da341da33ea955ee31877ba02`
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
# Thu, 20 Aug 2020 23:19:49 GMT
ARG KONG_VERSION=2.1.3
# Thu, 20 Aug 2020 23:19:49 GMT
ENV KONG_VERSION=2.1.3
# Thu, 20 Aug 2020 23:19:49 GMT
ARG KONG_SHA256=2f2a73d468d95f3ded495aa4199b55d2148d1ad5cb5050372621a1768b34ba8a
# Thu, 20 Aug 2020 23:19:55 GMT
# ARGS: KONG_SHA256=2f2a73d468d95f3ded495aa4199b55d2148d1ad5cb5050372621a1768b34ba8a
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong; 	tar -C /kong -xzf /tmp/kong.tar.gz && 	mv /kong/usr/local/* /usr/local && 	mv /kong/etc/* /etc && 	rm -rf /kong && 	apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates && 	adduser -S kong && 	mkdir -p "/usr/local/kong" && 	chown -R kong:0 /usr/local/kong && 	chown kong:0 /usr/local/bin/kong && 	chmod -R g=u /usr/local/kong && 	rm -rf /tmp/kong.tar.gz &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Thu, 20 Aug 2020 23:19:55 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 20 Aug 2020 23:19:55 GMT
USER kong
# Thu, 20 Aug 2020 23:19:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 20 Aug 2020 23:19:56 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 20 Aug 2020 23:19:56 GMT
STOPSIGNAL SIGQUIT
# Thu, 20 Aug 2020 23:19:56 GMT
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
	-	`sha256:59f67e15df63b8d20592937e5d3cc7d55d5c2e0e3d5cf38f8cdc640bdc919394`  
		Last Modified: Thu, 20 Aug 2020 23:21:38 GMT  
		Size: 50.3 MB (50330658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985f1bf5706fb044dc193de9b6d0007ac3a07720ac24a5d500937e8dcabe1acf`  
		Last Modified: Thu, 20 Aug 2020 23:21:29 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.1.3-alpine`

```console
$ docker pull kong@sha256:da6a051abc306094600d9aeee1acf68361966450f516de38255125469b2d8f5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.1.3-alpine` - linux; amd64

```console
$ docker pull kong@sha256:723bf97cfdeaa1a406935e1759c2f592d327566d659b30202f80da02c78ffc62
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53144837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a62a8307bf7fd7fe6031f9b0ff3763a461143e6da341da33ea955ee31877ba02`
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
# Thu, 20 Aug 2020 23:19:49 GMT
ARG KONG_VERSION=2.1.3
# Thu, 20 Aug 2020 23:19:49 GMT
ENV KONG_VERSION=2.1.3
# Thu, 20 Aug 2020 23:19:49 GMT
ARG KONG_SHA256=2f2a73d468d95f3ded495aa4199b55d2148d1ad5cb5050372621a1768b34ba8a
# Thu, 20 Aug 2020 23:19:55 GMT
# ARGS: KONG_SHA256=2f2a73d468d95f3ded495aa4199b55d2148d1ad5cb5050372621a1768b34ba8a
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong; 	tar -C /kong -xzf /tmp/kong.tar.gz && 	mv /kong/usr/local/* /usr/local && 	mv /kong/etc/* /etc && 	rm -rf /kong && 	apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates && 	adduser -S kong && 	mkdir -p "/usr/local/kong" && 	chown -R kong:0 /usr/local/kong && 	chown kong:0 /usr/local/bin/kong && 	chmod -R g=u /usr/local/kong && 	rm -rf /tmp/kong.tar.gz &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Thu, 20 Aug 2020 23:19:55 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 20 Aug 2020 23:19:55 GMT
USER kong
# Thu, 20 Aug 2020 23:19:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 20 Aug 2020 23:19:56 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 20 Aug 2020 23:19:56 GMT
STOPSIGNAL SIGQUIT
# Thu, 20 Aug 2020 23:19:56 GMT
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
	-	`sha256:59f67e15df63b8d20592937e5d3cc7d55d5c2e0e3d5cf38f8cdc640bdc919394`  
		Last Modified: Thu, 20 Aug 2020 23:21:38 GMT  
		Size: 50.3 MB (50330658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985f1bf5706fb044dc193de9b6d0007ac3a07720ac24a5d500937e8dcabe1acf`  
		Last Modified: Thu, 20 Aug 2020 23:21:29 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.1.3-centos`

```console
$ docker pull kong@sha256:0534c9091405d883d076b23aaf37b148ee23c4395246ac13033755e7e3d2b534
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.1.3-centos` - linux; amd64

```console
$ docker pull kong@sha256:97a599c785a886947625e662e632e0559434ed959a86c539456f3679fc3ba8c3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.0 MB (127040636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91184190279322c37ed5a74b53067b55e82a9baf4eb1bae17754404bf9a2835a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:37:24 GMT
LABEL maintainer=Kong <support@konghq.com>
# Mon, 10 Aug 2020 18:37:24 GMT
ARG ASSET=ce
# Mon, 10 Aug 2020 18:37:25 GMT
ENV ASSET=ce
# Mon, 10 Aug 2020 18:37:25 GMT
ARG EE_PORTS
# Mon, 10 Aug 2020 18:37:25 GMT
COPY file:ff02c070e4c89f043b176279a7e41464b5fab8cb98cfcd6332fad2d2741fc41d in /tmp/kong.rpm 
# Thu, 20 Aug 2020 23:20:41 GMT
ARG KONG_VERSION=2.1.3
# Thu, 20 Aug 2020 23:20:41 GMT
ENV KONG_VERSION=2.1.3
# Fri, 28 Aug 2020 19:50:17 GMT
ARG KONG_SHA256=c39e596ac3aac771377fc67eb4fb151216daeba6e8b1595c670e8c571b5cd3a0
# Fri, 28 Aug 2020 19:50:50 GMT
# ARGS: KONG_SHA256=c39e596ac3aac771377fc67eb4fb151216daeba6e8b1595c670e8c571b5cd3a0
RUN set -ex; 	if [ "$ASSET" = "ce" ] ; then 		curl -fL "https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm" -o /tmp/kong.rpm 		&& echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -; 	fi; 	yum install -y -q unzip shadow-utils git 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki 	&& useradd kong 	&& mkdir -p "/usr/local/kong" 	&& yum --nogpgcheck localinstall -y /tmp/kong.rpm 	&& yum clean all 	&& rm /tmp/kong.rpm 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Fri, 28 Aug 2020 19:50:51 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Fri, 28 Aug 2020 19:50:51 GMT
USER kong
# Fri, 28 Aug 2020 19:50:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 28 Aug 2020 19:50:52 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 28 Aug 2020 19:50:52 GMT
STOPSIGNAL SIGQUIT
# Fri, 28 Aug 2020 19:50:52 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c636c1fa5b3254b7692cb41da3aee6a2547a919e7a84290bd6f7c05f9ef334`  
		Last Modified: Mon, 10 Aug 2020 18:39:00 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5b39764476fabfd67cf365cf33641b81d16a210aa4a68086804025427365d5a`  
		Last Modified: Fri, 28 Aug 2020 19:52:21 GMT  
		Size: 51.2 MB (51176587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd23a9600919cc54b1000cc18412d188688763e6b9a3398d123cf6e7737e9d11`  
		Last Modified: Fri, 28 Aug 2020 19:52:10 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.1.3-ubuntu`

```console
$ docker pull kong@sha256:8e6b00c4f03fd7efe48f452617c5234c2749ff2657d38c54310215aa21abaddd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.1.3-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:188bd7ebf66818f81c7cbb546414f8476125feb52ac81901c48a8875ff952b15
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107353589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d71ed9c5bbb1e1a941415654f5598b970ee67c8d1219920550215c08c70ef339`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 19 Aug 2020 21:16:18 GMT
ADD file:144835a276ed2d8eaf6e893d5560444fe0d6a6f9b9bdadec1eb56e7bd9814427 in / 
# Wed, 19 Aug 2020 21:16:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:16:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:16:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:16:22 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 23:17:58 GMT
ARG ASSET=ce
# Wed, 19 Aug 2020 23:17:58 GMT
ENV ASSET=ce
# Wed, 19 Aug 2020 23:17:58 GMT
ARG EE_PORTS
# Wed, 19 Aug 2020 23:17:59 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Thu, 20 Aug 2020 23:20:01 GMT
ARG KONG_VERSION=2.1.3
# Thu, 20 Aug 2020 23:20:01 GMT
ENV KONG_VERSION=2.1.3
# Fri, 28 Aug 2020 19:50:05 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt install --yes /tmp/kong.deb 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Fri, 28 Aug 2020 19:50:05 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Fri, 28 Aug 2020 19:50:06 GMT
USER kong
# Fri, 28 Aug 2020 19:50:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 28 Aug 2020 19:50:06 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 28 Aug 2020 19:50:06 GMT
STOPSIGNAL SIGQUIT
# Fri, 28 Aug 2020 19:50:06 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:8e097b52bfb8e743e52ccd2dfbd5a0363e48a00b06cdd3728a6fd4d1f3a34280`  
		Last Modified: Sat, 08 Aug 2020 13:20:06 GMT  
		Size: 44.4 MB (44447543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a613a9b4553ca86fac22546f2f79e2ff3d17d8d6aeea8b97d67862a5a40ad8ec`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc000f015361df35e770a910ce03d30691e35aa10d52f4a4f432f183a6c03db`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73eef93b7466c41f22f32d28aae5eb87e1ebc0c4d232c5f5e68c955d0e798dca`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d9e2e687753968754b433529f6c4aa4e47c99d475b990fac64438b40a5471b`  
		Last Modified: Wed, 19 Aug 2020 23:19:58 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9545aba2ff9867f9301774dc4869cede0de90571ca558a36f435ca004c3e1fa1`  
		Last Modified: Fri, 28 Aug 2020 19:52:06 GMT  
		Size: 62.9 MB (62903681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f7a8299fe5bbc3f4aaea4aed2b665eba6284cc07c42d77a19ba8609939ffff9`  
		Last Modified: Fri, 28 Aug 2020 19:51:29 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.1.3-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:1e918d483fefce686fb6d5232d343a310ffdf157356117292289a9437354ec57
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99355690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3a47b32757175cdd7183d2a31d58834b06dfa4252bf1dea4741ef00fae22d56`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 19 Aug 2020 21:31:42 GMT
ADD file:20ffb81d6b7edd3826c028369ed1774914394328d1ccef79ecee109f5cfbcc5f in / 
# Wed, 19 Aug 2020 21:31:45 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:31:49 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:31:51 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:31:52 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:17:19 GMT
ARG ASSET=ce
# Wed, 19 Aug 2020 22:17:19 GMT
ENV ASSET=ce
# Wed, 19 Aug 2020 22:17:20 GMT
ARG EE_PORTS
# Wed, 19 Aug 2020 22:17:20 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Thu, 20 Aug 2020 23:39:48 GMT
ARG KONG_VERSION=2.1.3
# Thu, 20 Aug 2020 23:39:49 GMT
ENV KONG_VERSION=2.1.3
# Fri, 28 Aug 2020 19:38:40 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt install --yes /tmp/kong.deb 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Fri, 28 Aug 2020 19:38:42 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Fri, 28 Aug 2020 19:38:43 GMT
USER kong
# Fri, 28 Aug 2020 19:38:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 28 Aug 2020 19:38:44 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 28 Aug 2020 19:38:44 GMT
STOPSIGNAL SIGQUIT
# Fri, 28 Aug 2020 19:38:45 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:3266c9b0302777bdc8ccdffab895ef058fb0777dc7600b0fe0b6c80dd3e71f9b`  
		Last Modified: Sat, 08 Aug 2020 00:25:28 GMT  
		Size: 40.1 MB (40073893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5240d1a89e17ed7dda51e3b38d3749e4ab3fb2fc2433de69ea23a838bb00c7`  
		Last Modified: Wed, 19 Aug 2020 21:33:04 GMT  
		Size: 469.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be065fa7bcd4d9f2540e1fec00c455a04755974444b17fb108b73cd4b15963a1`  
		Last Modified: Wed, 19 Aug 2020 21:33:04 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75305dc60d93c15276fd1b3dc21a09ef1ce9c248393c85eb1a5caf2be6e02671`  
		Last Modified: Wed, 19 Aug 2020 21:33:04 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45ba64437d430dfa5c413933a6334001af251dcf5e59d73ed032c39ba207c70`  
		Last Modified: Wed, 19 Aug 2020 22:19:41 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d7541d7d1a3984816b2213a98ca2f760264860a21389356d143f172c712d89`  
		Last Modified: Fri, 28 Aug 2020 19:39:28 GMT  
		Size: 59.3 MB (59279490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b7fe1cc3aa138a33a57c23c7ce1b63afc78ed15590162e1796971fdd78a0437`  
		Last Modified: Fri, 28 Aug 2020 19:39:08 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.1-alpine`

```console
$ docker pull kong@sha256:da6a051abc306094600d9aeee1acf68361966450f516de38255125469b2d8f5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.1-alpine` - linux; amd64

```console
$ docker pull kong@sha256:723bf97cfdeaa1a406935e1759c2f592d327566d659b30202f80da02c78ffc62
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53144837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a62a8307bf7fd7fe6031f9b0ff3763a461143e6da341da33ea955ee31877ba02`
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
# Thu, 20 Aug 2020 23:19:49 GMT
ARG KONG_VERSION=2.1.3
# Thu, 20 Aug 2020 23:19:49 GMT
ENV KONG_VERSION=2.1.3
# Thu, 20 Aug 2020 23:19:49 GMT
ARG KONG_SHA256=2f2a73d468d95f3ded495aa4199b55d2148d1ad5cb5050372621a1768b34ba8a
# Thu, 20 Aug 2020 23:19:55 GMT
# ARGS: KONG_SHA256=2f2a73d468d95f3ded495aa4199b55d2148d1ad5cb5050372621a1768b34ba8a
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong; 	tar -C /kong -xzf /tmp/kong.tar.gz && 	mv /kong/usr/local/* /usr/local && 	mv /kong/etc/* /etc && 	rm -rf /kong && 	apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates && 	adduser -S kong && 	mkdir -p "/usr/local/kong" && 	chown -R kong:0 /usr/local/kong && 	chown kong:0 /usr/local/bin/kong && 	chmod -R g=u /usr/local/kong && 	rm -rf /tmp/kong.tar.gz &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Thu, 20 Aug 2020 23:19:55 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 20 Aug 2020 23:19:55 GMT
USER kong
# Thu, 20 Aug 2020 23:19:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 20 Aug 2020 23:19:56 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 20 Aug 2020 23:19:56 GMT
STOPSIGNAL SIGQUIT
# Thu, 20 Aug 2020 23:19:56 GMT
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
	-	`sha256:59f67e15df63b8d20592937e5d3cc7d55d5c2e0e3d5cf38f8cdc640bdc919394`  
		Last Modified: Thu, 20 Aug 2020 23:21:38 GMT  
		Size: 50.3 MB (50330658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985f1bf5706fb044dc193de9b6d0007ac3a07720ac24a5d500937e8dcabe1acf`  
		Last Modified: Thu, 20 Aug 2020 23:21:29 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.1-centos`

```console
$ docker pull kong@sha256:0534c9091405d883d076b23aaf37b148ee23c4395246ac13033755e7e3d2b534
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.1-centos` - linux; amd64

```console
$ docker pull kong@sha256:97a599c785a886947625e662e632e0559434ed959a86c539456f3679fc3ba8c3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.0 MB (127040636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91184190279322c37ed5a74b53067b55e82a9baf4eb1bae17754404bf9a2835a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:37:24 GMT
LABEL maintainer=Kong <support@konghq.com>
# Mon, 10 Aug 2020 18:37:24 GMT
ARG ASSET=ce
# Mon, 10 Aug 2020 18:37:25 GMT
ENV ASSET=ce
# Mon, 10 Aug 2020 18:37:25 GMT
ARG EE_PORTS
# Mon, 10 Aug 2020 18:37:25 GMT
COPY file:ff02c070e4c89f043b176279a7e41464b5fab8cb98cfcd6332fad2d2741fc41d in /tmp/kong.rpm 
# Thu, 20 Aug 2020 23:20:41 GMT
ARG KONG_VERSION=2.1.3
# Thu, 20 Aug 2020 23:20:41 GMT
ENV KONG_VERSION=2.1.3
# Fri, 28 Aug 2020 19:50:17 GMT
ARG KONG_SHA256=c39e596ac3aac771377fc67eb4fb151216daeba6e8b1595c670e8c571b5cd3a0
# Fri, 28 Aug 2020 19:50:50 GMT
# ARGS: KONG_SHA256=c39e596ac3aac771377fc67eb4fb151216daeba6e8b1595c670e8c571b5cd3a0
RUN set -ex; 	if [ "$ASSET" = "ce" ] ; then 		curl -fL "https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm" -o /tmp/kong.rpm 		&& echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -; 	fi; 	yum install -y -q unzip shadow-utils git 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki 	&& useradd kong 	&& mkdir -p "/usr/local/kong" 	&& yum --nogpgcheck localinstall -y /tmp/kong.rpm 	&& yum clean all 	&& rm /tmp/kong.rpm 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Fri, 28 Aug 2020 19:50:51 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Fri, 28 Aug 2020 19:50:51 GMT
USER kong
# Fri, 28 Aug 2020 19:50:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 28 Aug 2020 19:50:52 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 28 Aug 2020 19:50:52 GMT
STOPSIGNAL SIGQUIT
# Fri, 28 Aug 2020 19:50:52 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c636c1fa5b3254b7692cb41da3aee6a2547a919e7a84290bd6f7c05f9ef334`  
		Last Modified: Mon, 10 Aug 2020 18:39:00 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5b39764476fabfd67cf365cf33641b81d16a210aa4a68086804025427365d5a`  
		Last Modified: Fri, 28 Aug 2020 19:52:21 GMT  
		Size: 51.2 MB (51176587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd23a9600919cc54b1000cc18412d188688763e6b9a3398d123cf6e7737e9d11`  
		Last Modified: Fri, 28 Aug 2020 19:52:10 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.1-ubuntu`

```console
$ docker pull kong@sha256:8e6b00c4f03fd7efe48f452617c5234c2749ff2657d38c54310215aa21abaddd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.1-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:188bd7ebf66818f81c7cbb546414f8476125feb52ac81901c48a8875ff952b15
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107353589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d71ed9c5bbb1e1a941415654f5598b970ee67c8d1219920550215c08c70ef339`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 19 Aug 2020 21:16:18 GMT
ADD file:144835a276ed2d8eaf6e893d5560444fe0d6a6f9b9bdadec1eb56e7bd9814427 in / 
# Wed, 19 Aug 2020 21:16:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:16:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:16:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:16:22 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 23:17:58 GMT
ARG ASSET=ce
# Wed, 19 Aug 2020 23:17:58 GMT
ENV ASSET=ce
# Wed, 19 Aug 2020 23:17:58 GMT
ARG EE_PORTS
# Wed, 19 Aug 2020 23:17:59 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Thu, 20 Aug 2020 23:20:01 GMT
ARG KONG_VERSION=2.1.3
# Thu, 20 Aug 2020 23:20:01 GMT
ENV KONG_VERSION=2.1.3
# Fri, 28 Aug 2020 19:50:05 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt install --yes /tmp/kong.deb 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Fri, 28 Aug 2020 19:50:05 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Fri, 28 Aug 2020 19:50:06 GMT
USER kong
# Fri, 28 Aug 2020 19:50:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 28 Aug 2020 19:50:06 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 28 Aug 2020 19:50:06 GMT
STOPSIGNAL SIGQUIT
# Fri, 28 Aug 2020 19:50:06 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:8e097b52bfb8e743e52ccd2dfbd5a0363e48a00b06cdd3728a6fd4d1f3a34280`  
		Last Modified: Sat, 08 Aug 2020 13:20:06 GMT  
		Size: 44.4 MB (44447543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a613a9b4553ca86fac22546f2f79e2ff3d17d8d6aeea8b97d67862a5a40ad8ec`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc000f015361df35e770a910ce03d30691e35aa10d52f4a4f432f183a6c03db`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73eef93b7466c41f22f32d28aae5eb87e1ebc0c4d232c5f5e68c955d0e798dca`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d9e2e687753968754b433529f6c4aa4e47c99d475b990fac64438b40a5471b`  
		Last Modified: Wed, 19 Aug 2020 23:19:58 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9545aba2ff9867f9301774dc4869cede0de90571ca558a36f435ca004c3e1fa1`  
		Last Modified: Fri, 28 Aug 2020 19:52:06 GMT  
		Size: 62.9 MB (62903681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f7a8299fe5bbc3f4aaea4aed2b665eba6284cc07c42d77a19ba8609939ffff9`  
		Last Modified: Fri, 28 Aug 2020 19:51:29 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.1-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:1e918d483fefce686fb6d5232d343a310ffdf157356117292289a9437354ec57
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99355690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3a47b32757175cdd7183d2a31d58834b06dfa4252bf1dea4741ef00fae22d56`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 19 Aug 2020 21:31:42 GMT
ADD file:20ffb81d6b7edd3826c028369ed1774914394328d1ccef79ecee109f5cfbcc5f in / 
# Wed, 19 Aug 2020 21:31:45 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:31:49 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:31:51 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:31:52 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:17:19 GMT
ARG ASSET=ce
# Wed, 19 Aug 2020 22:17:19 GMT
ENV ASSET=ce
# Wed, 19 Aug 2020 22:17:20 GMT
ARG EE_PORTS
# Wed, 19 Aug 2020 22:17:20 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Thu, 20 Aug 2020 23:39:48 GMT
ARG KONG_VERSION=2.1.3
# Thu, 20 Aug 2020 23:39:49 GMT
ENV KONG_VERSION=2.1.3
# Fri, 28 Aug 2020 19:38:40 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt install --yes /tmp/kong.deb 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Fri, 28 Aug 2020 19:38:42 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Fri, 28 Aug 2020 19:38:43 GMT
USER kong
# Fri, 28 Aug 2020 19:38:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 28 Aug 2020 19:38:44 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 28 Aug 2020 19:38:44 GMT
STOPSIGNAL SIGQUIT
# Fri, 28 Aug 2020 19:38:45 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:3266c9b0302777bdc8ccdffab895ef058fb0777dc7600b0fe0b6c80dd3e71f9b`  
		Last Modified: Sat, 08 Aug 2020 00:25:28 GMT  
		Size: 40.1 MB (40073893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5240d1a89e17ed7dda51e3b38d3749e4ab3fb2fc2433de69ea23a838bb00c7`  
		Last Modified: Wed, 19 Aug 2020 21:33:04 GMT  
		Size: 469.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be065fa7bcd4d9f2540e1fec00c455a04755974444b17fb108b73cd4b15963a1`  
		Last Modified: Wed, 19 Aug 2020 21:33:04 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75305dc60d93c15276fd1b3dc21a09ef1ce9c248393c85eb1a5caf2be6e02671`  
		Last Modified: Wed, 19 Aug 2020 21:33:04 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45ba64437d430dfa5c413933a6334001af251dcf5e59d73ed032c39ba207c70`  
		Last Modified: Wed, 19 Aug 2020 22:19:41 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d7541d7d1a3984816b2213a98ca2f760264860a21389356d143f172c712d89`  
		Last Modified: Fri, 28 Aug 2020 19:39:28 GMT  
		Size: 59.3 MB (59279490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b7fe1cc3aa138a33a57c23c7ce1b63afc78ed15590162e1796971fdd78a0437`  
		Last Modified: Fri, 28 Aug 2020 19:39:08 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:alpine`

```console
$ docker pull kong@sha256:da6a051abc306094600d9aeee1acf68361966450f516de38255125469b2d8f5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:alpine` - linux; amd64

```console
$ docker pull kong@sha256:723bf97cfdeaa1a406935e1759c2f592d327566d659b30202f80da02c78ffc62
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53144837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a62a8307bf7fd7fe6031f9b0ff3763a461143e6da341da33ea955ee31877ba02`
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
# Thu, 20 Aug 2020 23:19:49 GMT
ARG KONG_VERSION=2.1.3
# Thu, 20 Aug 2020 23:19:49 GMT
ENV KONG_VERSION=2.1.3
# Thu, 20 Aug 2020 23:19:49 GMT
ARG KONG_SHA256=2f2a73d468d95f3ded495aa4199b55d2148d1ad5cb5050372621a1768b34ba8a
# Thu, 20 Aug 2020 23:19:55 GMT
# ARGS: KONG_SHA256=2f2a73d468d95f3ded495aa4199b55d2148d1ad5cb5050372621a1768b34ba8a
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong; 	tar -C /kong -xzf /tmp/kong.tar.gz && 	mv /kong/usr/local/* /usr/local && 	mv /kong/etc/* /etc && 	rm -rf /kong && 	apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates && 	adduser -S kong && 	mkdir -p "/usr/local/kong" && 	chown -R kong:0 /usr/local/kong && 	chown kong:0 /usr/local/bin/kong && 	chmod -R g=u /usr/local/kong && 	rm -rf /tmp/kong.tar.gz &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Thu, 20 Aug 2020 23:19:55 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 20 Aug 2020 23:19:55 GMT
USER kong
# Thu, 20 Aug 2020 23:19:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 20 Aug 2020 23:19:56 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 20 Aug 2020 23:19:56 GMT
STOPSIGNAL SIGQUIT
# Thu, 20 Aug 2020 23:19:56 GMT
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
	-	`sha256:59f67e15df63b8d20592937e5d3cc7d55d5c2e0e3d5cf38f8cdc640bdc919394`  
		Last Modified: Thu, 20 Aug 2020 23:21:38 GMT  
		Size: 50.3 MB (50330658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985f1bf5706fb044dc193de9b6d0007ac3a07720ac24a5d500937e8dcabe1acf`  
		Last Modified: Thu, 20 Aug 2020 23:21:29 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:centos`

```console
$ docker pull kong@sha256:0534c9091405d883d076b23aaf37b148ee23c4395246ac13033755e7e3d2b534
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:centos` - linux; amd64

```console
$ docker pull kong@sha256:97a599c785a886947625e662e632e0559434ed959a86c539456f3679fc3ba8c3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.0 MB (127040636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91184190279322c37ed5a74b53067b55e82a9baf4eb1bae17754404bf9a2835a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Mon, 10 Aug 2020 18:20:08 GMT
ADD file:61908381d3142ffba798ae9a904476d19b197ab79d0338f14bec0f76649df8d4 in / 
# Mon, 10 Aug 2020 18:20:09 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200809 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-08-09 00:00:00+01:00
# Mon, 10 Aug 2020 18:20:09 GMT
CMD ["/bin/bash"]
# Mon, 10 Aug 2020 18:37:24 GMT
LABEL maintainer=Kong <support@konghq.com>
# Mon, 10 Aug 2020 18:37:24 GMT
ARG ASSET=ce
# Mon, 10 Aug 2020 18:37:25 GMT
ENV ASSET=ce
# Mon, 10 Aug 2020 18:37:25 GMT
ARG EE_PORTS
# Mon, 10 Aug 2020 18:37:25 GMT
COPY file:ff02c070e4c89f043b176279a7e41464b5fab8cb98cfcd6332fad2d2741fc41d in /tmp/kong.rpm 
# Thu, 20 Aug 2020 23:20:41 GMT
ARG KONG_VERSION=2.1.3
# Thu, 20 Aug 2020 23:20:41 GMT
ENV KONG_VERSION=2.1.3
# Fri, 28 Aug 2020 19:50:17 GMT
ARG KONG_SHA256=c39e596ac3aac771377fc67eb4fb151216daeba6e8b1595c670e8c571b5cd3a0
# Fri, 28 Aug 2020 19:50:50 GMT
# ARGS: KONG_SHA256=c39e596ac3aac771377fc67eb4fb151216daeba6e8b1595c670e8c571b5cd3a0
RUN set -ex; 	if [ "$ASSET" = "ce" ] ; then 		curl -fL "https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm" -o /tmp/kong.rpm 		&& echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -; 	fi; 	yum install -y -q unzip shadow-utils git 	&& yum clean all -q 	&& rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki 	&& useradd kong 	&& mkdir -p "/usr/local/kong" 	&& yum --nogpgcheck localinstall -y /tmp/kong.rpm 	&& yum clean all 	&& rm /tmp/kong.rpm 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Fri, 28 Aug 2020 19:50:51 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Fri, 28 Aug 2020 19:50:51 GMT
USER kong
# Fri, 28 Aug 2020 19:50:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 28 Aug 2020 19:50:52 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 28 Aug 2020 19:50:52 GMT
STOPSIGNAL SIGQUIT
# Fri, 28 Aug 2020 19:50:52 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:75f829a71a1c5277a7abf55495ac8d16759691d980bf1d931795e5eb68a294c0`  
		Last Modified: Mon, 10 Aug 2020 18:21:46 GMT  
		Size: 75.9 MB (75863188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c636c1fa5b3254b7692cb41da3aee6a2547a919e7a84290bd6f7c05f9ef334`  
		Last Modified: Mon, 10 Aug 2020 18:39:00 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5b39764476fabfd67cf365cf33641b81d16a210aa4a68086804025427365d5a`  
		Last Modified: Fri, 28 Aug 2020 19:52:21 GMT  
		Size: 51.2 MB (51176587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd23a9600919cc54b1000cc18412d188688763e6b9a3398d123cf6e7737e9d11`  
		Last Modified: Fri, 28 Aug 2020 19:52:10 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:latest`

```console
$ docker pull kong@sha256:da6a051abc306094600d9aeee1acf68361966450f516de38255125469b2d8f5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:latest` - linux; amd64

```console
$ docker pull kong@sha256:723bf97cfdeaa1a406935e1759c2f592d327566d659b30202f80da02c78ffc62
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53144837 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a62a8307bf7fd7fe6031f9b0ff3763a461143e6da341da33ea955ee31877ba02`
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
# Thu, 20 Aug 2020 23:19:49 GMT
ARG KONG_VERSION=2.1.3
# Thu, 20 Aug 2020 23:19:49 GMT
ENV KONG_VERSION=2.1.3
# Thu, 20 Aug 2020 23:19:49 GMT
ARG KONG_SHA256=2f2a73d468d95f3ded495aa4199b55d2148d1ad5cb5050372621a1768b34ba8a
# Thu, 20 Aug 2020 23:19:55 GMT
# ARGS: KONG_SHA256=2f2a73d468d95f3ded495aa4199b55d2148d1ad5cb5050372621a1768b34ba8a
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.amd64.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong; 	tar -C /kong -xzf /tmp/kong.tar.gz && 	mv /kong/usr/local/* /usr/local && 	mv /kong/etc/* /etc && 	rm -rf /kong && 	apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates && 	adduser -S kong && 	mkdir -p "/usr/local/kong" && 	chown -R kong:0 /usr/local/kong && 	chown kong:0 /usr/local/bin/kong && 	chmod -R g=u /usr/local/kong && 	rm -rf /tmp/kong.tar.gz &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Thu, 20 Aug 2020 23:19:55 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 20 Aug 2020 23:19:55 GMT
USER kong
# Thu, 20 Aug 2020 23:19:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 20 Aug 2020 23:19:56 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 20 Aug 2020 23:19:56 GMT
STOPSIGNAL SIGQUIT
# Thu, 20 Aug 2020 23:19:56 GMT
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
	-	`sha256:59f67e15df63b8d20592937e5d3cc7d55d5c2e0e3d5cf38f8cdc640bdc919394`  
		Last Modified: Thu, 20 Aug 2020 23:21:38 GMT  
		Size: 50.3 MB (50330658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985f1bf5706fb044dc193de9b6d0007ac3a07720ac24a5d500937e8dcabe1acf`  
		Last Modified: Thu, 20 Aug 2020 23:21:29 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:ubuntu`

```console
$ docker pull kong@sha256:8e6b00c4f03fd7efe48f452617c5234c2749ff2657d38c54310215aa21abaddd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:188bd7ebf66818f81c7cbb546414f8476125feb52ac81901c48a8875ff952b15
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107353589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d71ed9c5bbb1e1a941415654f5598b970ee67c8d1219920550215c08c70ef339`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 19 Aug 2020 21:16:18 GMT
ADD file:144835a276ed2d8eaf6e893d5560444fe0d6a6f9b9bdadec1eb56e7bd9814427 in / 
# Wed, 19 Aug 2020 21:16:19 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:16:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:16:22 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:16:22 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 23:17:58 GMT
ARG ASSET=ce
# Wed, 19 Aug 2020 23:17:58 GMT
ENV ASSET=ce
# Wed, 19 Aug 2020 23:17:58 GMT
ARG EE_PORTS
# Wed, 19 Aug 2020 23:17:59 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Thu, 20 Aug 2020 23:20:01 GMT
ARG KONG_VERSION=2.1.3
# Thu, 20 Aug 2020 23:20:01 GMT
ENV KONG_VERSION=2.1.3
# Fri, 28 Aug 2020 19:50:05 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt install --yes /tmp/kong.deb 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Fri, 28 Aug 2020 19:50:05 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Fri, 28 Aug 2020 19:50:06 GMT
USER kong
# Fri, 28 Aug 2020 19:50:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 28 Aug 2020 19:50:06 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 28 Aug 2020 19:50:06 GMT
STOPSIGNAL SIGQUIT
# Fri, 28 Aug 2020 19:50:06 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:8e097b52bfb8e743e52ccd2dfbd5a0363e48a00b06cdd3728a6fd4d1f3a34280`  
		Last Modified: Sat, 08 Aug 2020 13:20:06 GMT  
		Size: 44.4 MB (44447543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a613a9b4553ca86fac22546f2f79e2ff3d17d8d6aeea8b97d67862a5a40ad8ec`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc000f015361df35e770a910ce03d30691e35aa10d52f4a4f432f183a6c03db`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73eef93b7466c41f22f32d28aae5eb87e1ebc0c4d232c5f5e68c955d0e798dca`  
		Last Modified: Wed, 19 Aug 2020 21:17:23 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d9e2e687753968754b433529f6c4aa4e47c99d475b990fac64438b40a5471b`  
		Last Modified: Wed, 19 Aug 2020 23:19:58 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9545aba2ff9867f9301774dc4869cede0de90571ca558a36f435ca004c3e1fa1`  
		Last Modified: Fri, 28 Aug 2020 19:52:06 GMT  
		Size: 62.9 MB (62903681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f7a8299fe5bbc3f4aaea4aed2b665eba6284cc07c42d77a19ba8609939ffff9`  
		Last Modified: Fri, 28 Aug 2020 19:51:29 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:1e918d483fefce686fb6d5232d343a310ffdf157356117292289a9437354ec57
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.4 MB (99355690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3a47b32757175cdd7183d2a31d58834b06dfa4252bf1dea4741ef00fae22d56`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 19 Aug 2020 21:31:42 GMT
ADD file:20ffb81d6b7edd3826c028369ed1774914394328d1ccef79ecee109f5cfbcc5f in / 
# Wed, 19 Aug 2020 21:31:45 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 19 Aug 2020 21:31:49 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:31:51 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:31:52 GMT
CMD ["/bin/bash"]
# Wed, 19 Aug 2020 22:17:19 GMT
ARG ASSET=ce
# Wed, 19 Aug 2020 22:17:19 GMT
ENV ASSET=ce
# Wed, 19 Aug 2020 22:17:20 GMT
ARG EE_PORTS
# Wed, 19 Aug 2020 22:17:20 GMT
COPY file:c24b3b9739a4614fa0679c1a90bac51eb61f9f84b2b02c5c24925e0c84878649 in /tmp/kong.deb 
# Thu, 20 Aug 2020 23:39:48 GMT
ARG KONG_VERSION=2.1.3
# Thu, 20 Aug 2020 23:39:49 GMT
ENV KONG_VERSION=2.1.3
# Fri, 28 Aug 2020 19:38:40 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt install --yes /tmp/kong.deb 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Fri, 28 Aug 2020 19:38:42 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Fri, 28 Aug 2020 19:38:43 GMT
USER kong
# Fri, 28 Aug 2020 19:38:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 28 Aug 2020 19:38:44 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 28 Aug 2020 19:38:44 GMT
STOPSIGNAL SIGQUIT
# Fri, 28 Aug 2020 19:38:45 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:3266c9b0302777bdc8ccdffab895ef058fb0777dc7600b0fe0b6c80dd3e71f9b`  
		Last Modified: Sat, 08 Aug 2020 00:25:28 GMT  
		Size: 40.1 MB (40073893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5240d1a89e17ed7dda51e3b38d3749e4ab3fb2fc2433de69ea23a838bb00c7`  
		Last Modified: Wed, 19 Aug 2020 21:33:04 GMT  
		Size: 469.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be065fa7bcd4d9f2540e1fec00c455a04755974444b17fb108b73cd4b15963a1`  
		Last Modified: Wed, 19 Aug 2020 21:33:04 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75305dc60d93c15276fd1b3dc21a09ef1ce9c248393c85eb1a5caf2be6e02671`  
		Last Modified: Wed, 19 Aug 2020 21:33:04 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45ba64437d430dfa5c413933a6334001af251dcf5e59d73ed032c39ba207c70`  
		Last Modified: Wed, 19 Aug 2020 22:19:41 GMT  
		Size: 130.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d7541d7d1a3984816b2213a98ca2f760264860a21389356d143f172c712d89`  
		Last Modified: Fri, 28 Aug 2020 19:39:28 GMT  
		Size: 59.3 MB (59279490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b7fe1cc3aa138a33a57c23c7ce1b63afc78ed15590162e1796971fdd78a0437`  
		Last Modified: Fri, 28 Aug 2020 19:39:08 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
