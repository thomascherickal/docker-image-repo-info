## `rakudo-star:alpine`

```console
$ docker pull rakudo-star@sha256:06bb95ba41343613d59ea5afd3bc1e393a64bf25914d1b3c0b128bb9fbd5aa81
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `rakudo-star:alpine` - linux; amd64

```console
$ docker pull rakudo-star@sha256:5a09c0c21cc111c345b0d96f8e5fb40760d6c325baa3868927234d9ec77bd132
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.1 MB (42148297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62ea84e3ecd0403a2b642b2241e9c8dba8b230162f22561e12c9265d504f2422`
-	Default Command: `["raku"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:54:05 GMT
RUN addgroup -S raku && adduser -S raku -G raku
# Fri, 29 Sep 2023 02:54:06 GMT
ARG rakudo_version=2023.08-01
# Fri, 29 Sep 2023 02:54:06 GMT
ENV rakudo_version=2023.08-01
# Fri, 29 Sep 2023 03:17:45 GMT
RUN buildDeps='         bash         gcc         gnupg         libc-dev         make         perl     '         url="https://rakudo.org/dl/star/rakudo-star-${rakudo_version}.tar.gz"     keyfp="3E7E3C6EAF916676AC549285A2919382E961E2EE"     pubkeyurl="https://rakudo.org/keys/rakudo_github_automation-${keyfp}.asc"     tmpdir="$(mktemp -d)"     && set -eux     && export GNUPGHOME="${tmpdir}/gnupg"     && mkdir $GNUPGHOME     && apk add --no-cache --virtual .build-deps $buildDeps     && apk add --no-cache readline     && mkdir ${tmpdir}/rakudo         && wget ${url}.asc -O ${tmpdir}/rakudo.tar.gz.asc     && wget $url -O ${tmpdir}/rakudo.tar.gz     && wget $pubkeyurl -O ${tmpdir}/key.asc         && gpg --batch --import ${tmpdir}/key.asc     && gpg --batch --export $keyfp > ${tmpdir}/${keyfp}.asc     && rm -rf $GNUPGHOME     && mkdir $GNUPGHOME     && gpg --batch --import ${tmpdir}/${keyfp}.asc     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && bash bin/rstar install -p /usr     )     && rm -rf $tmpdir     && apk del --no-network .build-deps
# Fri, 29 Sep 2023 03:17:46 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/core/bin:/usr/share/perl6/site/bin:/usr/share/perl6/vendor/bin
# Fri, 29 Sep 2023 03:17:46 GMT
CMD ["raku"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e918c9a7030145a5163b42d5a151cce0c73a79574ddeeb5cf292eb3ecf0694`  
		Last Modified: Fri, 29 Sep 2023 03:18:08 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2d7000f97db4a652ae9ed02b71e135fa5c2918d74eb46fed4760d538df4211f`  
		Last Modified: Fri, 29 Sep 2023 03:18:16 GMT  
		Size: 38.7 MB (38745062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rakudo-star:alpine` - linux; arm64 variant v8

```console
$ docker pull rakudo-star@sha256:8159933ae8d9af3bd3f696c41575a308ad257aa73d588dda66f803fd8fa52557
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41936144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a847cd5c3863c0a28ca72c6f8e099eb9c7359670855452a734ccb5ab6dc962a`
-	Default Command: `["raku"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:25:28 GMT
RUN addgroup -S raku && adduser -S raku -G raku
# Fri, 29 Sep 2023 02:25:28 GMT
ARG rakudo_version=2023.08-01
# Fri, 29 Sep 2023 02:25:29 GMT
ENV rakudo_version=2023.08-01
# Fri, 29 Sep 2023 02:45:41 GMT
RUN buildDeps='         bash         gcc         gnupg         libc-dev         make         perl     '         url="https://rakudo.org/dl/star/rakudo-star-${rakudo_version}.tar.gz"     keyfp="3E7E3C6EAF916676AC549285A2919382E961E2EE"     pubkeyurl="https://rakudo.org/keys/rakudo_github_automation-${keyfp}.asc"     tmpdir="$(mktemp -d)"     && set -eux     && export GNUPGHOME="${tmpdir}/gnupg"     && mkdir $GNUPGHOME     && apk add --no-cache --virtual .build-deps $buildDeps     && apk add --no-cache readline     && mkdir ${tmpdir}/rakudo         && wget ${url}.asc -O ${tmpdir}/rakudo.tar.gz.asc     && wget $url -O ${tmpdir}/rakudo.tar.gz     && wget $pubkeyurl -O ${tmpdir}/key.asc         && gpg --batch --import ${tmpdir}/key.asc     && gpg --batch --export $keyfp > ${tmpdir}/${keyfp}.asc     && rm -rf $GNUPGHOME     && mkdir $GNUPGHOME     && gpg --batch --import ${tmpdir}/${keyfp}.asc     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && bash bin/rstar install -p /usr     )     && rm -rf $tmpdir     && apk del --no-network .build-deps
# Fri, 29 Sep 2023 02:45:42 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/core/bin:/usr/share/perl6/site/bin:/usr/share/perl6/vendor/bin
# Fri, 29 Sep 2023 02:45:42 GMT
CMD ["raku"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6341b984c56d6b7713998c56a1241f2c89d5c80a8b6e66b78a1cbe56886ad6a`  
		Last Modified: Fri, 29 Sep 2023 02:45:59 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a120665686416ba5e70667c98a886174b6f3155ae2fda199bf797c37e44db3e5`  
		Last Modified: Fri, 29 Sep 2023 02:46:05 GMT  
		Size: 38.6 MB (38603047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
