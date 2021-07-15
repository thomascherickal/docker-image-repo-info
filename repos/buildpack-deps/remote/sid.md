## `buildpack-deps:sid`

```console
$ docker pull buildpack-deps@sha256:96d46ae215d6de8e791db6b277ebfc1165dcce6669664dd7ac50ee1c9b3574e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:sid` - linux; amd64

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

### `buildpack-deps:sid` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:17b574e9fc3583671442fe009e7fb10d68edd6f6b497c93c0c482f6019bea57d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.7 MB (295682509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5182cd59cdd0514d634308e4d734b360246a9e75372b93e5e9af23b1ec068702`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 22 Jun 2021 23:51:21 GMT
ADD file:6f138ddb818c5f09c669ab36feab96f8445d36fb1cf1263f9c3fa7ed334d14a9 in / 
# Tue, 22 Jun 2021 23:51:23 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:43:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 05:43:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 05:44:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 05:46:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a4336d4df3d0160b4c6137b83e3c61fb0dcc6d38a51f2eccbe2cb96b75500f65`  
		Last Modified: Wed, 23 Jun 2021 00:03:50 GMT  
		Size: 52.4 MB (52440085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da427d5f1beeee9b5703b32a33e4b43db3a9512ed77d21591733d938dd07a245`  
		Last Modified: Wed, 23 Jun 2021 06:00:34 GMT  
		Size: 5.1 MB (5075069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f83f214b11d05abfca12f1b6f7c7ea433c7a204d7f6b4113383a0600cbba119e`  
		Last Modified: Wed, 23 Jun 2021 06:00:36 GMT  
		Size: 10.6 MB (10571940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54e2fc2ec25ce2da62055fb0589733c080b3749628cabcc0bb9f2f1880f89de`  
		Last Modified: Wed, 23 Jun 2021 06:01:28 GMT  
		Size: 53.0 MB (52967025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee8354312985f505595f3b37187732cc3687a05a04533a2010ab513aa51aa4f7`  
		Last Modified: Wed, 23 Jun 2021 06:03:32 GMT  
		Size: 174.6 MB (174628390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:3bbba69fa1aa24a477bdf97e8d118be9d230ead53f6e3dd145b68c38bdfca8ff
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **283.1 MB (283065433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86550c2a375251e8b24ca5fefc6d52e668c5a2e84d7224c0849b9276d50c51ad`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 23 Jun 2021 00:21:40 GMT
ADD file:10ae021b5b2998c7ee0904a6d9b6a3697ef580d3a6b0a0980c2f209a6ad2bb29 in / 
# Wed, 23 Jun 2021 00:21:42 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:49:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 05:49:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 05:50:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 05:52:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2bb9348ee5f2e424d70e44ac1d1e0b029bb37d72f6050453f93408edc2af9176`  
		Last Modified: Wed, 23 Jun 2021 00:33:47 GMT  
		Size: 50.1 MB (50105618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc10d3401b65a0651a08c5c29f2e1207dc4ca1027e80abc9b35cf15c88d96958`  
		Last Modified: Wed, 23 Jun 2021 06:21:43 GMT  
		Size: 4.9 MB (4936190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5dd2865193f1b761bf000f90190639fb8bfea0ce5033bf2de30ad2d9738789`  
		Last Modified: Wed, 23 Jun 2021 06:21:45 GMT  
		Size: 10.2 MB (10217331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f72f157f0331915f121358a516bb24081ca7d6310badb3e864d7a50a1e81882`  
		Last Modified: Wed, 23 Jun 2021 06:22:33 GMT  
		Size: 50.9 MB (50925879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de5a5d55da3a2a47047b4d592aed541e05a5e2b126f24f8000a484749c63b7a`  
		Last Modified: Wed, 23 Jun 2021 06:24:29 GMT  
		Size: 166.9 MB (166880415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm64 variant v8

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

### `buildpack-deps:sid` - linux; 386

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

### `buildpack-deps:sid` - linux; mips64le

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

### `buildpack-deps:sid` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:c8c03893f4ef0f32ecf8097915982622171503c6738f04dfe46193c52e115f86
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.4 MB (337398197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:115c1cfcf076dc5b9b920946ebafaa7cf9eddccd045e13ada9bce0fce4a0370b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Jul 2021 15:58:42 GMT
ADD file:9d5a0ba0a24f9a37f3d9812637e4beef52ef27fa65d76c97dffa3f4933633701 in / 
# Fri, 09 Jul 2021 15:58:46 GMT
CMD ["bash"]
# Sat, 10 Jul 2021 06:40:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Jul 2021 06:41:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Jul 2021 06:43:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 10 Jul 2021 06:59:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:28a36a9b0ca23da4474256976c303c139c5800da883d61fb1e52bc74123ba134`  
		Last Modified: Wed, 23 Jun 2021 00:37:34 GMT  
		Size: 58.8 MB (58812906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c65c32ac33fcec60fedd0b9e713bcf0f7b704d59b14cce6afa4a06e55e315a1`  
		Last Modified: Sat, 10 Jul 2021 07:07:55 GMT  
		Size: 5.4 MB (5421908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57141b1c3dd2e33c1dc87ff3220529d62b3a28a6e52333c04f525f64ebea0006`  
		Last Modified: Sat, 10 Jul 2021 07:07:56 GMT  
		Size: 11.6 MB (11626506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd24e3c55ddd1ed96c7c862a05ae38a752d0f3a6e31ccd516d38b1305735e85`  
		Last Modified: Sat, 10 Jul 2021 07:08:20 GMT  
		Size: 59.7 MB (59667524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50807d3f45f2c70b78120e0bf7f60ea2a799c8b6adac4543d279a5167b07211a`  
		Last Modified: Sat, 10 Jul 2021 07:09:10 GMT  
		Size: 201.9 MB (201869353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:cafc1096e97f614a35bda2b3c136cbbca99f0a28ce90b462988d10fade98ccb2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.8 MB (300802642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93c170809d79a559e7340aa64469dda75d91b0b51a6bfb8ad0043507e24189fd`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 09 Jul 2021 02:50:46 GMT
ADD file:b2361f35b2807ada58f66b4f4f160b2133140a85db4ecd56889a15f080793790 in / 
# Fri, 09 Jul 2021 02:50:47 GMT
CMD ["bash"]
# Fri, 09 Jul 2021 03:45:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 09 Jul 2021 03:45:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 09 Jul 2021 03:45:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 09 Jul 2021 03:46:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:247ed76d4285ef2f620cc0d1ec3492f8a6d1b0cc613aadf4e236db73dc508cca`  
		Last Modified: Tue, 22 Jun 2021 23:45:59 GMT  
		Size: 53.2 MB (53184006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505ec6d09330482331a9028eae33a47ea63d93e1a9bc54bfa42d38acb5c49897`  
		Last Modified: Fri, 09 Jul 2021 03:52:25 GMT  
		Size: 5.2 MB (5152860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8deb9378139bc861b4f2d0bfd585ffc68556ca4e04c5183ea8b580cc82fb78e5`  
		Last Modified: Fri, 09 Jul 2021 03:52:26 GMT  
		Size: 10.8 MB (10763673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f70171ecb5957ac50a462e5f13de93884a90b3e113360311ab69d31a57639c81`  
		Last Modified: Fri, 09 Jul 2021 03:52:41 GMT  
		Size: 54.7 MB (54714913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d5837648e9bfab3121e812b06600d37490dd5ac0cd2c56788312c4d35a62866`  
		Last Modified: Fri, 09 Jul 2021 03:53:10 GMT  
		Size: 177.0 MB (176987190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
