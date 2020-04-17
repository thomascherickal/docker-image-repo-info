<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `rakudo-star`

-	[`rakudo-star:2019.03`](#rakudo-star201903)
-	[`rakudo-star:2019.03-alpine`](#rakudo-star201903-alpine)
-	[`rakudo-star:alpine`](#rakudo-staralpine)
-	[`rakudo-star:latest`](#rakudo-starlatest)

## `rakudo-star:2019.03`

```console
$ docker pull rakudo-star@sha256:3c6f0fa6096c13668e5686c21366a0b914168ef52d42e64cc33b4222d75efdcf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `rakudo-star:2019.03` - linux; amd64

```console
$ docker pull rakudo-star@sha256:e86ce9ece60f92e006a82423674d171c4b2ef78d6d757a187eab7c15a73c2c59
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.2 MB (138195676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90556b8ba3af9a3af75c15fb4a6f3b60e5f4108ce23cecf55a929c135483f854`
-	Default Command: `["perl6"]`

```dockerfile
# Tue, 31 Mar 2020 01:23:50 GMT
ADD file:774b5e2033bb42ad97daa64267a5f041124cc0b05ec0198f1b5578ceea5a48e4 in / 
# Tue, 31 Mar 2020 01:23:51 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 02:06:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 02:06:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Mar 2020 02:07:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Apr 2020 01:30:23 GMT
MAINTAINER Rob Hoelz
# Wed, 01 Apr 2020 01:30:24 GMT
RUN groupadd -r perl6 && useradd -r -g perl6 perl6
# Wed, 01 Apr 2020 01:30:24 GMT
ARG rakudo_version=2019.03
# Wed, 01 Apr 2020 01:30:24 GMT
ENV rakudo_version=2019.03
# Wed, 01 Apr 2020 01:51:22 GMT
RUN buildDeps='         gcc         libc6-dev         libencode-perl         make     '         url="https://rakudostar.com/files/star/rakudo-star-${rakudo_version}.tar.gz"     keyserver='ha.pool.sks-keyservers.net'     keyfp='ECF8B611205B447E091246AF959E3D6197190DD5 7A6C9EB8809CFEAF0ED4E09F18C438E6FF24326D'     tmpdir="$(mktemp -d)"     && set -x     && export GNUPGHOME="$tmpdir"     && apt-get update     && apt-get --yes install --no-install-recommends $buildDeps     && rm -rf /var/lib/apt/lists/*     && mkdir ${tmpdir}/rakudo         && curl -fsSL ${url}.asc -o ${tmpdir}/rakudo.tar.gz.asc     && curl -fsSL $url -o ${tmpdir}/rakudo.tar.gz     && gpg --batch --keyserver $keyserver --recv-keys $keyfp     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && perl Configure.pl --prefix=/usr --gen-moar         && make install     )     && rm -rf $tmpdir     && apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Apr 2020 01:51:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/site/bin
# Wed, 01 Apr 2020 01:51:22 GMT
CMD ["perl6"]
```

-	Layers:
	-	`sha256:56da78ce36e97a8ba1f860575bb1422d1cb6ab4dade70b06ddf1651302dde955`  
		Last Modified: Tue, 31 Mar 2020 01:29:15 GMT  
		Size: 45.4 MB (45375928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbfe0f13ac4531fb6d077fda0e94ced4b9ed8a354c54b4efced9b7755d3f39d1`  
		Last Modified: Tue, 31 Mar 2020 02:12:44 GMT  
		Size: 10.8 MB (10797329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6254ff6d0e6052b7bead70e37703002eda28ac40f9a1167ea9bf813bf9c17d7f`  
		Last Modified: Tue, 31 Mar 2020 02:12:43 GMT  
		Size: 4.3 MB (4340113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e1e13bd9f6c381f158a5366b3eff242e8b4a4decfa940e915b1d5705ef4a28`  
		Last Modified: Tue, 31 Mar 2020 02:12:58 GMT  
		Size: 50.1 MB (50071604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae38a9146e7236ea4613bb440a10f063041d4843da7fe6e8b47897d56f48d16`  
		Last Modified: Wed, 01 Apr 2020 01:51:42 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b40382bb51aa4d18a3bdbb4ec32dfc8629342343aeb675a617c6050b51c3cd12`  
		Last Modified: Wed, 01 Apr 2020 01:51:49 GMT  
		Size: 27.6 MB (27608935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rakudo-star:2019.03` - linux; arm64 variant v8

```console
$ docker pull rakudo-star@sha256:cef53b2c6823f79b471ae230ef0848d8d1bed33dace8e955db47bfcc4e55417b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.3 MB (132348626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9195f2d025ede94e1d23632dcbebb91052e3a97961e32ebf0bbf147f1233e3d6`
-	Default Command: `["perl6"]`

```dockerfile
# Thu, 16 Apr 2020 02:44:49 GMT
ADD file:6d09304a2db2752e78b9ce9610594102dc756aa4cd210f85bbfa21105c7dd88f in / 
# Thu, 16 Apr 2020 02:44:52 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 03:21:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 03:21:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 03:22:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 23:29:18 GMT
MAINTAINER Rob Hoelz
# Thu, 16 Apr 2020 23:29:21 GMT
RUN groupadd -r perl6 && useradd -r -g perl6 perl6
# Thu, 16 Apr 2020 23:29:22 GMT
ARG rakudo_version=2019.03
# Thu, 16 Apr 2020 23:29:22 GMT
ENV rakudo_version=2019.03
# Fri, 17 Apr 2020 00:02:53 GMT
RUN buildDeps='         gcc         libc6-dev         libencode-perl         make     '         url="https://rakudostar.com/files/star/rakudo-star-${rakudo_version}.tar.gz"     keyserver='ha.pool.sks-keyservers.net'     keyfp='ECF8B611205B447E091246AF959E3D6197190DD5 7A6C9EB8809CFEAF0ED4E09F18C438E6FF24326D'     tmpdir="$(mktemp -d)"     && set -x     && export GNUPGHOME="$tmpdir"     && apt-get update     && apt-get --yes install --no-install-recommends $buildDeps     && rm -rf /var/lib/apt/lists/*     && mkdir ${tmpdir}/rakudo         && curl -fsSL ${url}.asc -o ${tmpdir}/rakudo.tar.gz.asc     && curl -fsSL $url -o ${tmpdir}/rakudo.tar.gz     && gpg --batch --keyserver $keyserver --recv-keys $keyfp     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && perl Configure.pl --prefix=/usr --gen-moar         && make install     )     && rm -rf $tmpdir     && apt-get purge -y --auto-remove $buildDeps
# Fri, 17 Apr 2020 00:02:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/site/bin
# Fri, 17 Apr 2020 00:02:56 GMT
CMD ["perl6"]
```

-	Layers:
	-	`sha256:65d54b492d599e7c785a582a0f70195e1f09f0886e54cb7788f1021f383eb4ed`  
		Last Modified: Thu, 16 Apr 2020 02:51:10 GMT  
		Size: 43.2 MB (43159230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be35cdee43e0bbb89c0867d201ff274ba25b6ea9bfe7f8f0c1d1d6de36ab08a`  
		Last Modified: Thu, 16 Apr 2020 03:30:52 GMT  
		Size: 9.7 MB (9748442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b803ac2c0e69edab9b8db20bee0f9dfc0191a7975c94d4d2ea0088d5a1759be8`  
		Last Modified: Thu, 16 Apr 2020 03:30:51 GMT  
		Size: 4.1 MB (4094379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56b7aa1f85cab0d60a62bc0cefa5ec56563f6681054c670ba97d559b4e7ba34`  
		Last Modified: Thu, 16 Apr 2020 03:31:12 GMT  
		Size: 48.0 MB (48027596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8879e78164926002c360f5a1b459371d03dc18960f7584a7031d0a3bfb9ce3c1`  
		Last Modified: Fri, 17 Apr 2020 00:03:24 GMT  
		Size: 1.8 KB (1770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9a195406aecaab594a9cc172eb55c70084efa1c9a20ced3c8ef74d9ce1d678`  
		Last Modified: Fri, 17 Apr 2020 00:03:34 GMT  
		Size: 27.3 MB (27317209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rakudo-star:2019.03-alpine`

```console
$ docker pull rakudo-star@sha256:5f04312a8e5805414aee67ddc4e61fd9ac3bccd9f68635410994dbbd16dee3d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `rakudo-star:2019.03-alpine` - linux; amd64

```console
$ docker pull rakudo-star@sha256:f455ce97de76478b475915eec6015157f91de4f8dd460efaee855bfa6abd6452
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.1 MB (30053992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ae6daca675b8efb6ebf8eb66736153b061e05b70fa06c98452183afb7d98e71`
-	Default Command: `["perl6"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 22:19:53 GMT
RUN addgroup -S perl6 && adduser -S perl6 -G perl6
# Thu, 23 Jan 2020 22:19:53 GMT
ARG rakudo_version=2019.03
# Thu, 23 Jan 2020 22:19:53 GMT
ENV rakudo_version=2019.03
# Thu, 23 Jan 2020 22:42:29 GMT
RUN buildDeps='         gnupg         perl         perl-encode         gcc         libc-dev         make     '         url="https://rakudostar.com/files/star/rakudo-star-${rakudo_version}.tar.gz"     keyserver='ha.pool.sks-keyservers.net'     keyfp='ECF8B611205B447E091246AF959E3D6197190DD5 7A6C9EB8809CFEAF0ED4E09F18C438E6FF24326D'     tmpdir="$(mktemp -d)"     && set -x     && export GNUPGHOME="$tmpdir"     && apk add --no-cache --virtual .build-deps $buildDeps     && mkdir ${tmpdir}/rakudo         && wget ${url}.asc -O ${tmpdir}/rakudo.tar.gz.asc     && wget $url -O ${tmpdir}/rakudo.tar.gz     && gpg --batch --keyserver $keyserver --recv-keys $keyfp     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && perl Configure.pl --prefix=/usr --gen-moar         && make install     )     && rm -rf $tmpdir     && apk del .build-deps
# Thu, 23 Jan 2020 22:42:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/site/bin
# Thu, 23 Jan 2020 22:42:29 GMT
CMD ["perl6"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fd1b886c5caeb9c93e822b4e5d00d482308c2da8170e1fba4668dae85670843`  
		Last Modified: Thu, 23 Jan 2020 22:42:41 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ec5e1f0e6dd884dfb59272800d2d689125b3b40246cefa48b1ef0018b5b752`  
		Last Modified: Thu, 23 Jan 2020 22:43:03 GMT  
		Size: 27.3 MB (27265770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rakudo-star:2019.03-alpine` - linux; arm64 variant v8

```console
$ docker pull rakudo-star@sha256:04d70f918da5d405ebe3cbc0d1a027d1e71c0bab07d76bf69c1fad978c90e2a7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.6 MB (29610759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:759165c83e3b8566c465cd83c1e5eb0931b32a9b71b9bcf152d440df1f19bcee`
-	Default Command: `["perl6"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:39 GMT
ADD file:bdfbd4b0dfb53eecc80bac65894d1e2fcfafb27dcf24ab019176e2c9f60b9a39 in / 
# Thu, 23 Jan 2020 16:54:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 22:23:24 GMT
RUN addgroup -S perl6 && adduser -S perl6 -G perl6
# Thu, 23 Jan 2020 22:23:24 GMT
ARG rakudo_version=2019.03
# Thu, 23 Jan 2020 22:23:25 GMT
ENV rakudo_version=2019.03
# Thu, 23 Jan 2020 23:00:31 GMT
RUN buildDeps='         gnupg         perl         perl-encode         gcc         libc-dev         make     '         url="https://rakudostar.com/files/star/rakudo-star-${rakudo_version}.tar.gz"     keyserver='ha.pool.sks-keyservers.net'     keyfp='ECF8B611205B447E091246AF959E3D6197190DD5 7A6C9EB8809CFEAF0ED4E09F18C438E6FF24326D'     tmpdir="$(mktemp -d)"     && set -x     && export GNUPGHOME="$tmpdir"     && apk add --no-cache --virtual .build-deps $buildDeps     && mkdir ${tmpdir}/rakudo         && wget ${url}.asc -O ${tmpdir}/rakudo.tar.gz.asc     && wget $url -O ${tmpdir}/rakudo.tar.gz     && gpg --batch --keyserver $keyserver --recv-keys $keyfp     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && perl Configure.pl --prefix=/usr --gen-moar         && make install     )     && rm -rf $tmpdir     && apk del .build-deps
# Thu, 23 Jan 2020 23:00:34 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/site/bin
# Thu, 23 Jan 2020 23:00:36 GMT
CMD ["perl6"]
```

-	Layers:
	-	`sha256:f07e4bcf42b862c240f4c00f2f7ed362d7d93ca15151de547beda593f3b669e5`  
		Last Modified: Thu, 23 Jan 2020 16:55:24 GMT  
		Size: 2.7 MB (2717732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f1177d01116b50429bddd1a67f102e1267c9a241e437f07bcf06a8bef85092`  
		Last Modified: Thu, 23 Jan 2020 23:00:49 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83b6b0cda86e0b249946b6e684d6e31b3780d49932c1360129c3b693316bfad9`  
		Last Modified: Thu, 23 Jan 2020 23:00:58 GMT  
		Size: 26.9 MB (26891740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rakudo-star:alpine`

```console
$ docker pull rakudo-star@sha256:5f04312a8e5805414aee67ddc4e61fd9ac3bccd9f68635410994dbbd16dee3d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `rakudo-star:alpine` - linux; amd64

```console
$ docker pull rakudo-star@sha256:f455ce97de76478b475915eec6015157f91de4f8dd460efaee855bfa6abd6452
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.1 MB (30053992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ae6daca675b8efb6ebf8eb66736153b061e05b70fa06c98452183afb7d98e71`
-	Default Command: `["perl6"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 22:19:53 GMT
RUN addgroup -S perl6 && adduser -S perl6 -G perl6
# Thu, 23 Jan 2020 22:19:53 GMT
ARG rakudo_version=2019.03
# Thu, 23 Jan 2020 22:19:53 GMT
ENV rakudo_version=2019.03
# Thu, 23 Jan 2020 22:42:29 GMT
RUN buildDeps='         gnupg         perl         perl-encode         gcc         libc-dev         make     '         url="https://rakudostar.com/files/star/rakudo-star-${rakudo_version}.tar.gz"     keyserver='ha.pool.sks-keyservers.net'     keyfp='ECF8B611205B447E091246AF959E3D6197190DD5 7A6C9EB8809CFEAF0ED4E09F18C438E6FF24326D'     tmpdir="$(mktemp -d)"     && set -x     && export GNUPGHOME="$tmpdir"     && apk add --no-cache --virtual .build-deps $buildDeps     && mkdir ${tmpdir}/rakudo         && wget ${url}.asc -O ${tmpdir}/rakudo.tar.gz.asc     && wget $url -O ${tmpdir}/rakudo.tar.gz     && gpg --batch --keyserver $keyserver --recv-keys $keyfp     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && perl Configure.pl --prefix=/usr --gen-moar         && make install     )     && rm -rf $tmpdir     && apk del .build-deps
# Thu, 23 Jan 2020 22:42:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/site/bin
# Thu, 23 Jan 2020 22:42:29 GMT
CMD ["perl6"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fd1b886c5caeb9c93e822b4e5d00d482308c2da8170e1fba4668dae85670843`  
		Last Modified: Thu, 23 Jan 2020 22:42:41 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ec5e1f0e6dd884dfb59272800d2d689125b3b40246cefa48b1ef0018b5b752`  
		Last Modified: Thu, 23 Jan 2020 22:43:03 GMT  
		Size: 27.3 MB (27265770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rakudo-star:alpine` - linux; arm64 variant v8

```console
$ docker pull rakudo-star@sha256:04d70f918da5d405ebe3cbc0d1a027d1e71c0bab07d76bf69c1fad978c90e2a7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.6 MB (29610759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:759165c83e3b8566c465cd83c1e5eb0931b32a9b71b9bcf152d440df1f19bcee`
-	Default Command: `["perl6"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:39 GMT
ADD file:bdfbd4b0dfb53eecc80bac65894d1e2fcfafb27dcf24ab019176e2c9f60b9a39 in / 
# Thu, 23 Jan 2020 16:54:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 22:23:24 GMT
RUN addgroup -S perl6 && adduser -S perl6 -G perl6
# Thu, 23 Jan 2020 22:23:24 GMT
ARG rakudo_version=2019.03
# Thu, 23 Jan 2020 22:23:25 GMT
ENV rakudo_version=2019.03
# Thu, 23 Jan 2020 23:00:31 GMT
RUN buildDeps='         gnupg         perl         perl-encode         gcc         libc-dev         make     '         url="https://rakudostar.com/files/star/rakudo-star-${rakudo_version}.tar.gz"     keyserver='ha.pool.sks-keyservers.net'     keyfp='ECF8B611205B447E091246AF959E3D6197190DD5 7A6C9EB8809CFEAF0ED4E09F18C438E6FF24326D'     tmpdir="$(mktemp -d)"     && set -x     && export GNUPGHOME="$tmpdir"     && apk add --no-cache --virtual .build-deps $buildDeps     && mkdir ${tmpdir}/rakudo         && wget ${url}.asc -O ${tmpdir}/rakudo.tar.gz.asc     && wget $url -O ${tmpdir}/rakudo.tar.gz     && gpg --batch --keyserver $keyserver --recv-keys $keyfp     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && perl Configure.pl --prefix=/usr --gen-moar         && make install     )     && rm -rf $tmpdir     && apk del .build-deps
# Thu, 23 Jan 2020 23:00:34 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/site/bin
# Thu, 23 Jan 2020 23:00:36 GMT
CMD ["perl6"]
```

-	Layers:
	-	`sha256:f07e4bcf42b862c240f4c00f2f7ed362d7d93ca15151de547beda593f3b669e5`  
		Last Modified: Thu, 23 Jan 2020 16:55:24 GMT  
		Size: 2.7 MB (2717732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33f1177d01116b50429bddd1a67f102e1267c9a241e437f07bcf06a8bef85092`  
		Last Modified: Thu, 23 Jan 2020 23:00:49 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83b6b0cda86e0b249946b6e684d6e31b3780d49932c1360129c3b693316bfad9`  
		Last Modified: Thu, 23 Jan 2020 23:00:58 GMT  
		Size: 26.9 MB (26891740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rakudo-star:latest`

```console
$ docker pull rakudo-star@sha256:3c6f0fa6096c13668e5686c21366a0b914168ef52d42e64cc33b4222d75efdcf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `rakudo-star:latest` - linux; amd64

```console
$ docker pull rakudo-star@sha256:e86ce9ece60f92e006a82423674d171c4b2ef78d6d757a187eab7c15a73c2c59
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.2 MB (138195676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90556b8ba3af9a3af75c15fb4a6f3b60e5f4108ce23cecf55a929c135483f854`
-	Default Command: `["perl6"]`

```dockerfile
# Tue, 31 Mar 2020 01:23:50 GMT
ADD file:774b5e2033bb42ad97daa64267a5f041124cc0b05ec0198f1b5578ceea5a48e4 in / 
# Tue, 31 Mar 2020 01:23:51 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 02:06:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 02:06:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Mar 2020 02:07:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Apr 2020 01:30:23 GMT
MAINTAINER Rob Hoelz
# Wed, 01 Apr 2020 01:30:24 GMT
RUN groupadd -r perl6 && useradd -r -g perl6 perl6
# Wed, 01 Apr 2020 01:30:24 GMT
ARG rakudo_version=2019.03
# Wed, 01 Apr 2020 01:30:24 GMT
ENV rakudo_version=2019.03
# Wed, 01 Apr 2020 01:51:22 GMT
RUN buildDeps='         gcc         libc6-dev         libencode-perl         make     '         url="https://rakudostar.com/files/star/rakudo-star-${rakudo_version}.tar.gz"     keyserver='ha.pool.sks-keyservers.net'     keyfp='ECF8B611205B447E091246AF959E3D6197190DD5 7A6C9EB8809CFEAF0ED4E09F18C438E6FF24326D'     tmpdir="$(mktemp -d)"     && set -x     && export GNUPGHOME="$tmpdir"     && apt-get update     && apt-get --yes install --no-install-recommends $buildDeps     && rm -rf /var/lib/apt/lists/*     && mkdir ${tmpdir}/rakudo         && curl -fsSL ${url}.asc -o ${tmpdir}/rakudo.tar.gz.asc     && curl -fsSL $url -o ${tmpdir}/rakudo.tar.gz     && gpg --batch --keyserver $keyserver --recv-keys $keyfp     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && perl Configure.pl --prefix=/usr --gen-moar         && make install     )     && rm -rf $tmpdir     && apt-get purge -y --auto-remove $buildDeps
# Wed, 01 Apr 2020 01:51:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/site/bin
# Wed, 01 Apr 2020 01:51:22 GMT
CMD ["perl6"]
```

-	Layers:
	-	`sha256:56da78ce36e97a8ba1f860575bb1422d1cb6ab4dade70b06ddf1651302dde955`  
		Last Modified: Tue, 31 Mar 2020 01:29:15 GMT  
		Size: 45.4 MB (45375928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbfe0f13ac4531fb6d077fda0e94ced4b9ed8a354c54b4efced9b7755d3f39d1`  
		Last Modified: Tue, 31 Mar 2020 02:12:44 GMT  
		Size: 10.8 MB (10797329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6254ff6d0e6052b7bead70e37703002eda28ac40f9a1167ea9bf813bf9c17d7f`  
		Last Modified: Tue, 31 Mar 2020 02:12:43 GMT  
		Size: 4.3 MB (4340113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e1e13bd9f6c381f158a5366b3eff242e8b4a4decfa940e915b1d5705ef4a28`  
		Last Modified: Tue, 31 Mar 2020 02:12:58 GMT  
		Size: 50.1 MB (50071604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae38a9146e7236ea4613bb440a10f063041d4843da7fe6e8b47897d56f48d16`  
		Last Modified: Wed, 01 Apr 2020 01:51:42 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b40382bb51aa4d18a3bdbb4ec32dfc8629342343aeb675a617c6050b51c3cd12`  
		Last Modified: Wed, 01 Apr 2020 01:51:49 GMT  
		Size: 27.6 MB (27608935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rakudo-star:latest` - linux; arm64 variant v8

```console
$ docker pull rakudo-star@sha256:cef53b2c6823f79b471ae230ef0848d8d1bed33dace8e955db47bfcc4e55417b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.3 MB (132348626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9195f2d025ede94e1d23632dcbebb91052e3a97961e32ebf0bbf147f1233e3d6`
-	Default Command: `["perl6"]`

```dockerfile
# Thu, 16 Apr 2020 02:44:49 GMT
ADD file:6d09304a2db2752e78b9ce9610594102dc756aa4cd210f85bbfa21105c7dd88f in / 
# Thu, 16 Apr 2020 02:44:52 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 03:21:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 03:21:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 03:22:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 23:29:18 GMT
MAINTAINER Rob Hoelz
# Thu, 16 Apr 2020 23:29:21 GMT
RUN groupadd -r perl6 && useradd -r -g perl6 perl6
# Thu, 16 Apr 2020 23:29:22 GMT
ARG rakudo_version=2019.03
# Thu, 16 Apr 2020 23:29:22 GMT
ENV rakudo_version=2019.03
# Fri, 17 Apr 2020 00:02:53 GMT
RUN buildDeps='         gcc         libc6-dev         libencode-perl         make     '         url="https://rakudostar.com/files/star/rakudo-star-${rakudo_version}.tar.gz"     keyserver='ha.pool.sks-keyservers.net'     keyfp='ECF8B611205B447E091246AF959E3D6197190DD5 7A6C9EB8809CFEAF0ED4E09F18C438E6FF24326D'     tmpdir="$(mktemp -d)"     && set -x     && export GNUPGHOME="$tmpdir"     && apt-get update     && apt-get --yes install --no-install-recommends $buildDeps     && rm -rf /var/lib/apt/lists/*     && mkdir ${tmpdir}/rakudo         && curl -fsSL ${url}.asc -o ${tmpdir}/rakudo.tar.gz.asc     && curl -fsSL $url -o ${tmpdir}/rakudo.tar.gz     && gpg --batch --keyserver $keyserver --recv-keys $keyfp     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && perl Configure.pl --prefix=/usr --gen-moar         && make install     )     && rm -rf $tmpdir     && apt-get purge -y --auto-remove $buildDeps
# Fri, 17 Apr 2020 00:02:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/site/bin
# Fri, 17 Apr 2020 00:02:56 GMT
CMD ["perl6"]
```

-	Layers:
	-	`sha256:65d54b492d599e7c785a582a0f70195e1f09f0886e54cb7788f1021f383eb4ed`  
		Last Modified: Thu, 16 Apr 2020 02:51:10 GMT  
		Size: 43.2 MB (43159230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be35cdee43e0bbb89c0867d201ff274ba25b6ea9bfe7f8f0c1d1d6de36ab08a`  
		Last Modified: Thu, 16 Apr 2020 03:30:52 GMT  
		Size: 9.7 MB (9748442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b803ac2c0e69edab9b8db20bee0f9dfc0191a7975c94d4d2ea0088d5a1759be8`  
		Last Modified: Thu, 16 Apr 2020 03:30:51 GMT  
		Size: 4.1 MB (4094379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56b7aa1f85cab0d60a62bc0cefa5ec56563f6681054c670ba97d559b4e7ba34`  
		Last Modified: Thu, 16 Apr 2020 03:31:12 GMT  
		Size: 48.0 MB (48027596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8879e78164926002c360f5a1b459371d03dc18960f7584a7031d0a3bfb9ce3c1`  
		Last Modified: Fri, 17 Apr 2020 00:03:24 GMT  
		Size: 1.8 KB (1770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9a195406aecaab594a9cc172eb55c70084efa1c9a20ced3c8ef74d9ce1d678`  
		Last Modified: Fri, 17 Apr 2020 00:03:34 GMT  
		Size: 27.3 MB (27317209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
