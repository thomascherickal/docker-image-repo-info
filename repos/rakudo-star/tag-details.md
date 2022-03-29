<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `rakudo-star`

-	[`rakudo-star:2021.04`](#rakudo-star202104)
-	[`rakudo-star:2021.04-alpine`](#rakudo-star202104-alpine)
-	[`rakudo-star:alpine`](#rakudo-staralpine)
-	[`rakudo-star:latest`](#rakudo-starlatest)

## `rakudo-star:2021.04`

```console
$ docker pull rakudo-star@sha256:0b3c1828ad1b75ef687006f06bca5a705a48c933aa29a3feb171f250f981adbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rakudo-star:2021.04` - linux; amd64

```console
$ docker pull rakudo-star@sha256:ceada0ae4dbbe68e2fd74e01682602f7b28d7fd39131661f3021184803daaa4e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.9 MB (161880457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5bdf30dc23493f54a3cede4bebbb7f410a62126f3dc2cc726e515aaa06c3a73`
-	Default Command: `["raku"]`

```dockerfile
# Thu, 17 Mar 2022 04:04:10 GMT
ADD file:28eba36c2d43c343d9dfd5ace80db0043e1f92aa3afb4aa95d6cbb54d7e6efef in / 
# Thu, 17 Mar 2022 04:04:11 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 06:31:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 06:32:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Mar 2022 06:32:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 23:50:26 GMT
MAINTAINER Rob Hoelz
# Sat, 19 Mar 2022 23:50:27 GMT
RUN groupadd -r raku && useradd -m -r -g raku raku
# Sat, 19 Mar 2022 23:50:27 GMT
ARG rakudo_version=2021.04
# Sat, 19 Mar 2022 23:50:27 GMT
ENV rakudo_version=2021.04
# Sat, 19 Mar 2022 23:59:29 GMT
RUN buildDeps='         gcc         libc6-dev         make     '         url="https://rakudo.org/dl/star/rakudo-star-${rakudo_version}.tar.gz"     keyserver='ha.pool.sks-keyservers.net'     keyfp='B6F697742EFCAF5F23CE51D5031D65902E840821'     tmpdir="$(mktemp -d)"     && set -eux     && export GNUPGHOME="$tmpdir"     && apt-get update     && apt-get install -y --no-install-recommends $buildDeps     && rm -rf /var/lib/apt/lists/*     && mkdir ${tmpdir}/rakudo         && curl -fsSL ${url}.asc -o ${tmpdir}/rakudo.tar.gz.asc     && curl -fsSL $url -o ${tmpdir}/rakudo.tar.gz     && gpg --batch --keyserver $keyserver --recv-keys $keyfp     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && bash bin/rstar install -p /usr     )     && rm -rf $tmpdir     && apt-get purge -y --auto-remove $buildDeps
# Sat, 19 Mar 2022 23:59:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/core/bin:/usr/share/perl6/site/bin:/usr/share/perl6/vendor/bin
# Sat, 19 Mar 2022 23:59:30 GMT
CMD ["raku"]
```

-	Layers:
	-	`sha256:7d66b83ec869a899bc8364af9c9eb0f1a5ba6907f699ef52f3182e19e2598924`  
		Last Modified: Thu, 17 Mar 2022 04:10:29 GMT  
		Size: 50.4 MB (50437294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d88439e7b50a5f3923f67f432b6863c1e11adf4e45bf9740515d2cc01fd8e155`  
		Last Modified: Fri, 18 Mar 2022 07:04:47 GMT  
		Size: 7.8 MB (7834140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22360a9558f73f04bb5e4dbe6dbe1584cb913040ae66388a8db66fc2ed131002`  
		Last Modified: Fri, 18 Mar 2022 07:04:47 GMT  
		Size: 10.0 MB (9997260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f260dee23bc81622ef145aff36ad9816cca1c98bfa9361ad1bdf03c8975b104e`  
		Last Modified: Fri, 18 Mar 2022 07:05:07 GMT  
		Size: 51.8 MB (51843594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475e43b3b5843cc948933174e306b40c3e6957df2f13848c7ff5b77567937abe`  
		Last Modified: Sat, 19 Mar 2022 23:59:45 GMT  
		Size: 4.1 KB (4131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a51ab46ee5ec98ff33259d4cd5ef44fd3d8b2faffe5b825e45a748769f5fa57`  
		Last Modified: Sat, 19 Mar 2022 23:59:52 GMT  
		Size: 41.8 MB (41764038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rakudo-star:2021.04` - linux; arm64 variant v8

```console
$ docker pull rakudo-star@sha256:c7640cf9677f0de998ac75be7630c5caee0485f046c695b89b524622789acf8e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.7 MB (159719848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:287a097958254ce78bf5306d5fa2326dbdceefae89605c92017f5f579367148f`
-	Default Command: `["raku"]`

```dockerfile
# Thu, 17 Mar 2022 03:22:08 GMT
ADD file:37cabd1fec04269c22fc158f62ce5bc655934f2e58fb1ff3a1e366a33ba9bc18 in / 
# Thu, 17 Mar 2022 03:22:09 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 22:12:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 22:12:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Mar 2022 22:12:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 01:27:48 GMT
MAINTAINER Rob Hoelz
# Sat, 19 Mar 2022 01:27:49 GMT
RUN groupadd -r raku && useradd -m -r -g raku raku
# Sat, 19 Mar 2022 01:27:49 GMT
ARG rakudo_version=2021.04
# Sat, 19 Mar 2022 01:27:50 GMT
ENV rakudo_version=2021.04
# Sat, 19 Mar 2022 01:37:47 GMT
RUN buildDeps='         gcc         libc6-dev         make     '         url="https://rakudo.org/dl/star/rakudo-star-${rakudo_version}.tar.gz"     keyserver='ha.pool.sks-keyservers.net'     keyfp='B6F697742EFCAF5F23CE51D5031D65902E840821'     tmpdir="$(mktemp -d)"     && set -eux     && export GNUPGHOME="$tmpdir"     && apt-get update     && apt-get install -y --no-install-recommends $buildDeps     && rm -rf /var/lib/apt/lists/*     && mkdir ${tmpdir}/rakudo         && curl -fsSL ${url}.asc -o ${tmpdir}/rakudo.tar.gz.asc     && curl -fsSL $url -o ${tmpdir}/rakudo.tar.gz     && gpg --batch --keyserver $keyserver --recv-keys $keyfp     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && bash bin/rstar install -p /usr     )     && rm -rf $tmpdir     && apt-get purge -y --auto-remove $buildDeps
# Sat, 19 Mar 2022 01:37:47 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/core/bin:/usr/share/perl6/site/bin:/usr/share/perl6/vendor/bin
# Sat, 19 Mar 2022 01:37:48 GMT
CMD ["raku"]
```

-	Layers:
	-	`sha256:3996f04b7c6c17d8b25c04c7287353b896b4a0b10ab440f47d00573a7d5c3e17`  
		Last Modified: Thu, 17 Mar 2022 03:28:59 GMT  
		Size: 49.2 MB (49222993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80907b498681187ef4aa817ec6f39ba351e376afbb4fcf4415841ab9015cfc59`  
		Last Modified: Thu, 17 Mar 2022 22:22:15 GMT  
		Size: 7.7 MB (7695349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8327dc7899c1a628cf11f95bb594fca3c86e45d1f4f0eb73d2ba9058eba5927`  
		Last Modified: Thu, 17 Mar 2022 22:22:15 GMT  
		Size: 9.8 MB (9767203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1431347b40fe69ed685917a6ef1b8c28d5de6147f3c62ea11a1951ead75ccdd`  
		Last Modified: Thu, 17 Mar 2022 22:22:34 GMT  
		Size: 52.2 MB (52174886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fee11304a3fc0820f4b5dc6faa346614e1858d5f1ad4b80dc94e63ab3acdae1`  
		Last Modified: Sat, 19 Mar 2022 01:38:18 GMT  
		Size: 4.0 KB (4008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5cc29dda37328d52a7bd774bda0ccbf92f4f71540767aaa38493b4e0610d357`  
		Last Modified: Sat, 19 Mar 2022 01:38:27 GMT  
		Size: 40.9 MB (40855409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rakudo-star:2021.04-alpine`

```console
$ docker pull rakudo-star@sha256:47a741f8fa9ec963eff8694b35d6651a9db0f88bbbb35c361a7070d319eeb2d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rakudo-star:2021.04-alpine` - linux; amd64

```console
$ docker pull rakudo-star@sha256:7e99fb5a4c0843e7be220318fe39c1204762f7038738be585f693b62a27e4cf4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44260211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3e6615552a7e973ae360e0c9341ec7a36a43984c494fafe4a87d518d6fd15db`
-	Default Command: `["raku"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:46 GMT
ADD file:a2ef39a587aac85256b55bee81f17d73aaa7154b2a32a31527c7803fb889f2e7 in / 
# Tue, 29 Mar 2022 00:19:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 16:27:30 GMT
RUN addgroup -S raku && adduser -S raku -G raku
# Tue, 29 Mar 2022 16:27:30 GMT
ARG rakudo_version=2021.04
# Tue, 29 Mar 2022 16:27:30 GMT
ENV rakudo_version=2021.04
# Tue, 29 Mar 2022 16:38:18 GMT
RUN buildDeps='         bash         gcc         gnupg         libc-dev         make         perl     '         url="https://rakudo.org/dl/star/rakudo-star-${rakudo_version}.tar.gz"     keyserver='ha.pool.sks-keyservers.net'     keyfp='B6F697742EFCAF5F23CE51D5031D65902E840821'     tmpdir="$(mktemp -d)"     && set -eux     && export GNUPGHOME="$tmpdir"     && apk add --no-cache --virtual .build-deps $buildDeps     && mkdir ${tmpdir}/rakudo         && wget ${url}.asc -O ${tmpdir}/rakudo.tar.gz.asc     && wget $url -O ${tmpdir}/rakudo.tar.gz     && gpg --batch --keyserver $keyserver --recv-keys $keyfp     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && bash bin/rstar install -p /usr     )     && rm -rf $tmpdir     && apk del --no-network .build-deps
# Tue, 29 Mar 2022 16:38:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/core/bin:/usr/share/perl6/site/bin:/usr/share/perl6/vendor/bin
# Tue, 29 Mar 2022 16:38:18 GMT
CMD ["raku"]
```

-	Layers:
	-	`sha256:b9c05db88786fd3c89b78787631257301391f898c03ba50553b556630046a741`  
		Last Modified: Tue, 29 Mar 2022 00:20:43 GMT  
		Size: 2.8 MB (2819223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be43853149918db3a48ec21a02aa5f36b61f20e617e3276b94ac579fde8c637c`  
		Last Modified: Tue, 29 Mar 2022 16:38:31 GMT  
		Size: 1.3 KB (1254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e90d819e0af0890d0d0b8c18c6fba285f77c7d5d62c2c2d0d8d15fa56fd088`  
		Last Modified: Tue, 29 Mar 2022 16:38:39 GMT  
		Size: 41.4 MB (41439734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rakudo-star:2021.04-alpine` - linux; arm64 variant v8

```console
$ docker pull rakudo-star@sha256:4632162902f25af4ba454294fbbcc314654d983f928d1beb7b89a2b755f7e9b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43948587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2ab290aa36dbd7f1734aff1542c5c407e9f5424ec27fd3b122ba14857d919df`
-	Default Command: `["raku"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:18 GMT
ADD file:3b8e0dac20ca40faf2aaf084b69476a222952f177c0e6ec90804a10c91a51feb in / 
# Tue, 29 Mar 2022 00:40:19 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 18:29:27 GMT
RUN addgroup -S raku && adduser -S raku -G raku
# Tue, 29 Mar 2022 18:29:28 GMT
ARG rakudo_version=2021.04
# Tue, 29 Mar 2022 18:29:29 GMT
ENV rakudo_version=2021.04
# Tue, 29 Mar 2022 18:51:11 GMT
RUN buildDeps='         bash         gcc         gnupg         libc-dev         make         perl     '         url="https://rakudo.org/dl/star/rakudo-star-${rakudo_version}.tar.gz"     keyserver='ha.pool.sks-keyservers.net'     keyfp='B6F697742EFCAF5F23CE51D5031D65902E840821'     tmpdir="$(mktemp -d)"     && set -eux     && export GNUPGHOME="$tmpdir"     && apk add --no-cache --virtual .build-deps $buildDeps     && mkdir ${tmpdir}/rakudo         && wget ${url}.asc -O ${tmpdir}/rakudo.tar.gz.asc     && wget $url -O ${tmpdir}/rakudo.tar.gz     && gpg --batch --keyserver $keyserver --recv-keys $keyfp     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && bash bin/rstar install -p /usr     )     && rm -rf $tmpdir     && apk del --no-network .build-deps
# Tue, 29 Mar 2022 18:51:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/core/bin:/usr/share/perl6/site/bin:/usr/share/perl6/vendor/bin
# Tue, 29 Mar 2022 18:51:12 GMT
CMD ["raku"]
```

-	Layers:
	-	`sha256:4e7dd0becbc2dc968b69cba46c81a25fa500c88a644832ce17a5bb090925fa79`  
		Last Modified: Tue, 29 Mar 2022 00:41:37 GMT  
		Size: 2.7 MB (2720845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44540bca26eea25dec5c60a3dd735ae7c3ba058f4b32af8145ff9c902a36af01`  
		Last Modified: Tue, 29 Mar 2022 18:51:40 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8d037475d3940d9574b6ce8bd92cd1751526337369b678d4a6e4d54814ebad`  
		Last Modified: Tue, 29 Mar 2022 18:51:47 GMT  
		Size: 41.2 MB (41226513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rakudo-star:alpine`

```console
$ docker pull rakudo-star@sha256:47a741f8fa9ec963eff8694b35d6651a9db0f88bbbb35c361a7070d319eeb2d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rakudo-star:alpine` - linux; amd64

```console
$ docker pull rakudo-star@sha256:7e99fb5a4c0843e7be220318fe39c1204762f7038738be585f693b62a27e4cf4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44260211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3e6615552a7e973ae360e0c9341ec7a36a43984c494fafe4a87d518d6fd15db`
-	Default Command: `["raku"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:46 GMT
ADD file:a2ef39a587aac85256b55bee81f17d73aaa7154b2a32a31527c7803fb889f2e7 in / 
# Tue, 29 Mar 2022 00:19:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 16:27:30 GMT
RUN addgroup -S raku && adduser -S raku -G raku
# Tue, 29 Mar 2022 16:27:30 GMT
ARG rakudo_version=2021.04
# Tue, 29 Mar 2022 16:27:30 GMT
ENV rakudo_version=2021.04
# Tue, 29 Mar 2022 16:38:18 GMT
RUN buildDeps='         bash         gcc         gnupg         libc-dev         make         perl     '         url="https://rakudo.org/dl/star/rakudo-star-${rakudo_version}.tar.gz"     keyserver='ha.pool.sks-keyservers.net'     keyfp='B6F697742EFCAF5F23CE51D5031D65902E840821'     tmpdir="$(mktemp -d)"     && set -eux     && export GNUPGHOME="$tmpdir"     && apk add --no-cache --virtual .build-deps $buildDeps     && mkdir ${tmpdir}/rakudo         && wget ${url}.asc -O ${tmpdir}/rakudo.tar.gz.asc     && wget $url -O ${tmpdir}/rakudo.tar.gz     && gpg --batch --keyserver $keyserver --recv-keys $keyfp     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && bash bin/rstar install -p /usr     )     && rm -rf $tmpdir     && apk del --no-network .build-deps
# Tue, 29 Mar 2022 16:38:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/core/bin:/usr/share/perl6/site/bin:/usr/share/perl6/vendor/bin
# Tue, 29 Mar 2022 16:38:18 GMT
CMD ["raku"]
```

-	Layers:
	-	`sha256:b9c05db88786fd3c89b78787631257301391f898c03ba50553b556630046a741`  
		Last Modified: Tue, 29 Mar 2022 00:20:43 GMT  
		Size: 2.8 MB (2819223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be43853149918db3a48ec21a02aa5f36b61f20e617e3276b94ac579fde8c637c`  
		Last Modified: Tue, 29 Mar 2022 16:38:31 GMT  
		Size: 1.3 KB (1254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e90d819e0af0890d0d0b8c18c6fba285f77c7d5d62c2c2d0d8d15fa56fd088`  
		Last Modified: Tue, 29 Mar 2022 16:38:39 GMT  
		Size: 41.4 MB (41439734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rakudo-star:alpine` - linux; arm64 variant v8

```console
$ docker pull rakudo-star@sha256:4632162902f25af4ba454294fbbcc314654d983f928d1beb7b89a2b755f7e9b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43948587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2ab290aa36dbd7f1734aff1542c5c407e9f5424ec27fd3b122ba14857d919df`
-	Default Command: `["raku"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:18 GMT
ADD file:3b8e0dac20ca40faf2aaf084b69476a222952f177c0e6ec90804a10c91a51feb in / 
# Tue, 29 Mar 2022 00:40:19 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 18:29:27 GMT
RUN addgroup -S raku && adduser -S raku -G raku
# Tue, 29 Mar 2022 18:29:28 GMT
ARG rakudo_version=2021.04
# Tue, 29 Mar 2022 18:29:29 GMT
ENV rakudo_version=2021.04
# Tue, 29 Mar 2022 18:51:11 GMT
RUN buildDeps='         bash         gcc         gnupg         libc-dev         make         perl     '         url="https://rakudo.org/dl/star/rakudo-star-${rakudo_version}.tar.gz"     keyserver='ha.pool.sks-keyservers.net'     keyfp='B6F697742EFCAF5F23CE51D5031D65902E840821'     tmpdir="$(mktemp -d)"     && set -eux     && export GNUPGHOME="$tmpdir"     && apk add --no-cache --virtual .build-deps $buildDeps     && mkdir ${tmpdir}/rakudo         && wget ${url}.asc -O ${tmpdir}/rakudo.tar.gz.asc     && wget $url -O ${tmpdir}/rakudo.tar.gz     && gpg --batch --keyserver $keyserver --recv-keys $keyfp     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && bash bin/rstar install -p /usr     )     && rm -rf $tmpdir     && apk del --no-network .build-deps
# Tue, 29 Mar 2022 18:51:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/core/bin:/usr/share/perl6/site/bin:/usr/share/perl6/vendor/bin
# Tue, 29 Mar 2022 18:51:12 GMT
CMD ["raku"]
```

-	Layers:
	-	`sha256:4e7dd0becbc2dc968b69cba46c81a25fa500c88a644832ce17a5bb090925fa79`  
		Last Modified: Tue, 29 Mar 2022 00:41:37 GMT  
		Size: 2.7 MB (2720845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44540bca26eea25dec5c60a3dd735ae7c3ba058f4b32af8145ff9c902a36af01`  
		Last Modified: Tue, 29 Mar 2022 18:51:40 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8d037475d3940d9574b6ce8bd92cd1751526337369b678d4a6e4d54814ebad`  
		Last Modified: Tue, 29 Mar 2022 18:51:47 GMT  
		Size: 41.2 MB (41226513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rakudo-star:latest`

```console
$ docker pull rakudo-star@sha256:0b3c1828ad1b75ef687006f06bca5a705a48c933aa29a3feb171f250f981adbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rakudo-star:latest` - linux; amd64

```console
$ docker pull rakudo-star@sha256:ceada0ae4dbbe68e2fd74e01682602f7b28d7fd39131661f3021184803daaa4e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.9 MB (161880457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5bdf30dc23493f54a3cede4bebbb7f410a62126f3dc2cc726e515aaa06c3a73`
-	Default Command: `["raku"]`

```dockerfile
# Thu, 17 Mar 2022 04:04:10 GMT
ADD file:28eba36c2d43c343d9dfd5ace80db0043e1f92aa3afb4aa95d6cbb54d7e6efef in / 
# Thu, 17 Mar 2022 04:04:11 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 06:31:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 06:32:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Mar 2022 06:32:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 23:50:26 GMT
MAINTAINER Rob Hoelz
# Sat, 19 Mar 2022 23:50:27 GMT
RUN groupadd -r raku && useradd -m -r -g raku raku
# Sat, 19 Mar 2022 23:50:27 GMT
ARG rakudo_version=2021.04
# Sat, 19 Mar 2022 23:50:27 GMT
ENV rakudo_version=2021.04
# Sat, 19 Mar 2022 23:59:29 GMT
RUN buildDeps='         gcc         libc6-dev         make     '         url="https://rakudo.org/dl/star/rakudo-star-${rakudo_version}.tar.gz"     keyserver='ha.pool.sks-keyservers.net'     keyfp='B6F697742EFCAF5F23CE51D5031D65902E840821'     tmpdir="$(mktemp -d)"     && set -eux     && export GNUPGHOME="$tmpdir"     && apt-get update     && apt-get install -y --no-install-recommends $buildDeps     && rm -rf /var/lib/apt/lists/*     && mkdir ${tmpdir}/rakudo         && curl -fsSL ${url}.asc -o ${tmpdir}/rakudo.tar.gz.asc     && curl -fsSL $url -o ${tmpdir}/rakudo.tar.gz     && gpg --batch --keyserver $keyserver --recv-keys $keyfp     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && bash bin/rstar install -p /usr     )     && rm -rf $tmpdir     && apt-get purge -y --auto-remove $buildDeps
# Sat, 19 Mar 2022 23:59:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/core/bin:/usr/share/perl6/site/bin:/usr/share/perl6/vendor/bin
# Sat, 19 Mar 2022 23:59:30 GMT
CMD ["raku"]
```

-	Layers:
	-	`sha256:7d66b83ec869a899bc8364af9c9eb0f1a5ba6907f699ef52f3182e19e2598924`  
		Last Modified: Thu, 17 Mar 2022 04:10:29 GMT  
		Size: 50.4 MB (50437294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d88439e7b50a5f3923f67f432b6863c1e11adf4e45bf9740515d2cc01fd8e155`  
		Last Modified: Fri, 18 Mar 2022 07:04:47 GMT  
		Size: 7.8 MB (7834140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22360a9558f73f04bb5e4dbe6dbe1584cb913040ae66388a8db66fc2ed131002`  
		Last Modified: Fri, 18 Mar 2022 07:04:47 GMT  
		Size: 10.0 MB (9997260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f260dee23bc81622ef145aff36ad9816cca1c98bfa9361ad1bdf03c8975b104e`  
		Last Modified: Fri, 18 Mar 2022 07:05:07 GMT  
		Size: 51.8 MB (51843594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475e43b3b5843cc948933174e306b40c3e6957df2f13848c7ff5b77567937abe`  
		Last Modified: Sat, 19 Mar 2022 23:59:45 GMT  
		Size: 4.1 KB (4131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a51ab46ee5ec98ff33259d4cd5ef44fd3d8b2faffe5b825e45a748769f5fa57`  
		Last Modified: Sat, 19 Mar 2022 23:59:52 GMT  
		Size: 41.8 MB (41764038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rakudo-star:latest` - linux; arm64 variant v8

```console
$ docker pull rakudo-star@sha256:c7640cf9677f0de998ac75be7630c5caee0485f046c695b89b524622789acf8e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.7 MB (159719848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:287a097958254ce78bf5306d5fa2326dbdceefae89605c92017f5f579367148f`
-	Default Command: `["raku"]`

```dockerfile
# Thu, 17 Mar 2022 03:22:08 GMT
ADD file:37cabd1fec04269c22fc158f62ce5bc655934f2e58fb1ff3a1e366a33ba9bc18 in / 
# Thu, 17 Mar 2022 03:22:09 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 22:12:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 22:12:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Mar 2022 22:12:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 01:27:48 GMT
MAINTAINER Rob Hoelz
# Sat, 19 Mar 2022 01:27:49 GMT
RUN groupadd -r raku && useradd -m -r -g raku raku
# Sat, 19 Mar 2022 01:27:49 GMT
ARG rakudo_version=2021.04
# Sat, 19 Mar 2022 01:27:50 GMT
ENV rakudo_version=2021.04
# Sat, 19 Mar 2022 01:37:47 GMT
RUN buildDeps='         gcc         libc6-dev         make     '         url="https://rakudo.org/dl/star/rakudo-star-${rakudo_version}.tar.gz"     keyserver='ha.pool.sks-keyservers.net'     keyfp='B6F697742EFCAF5F23CE51D5031D65902E840821'     tmpdir="$(mktemp -d)"     && set -eux     && export GNUPGHOME="$tmpdir"     && apt-get update     && apt-get install -y --no-install-recommends $buildDeps     && rm -rf /var/lib/apt/lists/*     && mkdir ${tmpdir}/rakudo         && curl -fsSL ${url}.asc -o ${tmpdir}/rakudo.tar.gz.asc     && curl -fsSL $url -o ${tmpdir}/rakudo.tar.gz     && gpg --batch --keyserver $keyserver --recv-keys $keyfp     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && bash bin/rstar install -p /usr     )     && rm -rf $tmpdir     && apt-get purge -y --auto-remove $buildDeps
# Sat, 19 Mar 2022 01:37:47 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/core/bin:/usr/share/perl6/site/bin:/usr/share/perl6/vendor/bin
# Sat, 19 Mar 2022 01:37:48 GMT
CMD ["raku"]
```

-	Layers:
	-	`sha256:3996f04b7c6c17d8b25c04c7287353b896b4a0b10ab440f47d00573a7d5c3e17`  
		Last Modified: Thu, 17 Mar 2022 03:28:59 GMT  
		Size: 49.2 MB (49222993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80907b498681187ef4aa817ec6f39ba351e376afbb4fcf4415841ab9015cfc59`  
		Last Modified: Thu, 17 Mar 2022 22:22:15 GMT  
		Size: 7.7 MB (7695349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8327dc7899c1a628cf11f95bb594fca3c86e45d1f4f0eb73d2ba9058eba5927`  
		Last Modified: Thu, 17 Mar 2022 22:22:15 GMT  
		Size: 9.8 MB (9767203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1431347b40fe69ed685917a6ef1b8c28d5de6147f3c62ea11a1951ead75ccdd`  
		Last Modified: Thu, 17 Mar 2022 22:22:34 GMT  
		Size: 52.2 MB (52174886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fee11304a3fc0820f4b5dc6faa346614e1858d5f1ad4b80dc94e63ab3acdae1`  
		Last Modified: Sat, 19 Mar 2022 01:38:18 GMT  
		Size: 4.0 KB (4008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5cc29dda37328d52a7bd774bda0ccbf92f4f71540767aaa38493b4e0610d357`  
		Last Modified: Sat, 19 Mar 2022 01:38:27 GMT  
		Size: 40.9 MB (40855409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
