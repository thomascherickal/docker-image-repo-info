## `rakudo-star:alpine`

```console
$ docker pull rakudo-star@sha256:d540e3ab9bfd88e5239dc73778a9f9f6a7e7961cf0eb884fc3f553f2722e5ffa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `rakudo-star:alpine` - linux; amd64

```console
$ docker pull rakudo-star@sha256:f1392cb2d9c49f3d577b70fc64ddc4a1010113db7f36ef7aece170c0b0fd7139
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.5 MB (42503162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da208902968e5a30b98044d280426db55b9a4fc7515c1c5f47bc01e5406ac9e2`
-	Default Command: `["raku"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Fri, 06 Nov 2020 22:32:49 GMT
RUN addgroup -S raku && adduser -S raku -G raku
# Fri, 06 Nov 2020 22:32:49 GMT
ARG rakudo_version=2020.10
# Fri, 06 Nov 2020 22:32:49 GMT
ENV rakudo_version=2020.10
# Fri, 13 Nov 2020 19:50:04 GMT
RUN buildDeps='         bash         gcc         gnupg         libc-dev         make         perl     '         url="https://rakudo.org/dl/star/rakudo-star-${rakudo_version}.tar.gz"     keyserver='ha.pool.sks-keyservers.net'     keyfp='B6F697742EFCAF5F23CE51D5031D65902E840821'     tmpdir="$(mktemp -d)"     && set -eux     && export GNUPGHOME="$tmpdir"     && apk add --no-cache --virtual .build-deps $buildDeps     && mkdir ${tmpdir}/rakudo         && wget ${url}.asc -O ${tmpdir}/rakudo.tar.gz.asc     && wget $url -O ${tmpdir}/rakudo.tar.gz     && gpg --batch --keyserver $keyserver --recv-keys $keyfp     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && bash bin/rstar install -p /usr     )     && rm -rf $tmpdir     && apk del --no-network .build-deps
# Tue, 17 Nov 2020 21:16:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/core/bin:/usr/share/perl6/site/bin:/usr/share/perl6/vendor/bin
# Tue, 17 Nov 2020 21:16:33 GMT
CMD ["raku"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406cfbc4ad756e663752335e88cabb755c8d030849d683c60669928705b16abe`  
		Last Modified: Fri, 06 Nov 2020 22:44:16 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4f7f8e28530e2bc72e293a9c7e1f023a79c71b91edf0cff7465aea37718a437`  
		Last Modified: Fri, 13 Nov 2020 19:50:51 GMT  
		Size: 39.7 MB (39705072 bytes)  
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
