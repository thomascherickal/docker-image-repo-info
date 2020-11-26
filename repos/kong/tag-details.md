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
-	[`kong:2.2.0-alpine`](#kong220-alpine)
-	[`kong:2.2.0-centos`](#kong220-centos)
-	[`kong:2.2.0-ubuntu`](#kong220-ubuntu)
-	[`kong:2.2-alpine`](#kong22-alpine)
-	[`kong:2.2-centos`](#kong22-centos)
-	[`kong:2.2-ubuntu`](#kong22-ubuntu)
-	[`kong:alpine`](#kongalpine)
-	[`kong:centos`](#kongcentos)
-	[`kong:latest`](#konglatest)
-	[`kong:ubuntu`](#kongubuntu)

## `kong:2`

```console
$ docker pull kong@sha256:8b141da0a8fa843e1b745720089448db0236eb9d88999f009c8bf1f20d52c033
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2` - linux; amd64

```console
$ docker pull kong@sha256:19ee9b741cc0dec5276136131af486702441181180ce4a630dd55dfce6d17ded
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53143102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1550bbb81daedb5b1e1b32ff7cfebc601eb3f5e2fe0fc816b4da13e77fdfdbc9`
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
# Thu, 29 Oct 2020 18:21:14 GMT
ARG KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:21:14 GMT
ENV KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:21:21 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256='6adb706eab6cc535f2703bd8993a5d5259159cf8a630c3d3974973dbe6bbf5a6' ;; 		aarch64) arch='arm64'; KONG_SHA256='a93b1c015d86b5d8b4038f3fd73332bfef97fa1c768545f353af03f54cf97fb8' ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Thu, 29 Oct 2020 18:21:22 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 29 Oct 2020 18:21:22 GMT
USER kong
# Thu, 29 Oct 2020 18:21:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Oct 2020 18:21:22 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 29 Oct 2020 18:21:22 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Oct 2020 18:21:22 GMT
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
	-	`sha256:c25d97cc4039bd282d150d09da1590e01019a05e641c6f61495324fb35a0a6ea`  
		Last Modified: Thu, 29 Oct 2020 18:23:45 GMT  
		Size: 50.3 MB (50328923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98513f5777887ba304362c52a37f9686f876ad0af12cdb8b6e49d17de0a348a8`  
		Last Modified: Thu, 29 Oct 2020 18:23:36 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:0a0cad9b3779321b3c9a35ad077bf1e5645e291d7329e161183152692c5cb637
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.7 MB (52673538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d354929336a5e32ec6d0b868be426c01545ee0f07715f5d4f6574114013cb13`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Tue, 22 Sep 2020 19:05:32 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 22 Sep 2020 19:05:34 GMT
ARG ASSET=ce
# Tue, 22 Sep 2020 19:05:35 GMT
ENV ASSET=ce
# Tue, 22 Sep 2020 19:05:36 GMT
ARG EE_PORTS
# Tue, 22 Sep 2020 19:05:36 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 29 Oct 2020 18:42:33 GMT
ARG KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:42:33 GMT
ENV KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:42:46 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256='6adb706eab6cc535f2703bd8993a5d5259159cf8a630c3d3974973dbe6bbf5a6' ;; 		aarch64) arch='arm64'; KONG_SHA256='a93b1c015d86b5d8b4038f3fd73332bfef97fa1c768545f353af03f54cf97fb8' ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Thu, 29 Oct 2020 18:42:48 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 29 Oct 2020 18:42:48 GMT
USER kong
# Thu, 29 Oct 2020 18:42:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Oct 2020 18:42:49 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 29 Oct 2020 18:42:50 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Oct 2020 18:42:50 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f1f361b75deeea5140a58989e54db49d72c8f2794625392d9b60e5f6adea53`  
		Last Modified: Tue, 22 Sep 2020 19:08:54 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0562e5901c7c1412846095fddf0527b3aec71f8d310829523e905e5dec70db4a`  
		Last Modified: Thu, 29 Oct 2020 18:51:28 GMT  
		Size: 49.9 MB (49948248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b00d686849acde734efe3f6499685d14b6e6deea6307aa2194f32f58e7a026`  
		Last Modified: Thu, 29 Oct 2020 18:51:13 GMT  
		Size: 733.0 B  
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
$ docker pull kong@sha256:4118119ec391ab6f56518a7cba354cec470da750a6674671ba24ad6320cb213f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.0.5-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:596c716073c702ab620412ad0f617ff151943214b9c8c2875a34e4c6bd89fda3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.9 MB (100903184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:932f1c0ee31126d2b02c82e4d89d7de35023b5be4463402944a26a25667e8967`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 23 Oct 2020 17:33:08 GMT
ADD file:c1f3147c7b6710af5affd417ff822ee28df872d716003858d3d2e23d2277c981 in / 
# Fri, 23 Oct 2020 17:33:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:33:09 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 17:33:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:33:10 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 17:52:28 GMT
ARG ASSET=ce
# Fri, 23 Oct 2020 17:52:28 GMT
ENV ASSET=ce
# Fri, 23 Oct 2020 17:53:29 GMT
COPY file:5307743dbc5e81034b8adaf56f281bcb13b0da2d468cb6450d72fa5b77543ccf in /tmp/kong.deb 
# Fri, 23 Oct 2020 17:53:29 GMT
ARG KONG_VERSION=2.0.5
# Fri, 23 Oct 2020 17:53:30 GMT
ENV KONG_VERSION=2.0.5
# Fri, 23 Oct 2020 17:53:50 GMT
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apt-get update &&         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get update     && apt-get install -y --no-install-recommends perl unzip git zlib1g     && rm -rf /var/lib/apt/lists/* 	&& dpkg -i /tmp/kong.deb 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong 	&& kong version
# Fri, 23 Oct 2020 17:53:51 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Fri, 23 Oct 2020 17:53:51 GMT
USER kong
# Fri, 23 Oct 2020 17:53:52 GMT
RUN kong version
# Fri, 23 Oct 2020 17:53:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Oct 2020 17:53:52 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 23 Oct 2020 17:53:52 GMT
STOPSIGNAL SIGQUIT
# Fri, 23 Oct 2020 17:53:52 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:2c11b7cecaa5d3e2a57e290921ababbfb8572b549015168d4cbd91c340d2c566`  
		Last Modified: Wed, 14 Oct 2020 13:20:30 GMT  
		Size: 45.8 MB (45825714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04637fa562525a9366f00e8f4b08d04a347bded1ee513738451ef9d42b4dfc4e`  
		Last Modified: Fri, 23 Oct 2020 17:33:48 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e6af23a0f38c4a6511147d2a9dc06a07a7afa0669000cb62720c7eafe031ae`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a424de92ad71639c5cabadcdab0493e4067eb2f9cf109ffef40db178349238`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b999932a0fa429918aa85ab481a3b8fc630f558e9ed11545a568d88d1d986dd`  
		Last Modified: Fri, 23 Oct 2020 17:54:52 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff257bf6943fd0518b353dcf3978d220960d457c8417d18b54ede0b0db8ee35e`  
		Last Modified: Fri, 23 Oct 2020 17:55:04 GMT  
		Size: 55.1 MB (55075019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893c80d49482e175cc7a66c4627e4c2008f59865f9991bf9308e18da1fb2e7dc`  
		Last Modified: Fri, 23 Oct 2020 17:54:53 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfdca1a1c6d6c04fd0b8acd6206d2fef70ec3fe2205a867ee9ced2cf1f890bed`  
		Last Modified: Fri, 23 Oct 2020 17:54:52 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.0.5-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:0f300366bad5d9eba035bf1451aaff87ce06dafdeeb472e94dc2aafa4344a494
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.0 MB (93018128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd78574188a2781186eee913711bd8c62c1cef29fbbfe97a58e04bea92552997`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 25 Nov 2020 22:44:18 GMT
ADD file:a360b1e1db1ae9973dac11dfe4e549f6416e278f53c42eb5e98b3b3da8d2a5ae in / 
# Wed, 25 Nov 2020 22:44:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:44:23 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 22:44:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:44:26 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:26:02 GMT
ARG ASSET=ce
# Wed, 25 Nov 2020 23:26:04 GMT
ENV ASSET=ce
# Wed, 25 Nov 2020 23:28:34 GMT
COPY file:5307743dbc5e81034b8adaf56f281bcb13b0da2d468cb6450d72fa5b77543ccf in /tmp/kong.deb 
# Wed, 25 Nov 2020 23:28:35 GMT
ARG KONG_VERSION=2.0.5
# Wed, 25 Nov 2020 23:28:36 GMT
ENV KONG_VERSION=2.0.5
# Wed, 25 Nov 2020 23:29:18 GMT
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apt-get update &&         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get update     && apt-get install -y --no-install-recommends perl unzip git zlib1g     && rm -rf /var/lib/apt/lists/* 	&& dpkg -i /tmp/kong.deb 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong 	&& kong version
# Wed, 25 Nov 2020 23:29:20 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Wed, 25 Nov 2020 23:29:21 GMT
USER kong
# Wed, 25 Nov 2020 23:29:24 GMT
RUN kong version
# Wed, 25 Nov 2020 23:29:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 25 Nov 2020 23:29:29 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 25 Nov 2020 23:29:29 GMT
STOPSIGNAL SIGQUIT
# Wed, 25 Nov 2020 23:29:30 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:3e30c5e4609ac16f9e19faa3800699e28c77aadcfcbde2ddd5954606f80fa170`  
		Last Modified: Sat, 31 Oct 2020 00:25:13 GMT  
		Size: 40.8 MB (40826105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be82da0c7e998c509a8e86338f139501b62fde0df3908dd489a8249380ea3441`  
		Last Modified: Wed, 25 Nov 2020 22:45:42 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf04dffef88e5257b2388d643e5fb03a812316de0737ce92e3888a6722cea5e`  
		Last Modified: Wed, 25 Nov 2020 22:45:43 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2624f7934929e6e67f81a9becb317179367648ec1236d644e9bf3a00d3fe3772`  
		Last Modified: Wed, 25 Nov 2020 22:45:43 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80aa89518f435ec6f9a0a429a54fc0c1efe5506570de4a2b477b3831010738e0`  
		Last Modified: Wed, 25 Nov 2020 23:30:46 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0854eeddb2934af892b9ff7ac40e9ac77296c7b4b02ad9896ee723326092cb32`  
		Last Modified: Wed, 25 Nov 2020 23:31:00 GMT  
		Size: 52.2 MB (52189622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93860ffaeb22fb36c81b7a964a388a78d3762b6fd001005d8250b27269d74683`  
		Last Modified: Wed, 25 Nov 2020 23:30:46 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bca7345029988cc3db286d56438da2694c4f13b8374f6e8473820cee87abf4e`  
		Last Modified: Wed, 25 Nov 2020 23:30:46 GMT  
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
$ docker pull kong@sha256:4118119ec391ab6f56518a7cba354cec470da750a6674671ba24ad6320cb213f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.0-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:596c716073c702ab620412ad0f617ff151943214b9c8c2875a34e4c6bd89fda3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.9 MB (100903184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:932f1c0ee31126d2b02c82e4d89d7de35023b5be4463402944a26a25667e8967`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 23 Oct 2020 17:33:08 GMT
ADD file:c1f3147c7b6710af5affd417ff822ee28df872d716003858d3d2e23d2277c981 in / 
# Fri, 23 Oct 2020 17:33:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:33:09 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 17:33:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:33:10 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 17:52:28 GMT
ARG ASSET=ce
# Fri, 23 Oct 2020 17:52:28 GMT
ENV ASSET=ce
# Fri, 23 Oct 2020 17:53:29 GMT
COPY file:5307743dbc5e81034b8adaf56f281bcb13b0da2d468cb6450d72fa5b77543ccf in /tmp/kong.deb 
# Fri, 23 Oct 2020 17:53:29 GMT
ARG KONG_VERSION=2.0.5
# Fri, 23 Oct 2020 17:53:30 GMT
ENV KONG_VERSION=2.0.5
# Fri, 23 Oct 2020 17:53:50 GMT
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apt-get update &&         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get update     && apt-get install -y --no-install-recommends perl unzip git zlib1g     && rm -rf /var/lib/apt/lists/* 	&& dpkg -i /tmp/kong.deb 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong 	&& kong version
# Fri, 23 Oct 2020 17:53:51 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Fri, 23 Oct 2020 17:53:51 GMT
USER kong
# Fri, 23 Oct 2020 17:53:52 GMT
RUN kong version
# Fri, 23 Oct 2020 17:53:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Oct 2020 17:53:52 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 23 Oct 2020 17:53:52 GMT
STOPSIGNAL SIGQUIT
# Fri, 23 Oct 2020 17:53:52 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:2c11b7cecaa5d3e2a57e290921ababbfb8572b549015168d4cbd91c340d2c566`  
		Last Modified: Wed, 14 Oct 2020 13:20:30 GMT  
		Size: 45.8 MB (45825714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04637fa562525a9366f00e8f4b08d04a347bded1ee513738451ef9d42b4dfc4e`  
		Last Modified: Fri, 23 Oct 2020 17:33:48 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e6af23a0f38c4a6511147d2a9dc06a07a7afa0669000cb62720c7eafe031ae`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a424de92ad71639c5cabadcdab0493e4067eb2f9cf109ffef40db178349238`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b999932a0fa429918aa85ab481a3b8fc630f558e9ed11545a568d88d1d986dd`  
		Last Modified: Fri, 23 Oct 2020 17:54:52 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff257bf6943fd0518b353dcf3978d220960d457c8417d18b54ede0b0db8ee35e`  
		Last Modified: Fri, 23 Oct 2020 17:55:04 GMT  
		Size: 55.1 MB (55075019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893c80d49482e175cc7a66c4627e4c2008f59865f9991bf9308e18da1fb2e7dc`  
		Last Modified: Fri, 23 Oct 2020 17:54:53 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfdca1a1c6d6c04fd0b8acd6206d2fef70ec3fe2205a867ee9ced2cf1f890bed`  
		Last Modified: Fri, 23 Oct 2020 17:54:52 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.0-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:0f300366bad5d9eba035bf1451aaff87ce06dafdeeb472e94dc2aafa4344a494
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.0 MB (93018128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd78574188a2781186eee913711bd8c62c1cef29fbbfe97a58e04bea92552997`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 25 Nov 2020 22:44:18 GMT
ADD file:a360b1e1db1ae9973dac11dfe4e549f6416e278f53c42eb5e98b3b3da8d2a5ae in / 
# Wed, 25 Nov 2020 22:44:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:44:23 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 22:44:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:44:26 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:26:02 GMT
ARG ASSET=ce
# Wed, 25 Nov 2020 23:26:04 GMT
ENV ASSET=ce
# Wed, 25 Nov 2020 23:28:34 GMT
COPY file:5307743dbc5e81034b8adaf56f281bcb13b0da2d468cb6450d72fa5b77543ccf in /tmp/kong.deb 
# Wed, 25 Nov 2020 23:28:35 GMT
ARG KONG_VERSION=2.0.5
# Wed, 25 Nov 2020 23:28:36 GMT
ENV KONG_VERSION=2.0.5
# Wed, 25 Nov 2020 23:29:18 GMT
RUN set -ex;     if [ "$ASSET" = "ce" ] ; then         apt-get update &&         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get update     && apt-get install -y --no-install-recommends perl unzip git zlib1g     && rm -rf /var/lib/apt/lists/* 	&& dpkg -i /tmp/kong.deb 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong 	&& kong version
# Wed, 25 Nov 2020 23:29:20 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Wed, 25 Nov 2020 23:29:21 GMT
USER kong
# Wed, 25 Nov 2020 23:29:24 GMT
RUN kong version
# Wed, 25 Nov 2020 23:29:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 25 Nov 2020 23:29:29 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 25 Nov 2020 23:29:29 GMT
STOPSIGNAL SIGQUIT
# Wed, 25 Nov 2020 23:29:30 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:3e30c5e4609ac16f9e19faa3800699e28c77aadcfcbde2ddd5954606f80fa170`  
		Last Modified: Sat, 31 Oct 2020 00:25:13 GMT  
		Size: 40.8 MB (40826105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be82da0c7e998c509a8e86338f139501b62fde0df3908dd489a8249380ea3441`  
		Last Modified: Wed, 25 Nov 2020 22:45:42 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf04dffef88e5257b2388d643e5fb03a812316de0737ce92e3888a6722cea5e`  
		Last Modified: Wed, 25 Nov 2020 22:45:43 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2624f7934929e6e67f81a9becb317179367648ec1236d644e9bf3a00d3fe3772`  
		Last Modified: Wed, 25 Nov 2020 22:45:43 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80aa89518f435ec6f9a0a429a54fc0c1efe5506570de4a2b477b3831010738e0`  
		Last Modified: Wed, 25 Nov 2020 23:30:46 GMT  
		Size: 131.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0854eeddb2934af892b9ff7ac40e9ac77296c7b4b02ad9896ee723326092cb32`  
		Last Modified: Wed, 25 Nov 2020 23:31:00 GMT  
		Size: 52.2 MB (52189622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93860ffaeb22fb36c81b7a964a388a78d3762b6fd001005d8250b27269d74683`  
		Last Modified: Wed, 25 Nov 2020 23:30:46 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bca7345029988cc3db286d56438da2694c4f13b8374f6e8473820cee87abf4e`  
		Last Modified: Wed, 25 Nov 2020 23:30:46 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.1`

```console
$ docker pull kong@sha256:3988a79c97f08d85e4c5cfbefc4085d52904ee87de95413865d4a59d1b944f3c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.1` - linux; amd64

```console
$ docker pull kong@sha256:32aec5d7a1152fad8604b74dfbfe544f8c346c42651791a768fd5f0025bc59b1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53150431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d55bcda861cae15b7310f14adc6b1f942f3d867ef30b6ff8da9268ac0ebd58a1`
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
# Tue, 22 Sep 2020 18:32:31 GMT
ARG KONG_VERSION=2.1.4
# Tue, 22 Sep 2020 18:32:31 GMT
ENV KONG_VERSION=2.1.4
# Tue, 22 Sep 2020 18:32:37 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256='760cea1f7a058be6000e14dfecfeb73cc79245f696f18e0fcf0825935b944ab3' ;; 		aarch64) arch='arm64'; KONG_SHA256='08038f49f162ab5edc357d7712e90241f6571027cb8741b15ba0c951653764c2' ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong; 	tar -C /kong -xzf /tmp/kong.tar.gz && 	mv /kong/usr/local/* /usr/local && 	mv /kong/etc/* /etc && 	rm -rf /kong && 	apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates && 	adduser -S kong && 	mkdir -p "/usr/local/kong" && 	chown -R kong:0 /usr/local/kong && 	chown kong:0 /usr/local/bin/kong && 	chmod -R g=u /usr/local/kong && 	rm -rf /tmp/kong.tar.gz &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Tue, 22 Sep 2020 18:32:37 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Tue, 22 Sep 2020 18:32:37 GMT
USER kong
# Tue, 22 Sep 2020 18:32:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 22 Sep 2020 18:32:38 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 22 Sep 2020 18:32:38 GMT
STOPSIGNAL SIGQUIT
# Tue, 22 Sep 2020 18:32:38 GMT
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
	-	`sha256:7306b16482a5463a3999b475a70c541b3eafcd2c4d3b6da8b5ae4d53bc49be14`  
		Last Modified: Tue, 22 Sep 2020 18:34:57 GMT  
		Size: 50.3 MB (50336253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff24278e47024f951b5e7834bbcb0a5ce4e0ea9086924d0a929eb960a35b3542`  
		Last Modified: Tue, 22 Sep 2020 18:34:47 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.1` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:f93512ee31e30463969b469e34cac78840d361853f716e26c323bdc9d98ee067
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.7 MB (52670238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43f3c5137a40d5709b4d2bc75c83f6fe8491414ca66007819c2f8ea9ebaea1e3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Tue, 22 Sep 2020 19:05:32 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 22 Sep 2020 19:05:34 GMT
ARG ASSET=ce
# Tue, 22 Sep 2020 19:05:35 GMT
ENV ASSET=ce
# Tue, 22 Sep 2020 19:05:36 GMT
ARG EE_PORTS
# Tue, 22 Sep 2020 19:05:36 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 22 Sep 2020 19:05:41 GMT
ARG KONG_VERSION=2.1.4
# Tue, 22 Sep 2020 19:05:48 GMT
ENV KONG_VERSION=2.1.4
# Tue, 22 Sep 2020 19:06:05 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256='760cea1f7a058be6000e14dfecfeb73cc79245f696f18e0fcf0825935b944ab3' ;; 		aarch64) arch='arm64'; KONG_SHA256='08038f49f162ab5edc357d7712e90241f6571027cb8741b15ba0c951653764c2' ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong; 	tar -C /kong -xzf /tmp/kong.tar.gz && 	mv /kong/usr/local/* /usr/local && 	mv /kong/etc/* /etc && 	rm -rf /kong && 	apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates && 	adduser -S kong && 	mkdir -p "/usr/local/kong" && 	chown -R kong:0 /usr/local/kong && 	chown kong:0 /usr/local/bin/kong && 	chmod -R g=u /usr/local/kong && 	rm -rf /tmp/kong.tar.gz &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Tue, 22 Sep 2020 19:06:08 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Tue, 22 Sep 2020 19:06:08 GMT
USER kong
# Tue, 22 Sep 2020 19:06:09 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 22 Sep 2020 19:06:10 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 22 Sep 2020 19:06:10 GMT
STOPSIGNAL SIGQUIT
# Tue, 22 Sep 2020 19:06:11 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f1f361b75deeea5140a58989e54db49d72c8f2794625392d9b60e5f6adea53`  
		Last Modified: Tue, 22 Sep 2020 19:08:54 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715b0084f83b0d2b1feb234f814f8223cfc5574fb6863e5cdc425ff3e3b468a8`  
		Last Modified: Tue, 22 Sep 2020 19:09:11 GMT  
		Size: 49.9 MB (49944947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73656217c4f0421f0b017bae8d6959f82fe85783971bd97d00e89643a56c8f45`  
		Last Modified: Tue, 22 Sep 2020 19:08:54 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.1.4`

```console
$ docker pull kong@sha256:3988a79c97f08d85e4c5cfbefc4085d52904ee87de95413865d4a59d1b944f3c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.1.4` - linux; amd64

```console
$ docker pull kong@sha256:32aec5d7a1152fad8604b74dfbfe544f8c346c42651791a768fd5f0025bc59b1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53150431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d55bcda861cae15b7310f14adc6b1f942f3d867ef30b6ff8da9268ac0ebd58a1`
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
# Tue, 22 Sep 2020 18:32:31 GMT
ARG KONG_VERSION=2.1.4
# Tue, 22 Sep 2020 18:32:31 GMT
ENV KONG_VERSION=2.1.4
# Tue, 22 Sep 2020 18:32:37 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256='760cea1f7a058be6000e14dfecfeb73cc79245f696f18e0fcf0825935b944ab3' ;; 		aarch64) arch='arm64'; KONG_SHA256='08038f49f162ab5edc357d7712e90241f6571027cb8741b15ba0c951653764c2' ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong; 	tar -C /kong -xzf /tmp/kong.tar.gz && 	mv /kong/usr/local/* /usr/local && 	mv /kong/etc/* /etc && 	rm -rf /kong && 	apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates && 	adduser -S kong && 	mkdir -p "/usr/local/kong" && 	chown -R kong:0 /usr/local/kong && 	chown kong:0 /usr/local/bin/kong && 	chmod -R g=u /usr/local/kong && 	rm -rf /tmp/kong.tar.gz &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Tue, 22 Sep 2020 18:32:37 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Tue, 22 Sep 2020 18:32:37 GMT
USER kong
# Tue, 22 Sep 2020 18:32:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 22 Sep 2020 18:32:38 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 22 Sep 2020 18:32:38 GMT
STOPSIGNAL SIGQUIT
# Tue, 22 Sep 2020 18:32:38 GMT
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
	-	`sha256:7306b16482a5463a3999b475a70c541b3eafcd2c4d3b6da8b5ae4d53bc49be14`  
		Last Modified: Tue, 22 Sep 2020 18:34:57 GMT  
		Size: 50.3 MB (50336253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff24278e47024f951b5e7834bbcb0a5ce4e0ea9086924d0a929eb960a35b3542`  
		Last Modified: Tue, 22 Sep 2020 18:34:47 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.1.4` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:f93512ee31e30463969b469e34cac78840d361853f716e26c323bdc9d98ee067
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.7 MB (52670238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43f3c5137a40d5709b4d2bc75c83f6fe8491414ca66007819c2f8ea9ebaea1e3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Tue, 22 Sep 2020 19:05:32 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 22 Sep 2020 19:05:34 GMT
ARG ASSET=ce
# Tue, 22 Sep 2020 19:05:35 GMT
ENV ASSET=ce
# Tue, 22 Sep 2020 19:05:36 GMT
ARG EE_PORTS
# Tue, 22 Sep 2020 19:05:36 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 22 Sep 2020 19:05:41 GMT
ARG KONG_VERSION=2.1.4
# Tue, 22 Sep 2020 19:05:48 GMT
ENV KONG_VERSION=2.1.4
# Tue, 22 Sep 2020 19:06:05 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256='760cea1f7a058be6000e14dfecfeb73cc79245f696f18e0fcf0825935b944ab3' ;; 		aarch64) arch='arm64'; KONG_SHA256='08038f49f162ab5edc357d7712e90241f6571027cb8741b15ba0c951653764c2' ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong; 	tar -C /kong -xzf /tmp/kong.tar.gz && 	mv /kong/usr/local/* /usr/local && 	mv /kong/etc/* /etc && 	rm -rf /kong && 	apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates && 	adduser -S kong && 	mkdir -p "/usr/local/kong" && 	chown -R kong:0 /usr/local/kong && 	chown kong:0 /usr/local/bin/kong && 	chmod -R g=u /usr/local/kong && 	rm -rf /tmp/kong.tar.gz &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Tue, 22 Sep 2020 19:06:08 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Tue, 22 Sep 2020 19:06:08 GMT
USER kong
# Tue, 22 Sep 2020 19:06:09 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 22 Sep 2020 19:06:10 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 22 Sep 2020 19:06:10 GMT
STOPSIGNAL SIGQUIT
# Tue, 22 Sep 2020 19:06:11 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f1f361b75deeea5140a58989e54db49d72c8f2794625392d9b60e5f6adea53`  
		Last Modified: Tue, 22 Sep 2020 19:08:54 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715b0084f83b0d2b1feb234f814f8223cfc5574fb6863e5cdc425ff3e3b468a8`  
		Last Modified: Tue, 22 Sep 2020 19:09:11 GMT  
		Size: 49.9 MB (49944947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73656217c4f0421f0b017bae8d6959f82fe85783971bd97d00e89643a56c8f45`  
		Last Modified: Tue, 22 Sep 2020 19:08:54 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.1.4-alpine`

```console
$ docker pull kong@sha256:3988a79c97f08d85e4c5cfbefc4085d52904ee87de95413865d4a59d1b944f3c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.1.4-alpine` - linux; amd64

```console
$ docker pull kong@sha256:32aec5d7a1152fad8604b74dfbfe544f8c346c42651791a768fd5f0025bc59b1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53150431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d55bcda861cae15b7310f14adc6b1f942f3d867ef30b6ff8da9268ac0ebd58a1`
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
# Tue, 22 Sep 2020 18:32:31 GMT
ARG KONG_VERSION=2.1.4
# Tue, 22 Sep 2020 18:32:31 GMT
ENV KONG_VERSION=2.1.4
# Tue, 22 Sep 2020 18:32:37 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256='760cea1f7a058be6000e14dfecfeb73cc79245f696f18e0fcf0825935b944ab3' ;; 		aarch64) arch='arm64'; KONG_SHA256='08038f49f162ab5edc357d7712e90241f6571027cb8741b15ba0c951653764c2' ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong; 	tar -C /kong -xzf /tmp/kong.tar.gz && 	mv /kong/usr/local/* /usr/local && 	mv /kong/etc/* /etc && 	rm -rf /kong && 	apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates && 	adduser -S kong && 	mkdir -p "/usr/local/kong" && 	chown -R kong:0 /usr/local/kong && 	chown kong:0 /usr/local/bin/kong && 	chmod -R g=u /usr/local/kong && 	rm -rf /tmp/kong.tar.gz &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Tue, 22 Sep 2020 18:32:37 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Tue, 22 Sep 2020 18:32:37 GMT
USER kong
# Tue, 22 Sep 2020 18:32:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 22 Sep 2020 18:32:38 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 22 Sep 2020 18:32:38 GMT
STOPSIGNAL SIGQUIT
# Tue, 22 Sep 2020 18:32:38 GMT
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
	-	`sha256:7306b16482a5463a3999b475a70c541b3eafcd2c4d3b6da8b5ae4d53bc49be14`  
		Last Modified: Tue, 22 Sep 2020 18:34:57 GMT  
		Size: 50.3 MB (50336253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff24278e47024f951b5e7834bbcb0a5ce4e0ea9086924d0a929eb960a35b3542`  
		Last Modified: Tue, 22 Sep 2020 18:34:47 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.1.4-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:f93512ee31e30463969b469e34cac78840d361853f716e26c323bdc9d98ee067
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.7 MB (52670238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43f3c5137a40d5709b4d2bc75c83f6fe8491414ca66007819c2f8ea9ebaea1e3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Tue, 22 Sep 2020 19:05:32 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 22 Sep 2020 19:05:34 GMT
ARG ASSET=ce
# Tue, 22 Sep 2020 19:05:35 GMT
ENV ASSET=ce
# Tue, 22 Sep 2020 19:05:36 GMT
ARG EE_PORTS
# Tue, 22 Sep 2020 19:05:36 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 22 Sep 2020 19:05:41 GMT
ARG KONG_VERSION=2.1.4
# Tue, 22 Sep 2020 19:05:48 GMT
ENV KONG_VERSION=2.1.4
# Tue, 22 Sep 2020 19:06:05 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256='760cea1f7a058be6000e14dfecfeb73cc79245f696f18e0fcf0825935b944ab3' ;; 		aarch64) arch='arm64'; KONG_SHA256='08038f49f162ab5edc357d7712e90241f6571027cb8741b15ba0c951653764c2' ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong; 	tar -C /kong -xzf /tmp/kong.tar.gz && 	mv /kong/usr/local/* /usr/local && 	mv /kong/etc/* /etc && 	rm -rf /kong && 	apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates && 	adduser -S kong && 	mkdir -p "/usr/local/kong" && 	chown -R kong:0 /usr/local/kong && 	chown kong:0 /usr/local/bin/kong && 	chmod -R g=u /usr/local/kong && 	rm -rf /tmp/kong.tar.gz &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Tue, 22 Sep 2020 19:06:08 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Tue, 22 Sep 2020 19:06:08 GMT
USER kong
# Tue, 22 Sep 2020 19:06:09 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 22 Sep 2020 19:06:10 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 22 Sep 2020 19:06:10 GMT
STOPSIGNAL SIGQUIT
# Tue, 22 Sep 2020 19:06:11 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f1f361b75deeea5140a58989e54db49d72c8f2794625392d9b60e5f6adea53`  
		Last Modified: Tue, 22 Sep 2020 19:08:54 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715b0084f83b0d2b1feb234f814f8223cfc5574fb6863e5cdc425ff3e3b468a8`  
		Last Modified: Tue, 22 Sep 2020 19:09:11 GMT  
		Size: 49.9 MB (49944947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73656217c4f0421f0b017bae8d6959f82fe85783971bd97d00e89643a56c8f45`  
		Last Modified: Tue, 22 Sep 2020 19:08:54 GMT  
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
$ docker pull kong@sha256:1f82afc2e03216551a4c83866d416b698d99c6937f73f3c8298f7296808d4a25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.1.4-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:601a2e393957d07f59b8084621c7cfefc4a2f1e737f5562254d01e738cf61445
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.7 MB (133744712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d8e0d7855f9f178b003da8acda232350a1f77ae055d06acc0ffc695943d1152`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 23 Oct 2020 17:33:08 GMT
ADD file:c1f3147c7b6710af5affd417ff822ee28df872d716003858d3d2e23d2277c981 in / 
# Fri, 23 Oct 2020 17:33:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:33:09 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 17:33:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:33:10 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 17:52:28 GMT
ARG ASSET=ce
# Fri, 23 Oct 2020 17:52:28 GMT
ENV ASSET=ce
# Fri, 23 Oct 2020 17:52:28 GMT
ARG EE_PORTS
# Fri, 23 Oct 2020 17:52:28 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Fri, 23 Oct 2020 17:52:29 GMT
ARG KONG_VERSION=2.1.4
# Fri, 23 Oct 2020 17:52:29 GMT
ENV KONG_VERSION=2.1.4
# Fri, 23 Oct 2020 17:53:12 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt update 	&& apt install --yes /tmp/kong.deb 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Fri, 23 Oct 2020 17:53:13 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Fri, 23 Oct 2020 17:53:13 GMT
USER kong
# Fri, 23 Oct 2020 17:53:13 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Oct 2020 17:53:13 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 23 Oct 2020 17:53:13 GMT
STOPSIGNAL SIGQUIT
# Fri, 23 Oct 2020 17:53:13 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:2c11b7cecaa5d3e2a57e290921ababbfb8572b549015168d4cbd91c340d2c566`  
		Last Modified: Wed, 14 Oct 2020 13:20:30 GMT  
		Size: 45.8 MB (45825714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04637fa562525a9366f00e8f4b08d04a347bded1ee513738451ef9d42b4dfc4e`  
		Last Modified: Fri, 23 Oct 2020 17:33:48 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e6af23a0f38c4a6511147d2a9dc06a07a7afa0669000cb62720c7eafe031ae`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a424de92ad71639c5cabadcdab0493e4067eb2f9cf109ffef40db178349238`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a810599aaaccac955e7c0b605e6b1bc745018863e6127cfb34cfc8189e03fa01`  
		Last Modified: Fri, 23 Oct 2020 17:54:16 GMT  
		Size: 25.1 MB (25081963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8a847b57fd03e933b4bc8d5e501404999f821027463c5c478692d21e737d8b`  
		Last Modified: Fri, 23 Oct 2020 17:54:25 GMT  
		Size: 62.8 MB (62834801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59d96fe1bab2a48c9581b9e83b4de6cdc51f70bfab785ccaa37fce17358c6452`  
		Last Modified: Fri, 23 Oct 2020 17:54:13 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.1.4-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:cea3d52343c5817ef48fe86d8506860079d2fe09f080c79c8c76b0c5b35e8099
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.1 MB (125140620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c97c5646bb862a7acb33f6358832cd42f80960ccfd2b39ff2004ae7175488b56`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 25 Nov 2020 22:44:18 GMT
ADD file:a360b1e1db1ae9973dac11dfe4e549f6416e278f53c42eb5e98b3b3da8d2a5ae in / 
# Wed, 25 Nov 2020 22:44:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:44:23 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 22:44:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:44:26 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:26:02 GMT
ARG ASSET=ce
# Wed, 25 Nov 2020 23:26:04 GMT
ENV ASSET=ce
# Wed, 25 Nov 2020 23:26:04 GMT
ARG EE_PORTS
# Wed, 25 Nov 2020 23:26:05 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 25 Nov 2020 23:27:25 GMT
ARG KONG_VERSION=2.1.4
# Wed, 25 Nov 2020 23:27:25 GMT
ENV KONG_VERSION=2.1.4
# Wed, 25 Nov 2020 23:28:14 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt update 	&& apt install --yes /tmp/kong.deb 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Wed, 25 Nov 2020 23:28:17 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Wed, 25 Nov 2020 23:28:18 GMT
USER kong
# Wed, 25 Nov 2020 23:28:19 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 25 Nov 2020 23:28:20 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 25 Nov 2020 23:28:20 GMT
STOPSIGNAL SIGQUIT
# Wed, 25 Nov 2020 23:28:22 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:3e30c5e4609ac16f9e19faa3800699e28c77aadcfcbde2ddd5954606f80fa170`  
		Last Modified: Sat, 31 Oct 2020 00:25:13 GMT  
		Size: 40.8 MB (40826105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be82da0c7e998c509a8e86338f139501b62fde0df3908dd489a8249380ea3441`  
		Last Modified: Wed, 25 Nov 2020 22:45:42 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf04dffef88e5257b2388d643e5fb03a812316de0737ce92e3888a6722cea5e`  
		Last Modified: Wed, 25 Nov 2020 22:45:43 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2624f7934929e6e67f81a9becb317179367648ec1236d644e9bf3a00d3fe3772`  
		Last Modified: Wed, 25 Nov 2020 22:45:43 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6cba0c8b4d5e1def090992b7d3bc001ae633fa3ad938efa00a15d89e40a72c`  
		Last Modified: Wed, 25 Nov 2020 23:29:55 GMT  
		Size: 25.1 MB (25081968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3a4efe36ab888c3f372905cb6757dd8b84ffd0ce5a6bcf62019fc83672032e`  
		Last Modified: Wed, 25 Nov 2020 23:30:38 GMT  
		Size: 59.2 MB (59230369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8be18280aa22e5454cd135b7e8c766283000ea67203fc0dc2c5bbcda44be23`  
		Last Modified: Wed, 25 Nov 2020 23:30:20 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.1-alpine`

```console
$ docker pull kong@sha256:3988a79c97f08d85e4c5cfbefc4085d52904ee87de95413865d4a59d1b944f3c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.1-alpine` - linux; amd64

```console
$ docker pull kong@sha256:32aec5d7a1152fad8604b74dfbfe544f8c346c42651791a768fd5f0025bc59b1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53150431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d55bcda861cae15b7310f14adc6b1f942f3d867ef30b6ff8da9268ac0ebd58a1`
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
# Tue, 22 Sep 2020 18:32:31 GMT
ARG KONG_VERSION=2.1.4
# Tue, 22 Sep 2020 18:32:31 GMT
ENV KONG_VERSION=2.1.4
# Tue, 22 Sep 2020 18:32:37 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256='760cea1f7a058be6000e14dfecfeb73cc79245f696f18e0fcf0825935b944ab3' ;; 		aarch64) arch='arm64'; KONG_SHA256='08038f49f162ab5edc357d7712e90241f6571027cb8741b15ba0c951653764c2' ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong; 	tar -C /kong -xzf /tmp/kong.tar.gz && 	mv /kong/usr/local/* /usr/local && 	mv /kong/etc/* /etc && 	rm -rf /kong && 	apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates && 	adduser -S kong && 	mkdir -p "/usr/local/kong" && 	chown -R kong:0 /usr/local/kong && 	chown kong:0 /usr/local/bin/kong && 	chmod -R g=u /usr/local/kong && 	rm -rf /tmp/kong.tar.gz &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Tue, 22 Sep 2020 18:32:37 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Tue, 22 Sep 2020 18:32:37 GMT
USER kong
# Tue, 22 Sep 2020 18:32:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 22 Sep 2020 18:32:38 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 22 Sep 2020 18:32:38 GMT
STOPSIGNAL SIGQUIT
# Tue, 22 Sep 2020 18:32:38 GMT
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
	-	`sha256:7306b16482a5463a3999b475a70c541b3eafcd2c4d3b6da8b5ae4d53bc49be14`  
		Last Modified: Tue, 22 Sep 2020 18:34:57 GMT  
		Size: 50.3 MB (50336253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff24278e47024f951b5e7834bbcb0a5ce4e0ea9086924d0a929eb960a35b3542`  
		Last Modified: Tue, 22 Sep 2020 18:34:47 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.1-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:f93512ee31e30463969b469e34cac78840d361853f716e26c323bdc9d98ee067
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.7 MB (52670238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43f3c5137a40d5709b4d2bc75c83f6fe8491414ca66007819c2f8ea9ebaea1e3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Tue, 22 Sep 2020 19:05:32 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 22 Sep 2020 19:05:34 GMT
ARG ASSET=ce
# Tue, 22 Sep 2020 19:05:35 GMT
ENV ASSET=ce
# Tue, 22 Sep 2020 19:05:36 GMT
ARG EE_PORTS
# Tue, 22 Sep 2020 19:05:36 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Tue, 22 Sep 2020 19:05:41 GMT
ARG KONG_VERSION=2.1.4
# Tue, 22 Sep 2020 19:05:48 GMT
ENV KONG_VERSION=2.1.4
# Tue, 22 Sep 2020 19:06:05 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256='760cea1f7a058be6000e14dfecfeb73cc79245f696f18e0fcf0825935b944ab3' ;; 		aarch64) arch='arm64'; KONG_SHA256='08038f49f162ab5edc357d7712e90241f6571027cb8741b15ba0c951653764c2' ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong; 	tar -C /kong -xzf /tmp/kong.tar.gz && 	mv /kong/usr/local/* /usr/local && 	mv /kong/etc/* /etc && 	rm -rf /kong && 	apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash zlib zlib-dev git ca-certificates && 	adduser -S kong && 	mkdir -p "/usr/local/kong" && 	chown -R kong:0 /usr/local/kong && 	chown kong:0 /usr/local/bin/kong && 	chmod -R g=u /usr/local/kong && 	rm -rf /tmp/kong.tar.gz &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Tue, 22 Sep 2020 19:06:08 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Tue, 22 Sep 2020 19:06:08 GMT
USER kong
# Tue, 22 Sep 2020 19:06:09 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 22 Sep 2020 19:06:10 GMT
EXPOSE 8000 8001 8443 8444
# Tue, 22 Sep 2020 19:06:10 GMT
STOPSIGNAL SIGQUIT
# Tue, 22 Sep 2020 19:06:11 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f1f361b75deeea5140a58989e54db49d72c8f2794625392d9b60e5f6adea53`  
		Last Modified: Tue, 22 Sep 2020 19:08:54 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715b0084f83b0d2b1feb234f814f8223cfc5574fb6863e5cdc425ff3e3b468a8`  
		Last Modified: Tue, 22 Sep 2020 19:09:11 GMT  
		Size: 49.9 MB (49944947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73656217c4f0421f0b017bae8d6959f82fe85783971bd97d00e89643a56c8f45`  
		Last Modified: Tue, 22 Sep 2020 19:08:54 GMT  
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
$ docker pull kong@sha256:1f82afc2e03216551a4c83866d416b698d99c6937f73f3c8298f7296808d4a25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.1-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:601a2e393957d07f59b8084621c7cfefc4a2f1e737f5562254d01e738cf61445
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.7 MB (133744712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d8e0d7855f9f178b003da8acda232350a1f77ae055d06acc0ffc695943d1152`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 23 Oct 2020 17:33:08 GMT
ADD file:c1f3147c7b6710af5affd417ff822ee28df872d716003858d3d2e23d2277c981 in / 
# Fri, 23 Oct 2020 17:33:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:33:09 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 17:33:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:33:10 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 17:52:28 GMT
ARG ASSET=ce
# Fri, 23 Oct 2020 17:52:28 GMT
ENV ASSET=ce
# Fri, 23 Oct 2020 17:52:28 GMT
ARG EE_PORTS
# Fri, 23 Oct 2020 17:52:28 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Fri, 23 Oct 2020 17:52:29 GMT
ARG KONG_VERSION=2.1.4
# Fri, 23 Oct 2020 17:52:29 GMT
ENV KONG_VERSION=2.1.4
# Fri, 23 Oct 2020 17:53:12 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt update 	&& apt install --yes /tmp/kong.deb 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Fri, 23 Oct 2020 17:53:13 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Fri, 23 Oct 2020 17:53:13 GMT
USER kong
# Fri, 23 Oct 2020 17:53:13 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Oct 2020 17:53:13 GMT
EXPOSE 8000 8001 8443 8444
# Fri, 23 Oct 2020 17:53:13 GMT
STOPSIGNAL SIGQUIT
# Fri, 23 Oct 2020 17:53:13 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:2c11b7cecaa5d3e2a57e290921ababbfb8572b549015168d4cbd91c340d2c566`  
		Last Modified: Wed, 14 Oct 2020 13:20:30 GMT  
		Size: 45.8 MB (45825714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04637fa562525a9366f00e8f4b08d04a347bded1ee513738451ef9d42b4dfc4e`  
		Last Modified: Fri, 23 Oct 2020 17:33:48 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e6af23a0f38c4a6511147d2a9dc06a07a7afa0669000cb62720c7eafe031ae`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a424de92ad71639c5cabadcdab0493e4067eb2f9cf109ffef40db178349238`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a810599aaaccac955e7c0b605e6b1bc745018863e6127cfb34cfc8189e03fa01`  
		Last Modified: Fri, 23 Oct 2020 17:54:16 GMT  
		Size: 25.1 MB (25081963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8a847b57fd03e933b4bc8d5e501404999f821027463c5c478692d21e737d8b`  
		Last Modified: Fri, 23 Oct 2020 17:54:25 GMT  
		Size: 62.8 MB (62834801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59d96fe1bab2a48c9581b9e83b4de6cdc51f70bfab785ccaa37fce17358c6452`  
		Last Modified: Fri, 23 Oct 2020 17:54:13 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.1-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:cea3d52343c5817ef48fe86d8506860079d2fe09f080c79c8c76b0c5b35e8099
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.1 MB (125140620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c97c5646bb862a7acb33f6358832cd42f80960ccfd2b39ff2004ae7175488b56`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 25 Nov 2020 22:44:18 GMT
ADD file:a360b1e1db1ae9973dac11dfe4e549f6416e278f53c42eb5e98b3b3da8d2a5ae in / 
# Wed, 25 Nov 2020 22:44:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:44:23 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 22:44:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:44:26 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:26:02 GMT
ARG ASSET=ce
# Wed, 25 Nov 2020 23:26:04 GMT
ENV ASSET=ce
# Wed, 25 Nov 2020 23:26:04 GMT
ARG EE_PORTS
# Wed, 25 Nov 2020 23:26:05 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 25 Nov 2020 23:27:25 GMT
ARG KONG_VERSION=2.1.4
# Wed, 25 Nov 2020 23:27:25 GMT
ENV KONG_VERSION=2.1.4
# Wed, 25 Nov 2020 23:28:14 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt update 	&& apt install --yes /tmp/kong.deb 	&& rm -rf /var/lib/apt/lists/* 	&& rm -rf /tmp/kong.deb 	&& useradd -ms /bin/bash kong     && mkdir -p "/usr/local/kong" 	&& chown -R kong:0 /usr/local/kong 	&& chown kong:0 /usr/local/bin/kong 	&& chmod -R g=u /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Wed, 25 Nov 2020 23:28:17 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Wed, 25 Nov 2020 23:28:18 GMT
USER kong
# Wed, 25 Nov 2020 23:28:19 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 25 Nov 2020 23:28:20 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 25 Nov 2020 23:28:20 GMT
STOPSIGNAL SIGQUIT
# Wed, 25 Nov 2020 23:28:22 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:3e30c5e4609ac16f9e19faa3800699e28c77aadcfcbde2ddd5954606f80fa170`  
		Last Modified: Sat, 31 Oct 2020 00:25:13 GMT  
		Size: 40.8 MB (40826105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be82da0c7e998c509a8e86338f139501b62fde0df3908dd489a8249380ea3441`  
		Last Modified: Wed, 25 Nov 2020 22:45:42 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf04dffef88e5257b2388d643e5fb03a812316de0737ce92e3888a6722cea5e`  
		Last Modified: Wed, 25 Nov 2020 22:45:43 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2624f7934929e6e67f81a9becb317179367648ec1236d644e9bf3a00d3fe3772`  
		Last Modified: Wed, 25 Nov 2020 22:45:43 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6cba0c8b4d5e1def090992b7d3bc001ae633fa3ad938efa00a15d89e40a72c`  
		Last Modified: Wed, 25 Nov 2020 23:29:55 GMT  
		Size: 25.1 MB (25081968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3a4efe36ab888c3f372905cb6757dd8b84ffd0ce5a6bcf62019fc83672032e`  
		Last Modified: Wed, 25 Nov 2020 23:30:38 GMT  
		Size: 59.2 MB (59230369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8be18280aa22e5454cd135b7e8c766283000ea67203fc0dc2c5bbcda44be23`  
		Last Modified: Wed, 25 Nov 2020 23:30:20 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.2`

```console
$ docker pull kong@sha256:8b141da0a8fa843e1b745720089448db0236eb9d88999f009c8bf1f20d52c033
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.2` - linux; amd64

```console
$ docker pull kong@sha256:19ee9b741cc0dec5276136131af486702441181180ce4a630dd55dfce6d17ded
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53143102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1550bbb81daedb5b1e1b32ff7cfebc601eb3f5e2fe0fc816b4da13e77fdfdbc9`
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
# Thu, 29 Oct 2020 18:21:14 GMT
ARG KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:21:14 GMT
ENV KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:21:21 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256='6adb706eab6cc535f2703bd8993a5d5259159cf8a630c3d3974973dbe6bbf5a6' ;; 		aarch64) arch='arm64'; KONG_SHA256='a93b1c015d86b5d8b4038f3fd73332bfef97fa1c768545f353af03f54cf97fb8' ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Thu, 29 Oct 2020 18:21:22 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 29 Oct 2020 18:21:22 GMT
USER kong
# Thu, 29 Oct 2020 18:21:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Oct 2020 18:21:22 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 29 Oct 2020 18:21:22 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Oct 2020 18:21:22 GMT
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
	-	`sha256:c25d97cc4039bd282d150d09da1590e01019a05e641c6f61495324fb35a0a6ea`  
		Last Modified: Thu, 29 Oct 2020 18:23:45 GMT  
		Size: 50.3 MB (50328923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98513f5777887ba304362c52a37f9686f876ad0af12cdb8b6e49d17de0a348a8`  
		Last Modified: Thu, 29 Oct 2020 18:23:36 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.2` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:0a0cad9b3779321b3c9a35ad077bf1e5645e291d7329e161183152692c5cb637
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.7 MB (52673538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d354929336a5e32ec6d0b868be426c01545ee0f07715f5d4f6574114013cb13`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Tue, 22 Sep 2020 19:05:32 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 22 Sep 2020 19:05:34 GMT
ARG ASSET=ce
# Tue, 22 Sep 2020 19:05:35 GMT
ENV ASSET=ce
# Tue, 22 Sep 2020 19:05:36 GMT
ARG EE_PORTS
# Tue, 22 Sep 2020 19:05:36 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 29 Oct 2020 18:42:33 GMT
ARG KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:42:33 GMT
ENV KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:42:46 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256='6adb706eab6cc535f2703bd8993a5d5259159cf8a630c3d3974973dbe6bbf5a6' ;; 		aarch64) arch='arm64'; KONG_SHA256='a93b1c015d86b5d8b4038f3fd73332bfef97fa1c768545f353af03f54cf97fb8' ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Thu, 29 Oct 2020 18:42:48 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 29 Oct 2020 18:42:48 GMT
USER kong
# Thu, 29 Oct 2020 18:42:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Oct 2020 18:42:49 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 29 Oct 2020 18:42:50 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Oct 2020 18:42:50 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f1f361b75deeea5140a58989e54db49d72c8f2794625392d9b60e5f6adea53`  
		Last Modified: Tue, 22 Sep 2020 19:08:54 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0562e5901c7c1412846095fddf0527b3aec71f8d310829523e905e5dec70db4a`  
		Last Modified: Thu, 29 Oct 2020 18:51:28 GMT  
		Size: 49.9 MB (49948248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b00d686849acde734efe3f6499685d14b6e6deea6307aa2194f32f58e7a026`  
		Last Modified: Thu, 29 Oct 2020 18:51:13 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.2.0`

```console
$ docker pull kong@sha256:8b141da0a8fa843e1b745720089448db0236eb9d88999f009c8bf1f20d52c033
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.2.0` - linux; amd64

```console
$ docker pull kong@sha256:19ee9b741cc0dec5276136131af486702441181180ce4a630dd55dfce6d17ded
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53143102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1550bbb81daedb5b1e1b32ff7cfebc601eb3f5e2fe0fc816b4da13e77fdfdbc9`
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
# Thu, 29 Oct 2020 18:21:14 GMT
ARG KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:21:14 GMT
ENV KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:21:21 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256='6adb706eab6cc535f2703bd8993a5d5259159cf8a630c3d3974973dbe6bbf5a6' ;; 		aarch64) arch='arm64'; KONG_SHA256='a93b1c015d86b5d8b4038f3fd73332bfef97fa1c768545f353af03f54cf97fb8' ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Thu, 29 Oct 2020 18:21:22 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 29 Oct 2020 18:21:22 GMT
USER kong
# Thu, 29 Oct 2020 18:21:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Oct 2020 18:21:22 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 29 Oct 2020 18:21:22 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Oct 2020 18:21:22 GMT
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
	-	`sha256:c25d97cc4039bd282d150d09da1590e01019a05e641c6f61495324fb35a0a6ea`  
		Last Modified: Thu, 29 Oct 2020 18:23:45 GMT  
		Size: 50.3 MB (50328923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98513f5777887ba304362c52a37f9686f876ad0af12cdb8b6e49d17de0a348a8`  
		Last Modified: Thu, 29 Oct 2020 18:23:36 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.2.0` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:0a0cad9b3779321b3c9a35ad077bf1e5645e291d7329e161183152692c5cb637
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.7 MB (52673538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d354929336a5e32ec6d0b868be426c01545ee0f07715f5d4f6574114013cb13`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Tue, 22 Sep 2020 19:05:32 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 22 Sep 2020 19:05:34 GMT
ARG ASSET=ce
# Tue, 22 Sep 2020 19:05:35 GMT
ENV ASSET=ce
# Tue, 22 Sep 2020 19:05:36 GMT
ARG EE_PORTS
# Tue, 22 Sep 2020 19:05:36 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 29 Oct 2020 18:42:33 GMT
ARG KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:42:33 GMT
ENV KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:42:46 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256='6adb706eab6cc535f2703bd8993a5d5259159cf8a630c3d3974973dbe6bbf5a6' ;; 		aarch64) arch='arm64'; KONG_SHA256='a93b1c015d86b5d8b4038f3fd73332bfef97fa1c768545f353af03f54cf97fb8' ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Thu, 29 Oct 2020 18:42:48 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 29 Oct 2020 18:42:48 GMT
USER kong
# Thu, 29 Oct 2020 18:42:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Oct 2020 18:42:49 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 29 Oct 2020 18:42:50 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Oct 2020 18:42:50 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f1f361b75deeea5140a58989e54db49d72c8f2794625392d9b60e5f6adea53`  
		Last Modified: Tue, 22 Sep 2020 19:08:54 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0562e5901c7c1412846095fddf0527b3aec71f8d310829523e905e5dec70db4a`  
		Last Modified: Thu, 29 Oct 2020 18:51:28 GMT  
		Size: 49.9 MB (49948248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b00d686849acde734efe3f6499685d14b6e6deea6307aa2194f32f58e7a026`  
		Last Modified: Thu, 29 Oct 2020 18:51:13 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.2.0-alpine`

```console
$ docker pull kong@sha256:8b141da0a8fa843e1b745720089448db0236eb9d88999f009c8bf1f20d52c033
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.2.0-alpine` - linux; amd64

```console
$ docker pull kong@sha256:19ee9b741cc0dec5276136131af486702441181180ce4a630dd55dfce6d17ded
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53143102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1550bbb81daedb5b1e1b32ff7cfebc601eb3f5e2fe0fc816b4da13e77fdfdbc9`
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
# Thu, 29 Oct 2020 18:21:14 GMT
ARG KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:21:14 GMT
ENV KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:21:21 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256='6adb706eab6cc535f2703bd8993a5d5259159cf8a630c3d3974973dbe6bbf5a6' ;; 		aarch64) arch='arm64'; KONG_SHA256='a93b1c015d86b5d8b4038f3fd73332bfef97fa1c768545f353af03f54cf97fb8' ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Thu, 29 Oct 2020 18:21:22 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 29 Oct 2020 18:21:22 GMT
USER kong
# Thu, 29 Oct 2020 18:21:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Oct 2020 18:21:22 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 29 Oct 2020 18:21:22 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Oct 2020 18:21:22 GMT
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
	-	`sha256:c25d97cc4039bd282d150d09da1590e01019a05e641c6f61495324fb35a0a6ea`  
		Last Modified: Thu, 29 Oct 2020 18:23:45 GMT  
		Size: 50.3 MB (50328923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98513f5777887ba304362c52a37f9686f876ad0af12cdb8b6e49d17de0a348a8`  
		Last Modified: Thu, 29 Oct 2020 18:23:36 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.2.0-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:0a0cad9b3779321b3c9a35ad077bf1e5645e291d7329e161183152692c5cb637
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.7 MB (52673538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d354929336a5e32ec6d0b868be426c01545ee0f07715f5d4f6574114013cb13`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Tue, 22 Sep 2020 19:05:32 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 22 Sep 2020 19:05:34 GMT
ARG ASSET=ce
# Tue, 22 Sep 2020 19:05:35 GMT
ENV ASSET=ce
# Tue, 22 Sep 2020 19:05:36 GMT
ARG EE_PORTS
# Tue, 22 Sep 2020 19:05:36 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 29 Oct 2020 18:42:33 GMT
ARG KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:42:33 GMT
ENV KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:42:46 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256='6adb706eab6cc535f2703bd8993a5d5259159cf8a630c3d3974973dbe6bbf5a6' ;; 		aarch64) arch='arm64'; KONG_SHA256='a93b1c015d86b5d8b4038f3fd73332bfef97fa1c768545f353af03f54cf97fb8' ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Thu, 29 Oct 2020 18:42:48 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 29 Oct 2020 18:42:48 GMT
USER kong
# Thu, 29 Oct 2020 18:42:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Oct 2020 18:42:49 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 29 Oct 2020 18:42:50 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Oct 2020 18:42:50 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f1f361b75deeea5140a58989e54db49d72c8f2794625392d9b60e5f6adea53`  
		Last Modified: Tue, 22 Sep 2020 19:08:54 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0562e5901c7c1412846095fddf0527b3aec71f8d310829523e905e5dec70db4a`  
		Last Modified: Thu, 29 Oct 2020 18:51:28 GMT  
		Size: 49.9 MB (49948248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b00d686849acde734efe3f6499685d14b6e6deea6307aa2194f32f58e7a026`  
		Last Modified: Thu, 29 Oct 2020 18:51:13 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.2.0-centos`

```console
$ docker pull kong@sha256:b01587ced574fac8ee1c71ea54020e1c655e81ec361df74fcc7fe9b20933b097
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.2.0-centos` - linux; amd64

```console
$ docker pull kong@sha256:8e4ae834e2dd20844702ddbb9afc47970e1357e213eb0989690e46f178d62f26
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127355535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d266fdf93b29972e9458257e31fc7b14099d9acd49d1bd9a38e5a46a7e292c30`
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
# Sat, 14 Nov 2020 01:01:34 GMT
ARG KONG_VERSION=2.2.0
# Sat, 14 Nov 2020 01:01:34 GMT
ENV KONG_VERSION=2.2.0
# Sat, 14 Nov 2020 01:01:35 GMT
ARG KONG_SHA256=17f8a8f5084c7ff0b5807f0a161d900d08f410e4e6fa2c40d469c01604371557
# Sat, 14 Nov 2020 01:02:02 GMT
# ARGS: KONG_SHA256=17f8a8f5084c7ff0b5807f0a161d900d08f410e4e6fa2c40d469c01604371557
RUN set -ex;   if [ "$ASSET" = "ce" ] ; then     curl -fL "https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm" -o /tmp/kong.rpm     && echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -;   fi;   yum install -y -q unzip shadow-utils git   && yum clean all -q   && rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki   && { useradd kong || true ;}   && mkdir -p "/usr/local/kong"   && yum install -y /tmp/kong.rpm   && yum clean all   && rm /tmp/kong.rpm   && chown -R kong:0 /usr/local/kong   && chown kong:0 /usr/local/bin/kong   && chmod -R g=u /usr/local/kong &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Sat, 14 Nov 2020 01:02:02 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Sat, 14 Nov 2020 01:02:02 GMT
USER kong
# Sat, 14 Nov 2020 01:02:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 14 Nov 2020 01:02:03 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 14 Nov 2020 01:02:03 GMT
STOPSIGNAL SIGQUIT
# Sat, 14 Nov 2020 01:02:03 GMT
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
	-	`sha256:ab274f6dcbc712af64284828ae4bd4fb38972b9064904a721ec8c13480d15743`  
		Last Modified: Sat, 14 Nov 2020 01:03:53 GMT  
		Size: 51.3 MB (51257515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200a2ab328b94246c9e69f7992dafaa50c90e843e512020bde09d63203eed165`  
		Last Modified: Sat, 14 Nov 2020 01:03:42 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.2.0-ubuntu`

```console
$ docker pull kong@sha256:d3dac9be891a6c211acaba75097b9f6e8a4e0485fc466cabbe13573e482362ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.2.0-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:056ffd524e8849b89f710a671b10841e337a5734a372fa428e89826f2eaa54f6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135598240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c048ac8311203db66211353c0d2ff83bd3696b6f3f3637b35a3b77859a1d1549`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 23 Oct 2020 17:33:08 GMT
ADD file:c1f3147c7b6710af5affd417ff822ee28df872d716003858d3d2e23d2277c981 in / 
# Fri, 23 Oct 2020 17:33:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:33:09 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 17:33:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:33:10 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 17:52:28 GMT
ARG ASSET=ce
# Fri, 23 Oct 2020 17:52:28 GMT
ENV ASSET=ce
# Fri, 23 Oct 2020 17:52:28 GMT
ARG EE_PORTS
# Fri, 23 Oct 2020 17:52:28 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Thu, 29 Oct 2020 18:21:27 GMT
ARG KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:21:27 GMT
ENV KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:22:16 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt update     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && { useradd -ms /bin/bash kong || true ;}     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Thu, 29 Oct 2020 18:22:17 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Thu, 29 Oct 2020 18:22:17 GMT
USER kong
# Thu, 29 Oct 2020 18:22:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Oct 2020 18:22:17 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 29 Oct 2020 18:22:17 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Oct 2020 18:22:17 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:2c11b7cecaa5d3e2a57e290921ababbfb8572b549015168d4cbd91c340d2c566`  
		Last Modified: Wed, 14 Oct 2020 13:20:30 GMT  
		Size: 45.8 MB (45825714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04637fa562525a9366f00e8f4b08d04a347bded1ee513738451ef9d42b4dfc4e`  
		Last Modified: Fri, 23 Oct 2020 17:33:48 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e6af23a0f38c4a6511147d2a9dc06a07a7afa0669000cb62720c7eafe031ae`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a424de92ad71639c5cabadcdab0493e4067eb2f9cf109ffef40db178349238`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a810599aaaccac955e7c0b605e6b1bc745018863e6127cfb34cfc8189e03fa01`  
		Last Modified: Fri, 23 Oct 2020 17:54:16 GMT  
		Size: 25.1 MB (25081963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab89deb52ede76e668a6e5adf0b8f3373863c9d0dcaee49ba0928857ff72a0ae`  
		Last Modified: Thu, 29 Oct 2020 18:24:05 GMT  
		Size: 64.7 MB (64688329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbe067f92ac3cc8db17ae04fd765d1765205b10aee77351f9773f33d935ed40`  
		Last Modified: Thu, 29 Oct 2020 18:23:53 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.2.0-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:30803b0c1e4013c034a1c48c590fb417dcabbedc1ea6923bada942b0ef5bced6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125254699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03d113d93337f8b22b5385c8b45adcc5024b06b83a3f5198116a9a75e730054f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 25 Nov 2020 22:44:18 GMT
ADD file:a360b1e1db1ae9973dac11dfe4e549f6416e278f53c42eb5e98b3b3da8d2a5ae in / 
# Wed, 25 Nov 2020 22:44:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:44:23 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 22:44:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:44:26 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:26:02 GMT
ARG ASSET=ce
# Wed, 25 Nov 2020 23:26:04 GMT
ENV ASSET=ce
# Wed, 25 Nov 2020 23:26:04 GMT
ARG EE_PORTS
# Wed, 25 Nov 2020 23:26:05 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 25 Nov 2020 23:26:06 GMT
ARG KONG_VERSION=2.2.0
# Wed, 25 Nov 2020 23:26:07 GMT
ENV KONG_VERSION=2.2.0
# Wed, 25 Nov 2020 23:26:55 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt update     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && { useradd -ms /bin/bash kong || true ;}     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Wed, 25 Nov 2020 23:26:57 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Wed, 25 Nov 2020 23:26:58 GMT
USER kong
# Wed, 25 Nov 2020 23:27:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 25 Nov 2020 23:27:02 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 25 Nov 2020 23:27:02 GMT
STOPSIGNAL SIGQUIT
# Wed, 25 Nov 2020 23:27:03 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:3e30c5e4609ac16f9e19faa3800699e28c77aadcfcbde2ddd5954606f80fa170`  
		Last Modified: Sat, 31 Oct 2020 00:25:13 GMT  
		Size: 40.8 MB (40826105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be82da0c7e998c509a8e86338f139501b62fde0df3908dd489a8249380ea3441`  
		Last Modified: Wed, 25 Nov 2020 22:45:42 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf04dffef88e5257b2388d643e5fb03a812316de0737ce92e3888a6722cea5e`  
		Last Modified: Wed, 25 Nov 2020 22:45:43 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2624f7934929e6e67f81a9becb317179367648ec1236d644e9bf3a00d3fe3772`  
		Last Modified: Wed, 25 Nov 2020 22:45:43 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6cba0c8b4d5e1def090992b7d3bc001ae633fa3ad938efa00a15d89e40a72c`  
		Last Modified: Wed, 25 Nov 2020 23:29:55 GMT  
		Size: 25.1 MB (25081968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b8573e52de26f1031729ff4851c3078a0bc20949b09fa5e3dcfb7e805fbf74`  
		Last Modified: Wed, 25 Nov 2020 23:30:09 GMT  
		Size: 59.3 MB (59344448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407742a2e372871244d9b6638b826e92677372d7e4b9f50ec8322ed91223c3bd`  
		Last Modified: Wed, 25 Nov 2020 23:29:52 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.2-alpine`

```console
$ docker pull kong@sha256:8b141da0a8fa843e1b745720089448db0236eb9d88999f009c8bf1f20d52c033
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.2-alpine` - linux; amd64

```console
$ docker pull kong@sha256:19ee9b741cc0dec5276136131af486702441181180ce4a630dd55dfce6d17ded
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53143102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1550bbb81daedb5b1e1b32ff7cfebc601eb3f5e2fe0fc816b4da13e77fdfdbc9`
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
# Thu, 29 Oct 2020 18:21:14 GMT
ARG KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:21:14 GMT
ENV KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:21:21 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256='6adb706eab6cc535f2703bd8993a5d5259159cf8a630c3d3974973dbe6bbf5a6' ;; 		aarch64) arch='arm64'; KONG_SHA256='a93b1c015d86b5d8b4038f3fd73332bfef97fa1c768545f353af03f54cf97fb8' ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Thu, 29 Oct 2020 18:21:22 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 29 Oct 2020 18:21:22 GMT
USER kong
# Thu, 29 Oct 2020 18:21:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Oct 2020 18:21:22 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 29 Oct 2020 18:21:22 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Oct 2020 18:21:22 GMT
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
	-	`sha256:c25d97cc4039bd282d150d09da1590e01019a05e641c6f61495324fb35a0a6ea`  
		Last Modified: Thu, 29 Oct 2020 18:23:45 GMT  
		Size: 50.3 MB (50328923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98513f5777887ba304362c52a37f9686f876ad0af12cdb8b6e49d17de0a348a8`  
		Last Modified: Thu, 29 Oct 2020 18:23:36 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.2-alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:0a0cad9b3779321b3c9a35ad077bf1e5645e291d7329e161183152692c5cb637
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.7 MB (52673538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d354929336a5e32ec6d0b868be426c01545ee0f07715f5d4f6574114013cb13`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Tue, 22 Sep 2020 19:05:32 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 22 Sep 2020 19:05:34 GMT
ARG ASSET=ce
# Tue, 22 Sep 2020 19:05:35 GMT
ENV ASSET=ce
# Tue, 22 Sep 2020 19:05:36 GMT
ARG EE_PORTS
# Tue, 22 Sep 2020 19:05:36 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 29 Oct 2020 18:42:33 GMT
ARG KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:42:33 GMT
ENV KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:42:46 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256='6adb706eab6cc535f2703bd8993a5d5259159cf8a630c3d3974973dbe6bbf5a6' ;; 		aarch64) arch='arm64'; KONG_SHA256='a93b1c015d86b5d8b4038f3fd73332bfef97fa1c768545f353af03f54cf97fb8' ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Thu, 29 Oct 2020 18:42:48 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 29 Oct 2020 18:42:48 GMT
USER kong
# Thu, 29 Oct 2020 18:42:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Oct 2020 18:42:49 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 29 Oct 2020 18:42:50 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Oct 2020 18:42:50 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f1f361b75deeea5140a58989e54db49d72c8f2794625392d9b60e5f6adea53`  
		Last Modified: Tue, 22 Sep 2020 19:08:54 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0562e5901c7c1412846095fddf0527b3aec71f8d310829523e905e5dec70db4a`  
		Last Modified: Thu, 29 Oct 2020 18:51:28 GMT  
		Size: 49.9 MB (49948248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b00d686849acde734efe3f6499685d14b6e6deea6307aa2194f32f58e7a026`  
		Last Modified: Thu, 29 Oct 2020 18:51:13 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.2-centos`

```console
$ docker pull kong@sha256:b01587ced574fac8ee1c71ea54020e1c655e81ec361df74fcc7fe9b20933b097
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:2.2-centos` - linux; amd64

```console
$ docker pull kong@sha256:8e4ae834e2dd20844702ddbb9afc47970e1357e213eb0989690e46f178d62f26
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127355535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d266fdf93b29972e9458257e31fc7b14099d9acd49d1bd9a38e5a46a7e292c30`
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
# Sat, 14 Nov 2020 01:01:34 GMT
ARG KONG_VERSION=2.2.0
# Sat, 14 Nov 2020 01:01:34 GMT
ENV KONG_VERSION=2.2.0
# Sat, 14 Nov 2020 01:01:35 GMT
ARG KONG_SHA256=17f8a8f5084c7ff0b5807f0a161d900d08f410e4e6fa2c40d469c01604371557
# Sat, 14 Nov 2020 01:02:02 GMT
# ARGS: KONG_SHA256=17f8a8f5084c7ff0b5807f0a161d900d08f410e4e6fa2c40d469c01604371557
RUN set -ex;   if [ "$ASSET" = "ce" ] ; then     curl -fL "https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm" -o /tmp/kong.rpm     && echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -;   fi;   yum install -y -q unzip shadow-utils git   && yum clean all -q   && rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki   && { useradd kong || true ;}   && mkdir -p "/usr/local/kong"   && yum install -y /tmp/kong.rpm   && yum clean all   && rm /tmp/kong.rpm   && chown -R kong:0 /usr/local/kong   && chown kong:0 /usr/local/bin/kong   && chmod -R g=u /usr/local/kong &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Sat, 14 Nov 2020 01:02:02 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Sat, 14 Nov 2020 01:02:02 GMT
USER kong
# Sat, 14 Nov 2020 01:02:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 14 Nov 2020 01:02:03 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 14 Nov 2020 01:02:03 GMT
STOPSIGNAL SIGQUIT
# Sat, 14 Nov 2020 01:02:03 GMT
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
	-	`sha256:ab274f6dcbc712af64284828ae4bd4fb38972b9064904a721ec8c13480d15743`  
		Last Modified: Sat, 14 Nov 2020 01:03:53 GMT  
		Size: 51.3 MB (51257515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200a2ab328b94246c9e69f7992dafaa50c90e843e512020bde09d63203eed165`  
		Last Modified: Sat, 14 Nov 2020 01:03:42 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:2.2-ubuntu`

```console
$ docker pull kong@sha256:d3dac9be891a6c211acaba75097b9f6e8a4e0485fc466cabbe13573e482362ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:2.2-ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:056ffd524e8849b89f710a671b10841e337a5734a372fa428e89826f2eaa54f6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135598240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c048ac8311203db66211353c0d2ff83bd3696b6f3f3637b35a3b77859a1d1549`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 23 Oct 2020 17:33:08 GMT
ADD file:c1f3147c7b6710af5affd417ff822ee28df872d716003858d3d2e23d2277c981 in / 
# Fri, 23 Oct 2020 17:33:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:33:09 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 17:33:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:33:10 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 17:52:28 GMT
ARG ASSET=ce
# Fri, 23 Oct 2020 17:52:28 GMT
ENV ASSET=ce
# Fri, 23 Oct 2020 17:52:28 GMT
ARG EE_PORTS
# Fri, 23 Oct 2020 17:52:28 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Thu, 29 Oct 2020 18:21:27 GMT
ARG KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:21:27 GMT
ENV KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:22:16 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt update     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && { useradd -ms /bin/bash kong || true ;}     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Thu, 29 Oct 2020 18:22:17 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Thu, 29 Oct 2020 18:22:17 GMT
USER kong
# Thu, 29 Oct 2020 18:22:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Oct 2020 18:22:17 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 29 Oct 2020 18:22:17 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Oct 2020 18:22:17 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:2c11b7cecaa5d3e2a57e290921ababbfb8572b549015168d4cbd91c340d2c566`  
		Last Modified: Wed, 14 Oct 2020 13:20:30 GMT  
		Size: 45.8 MB (45825714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04637fa562525a9366f00e8f4b08d04a347bded1ee513738451ef9d42b4dfc4e`  
		Last Modified: Fri, 23 Oct 2020 17:33:48 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e6af23a0f38c4a6511147d2a9dc06a07a7afa0669000cb62720c7eafe031ae`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a424de92ad71639c5cabadcdab0493e4067eb2f9cf109ffef40db178349238`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a810599aaaccac955e7c0b605e6b1bc745018863e6127cfb34cfc8189e03fa01`  
		Last Modified: Fri, 23 Oct 2020 17:54:16 GMT  
		Size: 25.1 MB (25081963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab89deb52ede76e668a6e5adf0b8f3373863c9d0dcaee49ba0928857ff72a0ae`  
		Last Modified: Thu, 29 Oct 2020 18:24:05 GMT  
		Size: 64.7 MB (64688329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbe067f92ac3cc8db17ae04fd765d1765205b10aee77351f9773f33d935ed40`  
		Last Modified: Thu, 29 Oct 2020 18:23:53 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:2.2-ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:30803b0c1e4013c034a1c48c590fb417dcabbedc1ea6923bada942b0ef5bced6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125254699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03d113d93337f8b22b5385c8b45adcc5024b06b83a3f5198116a9a75e730054f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 25 Nov 2020 22:44:18 GMT
ADD file:a360b1e1db1ae9973dac11dfe4e549f6416e278f53c42eb5e98b3b3da8d2a5ae in / 
# Wed, 25 Nov 2020 22:44:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:44:23 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 22:44:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:44:26 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:26:02 GMT
ARG ASSET=ce
# Wed, 25 Nov 2020 23:26:04 GMT
ENV ASSET=ce
# Wed, 25 Nov 2020 23:26:04 GMT
ARG EE_PORTS
# Wed, 25 Nov 2020 23:26:05 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 25 Nov 2020 23:26:06 GMT
ARG KONG_VERSION=2.2.0
# Wed, 25 Nov 2020 23:26:07 GMT
ENV KONG_VERSION=2.2.0
# Wed, 25 Nov 2020 23:26:55 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt update     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && { useradd -ms /bin/bash kong || true ;}     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Wed, 25 Nov 2020 23:26:57 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Wed, 25 Nov 2020 23:26:58 GMT
USER kong
# Wed, 25 Nov 2020 23:27:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 25 Nov 2020 23:27:02 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 25 Nov 2020 23:27:02 GMT
STOPSIGNAL SIGQUIT
# Wed, 25 Nov 2020 23:27:03 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:3e30c5e4609ac16f9e19faa3800699e28c77aadcfcbde2ddd5954606f80fa170`  
		Last Modified: Sat, 31 Oct 2020 00:25:13 GMT  
		Size: 40.8 MB (40826105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be82da0c7e998c509a8e86338f139501b62fde0df3908dd489a8249380ea3441`  
		Last Modified: Wed, 25 Nov 2020 22:45:42 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf04dffef88e5257b2388d643e5fb03a812316de0737ce92e3888a6722cea5e`  
		Last Modified: Wed, 25 Nov 2020 22:45:43 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2624f7934929e6e67f81a9becb317179367648ec1236d644e9bf3a00d3fe3772`  
		Last Modified: Wed, 25 Nov 2020 22:45:43 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6cba0c8b4d5e1def090992b7d3bc001ae633fa3ad938efa00a15d89e40a72c`  
		Last Modified: Wed, 25 Nov 2020 23:29:55 GMT  
		Size: 25.1 MB (25081968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b8573e52de26f1031729ff4851c3078a0bc20949b09fa5e3dcfb7e805fbf74`  
		Last Modified: Wed, 25 Nov 2020 23:30:09 GMT  
		Size: 59.3 MB (59344448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407742a2e372871244d9b6638b826e92677372d7e4b9f50ec8322ed91223c3bd`  
		Last Modified: Wed, 25 Nov 2020 23:29:52 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:alpine`

```console
$ docker pull kong@sha256:8b141da0a8fa843e1b745720089448db0236eb9d88999f009c8bf1f20d52c033
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:alpine` - linux; amd64

```console
$ docker pull kong@sha256:19ee9b741cc0dec5276136131af486702441181180ce4a630dd55dfce6d17ded
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53143102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1550bbb81daedb5b1e1b32ff7cfebc601eb3f5e2fe0fc816b4da13e77fdfdbc9`
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
# Thu, 29 Oct 2020 18:21:14 GMT
ARG KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:21:14 GMT
ENV KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:21:21 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256='6adb706eab6cc535f2703bd8993a5d5259159cf8a630c3d3974973dbe6bbf5a6' ;; 		aarch64) arch='arm64'; KONG_SHA256='a93b1c015d86b5d8b4038f3fd73332bfef97fa1c768545f353af03f54cf97fb8' ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Thu, 29 Oct 2020 18:21:22 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 29 Oct 2020 18:21:22 GMT
USER kong
# Thu, 29 Oct 2020 18:21:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Oct 2020 18:21:22 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 29 Oct 2020 18:21:22 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Oct 2020 18:21:22 GMT
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
	-	`sha256:c25d97cc4039bd282d150d09da1590e01019a05e641c6f61495324fb35a0a6ea`  
		Last Modified: Thu, 29 Oct 2020 18:23:45 GMT  
		Size: 50.3 MB (50328923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98513f5777887ba304362c52a37f9686f876ad0af12cdb8b6e49d17de0a348a8`  
		Last Modified: Thu, 29 Oct 2020 18:23:36 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:alpine` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:0a0cad9b3779321b3c9a35ad077bf1e5645e291d7329e161183152692c5cb637
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.7 MB (52673538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d354929336a5e32ec6d0b868be426c01545ee0f07715f5d4f6574114013cb13`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Tue, 22 Sep 2020 19:05:32 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 22 Sep 2020 19:05:34 GMT
ARG ASSET=ce
# Tue, 22 Sep 2020 19:05:35 GMT
ENV ASSET=ce
# Tue, 22 Sep 2020 19:05:36 GMT
ARG EE_PORTS
# Tue, 22 Sep 2020 19:05:36 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 29 Oct 2020 18:42:33 GMT
ARG KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:42:33 GMT
ENV KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:42:46 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256='6adb706eab6cc535f2703bd8993a5d5259159cf8a630c3d3974973dbe6bbf5a6' ;; 		aarch64) arch='arm64'; KONG_SHA256='a93b1c015d86b5d8b4038f3fd73332bfef97fa1c768545f353af03f54cf97fb8' ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Thu, 29 Oct 2020 18:42:48 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 29 Oct 2020 18:42:48 GMT
USER kong
# Thu, 29 Oct 2020 18:42:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Oct 2020 18:42:49 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 29 Oct 2020 18:42:50 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Oct 2020 18:42:50 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f1f361b75deeea5140a58989e54db49d72c8f2794625392d9b60e5f6adea53`  
		Last Modified: Tue, 22 Sep 2020 19:08:54 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0562e5901c7c1412846095fddf0527b3aec71f8d310829523e905e5dec70db4a`  
		Last Modified: Thu, 29 Oct 2020 18:51:28 GMT  
		Size: 49.9 MB (49948248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b00d686849acde734efe3f6499685d14b6e6deea6307aa2194f32f58e7a026`  
		Last Modified: Thu, 29 Oct 2020 18:51:13 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:centos`

```console
$ docker pull kong@sha256:b01587ced574fac8ee1c71ea54020e1c655e81ec361df74fcc7fe9b20933b097
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `kong:centos` - linux; amd64

```console
$ docker pull kong@sha256:8e4ae834e2dd20844702ddbb9afc47970e1357e213eb0989690e46f178d62f26
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127355535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d266fdf93b29972e9458257e31fc7b14099d9acd49d1bd9a38e5a46a7e292c30`
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
# Sat, 14 Nov 2020 01:01:34 GMT
ARG KONG_VERSION=2.2.0
# Sat, 14 Nov 2020 01:01:34 GMT
ENV KONG_VERSION=2.2.0
# Sat, 14 Nov 2020 01:01:35 GMT
ARG KONG_SHA256=17f8a8f5084c7ff0b5807f0a161d900d08f410e4e6fa2c40d469c01604371557
# Sat, 14 Nov 2020 01:02:02 GMT
# ARGS: KONG_SHA256=17f8a8f5084c7ff0b5807f0a161d900d08f410e4e6fa2c40d469c01604371557
RUN set -ex;   if [ "$ASSET" = "ce" ] ; then     curl -fL "https://bintray.com/kong/kong-rpm/download_file?file_path=centos/7/kong-$KONG_VERSION.el7.amd64.rpm" -o /tmp/kong.rpm     && echo "$KONG_SHA256  /tmp/kong.rpm" | sha256sum -c -;   fi;   yum install -y -q unzip shadow-utils git   && yum clean all -q   && rm -fr /var/cache/yum/* /tmp/yum_save*.yumtx /root/.pki   && { useradd kong || true ;}   && mkdir -p "/usr/local/kong"   && yum install -y /tmp/kong.rpm   && yum clean all   && rm /tmp/kong.rpm   && chown -R kong:0 /usr/local/kong   && chown kong:0 /usr/local/bin/kong   && chmod -R g=u /usr/local/kong &&   if [ "$ASSET" = "ce" ] ; then     kong version ;   fi;
# Sat, 14 Nov 2020 01:02:02 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Sat, 14 Nov 2020 01:02:02 GMT
USER kong
# Sat, 14 Nov 2020 01:02:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 14 Nov 2020 01:02:03 GMT
EXPOSE 8000 8001 8443 8444
# Sat, 14 Nov 2020 01:02:03 GMT
STOPSIGNAL SIGQUIT
# Sat, 14 Nov 2020 01:02:03 GMT
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
	-	`sha256:ab274f6dcbc712af64284828ae4bd4fb38972b9064904a721ec8c13480d15743`  
		Last Modified: Sat, 14 Nov 2020 01:03:53 GMT  
		Size: 51.3 MB (51257515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200a2ab328b94246c9e69f7992dafaa50c90e843e512020bde09d63203eed165`  
		Last Modified: Sat, 14 Nov 2020 01:03:42 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:latest`

```console
$ docker pull kong@sha256:8b141da0a8fa843e1b745720089448db0236eb9d88999f009c8bf1f20d52c033
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:latest` - linux; amd64

```console
$ docker pull kong@sha256:19ee9b741cc0dec5276136131af486702441181180ce4a630dd55dfce6d17ded
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53143102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1550bbb81daedb5b1e1b32ff7cfebc601eb3f5e2fe0fc816b4da13e77fdfdbc9`
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
# Thu, 29 Oct 2020 18:21:14 GMT
ARG KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:21:14 GMT
ENV KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:21:21 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256='6adb706eab6cc535f2703bd8993a5d5259159cf8a630c3d3974973dbe6bbf5a6' ;; 		aarch64) arch='arm64'; KONG_SHA256='a93b1c015d86b5d8b4038f3fd73332bfef97fa1c768545f353af03f54cf97fb8' ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Thu, 29 Oct 2020 18:21:22 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 29 Oct 2020 18:21:22 GMT
USER kong
# Thu, 29 Oct 2020 18:21:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Oct 2020 18:21:22 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 29 Oct 2020 18:21:22 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Oct 2020 18:21:22 GMT
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
	-	`sha256:c25d97cc4039bd282d150d09da1590e01019a05e641c6f61495324fb35a0a6ea`  
		Last Modified: Thu, 29 Oct 2020 18:23:45 GMT  
		Size: 50.3 MB (50328923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98513f5777887ba304362c52a37f9686f876ad0af12cdb8b6e49d17de0a348a8`  
		Last Modified: Thu, 29 Oct 2020 18:23:36 GMT  
		Size: 734.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:latest` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:0a0cad9b3779321b3c9a35ad077bf1e5645e291d7329e161183152692c5cb637
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.7 MB (52673538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d354929336a5e32ec6d0b868be426c01545ee0f07715f5d4f6574114013cb13`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Tue, 22 Sep 2020 19:05:32 GMT
LABEL maintainer=Kong <support@konghq.com>
# Tue, 22 Sep 2020 19:05:34 GMT
ARG ASSET=ce
# Tue, 22 Sep 2020 19:05:35 GMT
ENV ASSET=ce
# Tue, 22 Sep 2020 19:05:36 GMT
ARG EE_PORTS
# Tue, 22 Sep 2020 19:05:36 GMT
COPY file:9073480627c34fa516ae48557d24314a31d17b88798bd04c46162029e368d39c in /tmp/kong.tar.gz 
# Thu, 29 Oct 2020 18:42:33 GMT
ARG KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:42:33 GMT
ENV KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:42:46 GMT
RUN set -eux; 	arch="$(apk --print-arch)"; 	case "${arch}" in 		x86_64) arch='amd64'; KONG_SHA256='6adb706eab6cc535f2703bd8993a5d5259159cf8a630c3d3974973dbe6bbf5a6' ;; 		aarch64) arch='arm64'; KONG_SHA256='a93b1c015d86b5d8b4038f3fd73332bfef97fa1c768545f353af03f54cf97fb8' ;; 	esac;     if [ "$ASSET" = "ce" ] ; then         apk add --no-cache --virtual .build-deps curl wget tar ca-certificates &&         curl -fL "https://bintray.com/kong/kong-alpine-tar/download_file?file_path=kong-$KONG_VERSION.$arch.apk.tar.gz" -o /tmp/kong.tar.gz &&         echo "$KONG_SHA256  /tmp/kong.tar.gz" | sha256sum -c -;         apk del .build-deps;     fi;     mkdir /kong;     tar -C /kong -xzf /tmp/kong.tar.gz &&     mv /kong/usr/local/* /usr/local &&     mv /kong/etc/* /etc &&     rm -rf /kong &&     apk add --no-cache libstdc++ libgcc openssl pcre perl tzdata libcap zip bash   zlib zlib-dev git ca-certificates &&     adduser -S kong &&     mkdir -p "/usr/local/kong" &&     chown -R kong:0 /usr/local/kong &&     chown kong:0 /usr/local/bin/kong &&     chmod -R g=u /usr/local/kong &&     rm -rf /tmp/kong.tar.gz &&     if [ "$ASSET" = "ce" ] ; then       kong version ;     fi;
# Thu, 29 Oct 2020 18:42:48 GMT
COPY file:c60e90d02b3d93627e1f0d577e2298e266f50cc620574d3ef11b8b30cd8a906c in /docker-entrypoint.sh 
# Thu, 29 Oct 2020 18:42:48 GMT
USER kong
# Thu, 29 Oct 2020 18:42:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Oct 2020 18:42:49 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 29 Oct 2020 18:42:50 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Oct 2020 18:42:50 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f1f361b75deeea5140a58989e54db49d72c8f2794625392d9b60e5f6adea53`  
		Last Modified: Tue, 22 Sep 2020 19:08:54 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0562e5901c7c1412846095fddf0527b3aec71f8d310829523e905e5dec70db4a`  
		Last Modified: Thu, 29 Oct 2020 18:51:28 GMT  
		Size: 49.9 MB (49948248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b00d686849acde734efe3f6499685d14b6e6deea6307aa2194f32f58e7a026`  
		Last Modified: Thu, 29 Oct 2020 18:51:13 GMT  
		Size: 733.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `kong:ubuntu`

```console
$ docker pull kong@sha256:d3dac9be891a6c211acaba75097b9f6e8a4e0485fc466cabbe13573e482362ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `kong:ubuntu` - linux; amd64

```console
$ docker pull kong@sha256:056ffd524e8849b89f710a671b10841e337a5734a372fa428e89826f2eaa54f6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135598240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c048ac8311203db66211353c0d2ff83bd3696b6f3f3637b35a3b77859a1d1549`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Fri, 23 Oct 2020 17:33:08 GMT
ADD file:c1f3147c7b6710af5affd417ff822ee28df872d716003858d3d2e23d2277c981 in / 
# Fri, 23 Oct 2020 17:33:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:33:09 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 17:33:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:33:10 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 17:52:28 GMT
ARG ASSET=ce
# Fri, 23 Oct 2020 17:52:28 GMT
ENV ASSET=ce
# Fri, 23 Oct 2020 17:52:28 GMT
ARG EE_PORTS
# Fri, 23 Oct 2020 17:52:28 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Thu, 29 Oct 2020 18:21:27 GMT
ARG KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:21:27 GMT
ENV KONG_VERSION=2.2.0
# Thu, 29 Oct 2020 18:22:16 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt update     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && { useradd -ms /bin/bash kong || true ;}     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Thu, 29 Oct 2020 18:22:17 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Thu, 29 Oct 2020 18:22:17 GMT
USER kong
# Thu, 29 Oct 2020 18:22:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Oct 2020 18:22:17 GMT
EXPOSE 8000 8001 8443 8444
# Thu, 29 Oct 2020 18:22:17 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Oct 2020 18:22:17 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:2c11b7cecaa5d3e2a57e290921ababbfb8572b549015168d4cbd91c340d2c566`  
		Last Modified: Wed, 14 Oct 2020 13:20:30 GMT  
		Size: 45.8 MB (45825714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04637fa562525a9366f00e8f4b08d04a347bded1ee513738451ef9d42b4dfc4e`  
		Last Modified: Fri, 23 Oct 2020 17:33:48 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e6af23a0f38c4a6511147d2a9dc06a07a7afa0669000cb62720c7eafe031ae`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a424de92ad71639c5cabadcdab0493e4067eb2f9cf109ffef40db178349238`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a810599aaaccac955e7c0b605e6b1bc745018863e6127cfb34cfc8189e03fa01`  
		Last Modified: Fri, 23 Oct 2020 17:54:16 GMT  
		Size: 25.1 MB (25081963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab89deb52ede76e668a6e5adf0b8f3373863c9d0dcaee49ba0928857ff72a0ae`  
		Last Modified: Thu, 29 Oct 2020 18:24:05 GMT  
		Size: 64.7 MB (64688329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbe067f92ac3cc8db17ae04fd765d1765205b10aee77351f9773f33d935ed40`  
		Last Modified: Thu, 29 Oct 2020 18:23:53 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `kong:ubuntu` - linux; arm64 variant v8

```console
$ docker pull kong@sha256:30803b0c1e4013c034a1c48c590fb417dcabbedc1ea6923bada942b0ef5bced6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.3 MB (125254699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03d113d93337f8b22b5385c8b45adcc5024b06b83a3f5198116a9a75e730054f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["kong","docker-start"]`

```dockerfile
# Wed, 25 Nov 2020 22:44:18 GMT
ADD file:a360b1e1db1ae9973dac11dfe4e549f6416e278f53c42eb5e98b3b3da8d2a5ae in / 
# Wed, 25 Nov 2020 22:44:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:44:23 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 22:44:25 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:44:26 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:26:02 GMT
ARG ASSET=ce
# Wed, 25 Nov 2020 23:26:04 GMT
ENV ASSET=ce
# Wed, 25 Nov 2020 23:26:04 GMT
ARG EE_PORTS
# Wed, 25 Nov 2020 23:26:05 GMT
COPY file:5da22ad111df95d5c0f9c17c60cd4123a51ad46a41d3f442fca7b2bcc8d7d11b in /tmp/kong.deb 
# Wed, 25 Nov 2020 23:26:06 GMT
ARG KONG_VERSION=2.2.0
# Wed, 25 Nov 2020 23:26:07 GMT
ENV KONG_VERSION=2.2.0
# Wed, 25 Nov 2020 23:26:55 GMT
RUN set -ex;     apt-get update &&     if [ "$ASSET" = "ce" ] ; then         apt-get install -y curl &&         curl -fL "https://bintray.com/kong/kong-deb/download_file?file_path=kong-$KONG_VERSION.xenial.$(dpkg --print-architecture).deb" -o /tmp/kong.deb         && apt-get purge -y curl;     fi;     apt-get install -y --no-install-recommends unzip git 	&& apt update     && apt install --yes /tmp/kong.deb     && rm -rf /var/lib/apt/lists/*     && rm -rf /tmp/kong.deb     && { useradd -ms /bin/bash kong || true ;}     && mkdir -p "/usr/local/kong"     && chown -R kong:0 /usr/local/kong     && chown kong:0 /usr/local/bin/kong     && chmod -R g=u /usr/local/kong     && if [ "$ASSET" = "ce" ] ; then         kong version ;     fi;
# Wed, 25 Nov 2020 23:26:57 GMT
COPY file:3f0ac4e41f7591702adf841081157578863b364bb31cfb02189411168744a26e in /docker-entrypoint.sh 
# Wed, 25 Nov 2020 23:26:58 GMT
USER kong
# Wed, 25 Nov 2020 23:27:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 25 Nov 2020 23:27:02 GMT
EXPOSE 8000 8001 8443 8444
# Wed, 25 Nov 2020 23:27:02 GMT
STOPSIGNAL SIGQUIT
# Wed, 25 Nov 2020 23:27:03 GMT
CMD ["kong" "docker-start"]
```

-	Layers:
	-	`sha256:3e30c5e4609ac16f9e19faa3800699e28c77aadcfcbde2ddd5954606f80fa170`  
		Last Modified: Sat, 31 Oct 2020 00:25:13 GMT  
		Size: 40.8 MB (40826105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be82da0c7e998c509a8e86338f139501b62fde0df3908dd489a8249380ea3441`  
		Last Modified: Wed, 25 Nov 2020 22:45:42 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf04dffef88e5257b2388d643e5fb03a812316de0737ce92e3888a6722cea5e`  
		Last Modified: Wed, 25 Nov 2020 22:45:43 GMT  
		Size: 467.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2624f7934929e6e67f81a9becb317179367648ec1236d644e9bf3a00d3fe3772`  
		Last Modified: Wed, 25 Nov 2020 22:45:43 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6cba0c8b4d5e1def090992b7d3bc001ae633fa3ad938efa00a15d89e40a72c`  
		Last Modified: Wed, 25 Nov 2020 23:29:55 GMT  
		Size: 25.1 MB (25081968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b8573e52de26f1031729ff4851c3078a0bc20949b09fa5e3dcfb7e805fbf74`  
		Last Modified: Wed, 25 Nov 2020 23:30:09 GMT  
		Size: 59.3 MB (59344448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407742a2e372871244d9b6638b826e92677372d7e4b9f50ec8322ed91223c3bd`  
		Last Modified: Wed, 25 Nov 2020 23:29:52 GMT  
		Size: 689.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
