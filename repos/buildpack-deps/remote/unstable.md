## `buildpack-deps:unstable`

```console
$ docker pull buildpack-deps@sha256:895ae7a594d3441c911a779ac753c4fa13954fa0793734f78e741e83d248e8be
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
$ docker pull buildpack-deps@sha256:22c1e534c3e578517b1ea760e01644e61a3b7740d3103e4f40fc154e707eaf29
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **566.5 MB (566505226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c1cab691ffc57745b6e37b92106d9a56c5f99afa144a4b616b118be861e067c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:09 GMT
ADD file:e5210ca55e6714aec9564543eeb4b4a748c57e62c0ae0c741dd0f3eb75ab72de in / 
# Tue, 17 Nov 2020 20:23:09 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 00:39:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 00:40:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 Nov 2020 00:40:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 00:42:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:648de6ce4c8700aa65bb00de61082bc80448ba5410d2558ccd0f8c5e5616dbdf`  
		Last Modified: Tue, 17 Nov 2020 20:29:13 GMT  
		Size: 56.0 MB (55978493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330a58a1358b2808071560abfa71693ca944d1732a1543c107859d521b29bd65`  
		Last Modified: Wed, 18 Nov 2020 00:52:36 GMT  
		Size: 5.1 MB (5063542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a3e6e253f47148f777fe41db1237b0eba7f14df71ec26f973f35c05182b4173`  
		Last Modified: Wed, 18 Nov 2020 00:52:36 GMT  
		Size: 10.6 MB (10646140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae65daff77b5d6ac0619bc955c2b1edd6ad35d46f9ad26b02f3de5bcd0951da7`  
		Last Modified: Wed, 18 Nov 2020 00:52:58 GMT  
		Size: 53.8 MB (53755325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155b9a2d4912e6c32ac6b9883f0eab9b129add3d6156e21d1d7cf0df74321895`  
		Last Modified: Wed, 18 Nov 2020 00:54:28 GMT  
		Size: 441.1 MB (441061726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:430bef2ee6157d5117c286b607bcee4a1bd8708941cf6e84fcbbd195093a96ce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **457.7 MB (457732851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:210e1a03754642ad449df07477a466af2bf2183b010d8d89f4a6e3805f5cd224`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:07:43 GMT
ADD file:a57353f597051225232a9e7abed847b86e4c6dddd2072732b4625acbac7128fd in / 
# Fri, 11 Dec 2020 02:07:47 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:50:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 02:50:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 11 Dec 2020 02:51:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 02:56:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:af6b8b544b162386c7b3c6d5c131158e341ff3b454198faf077cc6c1427321df`  
		Last Modified: Fri, 11 Dec 2020 02:17:13 GMT  
		Size: 51.3 MB (51288429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e601c83f1a1756a052d156762b6629539a7e67063cb8852d73fb18958f7726`  
		Last Modified: Fri, 11 Dec 2020 03:08:38 GMT  
		Size: 7.5 MB (7464314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6a25346e41f4aa7fbe4f2fbf817bc776305935298bbe8403d2b5fd5ebec3a8`  
		Last Modified: Fri, 11 Dec 2020 03:08:38 GMT  
		Size: 10.3 MB (10335112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e79e0e8b81251e6ee4cee77ecbab7ff5bb7a5ab9d1f135cf518b6b99ca6886`  
		Last Modified: Fri, 11 Dec 2020 03:09:05 GMT  
		Size: 51.5 MB (51532233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6962025ca49fb9f2d78bd22322e3b7ed1315da7e48cc64cab6435677183af402`  
		Last Modified: Fri, 11 Dec 2020 03:10:48 GMT  
		Size: 337.1 MB (337112763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:49a5d31c6670bf46eb98acde17b1183cd65d49092a1413e77b15f3adb4425fe9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **431.4 MB (431445583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93924d62d3248da32a32b352662359bb1d3dbe0424da4a978f76b83e88af683f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:26:33 GMT
ADD file:fa1941c40adf31f1de7cad83033e24d208bc560e0818d6c0977fe2e74ef87e0d in / 
# Fri, 11 Dec 2020 02:26:39 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:29:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:29:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 11 Dec 2020 16:30:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:34:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:54bf394474a2aad8c49632d0f0974854752ca4ff40354a996cb0806ea65d7253`  
		Last Modified: Fri, 11 Dec 2020 02:35:33 GMT  
		Size: 49.0 MB (48987318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d959969d53555f2806838ef7825603115e52bc31662dcb17623ba77bf941b1a`  
		Last Modified: Fri, 11 Dec 2020 16:45:13 GMT  
		Size: 7.2 MB (7203302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f104a599ccc89fa932a5c9977f3f9e107d9364f7c408f3d954dd2fc7475cd05c`  
		Last Modified: Fri, 11 Dec 2020 16:45:14 GMT  
		Size: 10.0 MB (9974214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc95b5f2d19ce2f5db34e78db2ba59c101fa341c37c56cee3b9c474bbd05b03`  
		Last Modified: Fri, 11 Dec 2020 16:45:39 GMT  
		Size: 49.6 MB (49589026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677d2e7e1dba8c8d8230282167bf2c8666cba3b933e1fdbd62010d6ec104ac2b`  
		Last Modified: Fri, 11 Dec 2020 16:47:10 GMT  
		Size: 315.7 MB (315691723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:fe2ca744afaf8b05bd61b87a692f26e6bff4bd81bf419a3704b0aef228ca4b51
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.3 MB (542337960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d48d27c58f4e0d671c7f4cbb8abb7f00892116b3108ebdd9c55e30496173c863`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:24:57 GMT
ADD file:dd38237d30f418925f9d05a463817130964bc613d39a38eeea7b87b9b5d62608 in / 
# Tue, 17 Nov 2020 20:25:15 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:24:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:24:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Nov 2020 22:25:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:28:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:28adf41b7f9d0f64232c0970a16416d0ef2eaa00df57f3caf5d257ccbd3b206c`  
		Last Modified: Tue, 17 Nov 2020 20:33:04 GMT  
		Size: 54.7 MB (54719929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516539a7ff1b41bcd60f56a25019366722df8db637f7a409ba85ab9918633b31`  
		Last Modified: Tue, 17 Nov 2020 22:38:10 GMT  
		Size: 5.1 MB (5055909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58beb0eca7357870a7d9572e6897310b7dbb65ea59a9f76afc5b75a63c11820`  
		Last Modified: Tue, 17 Nov 2020 22:38:10 GMT  
		Size: 10.6 MB (10648403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ffef1fd67608c1c75fe7d564719a6e2a098fe43f43dfddc1dac311b1fccbd61`  
		Last Modified: Tue, 17 Nov 2020 22:38:34 GMT  
		Size: 53.9 MB (53856622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bddf2c576d92722b49ba9e3fa4118f5d40203cb0a93d662a0bef0608dd5337c`  
		Last Modified: Tue, 17 Nov 2020 22:40:25 GMT  
		Size: 418.1 MB (418057097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:b4f48f5081530f06a9688d64f0b6886611d0db989156ab446429327cbae3aa72
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.6 MB (327584509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f38ec6dc2e66a432e7b8ba09e78000c8a74114de074c4f64de702767626aa22a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:59 GMT
ADD file:6d6afa8490ae5ac639c8369b0f5d9f8e49c675672ebd5348a955a3c9656453f5 in / 
# Tue, 17 Nov 2020 20:22:00 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 21:17:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:17:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Nov 2020 21:17:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:18:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be81561500ea27b67d364b1567d73e6fbfac19e1739e5b1e5674dbea758abedd`  
		Last Modified: Tue, 17 Nov 2020 20:28:52 GMT  
		Size: 57.1 MB (57102236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc436cb880e1d23236f4f748fe380b16b0e16955049a2c0c1ab65456f67c2a49`  
		Last Modified: Tue, 17 Nov 2020 21:26:18 GMT  
		Size: 5.2 MB (5183137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca3e53afca84ddbe3333e0b6c779a68bb454199b167cfb74eda23f74fbea675`  
		Last Modified: Tue, 17 Nov 2020 21:26:19 GMT  
		Size: 11.0 MB (11022846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c97dd1237dfa1a40c9c2255e2dcdec27f7d739925bf6b97716b25759ca483baf`  
		Last Modified: Tue, 17 Nov 2020 21:26:43 GMT  
		Size: 55.1 MB (55068291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55cd3cf76c418768fcf3ace450c7c1799978e869f11ca050afa9e8bd5cf872cd`  
		Last Modified: Tue, 17 Nov 2020 21:27:39 GMT  
		Size: 199.2 MB (199207999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:a1a6aad8675f931dfdefb3e83e3020eeb3df281efea42d74c1b16eac9e9cbf82
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.0 MB (306970428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d8c83b541ef707dd52683ba53770359be38b0f9b16823c6d39d8c2ee25a02f5`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:55 GMT
ADD file:144f263fbf8197586830814ff675d3c7d3ac8e3df7debe6633a1e91f84ff845b in / 
# Fri, 11 Dec 2020 02:03:56 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:54:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 02:55:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 11 Dec 2020 02:55:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 02:58:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b60fb1f705939e8d3e124cd99cb825ac48613619a7a75de5656f0bde8bb1f05`  
		Last Modified: Fri, 11 Dec 2020 02:11:04 GMT  
		Size: 52.1 MB (52069726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dc2b81267c2dccbb94aa4a39fbd561e967b04505581d2d37c94c116454be253`  
		Last Modified: Fri, 11 Dec 2020 03:05:44 GMT  
		Size: 7.4 MB (7430898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d8b7d4e3509bc9ab5283dda924581973c2fe390d34bf794abb077b094d9c66`  
		Last Modified: Fri, 11 Dec 2020 03:05:44 GMT  
		Size: 10.7 MB (10656680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8630910440ff90347edf0df6f5aa5bbd3ea4e62bc74dcb04c8d9258f587cea26`  
		Last Modified: Fri, 11 Dec 2020 03:06:35 GMT  
		Size: 52.6 MB (52583421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f69ed486ad3ec09eb62cc8759474df0a318fe49478c4a6db9337fdf634e7e94`  
		Last Modified: Fri, 11 Dec 2020 03:08:46 GMT  
		Size: 184.2 MB (184229703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:3dd6d337cddaea0c306988075494019f277996e3f2cde8348e5213fbfbf07b93
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **554.3 MB (554282455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2186507bc8952aad46980914c18d99b230abf0d4324161a077b16d9d48c2bca`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 23:23:29 GMT
ADD file:d9f4936d2b1902ef4008c438adfc5b11813d611494bbe59a59f77de4d57c5c8a in / 
# Tue, 17 Nov 2020 23:23:40 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 01:22:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 01:24:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 Nov 2020 01:26:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 01:44:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e7c5331f40f844384a2b7c7835ce9547f6d5cb22a3b99e72b08ef585bea2c3bb`  
		Last Modified: Tue, 17 Nov 2020 23:34:29 GMT  
		Size: 60.2 MB (60189345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c542ef20d7487b58e220d23902720f3093c22a2ac72bde481e08d93fac8c924`  
		Last Modified: Wed, 18 Nov 2020 01:58:07 GMT  
		Size: 5.3 MB (5302640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c93377737fbee467c96f243247282c2535ef88e661736d10f42cdc6bc9e340f5`  
		Last Modified: Wed, 18 Nov 2020 01:58:04 GMT  
		Size: 11.4 MB (11408357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c985b343229d58a1bfd5aec2d9290e1a79d9d409d1b346405b6d8d976d3de80c`  
		Last Modified: Wed, 18 Nov 2020 01:59:51 GMT  
		Size: 58.1 MB (58113996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4402ba2d44ea224fd7243a4aadb54aa58545b00679d88b41e00f6327c690f0d`  
		Last Modified: Wed, 18 Nov 2020 02:05:31 GMT  
		Size: 419.3 MB (419268117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:d4ce960f6250b59569f68058399c00c1927dcfdb5080792a7baf754ac3a4bb98
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **431.7 MB (431654726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6ab976c1d143015edb1d841c3c527ade12b75d60269eb8cd44abf98797ac97e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:12:29 GMT
ADD file:81f25bd988cd2db6809416e7139b279a1a04ce8e2b864c71e35768d7211232db in / 
# Fri, 11 Dec 2020 02:12:36 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:07:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:07:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 11 Dec 2020 16:07:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:11:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d882124dbf8a54501109f018ee08c93cb805beed092d3bf2e6979740fad5f861`  
		Last Modified: Fri, 11 Dec 2020 02:17:27 GMT  
		Size: 51.9 MB (51894888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf6b2001d1a8b91d37dd19d21d1f31ce0dfcc83648225746fdc024ebfa8f686`  
		Last Modified: Fri, 11 Dec 2020 16:16:50 GMT  
		Size: 7.6 MB (7585246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c42824152b87e26d9c06509c0a9035c25ec1a1740793c472931585f433c904`  
		Last Modified: Fri, 11 Dec 2020 16:16:50 GMT  
		Size: 10.5 MB (10525335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeaadbfa1d0a0ab4d448f235e351c619f71777466221df7ff844225f0a1e6221`  
		Last Modified: Fri, 11 Dec 2020 16:17:11 GMT  
		Size: 53.3 MB (53324935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4744a27ddee31a26edb928ce537ef044ce60cbc7c2a081bf2a6890c47684d827`  
		Last Modified: Fri, 11 Dec 2020 16:18:05 GMT  
		Size: 308.3 MB (308324322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
