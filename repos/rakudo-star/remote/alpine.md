## `rakudo-star:alpine`

```console
$ docker pull rakudo-star@sha256:ac19e8d79eed9977f9eea732e9c84914f5ab4ae2c74ea642b98d99402264947c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rakudo-star:alpine` - linux; amd64

```console
$ docker pull rakudo-star@sha256:1dd051b6a9c498cad600e33d285a79cb265526fb736ac4ff781f18174d21d7ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.4 MB (38442405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0b309385d657eaf0ed037699ae26a41b0ca470d47cd16823dea2039390553ae`
-	Default Command: `["raku"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 07:57:08 GMT
RUN addgroup -S raku && adduser -S raku -G raku
# Sat, 12 Nov 2022 07:57:08 GMT
ARG rakudo_version=2022.07-01
# Sat, 12 Nov 2022 07:57:08 GMT
ENV rakudo_version=2022.07-01
# Sat, 12 Nov 2022 08:06:57 GMT
RUN buildDeps='         bash         gcc         gnupg         libc-dev         make         perl     '         url="https://rakudo.org/dl/star/rakudo-star-${rakudo_version}.tar.gz"     keyfp="3E7E3C6EAF916676AC549285A2919382E961E2EE"     pubkeyurl="https://rakudo.org/keys/rakudo_github_automation-${keyfp}.asc"     tmpdir="$(mktemp -d)"     && set -eux     && export GNUPGHOME="${tmpdir}/gnupg"     && mkdir $GNUPGHOME     && apk add --no-cache --virtual .build-deps $buildDeps     && mkdir ${tmpdir}/rakudo         && wget ${url}.asc -O ${tmpdir}/rakudo.tar.gz.asc     && wget $url -O ${tmpdir}/rakudo.tar.gz     && wget $pubkeyurl -O ${tmpdir}/key.asc         && gpg --import ${tmpdir}/key.asc     && gpg --export $keyfp > ${tmpdir}/${keyfp}.asc     && rm -rf $GNUPGHOME     && mkdir $GNUPGHOME     && gpg --import ${tmpdir}/${keyfp}.asc     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && bash bin/rstar install -p /usr     )     && rm -rf $tmpdir     && apk del --no-network .build-deps
# Sat, 12 Nov 2022 08:06:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/core/bin:/usr/share/perl6/site/bin:/usr/share/perl6/vendor/bin
# Sat, 12 Nov 2022 08:06:58 GMT
CMD ["raku"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d606a43dd671b3663ef5e85e1c2a03b1ed24d8bf23512546fe90fa960e38338`  
		Last Modified: Sat, 12 Nov 2022 08:07:10 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9e4518e70d481a9f6449c07564e29b32936b7ee463db402e29929865826c62`  
		Last Modified: Sat, 12 Nov 2022 08:07:17 GMT  
		Size: 35.6 MB (35634867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rakudo-star:alpine` - linux; arm64 variant v8

```console
$ docker pull rakudo-star@sha256:ef22e773d514a1ded52432d95580f1475146641e9a33bd8c4c1767fcaf27c1e0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.8 MB (35787379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a088a03cfe244ead14ec1f105f5ea0e284c492f9ef8af8d9b15d542cced2203`
-	Default Command: `["raku"]`

```dockerfile
# Sat, 12 Nov 2022 03:39:38 GMT
ADD file:57d621536158358b14d15155826ef2dd4ca034278044111ec0aaf6717016e569 in / 
# Sat, 12 Nov 2022 03:39:38 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 05:54:44 GMT
RUN addgroup -S raku && adduser -S raku -G raku
# Sat, 12 Nov 2022 05:54:44 GMT
ARG rakudo_version=2022.07-01
# Sat, 12 Nov 2022 05:54:44 GMT
ENV rakudo_version=2022.07-01
# Sat, 12 Nov 2022 06:02:17 GMT
RUN buildDeps='         bash         gcc         gnupg         libc-dev         make         perl     '         url="https://rakudo.org/dl/star/rakudo-star-${rakudo_version}.tar.gz"     keyfp="3E7E3C6EAF916676AC549285A2919382E961E2EE"     pubkeyurl="https://rakudo.org/keys/rakudo_github_automation-${keyfp}.asc"     tmpdir="$(mktemp -d)"     && set -eux     && export GNUPGHOME="${tmpdir}/gnupg"     && mkdir $GNUPGHOME     && apk add --no-cache --virtual .build-deps $buildDeps     && mkdir ${tmpdir}/rakudo         && wget ${url}.asc -O ${tmpdir}/rakudo.tar.gz.asc     && wget $url -O ${tmpdir}/rakudo.tar.gz     && wget $pubkeyurl -O ${tmpdir}/key.asc         && gpg --import ${tmpdir}/key.asc     && gpg --export $keyfp > ${tmpdir}/${keyfp}.asc     && rm -rf $GNUPGHOME     && mkdir $GNUPGHOME     && gpg --import ${tmpdir}/${keyfp}.asc     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && bash bin/rstar install -p /usr     )     && rm -rf $tmpdir     && apk del --no-network .build-deps
# Sat, 12 Nov 2022 06:02:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/core/bin:/usr/share/perl6/site/bin:/usr/share/perl6/vendor/bin
# Sat, 12 Nov 2022 06:02:17 GMT
CMD ["raku"]
```

-	Layers:
	-	`sha256:6875df1f535433e5affe18ecfde9acb7950ab5f76887980ff06c5cdd48cf98f4`  
		Last Modified: Sat, 12 Nov 2022 03:40:05 GMT  
		Size: 2.7 MB (2707756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cdf9d87fb328f94c616f56770eaebe8a873dadf5c9b26b1f0b0002a94eb6abb`  
		Last Modified: Sat, 12 Nov 2022 06:02:30 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84bdc00236ac88eb216ba828fd789bb457cd0ba891844d23df2b1a88942121b1`  
		Last Modified: Sat, 12 Nov 2022 06:02:36 GMT  
		Size: 33.1 MB (33078357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
