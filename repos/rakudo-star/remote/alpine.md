## `rakudo-star:alpine`

```console
$ docker pull rakudo-star@sha256:27e38b11efa762c6bc756d072bca310bea9ec5962e353a64dd4f71b693a2ae8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rakudo-star:alpine` - linux; amd64

```console
$ docker pull rakudo-star@sha256:211a5364adddb3c40ffeee91c72e0737aeea0150b2bd85c79ead9e0b540df101
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34365975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2116ba80a51349162a37d66cead1b1165ef87f5153778860d2adfb115d100bdb`
-	Default Command: `["raku"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 01:38:20 GMT
RUN addgroup -S raku && adduser -S raku -G raku
# Thu, 30 Mar 2023 01:38:20 GMT
ARG rakudo_version=2023.02-01
# Thu, 30 Mar 2023 01:38:20 GMT
ENV rakudo_version=2023.02-01
# Thu, 30 Mar 2023 01:46:31 GMT
RUN buildDeps='         bash         gcc         gnupg         libc-dev         make         perl     '         url="https://rakudo.org/dl/star/rakudo-star-${rakudo_version}.tar.gz"     keyfp="3E7E3C6EAF916676AC549285A2919382E961E2EE"     pubkeyurl="https://rakudo.org/keys/rakudo_github_automation-${keyfp}.asc"     tmpdir="$(mktemp -d)"     && set -eux     && export GNUPGHOME="${tmpdir}/gnupg"     && mkdir $GNUPGHOME     && apk add --no-cache --virtual .build-deps $buildDeps     && apk add --no-cache readline     && mkdir ${tmpdir}/rakudo         && wget ${url}.asc -O ${tmpdir}/rakudo.tar.gz.asc     && wget $url -O ${tmpdir}/rakudo.tar.gz     && wget $pubkeyurl -O ${tmpdir}/key.asc         && gpg --batch --import ${tmpdir}/key.asc     && gpg --batch --export $keyfp > ${tmpdir}/${keyfp}.asc     && rm -rf $GNUPGHOME     && mkdir $GNUPGHOME     && gpg --batch --import ${tmpdir}/${keyfp}.asc     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && bash bin/rstar install -p /usr     )     && rm -rf $tmpdir     && apk del --no-network .build-deps
# Thu, 30 Mar 2023 01:46:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/core/bin:/usr/share/perl6/site/bin:/usr/share/perl6/vendor/bin
# Thu, 30 Mar 2023 01:46:31 GMT
CMD ["raku"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c1896d24c03a78862a7e88a9ea83931dc38ef31f1462c5e2b9f340d49f918e`  
		Last Modified: Thu, 30 Mar 2023 01:46:49 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee272549e32e28a6cbeeaa80a9c1d42d81ff1eb22fa5397a8a7071923a3a4a27`  
		Last Modified: Thu, 30 Mar 2023 01:46:55 GMT  
		Size: 31.0 MB (30990146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rakudo-star:alpine` - linux; arm64 variant v8

```console
$ docker pull rakudo-star@sha256:b6c723a17cb464e3d645e21a93f3379b1bc526844e1c173cbdbf52acd73c899c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34083640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:645ff7ffa7cf88e68914bc62e76f25484d81a0a8382041ee4a738da2e95885e0`
-	Default Command: `["raku"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:22:15 GMT
RUN addgroup -S raku && adduser -S raku -G raku
# Thu, 30 Mar 2023 00:22:15 GMT
ARG rakudo_version=2023.02-01
# Thu, 30 Mar 2023 00:22:16 GMT
ENV rakudo_version=2023.02-01
# Fri, 07 Apr 2023 23:54:24 GMT
RUN buildDeps='         bash         gcc         gnupg         libc-dev         make         perl     '         url="https://rakudo.org/dl/star/rakudo-star-${rakudo_version}.tar.gz"     keyfp="3E7E3C6EAF916676AC549285A2919382E961E2EE"     pubkeyurl="https://rakudo.org/keys/rakudo_github_automation-${keyfp}.asc"     tmpdir="$(mktemp -d)"     && set -eux     && export GNUPGHOME="${tmpdir}/gnupg"     && mkdir $GNUPGHOME     && apk add --no-cache --virtual .build-deps $buildDeps     && apk add --no-cache readline     && mkdir ${tmpdir}/rakudo         && wget ${url}.asc -O ${tmpdir}/rakudo.tar.gz.asc     && wget $url -O ${tmpdir}/rakudo.tar.gz     && wget $pubkeyurl -O ${tmpdir}/key.asc         && gpg --batch --import ${tmpdir}/key.asc     && gpg --batch --export $keyfp > ${tmpdir}/${keyfp}.asc     && rm -rf $GNUPGHOME     && mkdir $GNUPGHOME     && gpg --batch --import ${tmpdir}/${keyfp}.asc     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && bash bin/rstar install -p /usr     )     && rm -rf $tmpdir     && apk del --no-network .build-deps
# Fri, 07 Apr 2023 23:54:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/core/bin:/usr/share/perl6/site/bin:/usr/share/perl6/vendor/bin
# Fri, 07 Apr 2023 23:54:24 GMT
CMD ["raku"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6243dfb5a8140ba100d3135118ccd3428c9ad3d11b9bbc8780e1fc90a1c8fbfe`  
		Last Modified: Fri, 07 Apr 2023 23:54:33 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca573fc1ae15bed3901fa7ec0ebf9bb04e53afb53e1383f0a80ef4b4a64ff070`  
		Last Modified: Fri, 07 Apr 2023 23:54:38 GMT  
		Size: 30.8 MB (30820523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
