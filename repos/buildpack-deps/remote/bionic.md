## `buildpack-deps:bionic`

```console
$ docker pull buildpack-deps@sha256:9fd1bd60ef4fb6123e4e4c8874cac211e0d563dad6b188f64574e33eed1094bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:bionic` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:8e193981b35a706985cdc98b60c03e5542e213ee488587b2d9958940c84561d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.4 MB (221393894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2608fa2156d0a642f6ac431b67743a605276f1e936f72ecc653a3da10b792ea4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:04 GMT
ADD file:ed601c56cf74241eeb1971b24ed969fb855cd2b9330276d3c5779ecdb0b28364 in / 
# Tue, 04 Oct 2022 23:35:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:00:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:00:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 01:01:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:04:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e706e0a9f42365312b366bf4caa22f3cdd8fc7fd8f6f49b4dd3782711f66aca7`  
		Last Modified: Tue, 04 Oct 2022 11:37:26 GMT  
		Size: 26.7 MB (26711852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14bb308d0caa16e5231c4d889948a8b0c06b9e2c461919c74887b27e349d490`  
		Last Modified: Wed, 05 Oct 2022 01:22:33 GMT  
		Size: 6.6 MB (6631019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd853d7120feb9f81650bf7bc95fac3a301e6f7fb667e27ff0c44f05fc3bd84`  
		Last Modified: Wed, 05 Oct 2022 01:22:33 GMT  
		Size: 3.0 MB (3023747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e261a80722021da4732449560d09c9be0f3a45bc7cd83a11ec75216c88d19d8`  
		Last Modified: Wed, 05 Oct 2022 01:22:50 GMT  
		Size: 45.5 MB (45498303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f4264228ed8e7647983ec917c22f259b84a520ddaee10cd3d968f9c68bff1ac`  
		Last Modified: Wed, 05 Oct 2022 01:23:19 GMT  
		Size: 139.5 MB (139528973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:8c42ce93b617d12c423261ac5d8a9b5949385d3ee604c85ab12add1f2354b260
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.6 MB (189554619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fd4e33dc0507b376b73e9f97cafb185f57745359d69c95771a51290fe3c978a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:13:31 GMT
ADD file:20e0d71059d38b1e18636b9db71f534d7297c3f571d73d45a75b4b8d3cac86c7 in / 
# Wed, 05 Oct 2022 00:13:32 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:40:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:40:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:41:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:42:24 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:91bb9a9844d67fd31f07ebd74dc8a4f4f18e2f959d3aa2166aca86ae57f353c6`  
		Last Modified: Wed, 05 Oct 2022 00:15:26 GMT  
		Size: 22.3 MB (22305721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5da5c18a3ec9c91b23737d7223b602b070f7de605771c25aadd8092545e561`  
		Last Modified: Wed, 05 Oct 2022 00:57:59 GMT  
		Size: 5.7 MB (5697196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327d003e6583d861f4c3df07410a51c18c3b7f4a0649fbfde6aab1ec77b4b110`  
		Last Modified: Wed, 05 Oct 2022 00:57:58 GMT  
		Size: 2.6 MB (2585088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdc6a2f528031e62d90580aa8ccad6d2351f1de9a49f1ebeed4945a07ffeed3`  
		Last Modified: Wed, 05 Oct 2022 00:58:23 GMT  
		Size: 40.7 MB (40690856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dbc06c808278c578a9ebcf12b02c2e632f8eb0c39fa50538a9faf7483bd4953`  
		Last Modified: Wed, 05 Oct 2022 00:59:02 GMT  
		Size: 118.3 MB (118275758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3e79fc3dd3b14b9bb575350832102635634b50d09fc0e17787f8ab9461363820
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.0 MB (205988599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:307ed33f4f8918cc97443f064b1a80b4169652a8a5830856adc59899d807e672`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:56 GMT
ADD file:585011162da73734395f2ef251ad89b72cfed0101c7da2435fac55061f99b516 in / 
# Tue, 25 Oct 2022 05:54:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:03:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:04:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:04:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:08:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a217cb16e35b382d60a7ab454a8c4db0fbe5e0aeec4b4c346e51eb1e77d34f8c`  
		Last Modified: Tue, 25 Oct 2022 05:55:45 GMT  
		Size: 23.7 MB (23735856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296237f400b08de0ee2566d1d70f0c0fa8e7334ec80823903e2aaf4904c5a49d`  
		Last Modified: Tue, 25 Oct 2022 08:33:20 GMT  
		Size: 6.1 MB (6074795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82de00773434d5186afe917dba4d4a8e731ffb220b4b8b348628c4df9f9e773e`  
		Last Modified: Tue, 25 Oct 2022 08:33:20 GMT  
		Size: 2.8 MB (2790789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ead073af2bd060ee0645628a8ca9a37e4f01b5c89e089690cff894da4eb30b`  
		Last Modified: Tue, 25 Oct 2022 08:33:34 GMT  
		Size: 43.3 MB (43296375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ac6f110046b149cfabf2ddff78dd4a130eeac7523196ddbe458ecf807d0656`  
		Last Modified: Tue, 25 Oct 2022 08:34:01 GMT  
		Size: 130.1 MB (130090784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; 386

```console
$ docker pull buildpack-deps@sha256:88842772446e48882fcdf20872ab09cd43f8fcb75681fa5f61b926dc8644445f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.2 MB (218240056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0daef8c85d992fa89d4cc85af6ebe982b049919dd5c9fd4465b81a65a9cd2bd9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:34:56 GMT
ADD file:40406c12653f21504e334fcfb19c00ee9eed94dbaa2eb7c7bfdb293677697aa6 in / 
# Tue, 25 Oct 2022 02:34:56 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 05:20:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:21:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 05:21:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 05:24:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1beb66ce54f29e44b5005bf3e2d004424176aa3361ee8e602a9ae10a8ee447cf`  
		Last Modified: Tue, 25 Oct 2022 02:35:33 GMT  
		Size: 27.2 MB (27166059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196f1fa30db3bbf53093b5c7d1d2add129bf1974ce53a6e094f0f0795c7881e7`  
		Last Modified: Tue, 25 Oct 2022 05:31:10 GMT  
		Size: 6.9 MB (6921884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f025677e2376712e8fb9824f1fcfefa2d3005ebe8cebe43324e65b6d2f3a106`  
		Last Modified: Tue, 25 Oct 2022 05:31:09 GMT  
		Size: 3.0 MB (3042023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5439394181cf9e8ac2e0b446f62199582c04aa5f5903de80e9b8474a01ca5c24`  
		Last Modified: Tue, 25 Oct 2022 05:31:28 GMT  
		Size: 47.1 MB (47083490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb1497899c9f48cc0c773769e863fb5f587546a5831104b7ee048453a776aebe`  
		Last Modified: Tue, 25 Oct 2022 05:31:56 GMT  
		Size: 134.0 MB (134026600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:443a00cd3f35125ff2856e16c19720e7963f64acd7ca5955fed24d8763ebaffa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.4 MB (246426888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70f27d2f9478275b6a5a2a4b9587a5ceea77a4af2af4a05be63e9ee1adb3ce8d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:25:34 GMT
ADD file:254e11be9bc865d645aba7c16a39a04f5ce227b7aa4280f7a42baec47b0c6ee0 in / 
# Tue, 25 Oct 2022 03:25:36 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:20:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:21:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:22:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:27:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:21b8f46bc1957ff60412d81678134500cf7a4f0e7f198ba384fedb2e5747d847`  
		Last Modified: Tue, 25 Oct 2022 03:27:21 GMT  
		Size: 30.4 MB (30443225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7a73c0177bc0907d9770e0863fb7f6949a870d385b401421a0817a32cd56be`  
		Last Modified: Tue, 25 Oct 2022 06:52:33 GMT  
		Size: 7.1 MB (7051025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f82d4b01549cae8ea6c3b7e9f210d370b148dd8004af19925715e43994e9ff`  
		Last Modified: Tue, 25 Oct 2022 06:52:32 GMT  
		Size: 3.7 MB (3740646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc5edd6bb0a218e937aacff2efa004bac7b35909a1d19740f14acbae1df7b87`  
		Last Modified: Tue, 25 Oct 2022 06:52:59 GMT  
		Size: 53.7 MB (53741147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600501f491d899f441f91702b04e48dda009fb613806254ab578645e5cc0307f`  
		Last Modified: Tue, 25 Oct 2022 06:53:48 GMT  
		Size: 151.5 MB (151450845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:16eceed169fc7d8e7dd3f213936244ab45f5e6ec0e5090ecd3f9a8f04e0f9e4c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.8 MB (205759274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ab91687893f8d5e47036caf530ff156ea86a4d93a7b61bf9ad5037e833453cf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:02 GMT
ADD file:0843e89b8865a30626cece7a42cf27708a86422aadb28029168b2f159a8768fa in / 
# Tue, 25 Oct 2022 01:23:03 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:34:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:34:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 02:35:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:37:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4cd692a206d359f66e10c4f4f2a37009c4162f022df78a9bb8e8c24def290167`  
		Last Modified: Tue, 25 Oct 2022 01:24:23 GMT  
		Size: 25.4 MB (25371461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1872edbfc35ad376faca8b8da8bfdde0ac95f27652b1188c2036672466ab8233`  
		Last Modified: Tue, 25 Oct 2022 02:51:21 GMT  
		Size: 6.3 MB (6326364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5dda90dab707bb33111b66abdc094ed182c70b7a83b6844b6b316ba93a0f779`  
		Last Modified: Tue, 25 Oct 2022 02:51:21 GMT  
		Size: 3.0 MB (2976628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feacbe49c2940d688c7c8200c29c610e8a5a65180c8b6d67c78b193f408418a7`  
		Last Modified: Tue, 25 Oct 2022 02:51:34 GMT  
		Size: 45.0 MB (45044933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74da665a3988b61dbc1e55c52dc97c4d3fcf3b2c58feb3f9664d6b471d420d91`  
		Last Modified: Tue, 25 Oct 2022 02:51:56 GMT  
		Size: 126.0 MB (126039888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
