## `buildpack-deps:unstable`

```console
$ docker pull buildpack-deps@sha256:4f2f252804eb433bce9b2bb24e06c5cd35bdfee86335948ab15980dfaa39d03b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:unstable` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:9db46c6b6efa582e2ef03bad4a763331d1bab07b4a9bf5fde69e9804a7e9b9c6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.6 MB (322632859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e3384ba5d9501679c04326b6688c3d116440164f33fc0956f9736e9bfe3ad9b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:21:14 GMT
ADD file:5745436941906af011c9450820c7baff61a091235f04da258ba218ca450622a5 in / 
# Wed, 23 Jun 2021 00:21:15 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:54:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 00:55:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:55:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bbd4da8ff6e19a9b86585f9b55dede690ca6dca9f96d946fa1fb6456182931cd`  
		Last Modified: Wed, 23 Jun 2021 00:26:45 GMT  
		Size: 54.9 MB (54902493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0246214aa0ecb6ede7631e54d50bebe607ad610e577d4fbf6857d6b158e7dbf`  
		Last Modified: Wed, 23 Jun 2021 01:03:11 GMT  
		Size: 5.2 MB (5170501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35d77eb31156f1996620962d6772ae81841ad63c839af8f4841118c8410fade`  
		Last Modified: Wed, 23 Jun 2021 01:03:11 GMT  
		Size: 10.9 MB (10872573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65c94a6468c400151537722b4a6b82a7e4fe16655ef49643f3ef4c591fa91fe`  
		Last Modified: Wed, 23 Jun 2021 01:03:34 GMT  
		Size: 55.3 MB (55259452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8979a9f403ece83ef006eff91f53633c90ffa29e460302aedafa85b8213024e2`  
		Last Modified: Wed, 23 Jun 2021 01:04:20 GMT  
		Size: 196.4 MB (196427840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:22805fc5ffbef00237b732f5f0d2569500281ce64235241e0c7f72e00009d22c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.6 MB (295582501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d34c5afbdf92d710875356612611f087e6812e142373531884b0fceadd77355e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 00:57:58 GMT
ADD file:74d49eb3680e0d1e7268c77ac09aadc6a9eaca2541a1941d02c05771fce80430 in / 
# Wed, 12 May 2021 00:58:17 GMT
CMD ["bash"]
# Thu, 27 May 2021 19:55:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 19:55:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 27 May 2021 19:56:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 19:57:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:992a8499bbce77a1397237914a5f442e2a2d90912c4dcf8d75ced68fa669452a`  
		Last Modified: Wed, 12 May 2021 01:11:33 GMT  
		Size: 52.4 MB (52438763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919c41d940ed14742ec6f26b83d52bccd7dc9e430c1dda8f4e8acdebb898ff0f`  
		Last Modified: Thu, 27 May 2021 20:06:51 GMT  
		Size: 5.1 MB (5074040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37054668f2f5a38fbe90534d3d0080b9438fb37e6c74493f206211677ac7fe91`  
		Last Modified: Thu, 27 May 2021 20:06:51 GMT  
		Size: 10.6 MB (10571286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c443380432daf1d44bb7dda7f7ef3ede16dedb3892444726dc30dbc068156e47`  
		Last Modified: Thu, 27 May 2021 20:07:20 GMT  
		Size: 52.9 MB (52878041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a3a6cdca96f14e4593f3e409233f848e01d41d1ee98c8828efbf7e97321796`  
		Last Modified: Thu, 27 May 2021 20:08:15 GMT  
		Size: 174.6 MB (174620371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:bf70305ad13e60172a93f9966cde5232d97820435d3e34f3437f0ad830022ccb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.0 MB (282967705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48086c43970e5d281d4ae1c31d59bc496773f90e5286cdc9b33d2a0d21133adc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:08:03 GMT
ADD file:45a139d5ba2871d3a6f990263a8fdb68998d0e072f5c70f796581383ed107962 in / 
# Wed, 12 May 2021 01:08:13 GMT
CMD ["bash"]
# Thu, 27 May 2021 00:42:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 00:42:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 27 May 2021 00:43:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 27 May 2021 00:44:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:187ecf03b42c9078bbaf7c041564e40178e23f795d23634e11536955cfc64143`  
		Last Modified: Wed, 12 May 2021 01:20:07 GMT  
		Size: 50.1 MB (50098265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4246453820c5b02c5c8b00dc0dde6bfb94015029c6b8005d49ade59af59c0f9f`  
		Last Modified: Thu, 27 May 2021 01:04:58 GMT  
		Size: 4.9 MB (4935074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb9c0bc52453d252747af83975a8f1a58fe5bf2a18c4d879befd805239279f6`  
		Last Modified: Thu, 27 May 2021 01:04:58 GMT  
		Size: 10.2 MB (10216618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b443e7da95eaa262c0259ec871bcc330143ddd0e04dd971d0f5b7f936a1ba7`  
		Last Modified: Thu, 27 May 2021 01:05:27 GMT  
		Size: 50.8 MB (50834521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fa178742ad707268472faaaffa70c7aa0010f32450097b2b4f35548ad7710be`  
		Last Modified: Thu, 27 May 2021 01:06:21 GMT  
		Size: 166.9 MB (166883227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:37b43474d9d60990ce02954596b9e0c5bb20f568f2ccf7318ccb5dc5c2334ab6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.3 MB (314342111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47692022ada6192ce178f8c129dd8d3967f87d867ac411dabda77929b8c9d193`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:14 GMT
ADD file:339319b02d36af7daf322a0b1295cc9416a58c021a5f5ba7a504f28717588cea in / 
# Tue, 22 Jun 2021 23:50:14 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:26:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:26:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 00:26:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:27:09 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e1aa4e0221ceafc83fb2f0929a4a51d5784e6bd00ecdfc3672853b28868fdf17`  
		Last Modified: Tue, 22 Jun 2021 23:56:31 GMT  
		Size: 53.6 MB (53586541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7626ab4adf6f17b187ebd4dddff8961986d7954ecf61d62b69eaa7ced1a128a9`  
		Last Modified: Wed, 23 Jun 2021 00:34:41 GMT  
		Size: 5.2 MB (5158799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f68a62ea25befd0307cf6cab1bf22ed625727daa8fcc5c452219a0bea940c1`  
		Last Modified: Wed, 23 Jun 2021 00:34:42 GMT  
		Size: 10.9 MB (10873185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6612ca213cc17f4e7c8e850bbd08e3342a7fb58ff637b59bc667f3bfb4792eb2`  
		Last Modified: Wed, 23 Jun 2021 00:35:03 GMT  
		Size: 55.4 MB (55405817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a7b55ef2967745751ffcdc770930af2e56f00a6eb4e686aa43ebe298175f9d`  
		Last Modified: Wed, 23 Jun 2021 00:35:43 GMT  
		Size: 189.3 MB (189317769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:181d47e67562d4c3f3b9ca903c35a03016f3f0c3efe212f1aea2d2e3359bd2cb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.5 MB (328482384 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a538e687e38e5b24dc8b7fd9930fdec147c20918b1f96d5f8bdb2b0ad792cf6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:40:18 GMT
ADD file:20378fd7bc859874d8620bd807402968cbe571a1ca281d0f344392ed5d8af55b in / 
# Tue, 22 Jun 2021 23:40:18 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:11:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:11:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 00:11:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:12:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ff9feaae647f307940e0b5cfdb30f3d3a877220cd3394859c1af4b3d653b2e97`  
		Last Modified: Tue, 22 Jun 2021 23:47:46 GMT  
		Size: 55.9 MB (55914853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5310b9c9dfb8fd34f5ff4cccb1d7af5e1baf20620d64357dc51a0e69717717e`  
		Last Modified: Wed, 23 Jun 2021 00:19:34 GMT  
		Size: 5.3 MB (5299879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bab8c3b07912881a8d38f2ca51a04fef6fa1d22c0163da069cd226eec7362a07`  
		Last Modified: Wed, 23 Jun 2021 00:19:35 GMT  
		Size: 11.3 MB (11250598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66c7b3456d19d1557f96e2c7bf74716f3187c850af8e39dbbccf8890f4c354e`  
		Last Modified: Wed, 23 Jun 2021 00:20:00 GMT  
		Size: 56.7 MB (56666110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2cab92909461cd5dd6672c529f1b219ba703293e42d3dd10ed7c87dc0273ca2`  
		Last Modified: Wed, 23 Jun 2021 00:20:54 GMT  
		Size: 199.4 MB (199350944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:511abc55782992064a483da2fd444eb687460144a37b75c2085ee9e8acc09aba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.1 MB (302140242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:880d83d58975791e6346b75fcd0c3f9d5b1afc7541692ef069d9f63b92dc8c85`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:09:56 GMT
ADD file:723b0881c85ba05a782aae0c0dfbbca4283e1a595a167af6a9a9b23b34916226 in / 
# Wed, 23 Jun 2021 00:09:57 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:46:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:46:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 00:47:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:49:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4f938924a38054ec92bd31be4d18e4f654308796e5e915428065faea9385c73d`  
		Last Modified: Wed, 23 Jun 2021 00:16:36 GMT  
		Size: 53.2 MB (53157176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df9715e9403d707b9879b1f23718b1730cb5cf3feb4f483c137a321c7a2dbab`  
		Last Modified: Wed, 23 Jun 2021 00:57:10 GMT  
		Size: 5.1 MB (5129996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b6704ed06dc069325a9235d3c57db6d14a34623f005bd10aaacc4acb2b42585`  
		Last Modified: Wed, 23 Jun 2021 00:57:12 GMT  
		Size: 10.9 MB (10873312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdace0ce09b260021353f35b35cc0d8e2dc930fe2d1cfb3cbf0cdc51c6f5c681`  
		Last Modified: Wed, 23 Jun 2021 00:58:02 GMT  
		Size: 54.1 MB (54061329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fedbff58288689e14975e33f2d0312f68b3e5973c80fb1dee47373ba2e592aea`  
		Last Modified: Wed, 23 Jun 2021 01:00:12 GMT  
		Size: 178.9 MB (178918429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:ebfcf9978cc911de84d47a51622855aedcbfd887fc972853f7ca078c5f77dad4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.7 MB (330685797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8001e0b5512ba3a6ad39d8e45e5ec323a3a2e819c2231cfe7bd324bb4925bba`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:35:19 GMT
ADD file:7d2dad47f7990dd0f8ed0b034505aa9c7d8afbd94956f80bb57feccf6f7e15fc in / 
# Wed, 12 May 2021 01:35:33 GMT
CMD ["bash"]
# Wed, 12 May 2021 04:02:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 04:02:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 04:04:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 04:13:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ec00b4432728c9f962251efa3d91b6e0339e74ff656fbaad7adad52ce998ea8c`  
		Last Modified: Wed, 12 May 2021 01:45:35 GMT  
		Size: 58.8 MB (58798847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785fbf7f2f224053db3ca18ebfb195a650ed240333b2b7bc423c9a3190693e63`  
		Last Modified: Wed, 12 May 2021 04:22:23 GMT  
		Size: 5.4 MB (5419993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cbba1e29d2e9ae70bab4c22a5dd913b1657725f350d6f9c4130d0f30ddc06ba`  
		Last Modified: Wed, 12 May 2021 04:22:26 GMT  
		Size: 11.6 MB (11625707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886cc000b70a733d57e8882fa72e96ba17fb8f09e9b18b39bc5dfb02aa1d8b7c`  
		Last Modified: Wed, 12 May 2021 04:23:34 GMT  
		Size: 59.1 MB (59131912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4063a6ba0148cd1e5c224e9402ecf9a1d8740bd82b6ad463aa916853e5f49f`  
		Last Modified: Wed, 12 May 2021 04:24:21 GMT  
		Size: 195.7 MB (195709338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:1a22c1b929dcfbd9ccc00112d24c2a9a4907f70ea45225a651185ed75a2ae6dd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.2 MB (296222611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:404b5641613e8d0b1b10da616068b9bc746ded71adc6f52a246636c2db786d17`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:42:38 GMT
ADD file:b2361f35b2807ada58f66b4f4f160b2133140a85db4ecd56889a15f080793790 in / 
# Tue, 22 Jun 2021 23:42:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:07:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:07:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 00:08:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:09:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:247ed76d4285ef2f620cc0d1ec3492f8a6d1b0cc613aadf4e236db73dc508cca`  
		Last Modified: Tue, 22 Jun 2021 23:45:59 GMT  
		Size: 53.2 MB (53184006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9061f67eb9da8a0f6f7f323fc5113c55d3782998f1d177170951d684d367502f`  
		Last Modified: Wed, 23 Jun 2021 00:13:01 GMT  
		Size: 5.2 MB (5152169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2261334caf31e69fc462c4f94347962e98bb4b7a074c0fedc944f1458fbd106`  
		Last Modified: Wed, 23 Jun 2021 00:13:01 GMT  
		Size: 10.8 MB (10763416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320655ef4ccf1f9b477d71c135860e6ad84c4248ddfdcebfca06d0fe6f6d1a5a`  
		Last Modified: Wed, 23 Jun 2021 00:13:16 GMT  
		Size: 54.7 MB (54713424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cadaa45f9922a247d081bc92e53517cbaa18cb9039abb2f65394a191bab93ce1`  
		Last Modified: Wed, 23 Jun 2021 00:13:43 GMT  
		Size: 172.4 MB (172409596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
