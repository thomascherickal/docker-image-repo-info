## `buildpack-deps:groovy`

```console
$ docker pull buildpack-deps@sha256:135a3fbf8309905f065d95ef212412f5aa68bfea8b82971d2da289433a86a9e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:groovy` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:00a3208510e32db027fe564749ca0e8496aa820bf1536ac002b55bc032fb144f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.5 MB (254505030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f79a412760d307af1b089bfecb571daee4de63a8f38c4f1d68188fd42d10fa30`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:29:45 GMT
ADD file:aa87e1d15a8d4e3640ec67e03ae6c4421158f4c64c838d701d82eb34722a2e3a in / 
# Tue, 13 Jul 2021 22:29:46 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:31:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:32:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Jul 2021 23:32:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:35:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:87103eef5146121c4b54992b41b2da8c9e671d21961ba24cfe5c1756737d5698`  
		Last Modified: Tue, 13 Jul 2021 22:31:40 GMT  
		Size: 31.3 MB (31341566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a187db8c68613bb56c28a4f1c711d24248f3be342e2b2e98c6d162d37b9286c2`  
		Last Modified: Tue, 13 Jul 2021 23:46:40 GMT  
		Size: 5.4 MB (5404370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dfd548091a4b68a282f178caf8f237861b35ad281d3b8408ad339223262a181`  
		Last Modified: Tue, 13 Jul 2021 23:46:39 GMT  
		Size: 3.7 MB (3663412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9b58b1633551f88d8de925d153919fb1ff355ddf5ec050f245a0bb38d85093`  
		Last Modified: Tue, 13 Jul 2021 23:47:00 GMT  
		Size: 55.5 MB (55477811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94015c831320e7849327203f81a72aa1948761a33bcfcda83e29b149826ab691`  
		Last Modified: Tue, 13 Jul 2021 23:47:34 GMT  
		Size: 158.6 MB (158617871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:cfefe6871c081a029b704048fea0ab885ba557e3fe7204a5375b02f0e297474f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.8 MB (214844248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73b40e41fc34b091288b7658320c453c24df7624485cbb7aedb366939ec4004a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:21:33 GMT
ADD file:80b5f21ffac906a8416f39204cb526afaf64f15559123cb3a8fb311e312a703f in / 
# Tue, 13 Jul 2021 23:21:34 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:55:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:55:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 14 Jul 2021 01:56:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:58:17 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7ad80ac50e31c20115b0366841c81a92d1916a7f2113255fe1125324250475e7`  
		Last Modified: Tue, 13 Jul 2021 23:26:54 GMT  
		Size: 26.3 MB (26312397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87836ed84bb5f0e1d7b61439e8458826efce0a52158d32f928c2efc41367ac4`  
		Last Modified: Wed, 14 Jul 2021 02:19:01 GMT  
		Size: 4.8 MB (4840704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4a0657bf22de96a1925b7c31d415ed9eff49f3b00971444459ee9b696832ef`  
		Last Modified: Wed, 14 Jul 2021 02:18:59 GMT  
		Size: 3.1 MB (3140633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e419af2ccab0c7223c92ce4cd8deaa2cdea7e08e02b9636ce5f7193b06162f6d`  
		Last Modified: Wed, 14 Jul 2021 02:19:51 GMT  
		Size: 50.3 MB (50301608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75d23fccf18c2c25afdbd5f5c752e3d98caedd067df7b81922dee720a356aba7`  
		Last Modified: Wed, 14 Jul 2021 02:21:27 GMT  
		Size: 130.2 MB (130248906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:74346f6689407d4b7d2c00f028c6bd43dfb7c3e4035c3f1ca17e8e4102b73dd6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.3 MB (246301438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6dd48a58460df909e36d1c39f7adad3da705448cb4ef6809aed0407f6ba65d8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:01:34 GMT
ADD file:8fe3c90118921d388c31ca28a21ff713dd718197e04654c6e0b7a09435f5287d in / 
# Tue, 13 Jul 2021 23:01:35 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:53:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:53:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Jul 2021 23:53:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:54:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3da8512ba050381848a454507530b9a467063e06b22a25eddc01311dbdf35301`  
		Last Modified: Tue, 13 Jul 2021 23:03:58 GMT  
		Size: 29.9 MB (29877377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055ca1e90e094916911d8a92553fa0422dd53e6e43fed33614623edae8ca22c9`  
		Last Modified: Wed, 14 Jul 2021 00:02:57 GMT  
		Size: 5.4 MB (5372770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:955901556b2298b0b4c51d2c60f4312309d050d4152c6e9cbf8a27cc02b9357d`  
		Last Modified: Wed, 14 Jul 2021 00:02:57 GMT  
		Size: 3.6 MB (3635077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc45f76631624206ef01b5b63f98f3e506bcaedcefd4804326ee884f3b4dcb53`  
		Last Modified: Wed, 14 Jul 2021 00:03:19 GMT  
		Size: 55.5 MB (55471055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d970087ecd9605efafb3ba6bbb018a6cd547297e1af14384cb1beb802de0ce31`  
		Last Modified: Wed, 14 Jul 2021 00:03:56 GMT  
		Size: 151.9 MB (151945159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:504e8ba181b570eaef3ef5c3d4d5cafecbef0673a95f350757e3487eee9b2f68
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.2 MB (273180579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1030cd605ec9b4d40447f0f22d1463d420e5206614def290ca4b9499a7442da4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:22:45 GMT
ADD file:d810eebdcea73da6a0b9c4546fc356b13b60da24827c29923375b8e08f2195b4 in / 
# Tue, 13 Jul 2021 23:22:53 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 02:27:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:30:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 14 Jul 2021 02:35:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:49:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:97b0da8da7b9eb227e28852cb467ba3f76ac379708648200f035c072d3bbf4eb`  
		Last Modified: Tue, 13 Jul 2021 23:28:00 GMT  
		Size: 36.6 MB (36562496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19019a66a1c7600fb2159a63b0e68f36b9d9f55e9e56ae7b70139ac7565616c1`  
		Last Modified: Wed, 14 Jul 2021 03:24:17 GMT  
		Size: 6.0 MB (6040945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b7e113d40008d7a4f01ffb65b6bee553ec1af6ea5935387bfc2677d6a9888ba`  
		Last Modified: Wed, 14 Jul 2021 03:24:01 GMT  
		Size: 4.5 MB (4522053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f499186162dbbd18ecdc41e48723d94384601a434160e441c62890afc5a08b62`  
		Last Modified: Wed, 14 Jul 2021 03:25:24 GMT  
		Size: 63.7 MB (63743445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c65e3158288b5ef034817618aa0df8c144e091a87018c0cd3a8c2d3d2ea551b3`  
		Last Modified: Wed, 14 Jul 2021 03:28:07 GMT  
		Size: 162.3 MB (162311640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:adbfe496e96596c1b9234df120224777fe084c8702e0d05df7de2c37f3b1732f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.4 MB (249444530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54d67063d599e64b7cd825ddc7de1dfef33eb6cdda5ed9c3652e8eb1a90b4ebc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 22:53:46 GMT
ADD file:02a1c687ec9417cdf601518590b3a21fe31a0ebd2cdeb9bc63792512b95de989 in / 
# Tue, 13 Jul 2021 22:53:49 GMT
CMD ["bash"]
# Tue, 13 Jul 2021 23:43:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:44:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Jul 2021 23:44:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jul 2021 23:45:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:412af85569a706b682c00eeeaf32aeacbe1a5df158e5b67ddff07842b7ba3080`  
		Last Modified: Tue, 13 Jul 2021 22:56:02 GMT  
		Size: 31.6 MB (31577497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25ed9de239c255124abaa7cd10a81a3e295829e47c8f990a740c9de4638d328e`  
		Last Modified: Tue, 13 Jul 2021 23:52:18 GMT  
		Size: 5.6 MB (5629821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f612d9fc542d056eb20ee90480c45cf9b38afd821365ceecc6ce517204872126`  
		Last Modified: Tue, 13 Jul 2021 23:52:17 GMT  
		Size: 4.2 MB (4156765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9768d4aa6766f231a99a9bffe76e6867dd9a5d208327f84e9e8997bf8989ad81`  
		Last Modified: Tue, 13 Jul 2021 23:52:34 GMT  
		Size: 60.7 MB (60667046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a3470b06ed7ef25f706bed791068196c18b4a6421cd62dbdbf2516a71c9b8a1`  
		Last Modified: Tue, 13 Jul 2021 23:53:02 GMT  
		Size: 147.4 MB (147413401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
