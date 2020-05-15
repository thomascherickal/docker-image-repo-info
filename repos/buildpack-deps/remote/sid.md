## `buildpack-deps:sid`

```console
$ docker pull buildpack-deps@sha256:f16f1bc1b793231706f48a6c0ae022f6f837417ae5be6f1a1c4751b3e39aafe3
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

### `buildpack-deps:sid` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:6a079b01241e582fafab864fc31abef84d9b710082509e60a134469ddf442863
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.7 MB (328654986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fd7ba6f68f410a93ce91965d26f4d6aa846c23f4b8290f7560c9ef4243562a6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:22:30 GMT
ADD file:1b99a100214a4a86a413bf6a826c70d07fee06a8c4e6d1f3ed1550fb08f9818e in / 
# Wed, 13 May 2020 21:22:30 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:37:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:37:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 22:37:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:38:57 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:268c82fb25093fc20c25872a9f96ca2bef121a19a81a91079b62afb96b725135`  
		Last Modified: Wed, 13 May 2020 21:28:35 GMT  
		Size: 51.4 MB (51390987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a426d8c659d27b64d66f82bd62c2bb3dccd6560447f354396111cb0c27bc0e8f`  
		Last Modified: Wed, 13 May 2020 22:47:30 GMT  
		Size: 7.9 MB (7934296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ac7ef969a4b66cfe2e8dae9867620b1821ab5b3d64e9e37b0a3ca56f574a44`  
		Last Modified: Wed, 13 May 2020 22:47:30 GMT  
		Size: 10.5 MB (10463093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f137f68410074c0abacbce781d17f5b40e894982fa38e5f1cf1edb52c3274181`  
		Last Modified: Wed, 13 May 2020 22:47:51 GMT  
		Size: 55.7 MB (55655088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816d87fc3f6b99afb170e02019b4151721bf371964a13121ebe826de533999fc`  
		Last Modified: Wed, 13 May 2020 22:48:36 GMT  
		Size: 203.2 MB (203211522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:1970cf421f06762620dd5472263b2dd18388bf08a7d07fecb463a6cbe41aa4d4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.2 MB (299220160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae5087b3f87f3623a6290411ddbb8943844cddd62a22e42246be20b3bcd16fa4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:53:19 GMT
ADD file:b96a79161ef28394a61231962b6b094cc6d55101ffa9e159bca48da52498c02f in / 
# Wed, 13 May 2020 21:53:23 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:43:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:43:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 22:44:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:47:21 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e01d6f3a75b2bb37376867eda5418ce8818270da85f9e637bc0f8131b3c49c32`  
		Last Modified: Wed, 13 May 2020 22:01:43 GMT  
		Size: 49.4 MB (49359537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4060fe458be3ad9bb5734b9386b2be633e551438da5fa5933a3caf2eef1d3084`  
		Last Modified: Wed, 13 May 2020 22:58:05 GMT  
		Size: 7.5 MB (7514215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32e846164403fa17ac3349dfde468323e0107f2f131933333cec4baa962c230c`  
		Last Modified: Wed, 13 May 2020 22:58:05 GMT  
		Size: 10.2 MB (10157674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3205e486be95e4ba1ae8b2d22f6ad94505d38726a1f4f4c6cef0287bcfc053`  
		Last Modified: Wed, 13 May 2020 22:58:38 GMT  
		Size: 53.3 MB (53294192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1a4dd837ee1f456b7c57f0cfaa4c8f178f9a85a8c9f3c5600e12c0cfc1e5cd`  
		Last Modified: Wed, 13 May 2020 22:59:38 GMT  
		Size: 178.9 MB (178894542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:43cce7c11b3242193a57703cd0facacb89cd4add910f9393bc59196d90f739ea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **288.7 MB (288705953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:670052abe69a64c4ca31f8342254e9117646f88e446c2d79cea132a4c9b151a6`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 01:04:08 GMT
ADD file:7bc7b5e94debaef8aabee3128de6e535c9867794ed42649aadb9ba63a66a547b in / 
# Fri, 15 May 2020 01:04:11 GMT
CMD ["bash"]
# Fri, 15 May 2020 10:44:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 10:44:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 10:45:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 10:48:03 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:921baaddbf45818850d057b247e93c5fa875838ac2dbf11e2913f526f5ac4d94`  
		Last Modified: Fri, 15 May 2020 01:13:34 GMT  
		Size: 47.2 MB (47179178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b833ddc7c9debd21799cd19fb7e5459feeaae463d767cea9ca2c02209d4e68`  
		Last Modified: Fri, 15 May 2020 10:59:56 GMT  
		Size: 7.3 MB (7257028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:004dd78efb72e462bafeddbe0df6aa29d83c9f987bcd797c2d1cb8c813c1bc59`  
		Last Modified: Fri, 15 May 2020 10:59:57 GMT  
		Size: 9.8 MB (9804694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ae802f2861549b9a8f8f8971dbe9e7155dc358caa0271ea51893756a3893e6`  
		Last Modified: Fri, 15 May 2020 11:00:21 GMT  
		Size: 51.1 MB (51082648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81480ea269f97b7c4e81533921fb4686a64639beb17501897cf196604cf5d2ce`  
		Last Modified: Fri, 15 May 2020 11:01:36 GMT  
		Size: 173.4 MB (173382405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a6baff858f8977facee2723a86eba8ca0995d25cada0541dd4cf14ffe51bceed
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **319.8 MB (319841831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7cd9c6be8b854958429181397f12fe7c4b39f2ed4608bd238108272831c6b9b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:45:26 GMT
ADD file:22517e10f0b5d2760fafa2367b5a187d7ecef96291f15a746c24bfa50f756219 in / 
# Wed, 13 May 2020 21:45:29 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:27:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:28:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 22:28:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:31:24 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ad0025dc69d6f0241b2f5b614e96cef6e1fd54c9ef07b726338235b4766714ea`  
		Last Modified: Wed, 13 May 2020 21:54:40 GMT  
		Size: 50.3 MB (50328664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de8e099b34fe681d2134dc5800a33dcf2d66893cc852ada1704e600b8e46fac`  
		Last Modified: Wed, 13 May 2020 22:41:03 GMT  
		Size: 7.8 MB (7809465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2735cc8b188a094edcf282e931946b14d50022e973d985f72d13b23f3a1a810`  
		Last Modified: Wed, 13 May 2020 22:41:04 GMT  
		Size: 10.5 MB (10459849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c718f2ae452283da0b15ae79d609faee60fe428710fa0ad565afc8198c9f8a`  
		Last Modified: Wed, 13 May 2020 22:41:27 GMT  
		Size: 55.8 MB (55801209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:975f7d3ddbf05343bff23f57a11c5dc16f5f78fe334cf1d7dced9b96afe37260`  
		Last Modified: Wed, 13 May 2020 22:42:26 GMT  
		Size: 195.4 MB (195442644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; 386

```console
$ docker pull buildpack-deps@sha256:3399538c85644f9c849590cce2e905f5ee78edce52e8b1814171092ff973320b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.0 MB (338035898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b558a9b83e0cee294393f8dfd071ec60ebe30053b366da53c961455c8ec4c0f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:41:18 GMT
ADD file:bbf57f6406dcdfbee8d207ada2ed9150a3e775fa2cb6e0784c3e35e1c3216d25 in / 
# Wed, 13 May 2020 21:41:18 GMT
CMD ["bash"]
# Wed, 13 May 2020 23:53:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:54:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 23:54:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:56:11 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:430f489239f0254d72f3974fb8f614ac80ef76f642ab0bddcc4f20a8d4a3c68e`  
		Last Modified: Wed, 13 May 2020 21:48:41 GMT  
		Size: 52.5 MB (52481574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e65cdd6becdc738c09b87ead3f88dbd9e0a0028929d1d7f9698c406b2edfafa`  
		Last Modified: Thu, 14 May 2020 00:04:50 GMT  
		Size: 8.1 MB (8112129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2540c9f9f0836e2023dc2dff06e7a2a5186841f2f2f6bc12a2a1a2e05d7fa7a`  
		Last Modified: Thu, 14 May 2020 00:04:50 GMT  
		Size: 10.8 MB (10841254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5e950621bf55f9c03a0f91ce71347a56174670ad12c9a44c1674da2b52bfd8`  
		Last Modified: Thu, 14 May 2020 00:05:17 GMT  
		Size: 57.5 MB (57519348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02c56a8665844d0fdff521373207af2266023d3738386d234db715b8273cc7f8`  
		Last Modified: Thu, 14 May 2020 00:06:27 GMT  
		Size: 209.1 MB (209081593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:c63824d7c82ba4e8bda7b0b0aebdef7a69ace86c6ec34871a756808bc86120fb
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.0 MB (304990505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30f125188437571fa65584aeb2218efcebbfe2cfa43fe9d29568e4e7ca72d66e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 04:49:44 GMT
ADD file:2c7c92015da849bc75eb25960609c90178c9ac455dab05aa4ef031806d26ad64 in / 
# Fri, 15 May 2020 04:49:45 GMT
CMD ["bash"]
# Fri, 15 May 2020 14:41:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 14:41:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 14:42:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 14:45:29 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:567e61b8ab78e586542d5b9fab62c3880de99927de482a73e9e8b5b304f5284c`  
		Last Modified: Fri, 15 May 2020 04:59:15 GMT  
		Size: 50.1 MB (50149003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171157d3bf1886098a7c08bef7ab08c3c7a0d9b292111e8a5b8f39eecf07c2eb`  
		Last Modified: Fri, 15 May 2020 14:54:53 GMT  
		Size: 7.5 MB (7460868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:093eefc9c96bf46513b1575ab2e19b673a8a64043aca4e9ae4db05a4c7f3e803`  
		Last Modified: Fri, 15 May 2020 14:54:53 GMT  
		Size: 10.5 MB (10484688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eb3ef87812e2dc9082a70deacd7c235df6ca129a598c7068a9e9847c0caf1ed`  
		Last Modified: Fri, 15 May 2020 14:55:49 GMT  
		Size: 54.6 MB (54595877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7e548cdc1ad94aa530100b55b109629ed7244b4b9088b2ca21f4c831040cab9`  
		Last Modified: Fri, 15 May 2020 14:58:42 GMT  
		Size: 182.3 MB (182300069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:596294dd7d3c8909a19bc67a3ab43642e2f957ead48716d7669c76708f5dbb80
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.8 MB (348753748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6edd71f8b2da39a89ebb4ac1c9f3418e06dc082436a8e9f63c3ac5e94b270a00`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:28:26 GMT
ADD file:7e16c349b13e97e4784ee396bb36ab2d3a069714388b0803f18ceb8d526be36a in / 
# Wed, 13 May 2020 22:28:35 GMT
CMD ["bash"]
# Wed, 13 May 2020 23:55:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:56:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 23:57:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 00:07:09 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b2aad5ee0ac7c9bdb0530f0a2f94bcadce58437453bcbdc7a2f20b5366c22799`  
		Last Modified: Wed, 13 May 2020 22:59:47 GMT  
		Size: 55.1 MB (55111830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7bb4a67eb9efabb0bee7a8a6ff0c8c5d8b09a6992b8574669e941eb06ffe22d`  
		Last Modified: Thu, 14 May 2020 00:33:24 GMT  
		Size: 8.4 MB (8356775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba850bd6d1e4314d0d2953223c98e2452ff03935b42d421bbd2d54ca027da5f4`  
		Last Modified: Thu, 14 May 2020 00:33:24 GMT  
		Size: 11.2 MB (11176751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85dc99aced2c3410b9c7fc622fe0d8acdcfb87cde0748b3dcf4eb683bbaabc75`  
		Last Modified: Thu, 14 May 2020 00:34:44 GMT  
		Size: 61.0 MB (61049801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bfb8ac6c8c068a55886224be2e4a5c5de176a66acdafe3ed54871b23e022290`  
		Last Modified: Thu, 14 May 2020 00:37:25 GMT  
		Size: 213.1 MB (213058591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:1d8680135895fd3840c605d2884cfdb65402b8a251c4ff4cdbb3ce57edb8eae6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.7 MB (308739457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f15a96a9bf88294b9c95495ae56f511227c10f15d1e5b63cee8ba7a47992d18b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:43:22 GMT
ADD file:e7473e4f1acf1308ed319dfcc667696c733d4173125423a8f1b2c67039e5f498 in / 
# Wed, 13 May 2020 21:43:24 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:42:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:42:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 22:42:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:43:36 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:23e07cfb1ab58da76b3f9f0fdc8f5c154643a262a86037b7b6d1c26b5959a166`  
		Last Modified: Wed, 13 May 2020 21:47:43 GMT  
		Size: 50.0 MB (50002084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67e62641450b73095b82a741ceaf6d58012156b7f78bf4f67b73575fb15b7a03`  
		Last Modified: Wed, 13 May 2020 22:49:18 GMT  
		Size: 7.6 MB (7600546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f55d4f91dc718f22796b06fd0faf568f26113eb77e940c765216272c8262472`  
		Last Modified: Wed, 13 May 2020 22:49:24 GMT  
		Size: 10.3 MB (10347816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4524f47c96e9e169805caad967eaff45bbd160c819137b91ec0a64201132afa`  
		Last Modified: Wed, 13 May 2020 22:49:38 GMT  
		Size: 54.9 MB (54898246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0daff607cc80d508398c1ea476a8c40f7341c5048ecc05aea5511464630047`  
		Last Modified: Wed, 13 May 2020 22:50:04 GMT  
		Size: 185.9 MB (185890765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
