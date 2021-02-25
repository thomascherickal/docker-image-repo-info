## `rakudo-star:alpine`

```console
$ docker pull rakudo-star@sha256:6922421ee38a62620c53d387f0f17a5a53f3aa4faae04b77326c536f871dfe2c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `rakudo-star:alpine` - linux; amd64

```console
$ docker pull rakudo-star@sha256:cca6c191b1ee1a72dec3875b230a8647a284026e4b89e746e283782d7d00cc72
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.5 MB (42507192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ac376e59b3c2344ac07662a640df6e9b7497a49feb247760f5f439679f9cf25`
-	Default Command: `["raku"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:03 GMT
ADD file:0dbb1cd66f708f54f7e6663eabf24095fcd53747bfb09912a118a77e737d9617 in / 
# Wed, 24 Feb 2021 20:20:03 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 02:23:06 GMT
RUN addgroup -S raku && adduser -S raku -G raku
# Thu, 25 Feb 2021 02:23:06 GMT
ARG rakudo_version=2020.10
# Thu, 25 Feb 2021 02:23:07 GMT
ENV rakudo_version=2020.10
# Thu, 25 Feb 2021 02:35:41 GMT
RUN buildDeps='         bash         gcc         gnupg         libc-dev         make         perl     '         url="https://rakudo.org/dl/star/rakudo-star-${rakudo_version}.tar.gz"     keyserver='ha.pool.sks-keyservers.net'     keyfp='B6F697742EFCAF5F23CE51D5031D65902E840821'     tmpdir="$(mktemp -d)"     && set -eux     && export GNUPGHOME="$tmpdir"     && apk add --no-cache --virtual .build-deps $buildDeps     && mkdir ${tmpdir}/rakudo         && wget ${url}.asc -O ${tmpdir}/rakudo.tar.gz.asc     && wget $url -O ${tmpdir}/rakudo.tar.gz     && gpg --batch --keyserver $keyserver --recv-keys $keyfp     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && bash bin/rstar install -p /usr     )     && rm -rf $tmpdir     && apk del --no-network .build-deps
# Thu, 25 Feb 2021 02:35:41 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/core/bin:/usr/share/perl6/site/bin:/usr/share/perl6/vendor/bin
# Thu, 25 Feb 2021 02:35:41 GMT
CMD ["raku"]
```

-	Layers:
	-	`sha256:f84cab65f19f5d625a4b5f895cdf37ad9f21e160bf201ec59a48d95b2a430145`  
		Last Modified: Wed, 24 Feb 2021 20:20:39 GMT  
		Size: 2.8 MB (2799493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db7170db2b42563b5043e7ab1c431454625054c3d8d34632d3e4fb5b297940f5`  
		Last Modified: Thu, 25 Feb 2021 02:35:55 GMT  
		Size: 1.2 KB (1228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d50a8367e89fc363f87489bbff0c4ecbf730519178c071f571718f92cf493e`  
		Last Modified: Thu, 25 Feb 2021 02:36:04 GMT  
		Size: 39.7 MB (39706471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rakudo-star:alpine` - linux; arm64 variant v8

```console
$ docker pull rakudo-star@sha256:f941ddd6b80f37f038bb134802ffc4785b137647d7e6676bde74148e93cc7852
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.2 MB (42209149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3f974c57aa0a942e8494df54917a4df0da6196347d0b020acebf5bda8c0d3f7`
-	Default Command: `["raku"]`

```dockerfile
# Wed, 24 Feb 2021 20:39:39 GMT
ADD file:7e82858ef85f6db90c131ed835a390d736cfdbd1a0cf8bccaeed8f7e30172ddb in / 
# Wed, 24 Feb 2021 20:39:40 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 03:50:21 GMT
RUN addgroup -S raku && adduser -S raku -G raku
# Thu, 25 Feb 2021 03:50:22 GMT
ARG rakudo_version=2020.10
# Thu, 25 Feb 2021 03:50:23 GMT
ENV rakudo_version=2020.10
# Thu, 25 Feb 2021 04:12:09 GMT
RUN buildDeps='         bash         gcc         gnupg         libc-dev         make         perl     '         url="https://rakudo.org/dl/star/rakudo-star-${rakudo_version}.tar.gz"     keyserver='ha.pool.sks-keyservers.net'     keyfp='B6F697742EFCAF5F23CE51D5031D65902E840821'     tmpdir="$(mktemp -d)"     && set -eux     && export GNUPGHOME="$tmpdir"     && apk add --no-cache --virtual .build-deps $buildDeps     && mkdir ${tmpdir}/rakudo         && wget ${url}.asc -O ${tmpdir}/rakudo.tar.gz.asc     && wget $url -O ${tmpdir}/rakudo.tar.gz     && gpg --batch --keyserver $keyserver --recv-keys $keyfp     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && bash bin/rstar install -p /usr     )     && rm -rf $tmpdir     && apk del --no-network .build-deps
# Thu, 25 Feb 2021 04:12:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/core/bin:/usr/share/perl6/site/bin:/usr/share/perl6/vendor/bin
# Thu, 25 Feb 2021 04:12:13 GMT
CMD ["raku"]
```

-	Layers:
	-	`sha256:dce8679b510e95d136241d02ababff86469dd14220812a7ce9202833c0e32f66`  
		Last Modified: Wed, 24 Feb 2021 20:40:26 GMT  
		Size: 2.7 MB (2709880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9d993b24eb35af28a879ac677d518272f14fabd25f35cb82b5be875ec8e86f4`  
		Last Modified: Thu, 25 Feb 2021 04:12:26 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70117a8bc8f66a4d5241d1371fc25ab608fab9c49688e61208c134675b687937`  
		Last Modified: Thu, 25 Feb 2021 04:12:42 GMT  
		Size: 39.5 MB (39498013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
