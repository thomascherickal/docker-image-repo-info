## `buildpack-deps:bookworm`

```console
$ docker pull buildpack-deps@sha256:2061a2c470af87747c3bec8e2dfc1efc7a241c8d0e3a22be224426b505132880
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

### `buildpack-deps:bookworm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:7d3febecfaee0066c271d56cf4d9ff4db2d11c84bee903e59dd77998d2559fad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.6 MB (344648174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fc869086722fb708453e59e77c90910944a91b539d4da0d5c8f43fad4786035`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:50:57 GMT
ADD file:59c477049f0246331c6723687b7f8995e7a8946172b967d10fb8b67146220c33 in / 
# Sat, 04 Feb 2023 06:50:58 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:20:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:20:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Feb 2023 07:20:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:22:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:20aeb9ca89f41415a92cd1a5e9ff6c0280e09a250e0f950c9df57d97b0d3efb5`  
		Last Modified: Sat, 04 Feb 2023 06:55:19 GMT  
		Size: 49.0 MB (49043016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd16dee5feec7a2da71bdef1f07b5a546389f1554d69d474530b8f847d0c1890`  
		Last Modified: Sat, 04 Feb 2023 07:28:22 GMT  
		Size: 9.0 MB (9033132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba40466925cfd251e3c9b97a519794ed3580ca83f2135be0ccea17e5b2d6f99`  
		Last Modified: Sat, 04 Feb 2023 07:28:23 GMT  
		Size: 11.4 MB (11354722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e5912b196c98527faa75de1f03b026f5c2740634e4a9498c536214352bbd910`  
		Last Modified: Sat, 04 Feb 2023 07:28:40 GMT  
		Size: 64.4 MB (64444820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ef8ca27ca4b3d886b88f1478d0aaf27aa1a473c66efce2cc36dc72160b423e`  
		Last Modified: Sat, 04 Feb 2023 07:29:16 GMT  
		Size: 210.8 MB (210772484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:911d51edac0adedf0e794af3776caf33a212603429d431318ab404b352f2c58b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.9 MB (313906409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25bd69faabfb49684f497e14c34b369d080e3c187499ddfc5fa5f933f38d88b6`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 02:45:51 GMT
ADD file:6283625dd02e5a15e67c45fb0ce9fec384c9086563a64fbd85ef7eec12283466 in / 
# Sat, 04 Feb 2023 02:45:52 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 03:13:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 03:13:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Feb 2023 03:13:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 03:16:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8a4b4311a2a6055167419fac8cc987d97e7a797e53f6176ee2b5d0e6edbde230`  
		Last Modified: Sat, 04 Feb 2023 02:50:25 GMT  
		Size: 48.0 MB (47993284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35559dda00a93e84323ff0a3cd944fd9cebe193cb866743b2bf5d33ac8f7ecd7`  
		Last Modified: Sat, 04 Feb 2023 03:21:50 GMT  
		Size: 8.5 MB (8481336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69dbad85bdc4db8aa9aaa97d1620037878a7830e27a0a13e6913172f0885cba0`  
		Last Modified: Sat, 04 Feb 2023 03:21:50 GMT  
		Size: 11.0 MB (11001821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b85ad8323370f7fbfbc955cee459d994385944146584314db17353d54e588b16`  
		Last Modified: Sat, 04 Feb 2023 03:22:13 GMT  
		Size: 62.0 MB (61978188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e9c0f54ea5320afaad6fac2f4c85b31f181810998dbb3f67fdb0396b69ce0b`  
		Last Modified: Sat, 04 Feb 2023 03:22:57 GMT  
		Size: 184.5 MB (184451780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:d354cd4f92f98fd85ba9681b2f5eff8449194d3fb46efcf29b650bd805a009a6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.2 MB (299240721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:060f8854eabbaa0140db38f3fd12c1abfd7d85487823d773fb00d9a1678b57e4`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 09:58:46 GMT
ADD file:7fa388eb21c424f9b3d978f277c454b5cb8a4c4fc0dac864298e9cf12161b132 in / 
# Sat, 04 Feb 2023 09:58:48 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 10:46:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 10:46:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Feb 2023 10:47:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 10:48:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:16b554b0ae696936d2556c56490dc1cb7af234f9a415a93932213ba90d19bd85`  
		Last Modified: Sat, 04 Feb 2023 10:05:12 GMT  
		Size: 45.8 MB (45794144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37939da9cb6c3ba4566c2d20c05dee5ec7361c07649557a19b8e8d844ef0cf4`  
		Last Modified: Sat, 04 Feb 2023 10:57:57 GMT  
		Size: 8.1 MB (8124732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20d72a01582fa10ad6cbabe8e802a8e57b4fb57dd818ac7cf92815d91a6a0a55`  
		Last Modified: Sat, 04 Feb 2023 10:57:57 GMT  
		Size: 10.6 MB (10635854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a385e0a6d4d5d7a96989b13b2566ab1876cc3c1183e9bb336d6f3fbfee7df420`  
		Last Modified: Sat, 04 Feb 2023 10:58:19 GMT  
		Size: 59.6 MB (59629907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726920a24cced39467d99f2c4569e91f54cfe6377422b1c702d0774f3e039417`  
		Last Modified: Sat, 04 Feb 2023 10:58:57 GMT  
		Size: 175.1 MB (175056084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:88cc2b989fa72d56437d6c5cc80d27eedabfff5568a8c129d65da94bf075cf8a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.8 MB (335793973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e15efaf3ff558b8e656be9c3b5ea2af453ced4461ab10c7667c735af9d65b76`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:08 GMT
ADD file:b40ad920bd7dd081e20adf36435db50381b9998a1de3d2eac6b2c45734ce60b3 in / 
# Sat, 04 Feb 2023 06:17:09 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:43:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 06:43:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Feb 2023 06:43:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 06:45:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a43b5d5927a7651097e784be4430a6ade09951f5b6879cd06b0f51fc7c4812af`  
		Last Modified: Sat, 04 Feb 2023 06:20:30 GMT  
		Size: 49.1 MB (49081538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f6dd523027aa16778d661d27e72bbe882cc841d9a40bcf7ba993f9653c66e5`  
		Last Modified: Sat, 04 Feb 2023 06:51:08 GMT  
		Size: 8.9 MB (8865599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef33a1f8ffdb43ea2d51e44c388d4de6bedede50060c1397f6ae0eff23cd307`  
		Last Modified: Sat, 04 Feb 2023 06:51:09 GMT  
		Size: 11.3 MB (11319794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f81f9fe3edb2827f590b523951ed4c6d26f17d9aa521c3b4da9f99c21d74bb`  
		Last Modified: Sat, 04 Feb 2023 06:51:25 GMT  
		Size: 64.3 MB (64337322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e60ca384af68da7f39c9a4d38819036b92341935e4eb94617faede0e25f6e5d`  
		Last Modified: Sat, 04 Feb 2023 06:51:54 GMT  
		Size: 202.2 MB (202189720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:4f003c11513c0b6ab61af9bbb9228e0858525f53ca1dfeb08d8b24535a9e0f7a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.9 MB (346853795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b31150f5b93bfee2f1531241c9e358a19a708605dbd0f4e8867112441a85d494`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 07:48:40 GMT
ADD file:71f93fd08314b2207fb2e5840185c4db4279fa8f008742cf35eaf4daf925d475 in / 
# Sat, 04 Feb 2023 07:48:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:17:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:17:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Feb 2023 08:17:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:19:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0b6e1871a6864b2026696c7ffe48da3030a97146a6a0f3ca18f87c19b1ed6e05`  
		Last Modified: Sat, 04 Feb 2023 07:53:55 GMT  
		Size: 50.1 MB (50093420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd7274669ca31ae25c99ffbeb62b7bf63cf6e70c0afea787b6483e8e1e233d5`  
		Last Modified: Sat, 04 Feb 2023 08:25:56 GMT  
		Size: 9.2 MB (9211501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:222e731d14a700e618d6e7298602f00a0ac9884fbe12a867349d9a13ae14bb4a`  
		Last Modified: Sat, 04 Feb 2023 08:25:56 GMT  
		Size: 11.6 MB (11557630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e9553d1e75be1e95f064cd22c826152b2da62a778c20ddc098b2c20f0575749`  
		Last Modified: Sat, 04 Feb 2023 08:26:15 GMT  
		Size: 66.3 MB (66316077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea46a0242002669ddfb4948fc0ce1d00941d8e3fa2de8699c0aea1d605498232`  
		Last Modified: Sat, 04 Feb 2023 08:26:50 GMT  
		Size: 209.7 MB (209675167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:e69e8f6879a0fd0432ef558dc0dd32f3b8a5b963528f37554406a3064df08c3f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.3 MB (321271968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecdc01153df0ddeb48ce721788df849fc1f7bbe378afaa25c0a6618c12739a72`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:18:13 GMT
ADD file:342f09d1a542544d0b028faf681c7e97bab2676412290d4af1ab83b550eb0404 in / 
# Sat, 04 Feb 2023 06:18:16 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 18:28:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 18:29:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Feb 2023 18:31:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 18:37:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:811d77d1a16ee11b725d10eee34b4675405052eeace5043fea40862dac9fd740`  
		Last Modified: Sat, 04 Feb 2023 06:26:25 GMT  
		Size: 49.0 MB (49040889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eafe731118197b5c6270a970451012408dca08211806ef6c76de0197dc4f22a8`  
		Last Modified: Sat, 04 Feb 2023 18:55:35 GMT  
		Size: 8.4 MB (8398884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c759c150dc8306fa76a100d6e285e0915607f68c337e5c8945cda21cd969e07`  
		Last Modified: Sat, 04 Feb 2023 18:55:35 GMT  
		Size: 11.1 MB (11105541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb4fb677a2bf15414c11724d537f9a7ebb14dc180003acbe2ea4e0dd362d3e3`  
		Last Modified: Sat, 04 Feb 2023 18:56:29 GMT  
		Size: 63.3 MB (63326700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f3fee7f92fc40e96c27bdf0b217e0cebd4c0ec300e18cbd3b5bd10a341f629`  
		Last Modified: Sat, 04 Feb 2023 18:58:40 GMT  
		Size: 189.4 MB (189399954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:3334473e3189565f9cdd7ab5830df11edbff1eb407b85d8f68d7af846a839574
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **358.6 MB (358624832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e9b53338974279ffd58fc5e14a4aaf0a5f159394af1f515267a4c6b993e6cf9`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 12:24:35 GMT
ADD file:75252aac3ef2cfeb95bfa5e27d34d7632e938a4cc508e662b033aebb438bf9ed in / 
# Sat, 04 Feb 2023 12:24:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 17:56:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 17:57:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Feb 2023 17:58:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 18:01:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ad7bb1bf81ba24a5e75d96e5759bfa08a04cf654eda26010b8b1bdd6eead92f2`  
		Last Modified: Sat, 04 Feb 2023 12:30:47 GMT  
		Size: 53.1 MB (53066627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a43d91cb4f1d38d440125ef18b21ed870c9dcca915dc7e20243430d8adac5f`  
		Last Modified: Sat, 04 Feb 2023 18:12:46 GMT  
		Size: 9.6 MB (9613419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42696410cee2c14decf6673c1f2af21d8399af5087bd8d0a8aa5836b6eb83e2`  
		Last Modified: Sat, 04 Feb 2023 18:12:47 GMT  
		Size: 12.1 MB (12114689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b254d8489afdf84cf599567f5cd06ddb9dba650b5f29b68b0ecdfae7fc17d0f6`  
		Last Modified: Sat, 04 Feb 2023 18:13:18 GMT  
		Size: 70.0 MB (69970306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8576d26009e4ee991f02ea471ea3e02a044c3b70ee6721405e66572465730c`  
		Last Modified: Sat, 04 Feb 2023 18:14:27 GMT  
		Size: 213.9 MB (213859791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:d43d58048dc72bbf79a62da9c29384f7d80b3417899c2c6ef67c8c7a07cb0df7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.6 MB (313623657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daa45557df4039ea181329faf4cf1746d95e1c5f1093b34b86b9631888bb5b33`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 04:05:23 GMT
ADD file:cac3f762206c0f8ad807211cb73145ac093d8917f5b8cf3a79eea3ef1fd14eea in / 
# Sat, 04 Feb 2023 04:05:26 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 04:30:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 04:30:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Feb 2023 04:30:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 04:31:48 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5788bb4f4cdc5bb0c03495b0d17914750f0dffcbdc053321669358a95967dbed`  
		Last Modified: Sat, 04 Feb 2023 04:09:43 GMT  
		Size: 47.4 MB (47429742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1e84e5465158af09efec27ef891007b9bd6994985807b81f054e6b39a0cdf0`  
		Last Modified: Sat, 04 Feb 2023 04:38:50 GMT  
		Size: 8.7 MB (8666425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a1fe479ceec98fa274b9f162d0d9d0a555e7ecadb9aaa64ad94b2423e5d22a1`  
		Last Modified: Sat, 04 Feb 2023 04:38:49 GMT  
		Size: 11.2 MB (11218182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b390826d9588a3304d3449fb7e5d2594d77558be4387e3fb22b9188f1bc4c4`  
		Last Modified: Sat, 04 Feb 2023 04:39:04 GMT  
		Size: 63.4 MB (63413204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f173695e8b20910d073734310e8db6aed8b8704417cdcacd4fb5c9fd9e69637`  
		Last Modified: Sat, 04 Feb 2023 04:39:31 GMT  
		Size: 182.9 MB (182896104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
