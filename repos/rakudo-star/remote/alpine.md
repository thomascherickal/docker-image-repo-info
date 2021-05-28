## `rakudo-star:alpine`

```console
$ docker pull rakudo-star@sha256:8a38114f00eb4744cd0d6f5f03cf753fc4609e1eb08d00364b8d2caf841ad8b2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `rakudo-star:alpine` - linux; amd64

```console
$ docker pull rakudo-star@sha256:eb1fcba1345a443fc974f2222a4e10bee905f217690b5962a33566d5ce5d7db0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.5 MB (42507805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fd30d373b3b24239267aa0eba0f37610b49ae83d972742bad263f10979248a1`
-	Default Command: `["raku"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:44:55 GMT
RUN addgroup -S raku && adduser -S raku -G raku
# Wed, 14 Apr 2021 23:44:55 GMT
ARG rakudo_version=2020.10
# Wed, 14 Apr 2021 23:44:55 GMT
ENV rakudo_version=2020.10
# Wed, 14 Apr 2021 23:58:02 GMT
RUN buildDeps='         bash         gcc         gnupg         libc-dev         make         perl     '         url="https://rakudo.org/dl/star/rakudo-star-${rakudo_version}.tar.gz"     keyserver='ha.pool.sks-keyservers.net'     keyfp='B6F697742EFCAF5F23CE51D5031D65902E840821'     tmpdir="$(mktemp -d)"     && set -eux     && export GNUPGHOME="$tmpdir"     && apk add --no-cache --virtual .build-deps $buildDeps     && mkdir ${tmpdir}/rakudo         && wget ${url}.asc -O ${tmpdir}/rakudo.tar.gz.asc     && wget $url -O ${tmpdir}/rakudo.tar.gz     && gpg --batch --keyserver $keyserver --recv-keys $keyfp     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && bash bin/rstar install -p /usr     )     && rm -rf $tmpdir     && apk del --no-network .build-deps
# Wed, 14 Apr 2021 23:58:03 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/core/bin:/usr/share/perl6/site/bin:/usr/share/perl6/vendor/bin
# Wed, 14 Apr 2021 23:58:03 GMT
CMD ["raku"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e22312896b25dccb3fc44b962ae073fba73d020dbcaa723324d3d1e199051f3`  
		Last Modified: Wed, 14 Apr 2021 23:58:19 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d0492aaa059e790811ad1a9f7df140b391d0854440aa709ba8dd6f6a23e42a`  
		Last Modified: Wed, 14 Apr 2021 23:58:28 GMT  
		Size: 39.7 MB (39705982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rakudo-star:alpine` - linux; arm64 variant v8

```console
$ docker pull rakudo-star@sha256:eb12738c4df5818a02f5482c8c3864e672a79a9eb630318afd1077e286aa6995
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.2 MB (42208945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:887224c9ae6f1de04ffba95bad2e6ace1c5c427f4652a7be2f54492ab48cc033`
-	Default Command: `["raku"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:54 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Wed, 14 Apr 2021 18:42:55 GMT
CMD ["/bin/sh"]
# Fri, 28 May 2021 11:13:45 GMT
RUN addgroup -S raku && adduser -S raku -G raku
# Fri, 28 May 2021 11:13:45 GMT
ARG rakudo_version=2020.10
# Fri, 28 May 2021 11:13:45 GMT
ENV rakudo_version=2020.10
# Fri, 28 May 2021 11:25:10 GMT
RUN buildDeps='         bash         gcc         gnupg         libc-dev         make         perl     '         url="https://rakudo.org/dl/star/rakudo-star-${rakudo_version}.tar.gz"     keyserver='ha.pool.sks-keyservers.net'     keyfp='B6F697742EFCAF5F23CE51D5031D65902E840821'     tmpdir="$(mktemp -d)"     && set -eux     && export GNUPGHOME="$tmpdir"     && apk add --no-cache --virtual .build-deps $buildDeps     && mkdir ${tmpdir}/rakudo         && wget ${url}.asc -O ${tmpdir}/rakudo.tar.gz.asc     && wget $url -O ${tmpdir}/rakudo.tar.gz     && gpg --batch --keyserver $keyserver --recv-keys $keyfp     && gpg --batch --verify ${tmpdir}/rakudo.tar.gz.asc ${tmpdir}/rakudo.tar.gz         && tar xzf ${tmpdir}/rakudo.tar.gz --strip-components=1 -C ${tmpdir}/rakudo     && (         cd ${tmpdir}/rakudo         && bash bin/rstar install -p /usr     )     && rm -rf $tmpdir     && apk del --no-network .build-deps
# Fri, 28 May 2021 11:25:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/share/perl6/core/bin:/usr/share/perl6/site/bin:/usr/share/perl6/vendor/bin
# Fri, 28 May 2021 11:25:11 GMT
CMD ["raku"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a1a3ef8ed22f59e56f4c136a3f0aa9f167b7e5f00a9c13dde85fe0d080cf9f`  
		Last Modified: Fri, 28 May 2021 11:25:49 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988bc508a443f626658cdd2678d201d6a294d26f3daf5fdc159566e8bede12c5`  
		Last Modified: Fri, 28 May 2021 11:25:59 GMT  
		Size: 39.5 MB (39496992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
