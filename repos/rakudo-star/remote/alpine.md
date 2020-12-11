## `rakudo-star:alpine`

```console
$ docker pull rakudo-star@sha256:2d5a29b8c819073dc237a9e8b1a72f0785eb42361628b3b5194b09e55bdaaa9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `rakudo-star:alpine` - linux; amd64

```console
$ docker pull rakudo-star@sha256:0db9120c1cb2157620bbb79ba2ad6dadcd463d59db6f5b00c35e8136a16c3a2e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.5 MB (42503293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b373b9f53058ac4d27ea68374552719ce83601d1db8ea31cc93a6ee669fa954`
-	Default Command: `["raku"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 13:25:18 GMT
RUN addgroup -S raku && adduser -S raku -G raku
# Fri, 11 Dec 2020 13:25:18 GMT
ARG rakudo_version=2020.10
# Fri, 11 Dec 2020 13:25:19 GMT
ENV rakudo_version=2020.10
# Fri, 11 Dec 2020 13:40:44 GMT
RUN buildDeps='         bash         gcc         gnupg         libc-dev         make         perl     '         url="https://rakudo.org/dl/star/rakudo-star-${rakudo_version}.tar.gz"     keyserver='ha.pool.sks-keyservers.net'     keyfp='B6F697742EFCAF5F23CE51D5031D65902E840821'     tmpdir="$(mktemp -d)"     && set -eux     && export GNUPGHOME="$tmpdir"     && apk add --no-cache --virtual .build-deps $buildDeps     && mkdir ${tmpdir}/rakudo         && wget ${url}.asc -O ${tmpdir}/rakudo.tar.gz.asc     && wget $url -O ${tmpdir}/rakudo.tar.gz     && gpg --batch --keyserver $keyserver --recv-keys $keyfp     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && bash bin/rstar install -p /usr     )     && rm -rf $tmpdir     && apk del --no-network .build-deps
# Fri, 11 Dec 2020 13:40:45 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/core/bin:/usr/share/perl6/site/bin:/usr/share/perl6/vendor/bin
# Fri, 11 Dec 2020 13:40:45 GMT
CMD ["raku"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9608f1b806966f762e33181092b8dfb341504119a530c9411db28f1e9cbe96f7`  
		Last Modified: Fri, 11 Dec 2020 13:41:10 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a1160a1d8f3e657f77f6dcce6b6e4c7a30f31e434f82957302eff5a0a3cb83`  
		Last Modified: Fri, 11 Dec 2020 13:41:20 GMT  
		Size: 39.7 MB (39705119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rakudo-star:alpine` - linux; arm64 variant v8

```console
$ docker pull rakudo-star@sha256:1b150b8c713f8c8e4a5f2ccd08e338e0df490103b9e2952f8337b80a73a2f8df
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42063171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fd3befdda8c6101aaa40b54a01fd0ae30331ffa564dc1acc1f4c0d907aba7a8`
-	Default Command: `["raku"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Fri, 06 Nov 2020 23:03:43 GMT
RUN addgroup -S raku && adduser -S raku -G raku
# Fri, 06 Nov 2020 23:03:44 GMT
ARG rakudo_version=2020.10
# Fri, 06 Nov 2020 23:03:44 GMT
ENV rakudo_version=2020.10
# Fri, 13 Nov 2020 20:30:53 GMT
RUN buildDeps='         bash         gcc         gnupg         libc-dev         make         perl     '         url="https://rakudo.org/dl/star/rakudo-star-${rakudo_version}.tar.gz"     keyserver='ha.pool.sks-keyservers.net'     keyfp='B6F697742EFCAF5F23CE51D5031D65902E840821'     tmpdir="$(mktemp -d)"     && set -eux     && export GNUPGHOME="$tmpdir"     && apk add --no-cache --virtual .build-deps $buildDeps     && mkdir ${tmpdir}/rakudo         && wget ${url}.asc -O ${tmpdir}/rakudo.tar.gz.asc     && wget $url -O ${tmpdir}/rakudo.tar.gz     && gpg --batch --keyserver $keyserver --recv-keys $keyfp     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && bash bin/rstar install -p /usr     )     && rm -rf $tmpdir     && apk del --no-network .build-deps
# Tue, 17 Nov 2020 21:05:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/core/bin:/usr/share/perl6/site/bin:/usr/share/perl6/vendor/bin
# Tue, 17 Nov 2020 21:05:10 GMT
CMD ["raku"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc5728765b93b28e9fccc30542ab407aad9836503ca530e964dc5e424f1d17f5`  
		Last Modified: Fri, 06 Nov 2020 23:33:15 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad4a9aad8e387a65d46e5f4a343fc09cff75098bf447e370a9ea5c8367e6b28e`  
		Last Modified: Fri, 13 Nov 2020 20:31:41 GMT  
		Size: 39.4 MB (39355357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
