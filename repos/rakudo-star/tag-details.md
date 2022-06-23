<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `rakudo-star`

-	[`rakudo-star:2021.04`](#rakudo-star202104)
-	[`rakudo-star:2021.04-alpine`](#rakudo-star202104-alpine)
-	[`rakudo-star:alpine`](#rakudo-staralpine)
-	[`rakudo-star:latest`](#rakudo-starlatest)

## `rakudo-star:2021.04`

```console
$ docker pull rakudo-star@sha256:92ade6b21f6ef1053d6059b1c44b2bc6a424f03d396132c778628d77d7e3e8a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rakudo-star:2021.04` - linux; amd64

```console
$ docker pull rakudo-star@sha256:9fc3e1034795811365ad5b271c9319106ee76d10cb1e7ec3d95b76535fa9ee80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.9 MB (161902814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3f99ea7091e8d209c957c8649503f65d61c5c6c2320d9056c9891b73b3571f0`
-	Default Command: `["raku"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:36 GMT
ADD file:2f32dd3ef1e51a4d2d6dcf55fbf766434df5b3ada802b087d5761f2fa0cdebf5 in / 
# Thu, 23 Jun 2022 00:20:36 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 00:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 00:51:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 00:51:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 15:24:31 GMT
MAINTAINER Rob Hoelz
# Thu, 23 Jun 2022 15:24:32 GMT
RUN groupadd -r raku && useradd -m -r -g raku raku
# Thu, 23 Jun 2022 15:24:32 GMT
ARG rakudo_version=2021.04
# Thu, 23 Jun 2022 15:24:32 GMT
ENV rakudo_version=2021.04
# Thu, 23 Jun 2022 15:33:47 GMT
RUN buildDeps='         gcc         libc6-dev         make     '         url="https://rakudo.org/dl/star/rakudo-star-${rakudo_version}.tar.gz"     keyserver='ha.pool.sks-keyservers.net'     keyfp='B6F697742EFCAF5F23CE51D5031D65902E840821'     tmpdir="$(mktemp -d)"     && set -eux     && export GNUPGHOME="$tmpdir"     && apt-get update     && apt-get install -y --no-install-recommends $buildDeps     && rm -rf /var/lib/apt/lists/*     && mkdir ${tmpdir}/rakudo         && curl -fsSL ${url}.asc -o ${tmpdir}/rakudo.tar.gz.asc     && curl -fsSL $url -o ${tmpdir}/rakudo.tar.gz     && gpg --batch --keyserver $keyserver --recv-keys $keyfp     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && bash bin/rstar install -p /usr     )     && rm -rf $tmpdir     && apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 15:33:47 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/core/bin:/usr/share/perl6/site/bin:/usr/share/perl6/vendor/bin
# Thu, 23 Jun 2022 15:33:47 GMT
CMD ["raku"]
```

-	Layers:
	-	`sha256:ea267e4631a981caf2841a7e9a1faf29cef9d020c4378fc64845802d17586531`  
		Last Modified: Thu, 23 Jun 2022 00:25:38 GMT  
		Size: 50.4 MB (50440811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a014c92148934973210d840dc7cfed53e0afba38d839afaa48ed5150eae19af`  
		Last Modified: Thu, 23 Jun 2022 00:59:51 GMT  
		Size: 7.9 MB (7856631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293ff1be7001d642a624409e2d5f90e7708ef7e6f1a75f4eb7362a9296e18d20`  
		Last Modified: Thu, 23 Jun 2022 00:59:50 GMT  
		Size: 10.0 MB (9997231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e42533e7311ad0a85fe19e9bc5fe3138f608853eeaaea70ee08b2a631b356c3`  
		Last Modified: Thu, 23 Jun 2022 01:00:09 GMT  
		Size: 51.8 MB (51843778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2386f1abfb906811f7db6fed4744c570218aa4f59bb54ec1365ee0ba31a3d0a2`  
		Last Modified: Thu, 23 Jun 2022 15:34:05 GMT  
		Size: 4.1 KB (4129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0312fce45026252a00f6f6bb6843582e944c8a6e1f18701194307948258e672`  
		Last Modified: Thu, 23 Jun 2022 15:34:13 GMT  
		Size: 41.8 MB (41760234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rakudo-star:2021.04` - linux; arm64 variant v8

```console
$ docker pull rakudo-star@sha256:e1c71cba81dc997a1d8d8e79dcf693f2c9812d96831a02e9ee65af02fd746606
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.2 MB (160208674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:976dce0b320a6874672f7726ebf5c72c7f431cc6fb3627675eadb18e0cda96ee`
-	Default Command: `["raku"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:54 GMT
ADD file:a5e3c0ffa9f9754a6d77fafd8288e699a70f7f6ff7c5912a065f1c69f1393e99 in / 
# Thu, 23 Jun 2022 00:40:55 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:12:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:12:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 01:13:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 19:57:13 GMT
MAINTAINER Rob Hoelz
# Thu, 23 Jun 2022 19:57:14 GMT
RUN groupadd -r raku && useradd -m -r -g raku raku
# Thu, 23 Jun 2022 19:57:14 GMT
ARG rakudo_version=2021.04
# Thu, 23 Jun 2022 19:57:15 GMT
ENV rakudo_version=2021.04
# Thu, 23 Jun 2022 20:07:19 GMT
RUN buildDeps='         gcc         libc6-dev         make     '         url="https://rakudo.org/dl/star/rakudo-star-${rakudo_version}.tar.gz"     keyserver='ha.pool.sks-keyservers.net'     keyfp='B6F697742EFCAF5F23CE51D5031D65902E840821'     tmpdir="$(mktemp -d)"     && set -eux     && export GNUPGHOME="$tmpdir"     && apt-get update     && apt-get install -y --no-install-recommends $buildDeps     && rm -rf /var/lib/apt/lists/*     && mkdir ${tmpdir}/rakudo         && curl -fsSL ${url}.asc -o ${tmpdir}/rakudo.tar.gz.asc     && curl -fsSL $url -o ${tmpdir}/rakudo.tar.gz     && gpg --batch --keyserver $keyserver --recv-keys $keyfp     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && bash bin/rstar install -p /usr     )     && rm -rf $tmpdir     && apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 20:07:19 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/core/bin:/usr/share/perl6/site/bin:/usr/share/perl6/vendor/bin
# Thu, 23 Jun 2022 20:07:20 GMT
CMD ["raku"]
```

-	Layers:
	-	`sha256:8d6f1451981514e25c21542f5c7ee9bb90052b8856b484ce47294cbf1fd5a234`  
		Last Modified: Thu, 23 Jun 2022 00:47:46 GMT  
		Size: 49.2 MB (49229092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ccc9fb4baf6e7f2e6ee18ed689c8ee1171c6751c8bbd317d580a193da27a5f1`  
		Last Modified: Thu, 23 Jun 2022 01:23:09 GMT  
		Size: 7.7 MB (7719858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:620d55693ed5943ab298346d9ccafefdd6d6f33994e6820a857737df89b65f3a`  
		Last Modified: Thu, 23 Jun 2022 01:23:08 GMT  
		Size: 9.8 MB (9767307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82dcb0fa2b6020cd95c3972ec0fe03da38862f57574fe03a49360713d6f415d6`  
		Last Modified: Thu, 23 Jun 2022 01:23:28 GMT  
		Size: 52.2 MB (52174988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6700afd1728f8155a040ac511292139ac9702e3ca452727192c612924a2c5c34`  
		Last Modified: Thu, 23 Jun 2022 20:07:47 GMT  
		Size: 4.0 KB (4011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41fc5228b751a20451cea24a18b790c087eab31527100e11c143f2a1349788da`  
		Last Modified: Thu, 23 Jun 2022 20:07:55 GMT  
		Size: 41.3 MB (41313418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rakudo-star:2021.04-alpine`

```console
$ docker pull rakudo-star@sha256:c768f5b3b4e6f4a3269bb24a1d0d4e9fb148059bd6108bc3723f9691f1370269
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rakudo-star:2021.04-alpine` - linux; amd64

```console
$ docker pull rakudo-star@sha256:921b32e33da1d2468ea5c99cc946ee0ff1876d2b7898b9c1665e2fc986fc0081
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44259618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c406d89a73519add4aeae3e3bc557abc7ae37eaccd700b97d15e37f3e1b6b53f`
-	Default Command: `["raku"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:14 GMT
ADD file:0f80c1db9ba5535d5020662b1c880624848316637bf3f9c189f459ab31f365d0 in / 
# Tue, 05 Apr 2022 00:20:14 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:30:58 GMT
RUN addgroup -S raku && adduser -S raku -G raku
# Tue, 05 Apr 2022 10:30:58 GMT
ARG rakudo_version=2021.04
# Tue, 05 Apr 2022 10:30:58 GMT
ENV rakudo_version=2021.04
# Tue, 05 Apr 2022 10:41:41 GMT
RUN buildDeps='         bash         gcc         gnupg         libc-dev         make         perl     '         url="https://rakudo.org/dl/star/rakudo-star-${rakudo_version}.tar.gz"     keyserver='ha.pool.sks-keyservers.net'     keyfp='B6F697742EFCAF5F23CE51D5031D65902E840821'     tmpdir="$(mktemp -d)"     && set -eux     && export GNUPGHOME="$tmpdir"     && apk add --no-cache --virtual .build-deps $buildDeps     && mkdir ${tmpdir}/rakudo         && wget ${url}.asc -O ${tmpdir}/rakudo.tar.gz.asc     && wget $url -O ${tmpdir}/rakudo.tar.gz     && gpg --batch --keyserver $keyserver --recv-keys $keyfp     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && bash bin/rstar install -p /usr     )     && rm -rf $tmpdir     && apk del --no-network .build-deps
# Tue, 05 Apr 2022 10:41:41 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/core/bin:/usr/share/perl6/site/bin:/usr/share/perl6/vendor/bin
# Tue, 05 Apr 2022 10:41:41 GMT
CMD ["raku"]
```

-	Layers:
	-	`sha256:6097bfa160c13665f946cea95b206a812a795d2517d7690a0a0796d64ec5f817`  
		Last Modified: Tue, 05 Apr 2022 00:21:00 GMT  
		Size: 2.8 MB (2819312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee4a74fe375c278bc484e562d37ca7494b9b6a62e1249aabbca0dd38a8ede06`  
		Last Modified: Tue, 05 Apr 2022 10:42:00 GMT  
		Size: 1.3 KB (1251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d43260fc9768ea8910786a7a1d7366c41df02461b1d8610fd1d00751aa1bc4`  
		Last Modified: Tue, 05 Apr 2022 10:42:08 GMT  
		Size: 41.4 MB (41439055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rakudo-star:2021.04-alpine` - linux; arm64 variant v8

```console
$ docker pull rakudo-star@sha256:89285bdb42fbe5a00b7bfcc1c79854ad9a5668def09c24a884808f2f77ea69e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43724021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dbae01f78e6deb54b411310056ad9caf18d77351041de54c8c0d3d7a906b783`
-	Default Command: `["raku"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:46 GMT
ADD file:535e6f58c2cf7520c1824c8a290dc38c5519485470ed49587748a27c0113d586 in / 
# Mon, 04 Apr 2022 23:39:46 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:53:42 GMT
RUN addgroup -S raku && adduser -S raku -G raku
# Tue, 05 Apr 2022 06:53:43 GMT
ARG rakudo_version=2021.04
# Tue, 05 Apr 2022 06:53:44 GMT
ENV rakudo_version=2021.04
# Tue, 05 Apr 2022 07:09:02 GMT
RUN buildDeps='         bash         gcc         gnupg         libc-dev         make         perl     '         url="https://rakudo.org/dl/star/rakudo-star-${rakudo_version}.tar.gz"     keyserver='ha.pool.sks-keyservers.net'     keyfp='B6F697742EFCAF5F23CE51D5031D65902E840821'     tmpdir="$(mktemp -d)"     && set -eux     && export GNUPGHOME="$tmpdir"     && apk add --no-cache --virtual .build-deps $buildDeps     && mkdir ${tmpdir}/rakudo         && wget ${url}.asc -O ${tmpdir}/rakudo.tar.gz.asc     && wget $url -O ${tmpdir}/rakudo.tar.gz     && gpg --batch --keyserver $keyserver --recv-keys $keyfp     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && bash bin/rstar install -p /usr     )     && rm -rf $tmpdir     && apk del --no-network .build-deps
# Tue, 05 Apr 2022 07:09:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/core/bin:/usr/share/perl6/site/bin:/usr/share/perl6/vendor/bin
# Tue, 05 Apr 2022 07:09:03 GMT
CMD ["raku"]
```

-	Layers:
	-	`sha256:edd30f0f17040c7b292e0960fa771cf3ea45f994d7a2577a14fe02ae7ce727e9`  
		Last Modified: Mon, 04 Apr 2022 23:40:51 GMT  
		Size: 2.7 MB (2720895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ca547acb27a3e0ccb1f06ea97957818c98bc358320f3de43237b95aa6cece3`  
		Last Modified: Tue, 05 Apr 2022 07:09:20 GMT  
		Size: 1.2 KB (1227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9750a11e7da66aa9e1db5cda79dafa1698ba42753a5251f0d3fc738eed05696b`  
		Last Modified: Tue, 05 Apr 2022 07:09:29 GMT  
		Size: 41.0 MB (41001899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rakudo-star:alpine`

```console
$ docker pull rakudo-star@sha256:c768f5b3b4e6f4a3269bb24a1d0d4e9fb148059bd6108bc3723f9691f1370269
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rakudo-star:alpine` - linux; amd64

```console
$ docker pull rakudo-star@sha256:921b32e33da1d2468ea5c99cc946ee0ff1876d2b7898b9c1665e2fc986fc0081
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44259618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c406d89a73519add4aeae3e3bc557abc7ae37eaccd700b97d15e37f3e1b6b53f`
-	Default Command: `["raku"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:14 GMT
ADD file:0f80c1db9ba5535d5020662b1c880624848316637bf3f9c189f459ab31f365d0 in / 
# Tue, 05 Apr 2022 00:20:14 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 10:30:58 GMT
RUN addgroup -S raku && adduser -S raku -G raku
# Tue, 05 Apr 2022 10:30:58 GMT
ARG rakudo_version=2021.04
# Tue, 05 Apr 2022 10:30:58 GMT
ENV rakudo_version=2021.04
# Tue, 05 Apr 2022 10:41:41 GMT
RUN buildDeps='         bash         gcc         gnupg         libc-dev         make         perl     '         url="https://rakudo.org/dl/star/rakudo-star-${rakudo_version}.tar.gz"     keyserver='ha.pool.sks-keyservers.net'     keyfp='B6F697742EFCAF5F23CE51D5031D65902E840821'     tmpdir="$(mktemp -d)"     && set -eux     && export GNUPGHOME="$tmpdir"     && apk add --no-cache --virtual .build-deps $buildDeps     && mkdir ${tmpdir}/rakudo         && wget ${url}.asc -O ${tmpdir}/rakudo.tar.gz.asc     && wget $url -O ${tmpdir}/rakudo.tar.gz     && gpg --batch --keyserver $keyserver --recv-keys $keyfp     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && bash bin/rstar install -p /usr     )     && rm -rf $tmpdir     && apk del --no-network .build-deps
# Tue, 05 Apr 2022 10:41:41 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/core/bin:/usr/share/perl6/site/bin:/usr/share/perl6/vendor/bin
# Tue, 05 Apr 2022 10:41:41 GMT
CMD ["raku"]
```

-	Layers:
	-	`sha256:6097bfa160c13665f946cea95b206a812a795d2517d7690a0a0796d64ec5f817`  
		Last Modified: Tue, 05 Apr 2022 00:21:00 GMT  
		Size: 2.8 MB (2819312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee4a74fe375c278bc484e562d37ca7494b9b6a62e1249aabbca0dd38a8ede06`  
		Last Modified: Tue, 05 Apr 2022 10:42:00 GMT  
		Size: 1.3 KB (1251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26d43260fc9768ea8910786a7a1d7366c41df02461b1d8610fd1d00751aa1bc4`  
		Last Modified: Tue, 05 Apr 2022 10:42:08 GMT  
		Size: 41.4 MB (41439055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rakudo-star:alpine` - linux; arm64 variant v8

```console
$ docker pull rakudo-star@sha256:89285bdb42fbe5a00b7bfcc1c79854ad9a5668def09c24a884808f2f77ea69e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43724021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dbae01f78e6deb54b411310056ad9caf18d77351041de54c8c0d3d7a906b783`
-	Default Command: `["raku"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:46 GMT
ADD file:535e6f58c2cf7520c1824c8a290dc38c5519485470ed49587748a27c0113d586 in / 
# Mon, 04 Apr 2022 23:39:46 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:53:42 GMT
RUN addgroup -S raku && adduser -S raku -G raku
# Tue, 05 Apr 2022 06:53:43 GMT
ARG rakudo_version=2021.04
# Tue, 05 Apr 2022 06:53:44 GMT
ENV rakudo_version=2021.04
# Tue, 05 Apr 2022 07:09:02 GMT
RUN buildDeps='         bash         gcc         gnupg         libc-dev         make         perl     '         url="https://rakudo.org/dl/star/rakudo-star-${rakudo_version}.tar.gz"     keyserver='ha.pool.sks-keyservers.net'     keyfp='B6F697742EFCAF5F23CE51D5031D65902E840821'     tmpdir="$(mktemp -d)"     && set -eux     && export GNUPGHOME="$tmpdir"     && apk add --no-cache --virtual .build-deps $buildDeps     && mkdir ${tmpdir}/rakudo         && wget ${url}.asc -O ${tmpdir}/rakudo.tar.gz.asc     && wget $url -O ${tmpdir}/rakudo.tar.gz     && gpg --batch --keyserver $keyserver --recv-keys $keyfp     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && bash bin/rstar install -p /usr     )     && rm -rf $tmpdir     && apk del --no-network .build-deps
# Tue, 05 Apr 2022 07:09:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/core/bin:/usr/share/perl6/site/bin:/usr/share/perl6/vendor/bin
# Tue, 05 Apr 2022 07:09:03 GMT
CMD ["raku"]
```

-	Layers:
	-	`sha256:edd30f0f17040c7b292e0960fa771cf3ea45f994d7a2577a14fe02ae7ce727e9`  
		Last Modified: Mon, 04 Apr 2022 23:40:51 GMT  
		Size: 2.7 MB (2720895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ca547acb27a3e0ccb1f06ea97957818c98bc358320f3de43237b95aa6cece3`  
		Last Modified: Tue, 05 Apr 2022 07:09:20 GMT  
		Size: 1.2 KB (1227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9750a11e7da66aa9e1db5cda79dafa1698ba42753a5251f0d3fc738eed05696b`  
		Last Modified: Tue, 05 Apr 2022 07:09:29 GMT  
		Size: 41.0 MB (41001899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rakudo-star:latest`

```console
$ docker pull rakudo-star@sha256:92ade6b21f6ef1053d6059b1c44b2bc6a424f03d396132c778628d77d7e3e8a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rakudo-star:latest` - linux; amd64

```console
$ docker pull rakudo-star@sha256:9fc3e1034795811365ad5b271c9319106ee76d10cb1e7ec3d95b76535fa9ee80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.9 MB (161902814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3f99ea7091e8d209c957c8649503f65d61c5c6c2320d9056c9891b73b3571f0`
-	Default Command: `["raku"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:36 GMT
ADD file:2f32dd3ef1e51a4d2d6dcf55fbf766434df5b3ada802b087d5761f2fa0cdebf5 in / 
# Thu, 23 Jun 2022 00:20:36 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 00:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 00:51:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 00:51:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 15:24:31 GMT
MAINTAINER Rob Hoelz
# Thu, 23 Jun 2022 15:24:32 GMT
RUN groupadd -r raku && useradd -m -r -g raku raku
# Thu, 23 Jun 2022 15:24:32 GMT
ARG rakudo_version=2021.04
# Thu, 23 Jun 2022 15:24:32 GMT
ENV rakudo_version=2021.04
# Thu, 23 Jun 2022 15:33:47 GMT
RUN buildDeps='         gcc         libc6-dev         make     '         url="https://rakudo.org/dl/star/rakudo-star-${rakudo_version}.tar.gz"     keyserver='ha.pool.sks-keyservers.net'     keyfp='B6F697742EFCAF5F23CE51D5031D65902E840821'     tmpdir="$(mktemp -d)"     && set -eux     && export GNUPGHOME="$tmpdir"     && apt-get update     && apt-get install -y --no-install-recommends $buildDeps     && rm -rf /var/lib/apt/lists/*     && mkdir ${tmpdir}/rakudo         && curl -fsSL ${url}.asc -o ${tmpdir}/rakudo.tar.gz.asc     && curl -fsSL $url -o ${tmpdir}/rakudo.tar.gz     && gpg --batch --keyserver $keyserver --recv-keys $keyfp     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && bash bin/rstar install -p /usr     )     && rm -rf $tmpdir     && apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 15:33:47 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/core/bin:/usr/share/perl6/site/bin:/usr/share/perl6/vendor/bin
# Thu, 23 Jun 2022 15:33:47 GMT
CMD ["raku"]
```

-	Layers:
	-	`sha256:ea267e4631a981caf2841a7e9a1faf29cef9d020c4378fc64845802d17586531`  
		Last Modified: Thu, 23 Jun 2022 00:25:38 GMT  
		Size: 50.4 MB (50440811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a014c92148934973210d840dc7cfed53e0afba38d839afaa48ed5150eae19af`  
		Last Modified: Thu, 23 Jun 2022 00:59:51 GMT  
		Size: 7.9 MB (7856631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293ff1be7001d642a624409e2d5f90e7708ef7e6f1a75f4eb7362a9296e18d20`  
		Last Modified: Thu, 23 Jun 2022 00:59:50 GMT  
		Size: 10.0 MB (9997231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e42533e7311ad0a85fe19e9bc5fe3138f608853eeaaea70ee08b2a631b356c3`  
		Last Modified: Thu, 23 Jun 2022 01:00:09 GMT  
		Size: 51.8 MB (51843778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2386f1abfb906811f7db6fed4744c570218aa4f59bb54ec1365ee0ba31a3d0a2`  
		Last Modified: Thu, 23 Jun 2022 15:34:05 GMT  
		Size: 4.1 KB (4129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0312fce45026252a00f6f6bb6843582e944c8a6e1f18701194307948258e672`  
		Last Modified: Thu, 23 Jun 2022 15:34:13 GMT  
		Size: 41.8 MB (41760234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rakudo-star:latest` - linux; arm64 variant v8

```console
$ docker pull rakudo-star@sha256:e1c71cba81dc997a1d8d8e79dcf693f2c9812d96831a02e9ee65af02fd746606
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.2 MB (160208674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:976dce0b320a6874672f7726ebf5c72c7f431cc6fb3627675eadb18e0cda96ee`
-	Default Command: `["raku"]`

```dockerfile
# Thu, 23 Jun 2022 00:40:54 GMT
ADD file:a5e3c0ffa9f9754a6d77fafd8288e699a70f7f6ff7c5912a065f1c69f1393e99 in / 
# Thu, 23 Jun 2022 00:40:55 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 01:12:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 01:12:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Jun 2022 01:13:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 19:57:13 GMT
MAINTAINER Rob Hoelz
# Thu, 23 Jun 2022 19:57:14 GMT
RUN groupadd -r raku && useradd -m -r -g raku raku
# Thu, 23 Jun 2022 19:57:14 GMT
ARG rakudo_version=2021.04
# Thu, 23 Jun 2022 19:57:15 GMT
ENV rakudo_version=2021.04
# Thu, 23 Jun 2022 20:07:19 GMT
RUN buildDeps='         gcc         libc6-dev         make     '         url="https://rakudo.org/dl/star/rakudo-star-${rakudo_version}.tar.gz"     keyserver='ha.pool.sks-keyservers.net'     keyfp='B6F697742EFCAF5F23CE51D5031D65902E840821'     tmpdir="$(mktemp -d)"     && set -eux     && export GNUPGHOME="$tmpdir"     && apt-get update     && apt-get install -y --no-install-recommends $buildDeps     && rm -rf /var/lib/apt/lists/*     && mkdir ${tmpdir}/rakudo         && curl -fsSL ${url}.asc -o ${tmpdir}/rakudo.tar.gz.asc     && curl -fsSL $url -o ${tmpdir}/rakudo.tar.gz     && gpg --batch --keyserver $keyserver --recv-keys $keyfp     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && bash bin/rstar install -p /usr     )     && rm -rf $tmpdir     && apt-get purge -y --auto-remove $buildDeps
# Thu, 23 Jun 2022 20:07:19 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/core/bin:/usr/share/perl6/site/bin:/usr/share/perl6/vendor/bin
# Thu, 23 Jun 2022 20:07:20 GMT
CMD ["raku"]
```

-	Layers:
	-	`sha256:8d6f1451981514e25c21542f5c7ee9bb90052b8856b484ce47294cbf1fd5a234`  
		Last Modified: Thu, 23 Jun 2022 00:47:46 GMT  
		Size: 49.2 MB (49229092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ccc9fb4baf6e7f2e6ee18ed689c8ee1171c6751c8bbd317d580a193da27a5f1`  
		Last Modified: Thu, 23 Jun 2022 01:23:09 GMT  
		Size: 7.7 MB (7719858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:620d55693ed5943ab298346d9ccafefdd6d6f33994e6820a857737df89b65f3a`  
		Last Modified: Thu, 23 Jun 2022 01:23:08 GMT  
		Size: 9.8 MB (9767307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82dcb0fa2b6020cd95c3972ec0fe03da38862f57574fe03a49360713d6f415d6`  
		Last Modified: Thu, 23 Jun 2022 01:23:28 GMT  
		Size: 52.2 MB (52174988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6700afd1728f8155a040ac511292139ac9702e3ca452727192c612924a2c5c34`  
		Last Modified: Thu, 23 Jun 2022 20:07:47 GMT  
		Size: 4.0 KB (4011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41fc5228b751a20451cea24a18b790c087eab31527100e11c143f2a1349788da`  
		Last Modified: Thu, 23 Jun 2022 20:07:55 GMT  
		Size: 41.3 MB (41313418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
