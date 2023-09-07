<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `rakudo-star`

-	[`rakudo-star:2023.08`](#rakudo-star202308)
-	[`rakudo-star:2023.08-alpine`](#rakudo-star202308-alpine)
-	[`rakudo-star:alpine`](#rakudo-staralpine)
-	[`rakudo-star:latest`](#rakudo-starlatest)

## `rakudo-star:2023.08`

```console
$ docker pull rakudo-star@sha256:867216eba9dbc9313e09810210a231918f14f975643f8c31a6a2a87c01dc78a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rakudo-star:2023.08` - linux; amd64

```console
$ docker pull rakudo-star@sha256:b84c4f5dc8cca86b4259f749894fd705afe5a15b03eac8ba910fc444f8e4e7d8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.3 MB (176334697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:058e6ee667735d0b3f6ed1bfd2523d14124a3a047f97ce27cf77e8a99cda7c31`
-	Default Command: `["raku"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:30 GMT
ADD file:3a6d159d80cb8abfacda5873c243a6ae635ff603708febc4df51f8eec26d3de7 in / 
# Wed, 16 Aug 2023 00:59:31 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 06:57:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 06:58:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:20:36 GMT
MAINTAINER Rob Hoelz
# Thu, 17 Aug 2023 01:20:36 GMT
RUN groupadd -r raku && useradd -m -r -g raku raku
# Fri, 25 Aug 2023 21:20:09 GMT
ARG rakudo_version=2023.08-01
# Fri, 25 Aug 2023 21:20:09 GMT
ENV rakudo_version=2023.08-01
# Fri, 25 Aug 2023 21:41:27 GMT
RUN buildDeps='         gcc         libc6-dev         make     '         url="https://rakudo.org/dl/star/rakudo-star-${rakudo_version}.tar.gz"     keyfp="3E7E3C6EAF916676AC549285A2919382E961E2EE"     pubkeyurl="https://rakudo.org/keys/rakudo_github_automation-${keyfp}.asc"     tmpdir="$(mktemp -d)"     && set -eux     && export GNUPGHOME="$tmpdir/gnupg"     && mkdir $GNUPGHOME     && apt-get update     && apt-get install -y --no-install-recommends $buildDeps     && rm -rf /var/lib/apt/lists/*     && mkdir ${tmpdir}/rakudo         && curl -fsSL ${url}.asc -o ${tmpdir}/rakudo.tar.gz.asc     && curl -fsSL $url -o ${tmpdir}/rakudo.tar.gz     && curl -fsSL $pubkeyurl -o ${tmpdir}/key.asc         && gpg --batch --import ${tmpdir}/key.asc     && gpg --batch --export $keyfp > ${tmpdir}/${keyfp}.asc     && rm -rf $GNUPGHOME     && mkdir $GNUPGHOME     && gpg --batch --import ${tmpdir}/${keyfp}.asc     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && bash bin/rstar install -p /usr     )     && rm -rf $tmpdir     && apt-get purge -y --auto-remove $buildDeps
# Fri, 25 Aug 2023 21:41:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/core/bin:/usr/share/perl6/site/bin:/usr/share/perl6/vendor/bin
# Fri, 25 Aug 2023 21:41:27 GMT
CMD ["raku"]
```

-	Layers:
	-	`sha256:de4cac68b6165c40cf6f8b30417948c31be03a968e233e55ee40221553a5e570`  
		Last Modified: Wed, 16 Aug 2023 01:04:06 GMT  
		Size: 49.6 MB (49557399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d31b0195ec5f04dfc78eca9d73b5d223fc36a29f54ee888bc4e0615b5839e692`  
		Last Modified: Wed, 16 Aug 2023 07:12:39 GMT  
		Size: 24.0 MB (24030511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b1fd34c30b75e7edb20c2fd09a9862697f302ef9ae357e521ef3c84d5534e3f`  
		Last Modified: Wed, 16 Aug 2023 07:12:59 GMT  
		Size: 64.1 MB (64112171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8b4a82ad91cd94dbc2d8a6f268a6c229225183d3fdb33360c3d565e895eedf`  
		Last Modified: Thu, 17 Aug 2023 01:40:40 GMT  
		Size: 3.3 KB (3292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a70a15c69ac4f47066ea37009e89b1aa989bddc79dce27876f201ea5ebc8e6`  
		Last Modified: Fri, 25 Aug 2023 22:04:12 GMT  
		Size: 38.6 MB (38631324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rakudo-star:2023.08` - linux; arm64 variant v8

```console
$ docker pull rakudo-star@sha256:634fa8227e018b89293b6164f38d967565a86ed800af0d6cfcae7cbb81930ee3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.6 MB (175633510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c9838e2a436b7190930b2ca3d18c5f385e6532c2d34745751c5ba2d041e0d94`
-	Default Command: `["raku"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:31 GMT
ADD file:f9dd2b1cc0ba261acd8a3e500c54f6b6e0a46131a32988bfd71cf3c6fc5a7d13 in / 
# Thu, 07 Sep 2023 00:39:32 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:51:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 06:51:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 17:48:11 GMT
MAINTAINER Rob Hoelz
# Thu, 07 Sep 2023 17:48:12 GMT
RUN groupadd -r raku && useradd -m -r -g raku raku
# Thu, 07 Sep 2023 17:48:12 GMT
ARG rakudo_version=2023.08-01
# Thu, 07 Sep 2023 17:48:12 GMT
ENV rakudo_version=2023.08-01
# Thu, 07 Sep 2023 18:07:36 GMT
RUN buildDeps='         gcc         libc6-dev         make     '         url="https://rakudo.org/dl/star/rakudo-star-${rakudo_version}.tar.gz"     keyfp="3E7E3C6EAF916676AC549285A2919382E961E2EE"     pubkeyurl="https://rakudo.org/keys/rakudo_github_automation-${keyfp}.asc"     tmpdir="$(mktemp -d)"     && set -eux     && export GNUPGHOME="$tmpdir/gnupg"     && mkdir $GNUPGHOME     && apt-get update     && apt-get install -y --no-install-recommends $buildDeps     && rm -rf /var/lib/apt/lists/*     && mkdir ${tmpdir}/rakudo         && curl -fsSL ${url}.asc -o ${tmpdir}/rakudo.tar.gz.asc     && curl -fsSL $url -o ${tmpdir}/rakudo.tar.gz     && curl -fsSL $pubkeyurl -o ${tmpdir}/key.asc         && gpg --batch --import ${tmpdir}/key.asc     && gpg --batch --export $keyfp > ${tmpdir}/${keyfp}.asc     && rm -rf $GNUPGHOME     && mkdir $GNUPGHOME     && gpg --batch --import ${tmpdir}/${keyfp}.asc     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && bash bin/rstar install -p /usr     )     && rm -rf $tmpdir     && apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 18:07:37 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/core/bin:/usr/share/perl6/site/bin:/usr/share/perl6/vendor/bin
# Thu, 07 Sep 2023 18:07:37 GMT
CMD ["raku"]
```

-	Layers:
	-	`sha256:fa34261389f3dee2ecffe9bfe38ae7fd05a1908e98a7486354905aee0f648a6e`  
		Last Modified: Thu, 07 Sep 2023 00:42:39 GMT  
		Size: 49.6 MB (49590783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993525952a483617183655b735562fd3eee4b3a85a472e3dc3c79a258adca100`  
		Last Modified: Thu, 07 Sep 2023 06:59:20 GMT  
		Size: 23.6 MB (23570086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12916f73f9de8e251c4eb4f2d079fa6cd63205b7ba8a7bd88e1f9446105e9ef1`  
		Last Modified: Thu, 07 Sep 2023 06:59:37 GMT  
		Size: 64.0 MB (63988504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86cce8bc692ed8213f7c102ef991279f3ab06ab9575a7d0906f95ea84cdae87`  
		Last Modified: Thu, 07 Sep 2023 18:07:59 GMT  
		Size: 3.3 KB (3291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0325c85e100600f7b4ddebe441b872d2883006af8304a7634802ce5be19c8459`  
		Last Modified: Thu, 07 Sep 2023 18:08:05 GMT  
		Size: 38.5 MB (38480846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rakudo-star:2023.08-alpine`

```console
$ docker pull rakudo-star@sha256:9aa1048e7b1c2f04b77b7ae88096e571506fd9b75e07891eb62b2aaa1af30bca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rakudo-star:2023.08-alpine` - linux; amd64

```console
$ docker pull rakudo-star@sha256:95a7188cc5143e3d419239f524589ff2c0474516df6059b8f4cdeea1bd3cc687
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (42044093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:367ee6cadfb0a141cc9a3c774d04906bf8d6f5e409f1b5b48131bbce693d5ce1`
-	Default Command: `["raku"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 03:06:27 GMT
RUN addgroup -S raku && adduser -S raku -G raku
# Fri, 25 Aug 2023 21:41:33 GMT
ARG rakudo_version=2023.08-01
# Fri, 25 Aug 2023 21:41:33 GMT
ENV rakudo_version=2023.08-01
# Fri, 25 Aug 2023 22:03:48 GMT
RUN buildDeps='         bash         gcc         gnupg         libc-dev         make         perl     '         url="https://rakudo.org/dl/star/rakudo-star-${rakudo_version}.tar.gz"     keyfp="3E7E3C6EAF916676AC549285A2919382E961E2EE"     pubkeyurl="https://rakudo.org/keys/rakudo_github_automation-${keyfp}.asc"     tmpdir="$(mktemp -d)"     && set -eux     && export GNUPGHOME="${tmpdir}/gnupg"     && mkdir $GNUPGHOME     && apk add --no-cache --virtual .build-deps $buildDeps     && apk add --no-cache readline     && mkdir ${tmpdir}/rakudo         && wget ${url}.asc -O ${tmpdir}/rakudo.tar.gz.asc     && wget $url -O ${tmpdir}/rakudo.tar.gz     && wget $pubkeyurl -O ${tmpdir}/key.asc         && gpg --batch --import ${tmpdir}/key.asc     && gpg --batch --export $keyfp > ${tmpdir}/${keyfp}.asc     && rm -rf $GNUPGHOME     && mkdir $GNUPGHOME     && gpg --batch --import ${tmpdir}/${keyfp}.asc     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && bash bin/rstar install -p /usr     )     && rm -rf $tmpdir     && apk del --no-network .build-deps
# Fri, 25 Aug 2023 22:03:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/core/bin:/usr/share/perl6/site/bin:/usr/share/perl6/vendor/bin
# Fri, 25 Aug 2023 22:03:49 GMT
CMD ["raku"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e8f9303d288bcbaaed127b89d9cda3acff18d9e2046758fef4faf5f87f213e0`  
		Last Modified: Wed, 09 Aug 2023 03:31:13 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3601f8cc7954be23c366d3e68583424c5f0a79ea3595e1632f461b5c4fab808`  
		Last Modified: Fri, 25 Aug 2023 22:04:28 GMT  
		Size: 38.6 MB (38641215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rakudo-star:2023.08-alpine` - linux; arm64 variant v8

```console
$ docker pull rakudo-star@sha256:9f35737048c6715a68e997cd302c0f6d099c169d808465a4cb4d8e4058c7f9b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.8 MB (41830503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8982adb13ea28bf3efed7b1b06f21d28a2794541720e1366abdbe66c17523f6b`
-	Default Command: `["raku"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 03:38:10 GMT
RUN addgroup -S raku && adduser -S raku -G raku
# Fri, 25 Aug 2023 22:21:50 GMT
ARG rakudo_version=2023.08-01
# Fri, 25 Aug 2023 22:21:50 GMT
ENV rakudo_version=2023.08-01
# Fri, 25 Aug 2023 22:40:57 GMT
RUN buildDeps='         bash         gcc         gnupg         libc-dev         make         perl     '         url="https://rakudo.org/dl/star/rakudo-star-${rakudo_version}.tar.gz"     keyfp="3E7E3C6EAF916676AC549285A2919382E961E2EE"     pubkeyurl="https://rakudo.org/keys/rakudo_github_automation-${keyfp}.asc"     tmpdir="$(mktemp -d)"     && set -eux     && export GNUPGHOME="${tmpdir}/gnupg"     && mkdir $GNUPGHOME     && apk add --no-cache --virtual .build-deps $buildDeps     && apk add --no-cache readline     && mkdir ${tmpdir}/rakudo         && wget ${url}.asc -O ${tmpdir}/rakudo.tar.gz.asc     && wget $url -O ${tmpdir}/rakudo.tar.gz     && wget $pubkeyurl -O ${tmpdir}/key.asc         && gpg --batch --import ${tmpdir}/key.asc     && gpg --batch --export $keyfp > ${tmpdir}/${keyfp}.asc     && rm -rf $GNUPGHOME     && mkdir $GNUPGHOME     && gpg --batch --import ${tmpdir}/${keyfp}.asc     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && bash bin/rstar install -p /usr     )     && rm -rf $tmpdir     && apk del --no-network .build-deps
# Fri, 25 Aug 2023 22:40:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/core/bin:/usr/share/perl6/site/bin:/usr/share/perl6/vendor/bin
# Fri, 25 Aug 2023 22:40:58 GMT
CMD ["raku"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1129ca0492a22dc461f59c1bd3dde511e14511245112b1df79afe64c570be804`  
		Last Modified: Wed, 09 Aug 2023 03:58:40 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8456908e2dbdbb25110057bc1b330b8a7843ba911b880f6f435c16ebbed309`  
		Last Modified: Fri, 25 Aug 2023 22:41:41 GMT  
		Size: 38.5 MB (38498472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rakudo-star:alpine`

```console
$ docker pull rakudo-star@sha256:9aa1048e7b1c2f04b77b7ae88096e571506fd9b75e07891eb62b2aaa1af30bca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rakudo-star:alpine` - linux; amd64

```console
$ docker pull rakudo-star@sha256:95a7188cc5143e3d419239f524589ff2c0474516df6059b8f4cdeea1bd3cc687
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (42044093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:367ee6cadfb0a141cc9a3c774d04906bf8d6f5e409f1b5b48131bbce693d5ce1`
-	Default Command: `["raku"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 03:06:27 GMT
RUN addgroup -S raku && adduser -S raku -G raku
# Fri, 25 Aug 2023 21:41:33 GMT
ARG rakudo_version=2023.08-01
# Fri, 25 Aug 2023 21:41:33 GMT
ENV rakudo_version=2023.08-01
# Fri, 25 Aug 2023 22:03:48 GMT
RUN buildDeps='         bash         gcc         gnupg         libc-dev         make         perl     '         url="https://rakudo.org/dl/star/rakudo-star-${rakudo_version}.tar.gz"     keyfp="3E7E3C6EAF916676AC549285A2919382E961E2EE"     pubkeyurl="https://rakudo.org/keys/rakudo_github_automation-${keyfp}.asc"     tmpdir="$(mktemp -d)"     && set -eux     && export GNUPGHOME="${tmpdir}/gnupg"     && mkdir $GNUPGHOME     && apk add --no-cache --virtual .build-deps $buildDeps     && apk add --no-cache readline     && mkdir ${tmpdir}/rakudo         && wget ${url}.asc -O ${tmpdir}/rakudo.tar.gz.asc     && wget $url -O ${tmpdir}/rakudo.tar.gz     && wget $pubkeyurl -O ${tmpdir}/key.asc         && gpg --batch --import ${tmpdir}/key.asc     && gpg --batch --export $keyfp > ${tmpdir}/${keyfp}.asc     && rm -rf $GNUPGHOME     && mkdir $GNUPGHOME     && gpg --batch --import ${tmpdir}/${keyfp}.asc     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && bash bin/rstar install -p /usr     )     && rm -rf $tmpdir     && apk del --no-network .build-deps
# Fri, 25 Aug 2023 22:03:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/core/bin:/usr/share/perl6/site/bin:/usr/share/perl6/vendor/bin
# Fri, 25 Aug 2023 22:03:49 GMT
CMD ["raku"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e8f9303d288bcbaaed127b89d9cda3acff18d9e2046758fef4faf5f87f213e0`  
		Last Modified: Wed, 09 Aug 2023 03:31:13 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3601f8cc7954be23c366d3e68583424c5f0a79ea3595e1632f461b5c4fab808`  
		Last Modified: Fri, 25 Aug 2023 22:04:28 GMT  
		Size: 38.6 MB (38641215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rakudo-star:alpine` - linux; arm64 variant v8

```console
$ docker pull rakudo-star@sha256:9f35737048c6715a68e997cd302c0f6d099c169d808465a4cb4d8e4058c7f9b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.8 MB (41830503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8982adb13ea28bf3efed7b1b06f21d28a2794541720e1366abdbe66c17523f6b`
-	Default Command: `["raku"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 03:38:10 GMT
RUN addgroup -S raku && adduser -S raku -G raku
# Fri, 25 Aug 2023 22:21:50 GMT
ARG rakudo_version=2023.08-01
# Fri, 25 Aug 2023 22:21:50 GMT
ENV rakudo_version=2023.08-01
# Fri, 25 Aug 2023 22:40:57 GMT
RUN buildDeps='         bash         gcc         gnupg         libc-dev         make         perl     '         url="https://rakudo.org/dl/star/rakudo-star-${rakudo_version}.tar.gz"     keyfp="3E7E3C6EAF916676AC549285A2919382E961E2EE"     pubkeyurl="https://rakudo.org/keys/rakudo_github_automation-${keyfp}.asc"     tmpdir="$(mktemp -d)"     && set -eux     && export GNUPGHOME="${tmpdir}/gnupg"     && mkdir $GNUPGHOME     && apk add --no-cache --virtual .build-deps $buildDeps     && apk add --no-cache readline     && mkdir ${tmpdir}/rakudo         && wget ${url}.asc -O ${tmpdir}/rakudo.tar.gz.asc     && wget $url -O ${tmpdir}/rakudo.tar.gz     && wget $pubkeyurl -O ${tmpdir}/key.asc         && gpg --batch --import ${tmpdir}/key.asc     && gpg --batch --export $keyfp > ${tmpdir}/${keyfp}.asc     && rm -rf $GNUPGHOME     && mkdir $GNUPGHOME     && gpg --batch --import ${tmpdir}/${keyfp}.asc     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && bash bin/rstar install -p /usr     )     && rm -rf $tmpdir     && apk del --no-network .build-deps
# Fri, 25 Aug 2023 22:40:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/core/bin:/usr/share/perl6/site/bin:/usr/share/perl6/vendor/bin
# Fri, 25 Aug 2023 22:40:58 GMT
CMD ["raku"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1129ca0492a22dc461f59c1bd3dde511e14511245112b1df79afe64c570be804`  
		Last Modified: Wed, 09 Aug 2023 03:58:40 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8456908e2dbdbb25110057bc1b330b8a7843ba911b880f6f435c16ebbed309`  
		Last Modified: Fri, 25 Aug 2023 22:41:41 GMT  
		Size: 38.5 MB (38498472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rakudo-star:latest`

```console
$ docker pull rakudo-star@sha256:867216eba9dbc9313e09810210a231918f14f975643f8c31a6a2a87c01dc78a5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rakudo-star:latest` - linux; amd64

```console
$ docker pull rakudo-star@sha256:b84c4f5dc8cca86b4259f749894fd705afe5a15b03eac8ba910fc444f8e4e7d8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.3 MB (176334697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:058e6ee667735d0b3f6ed1bfd2523d14124a3a047f97ce27cf77e8a99cda7c31`
-	Default Command: `["raku"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:30 GMT
ADD file:3a6d159d80cb8abfacda5873c243a6ae635ff603708febc4df51f8eec26d3de7 in / 
# Wed, 16 Aug 2023 00:59:31 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 06:57:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 06:58:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 01:20:36 GMT
MAINTAINER Rob Hoelz
# Thu, 17 Aug 2023 01:20:36 GMT
RUN groupadd -r raku && useradd -m -r -g raku raku
# Fri, 25 Aug 2023 21:20:09 GMT
ARG rakudo_version=2023.08-01
# Fri, 25 Aug 2023 21:20:09 GMT
ENV rakudo_version=2023.08-01
# Fri, 25 Aug 2023 21:41:27 GMT
RUN buildDeps='         gcc         libc6-dev         make     '         url="https://rakudo.org/dl/star/rakudo-star-${rakudo_version}.tar.gz"     keyfp="3E7E3C6EAF916676AC549285A2919382E961E2EE"     pubkeyurl="https://rakudo.org/keys/rakudo_github_automation-${keyfp}.asc"     tmpdir="$(mktemp -d)"     && set -eux     && export GNUPGHOME="$tmpdir/gnupg"     && mkdir $GNUPGHOME     && apt-get update     && apt-get install -y --no-install-recommends $buildDeps     && rm -rf /var/lib/apt/lists/*     && mkdir ${tmpdir}/rakudo         && curl -fsSL ${url}.asc -o ${tmpdir}/rakudo.tar.gz.asc     && curl -fsSL $url -o ${tmpdir}/rakudo.tar.gz     && curl -fsSL $pubkeyurl -o ${tmpdir}/key.asc         && gpg --batch --import ${tmpdir}/key.asc     && gpg --batch --export $keyfp > ${tmpdir}/${keyfp}.asc     && rm -rf $GNUPGHOME     && mkdir $GNUPGHOME     && gpg --batch --import ${tmpdir}/${keyfp}.asc     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && bash bin/rstar install -p /usr     )     && rm -rf $tmpdir     && apt-get purge -y --auto-remove $buildDeps
# Fri, 25 Aug 2023 21:41:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/core/bin:/usr/share/perl6/site/bin:/usr/share/perl6/vendor/bin
# Fri, 25 Aug 2023 21:41:27 GMT
CMD ["raku"]
```

-	Layers:
	-	`sha256:de4cac68b6165c40cf6f8b30417948c31be03a968e233e55ee40221553a5e570`  
		Last Modified: Wed, 16 Aug 2023 01:04:06 GMT  
		Size: 49.6 MB (49557399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d31b0195ec5f04dfc78eca9d73b5d223fc36a29f54ee888bc4e0615b5839e692`  
		Last Modified: Wed, 16 Aug 2023 07:12:39 GMT  
		Size: 24.0 MB (24030511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b1fd34c30b75e7edb20c2fd09a9862697f302ef9ae357e521ef3c84d5534e3f`  
		Last Modified: Wed, 16 Aug 2023 07:12:59 GMT  
		Size: 64.1 MB (64112171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8b4a82ad91cd94dbc2d8a6f268a6c229225183d3fdb33360c3d565e895eedf`  
		Last Modified: Thu, 17 Aug 2023 01:40:40 GMT  
		Size: 3.3 KB (3292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a70a15c69ac4f47066ea37009e89b1aa989bddc79dce27876f201ea5ebc8e6`  
		Last Modified: Fri, 25 Aug 2023 22:04:12 GMT  
		Size: 38.6 MB (38631324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rakudo-star:latest` - linux; arm64 variant v8

```console
$ docker pull rakudo-star@sha256:634fa8227e018b89293b6164f38d967565a86ed800af0d6cfcae7cbb81930ee3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.6 MB (175633510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c9838e2a436b7190930b2ca3d18c5f385e6532c2d34745751c5ba2d041e0d94`
-	Default Command: `["raku"]`

```dockerfile
# Thu, 07 Sep 2023 00:39:31 GMT
ADD file:f9dd2b1cc0ba261acd8a3e500c54f6b6e0a46131a32988bfd71cf3c6fc5a7d13 in / 
# Thu, 07 Sep 2023 00:39:32 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:51:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 06:51:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 17:48:11 GMT
MAINTAINER Rob Hoelz
# Thu, 07 Sep 2023 17:48:12 GMT
RUN groupadd -r raku && useradd -m -r -g raku raku
# Thu, 07 Sep 2023 17:48:12 GMT
ARG rakudo_version=2023.08-01
# Thu, 07 Sep 2023 17:48:12 GMT
ENV rakudo_version=2023.08-01
# Thu, 07 Sep 2023 18:07:36 GMT
RUN buildDeps='         gcc         libc6-dev         make     '         url="https://rakudo.org/dl/star/rakudo-star-${rakudo_version}.tar.gz"     keyfp="3E7E3C6EAF916676AC549285A2919382E961E2EE"     pubkeyurl="https://rakudo.org/keys/rakudo_github_automation-${keyfp}.asc"     tmpdir="$(mktemp -d)"     && set -eux     && export GNUPGHOME="$tmpdir/gnupg"     && mkdir $GNUPGHOME     && apt-get update     && apt-get install -y --no-install-recommends $buildDeps     && rm -rf /var/lib/apt/lists/*     && mkdir ${tmpdir}/rakudo         && curl -fsSL ${url}.asc -o ${tmpdir}/rakudo.tar.gz.asc     && curl -fsSL $url -o ${tmpdir}/rakudo.tar.gz     && curl -fsSL $pubkeyurl -o ${tmpdir}/key.asc         && gpg --batch --import ${tmpdir}/key.asc     && gpg --batch --export $keyfp > ${tmpdir}/${keyfp}.asc     && rm -rf $GNUPGHOME     && mkdir $GNUPGHOME     && gpg --batch --import ${tmpdir}/${keyfp}.asc     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && bash bin/rstar install -p /usr     )     && rm -rf $tmpdir     && apt-get purge -y --auto-remove $buildDeps
# Thu, 07 Sep 2023 18:07:37 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/core/bin:/usr/share/perl6/site/bin:/usr/share/perl6/vendor/bin
# Thu, 07 Sep 2023 18:07:37 GMT
CMD ["raku"]
```

-	Layers:
	-	`sha256:fa34261389f3dee2ecffe9bfe38ae7fd05a1908e98a7486354905aee0f648a6e`  
		Last Modified: Thu, 07 Sep 2023 00:42:39 GMT  
		Size: 49.6 MB (49590783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993525952a483617183655b735562fd3eee4b3a85a472e3dc3c79a258adca100`  
		Last Modified: Thu, 07 Sep 2023 06:59:20 GMT  
		Size: 23.6 MB (23570086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12916f73f9de8e251c4eb4f2d079fa6cd63205b7ba8a7bd88e1f9446105e9ef1`  
		Last Modified: Thu, 07 Sep 2023 06:59:37 GMT  
		Size: 64.0 MB (63988504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86cce8bc692ed8213f7c102ef991279f3ab06ab9575a7d0906f95ea84cdae87`  
		Last Modified: Thu, 07 Sep 2023 18:07:59 GMT  
		Size: 3.3 KB (3291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0325c85e100600f7b4ddebe441b872d2883006af8304a7634802ce5be19c8459`  
		Last Modified: Thu, 07 Sep 2023 18:08:05 GMT  
		Size: 38.5 MB (38480846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
