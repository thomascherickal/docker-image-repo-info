## `buildpack-deps:unstable`

```console
$ docker pull buildpack-deps@sha256:cc3a2ab2ca12e22a6974613f2c1ccd81edf37e12418cbaec4af1efa5506a13a6
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
$ docker pull buildpack-deps@sha256:2c251d8f3995d7069d86a9dcbae3e8accfac94113fb9038458d2e0b46a07e041
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.1 MB (322115713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dd4c1428fa5f6fc259cccefe8374b7be2991a0194d7f1f6325b908d02908db8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:22:07 GMT
ADD file:b00402c4b2c5828b18b251f8a057510f9f7da733f833cd147ed1a8fcb8d574db in / 
# Wed, 12 May 2021 01:22:08 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:57:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:57:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 01:57:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:59:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d2746b657344bbd3149c23794266413a61b32b44f53688f3619e485894c87b09`  
		Last Modified: Wed, 12 May 2021 01:28:33 GMT  
		Size: 54.9 MB (54896691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327df9aed8a8e57527a50678726f61121ed7fc1ff1b0c91e4268684ec7631ae7`  
		Last Modified: Wed, 12 May 2021 02:06:06 GMT  
		Size: 5.2 MB (5169357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b16c115b4ba04c02cb68097f3935495074622e8771a76d9f6a8c99d03331f9b`  
		Last Modified: Wed, 12 May 2021 02:06:07 GMT  
		Size: 10.9 MB (10871771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e08846e9f72bd9f6e8689fad90eb841b7acf03896b91e374d10f668c5abd250`  
		Last Modified: Wed, 12 May 2021 02:06:30 GMT  
		Size: 54.8 MB (54788476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b9b4723e12ff9b4c092d7301bf3c2863d963328e66a9fee2462a3b5caeb99b`  
		Last Modified: Wed, 12 May 2021 02:07:12 GMT  
		Size: 196.4 MB (196389418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:162830ceed4536f3edf0eac062ac425ca0cd908f8d77137cf7063297c4bac766
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.2 MB (295186291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a27de017a20d0609bfedac1199414a16a4bebb6caf7ae01193181fa46d719cae`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 00:57:58 GMT
ADD file:74d49eb3680e0d1e7268c77ac09aadc6a9eaca2541a1941d02c05771fce80430 in / 
# Wed, 12 May 2021 00:58:17 GMT
CMD ["bash"]
# Wed, 12 May 2021 02:33:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 02:34:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 02:35:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 02:37:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:992a8499bbce77a1397237914a5f442e2a2d90912c4dcf8d75ced68fa669452a`  
		Last Modified: Wed, 12 May 2021 01:11:33 GMT  
		Size: 52.4 MB (52438763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dbeeca774ae665bb974c9807245a126ddd59de992fc8b8627af4dd3cf6da38a`  
		Last Modified: Wed, 12 May 2021 02:47:42 GMT  
		Size: 5.1 MB (5074028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e28b75bd91c05df9e2403084c7a1160c21a93dce8b3591f4e77576118297aaa`  
		Last Modified: Wed, 12 May 2021 02:47:43 GMT  
		Size: 10.6 MB (10571291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04b31c8501e296694af462acc541dd996badb96b26a9b2c61f63551815e4a93b`  
		Last Modified: Wed, 12 May 2021 02:48:10 GMT  
		Size: 52.5 MB (52500158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8ffae387d5d5bf91bb6935cbbe998bfe34c00942ae85600c1f8c7bf0c4656f`  
		Last Modified: Wed, 12 May 2021 02:49:04 GMT  
		Size: 174.6 MB (174602051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f912292f15f822d363a5637a0671020c2c58c99a05ad874ae929159af91d604b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.6 MB (282583834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88e3f5ed34b6bdd5b62c4e0d768be0bffc8551688fcd1823f565084704401337`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 01:01:00 GMT
ADD file:b91b8d2ef6efe2bd9fc0625108290b82f4567ba3654aeea20bd4b9e7c9fcacca in / 
# Sat, 10 Apr 2021 01:01:05 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 06:09:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:09:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 06:10:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 06:11:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e9c76177d1ffa0bc1a85678dee6f5c61b2264a677790342fc5bb17961fb8015`  
		Last Modified: Sat, 10 Apr 2021 01:08:52 GMT  
		Size: 50.1 MB (50083439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26176a706c2fe768e7e54369121192f2b1336a3ac2985c3b017b574b99f4164e`  
		Last Modified: Sat, 10 Apr 2021 06:21:18 GMT  
		Size: 4.9 MB (4935049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55ba90a2781c4eed4854a1e54204b119cfe0e948ec34564b9e2235d443f69f1`  
		Last Modified: Sat, 10 Apr 2021 06:21:19 GMT  
		Size: 10.2 MB (10218224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91cd0a84cbd21a2be98dbced0d40b752d619473a031122610ee81667f9c56d22`  
		Last Modified: Sat, 10 Apr 2021 06:21:42 GMT  
		Size: 50.5 MB (50514802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2fcb6c699d8fb33a40e65446c562b6072c84b985e54e22a74694da9eed6c80`  
		Last Modified: Sat, 10 Apr 2021 06:22:33 GMT  
		Size: 166.8 MB (166832320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:5e5c0a419ca693ac63e48dd838ed2898905fb5b8292fc257122c547018092f17
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.8 MB (313799154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2abc553047aab20be2bae24f06282bbf493524ffb409a8ec6de5302804f8302`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 00:54:16 GMT
ADD file:bffb08485a063deee6d89343a52bf604c1b25c42687e69b289d304c56a35e425 in / 
# Wed, 12 May 2021 00:54:20 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:38:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:38:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 01:39:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:40:48 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:187d6bdc2d3198067fb9a19db77a105ae346c5a0de7d9892597e87e77c9d4b2b`  
		Last Modified: Wed, 12 May 2021 01:03:04 GMT  
		Size: 53.6 MB (53579726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8afada75acd21128a315d0521b9f088d01bca2afc87f040802bf44907e04d96`  
		Last Modified: Wed, 12 May 2021 01:49:51 GMT  
		Size: 5.2 MB (5157609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2228bbf9f1d8a87e7d8c1e33819ddc87db8595e963b10998927f5227f657bd4e`  
		Last Modified: Wed, 12 May 2021 01:49:51 GMT  
		Size: 10.9 MB (10872626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac554d26ec5eb2d355f9333f40db24c377de9ffe2e70ea3542bc84f7783302b6`  
		Last Modified: Wed, 12 May 2021 01:50:16 GMT  
		Size: 54.9 MB (54917401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a713096710a7bf08e0b43901d09bbe51d44c33d4813b010d93964935dcadb226`  
		Last Modified: Wed, 12 May 2021 01:51:10 GMT  
		Size: 189.3 MB (189271792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:50254fb03dadf4375c34daf5ea555ad6a0d40fcc4bfe6ae8e0a2d476ccd2ac5c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.0 MB (327997981 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:069b74b253590643215cb41daeef16e8db7777613afc4298b3ed0173b54eecfa`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 00:40:40 GMT
ADD file:d1e0da16153884c1e8fed94b01ed7a0d6215598889cf4b3ecda3e4e8e01a8a73 in / 
# Wed, 12 May 2021 00:40:41 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:11:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:11:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 01:11:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:12:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d1831ab5654d838d70f399ab69140b583b6195b99074487f0f45c8b5e2391a70`  
		Last Modified: Wed, 12 May 2021 00:47:50 GMT  
		Size: 55.9 MB (55915170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44aa5558f76b4b2d18bec73cdedd5fada6bf73f54d0205204e99072673252113`  
		Last Modified: Wed, 12 May 2021 01:19:30 GMT  
		Size: 5.3 MB (5298708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46130a767ef67e909c93d812e14d36740b2d6673db70121b3239657bf7bf4467`  
		Last Modified: Wed, 12 May 2021 01:19:30 GMT  
		Size: 11.3 MB (11250047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bad0ba82211377267c6c10f4369587ad3e14b683b7234f38f86b32b076233743`  
		Last Modified: Wed, 12 May 2021 01:19:56 GMT  
		Size: 56.2 MB (56201977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cacd7cc34eb54d99720a0d59224b942bb45d06576e89dbf6e87122556c49166`  
		Last Modified: Wed, 12 May 2021 01:20:45 GMT  
		Size: 199.3 MB (199332079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:e30e2cbd328c82a7ca3608cdb1cd186078f72d871870f9a28b52093949d71dc1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.6 MB (301586945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed2a1a1d3abbc0f16d3a25dbc916f36b195bb390b2e10fa588cbfc3ca0de8028`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 01:10:15 GMT
ADD file:dca45bb65ee8f7144352f7ac752f805807e971fc676ede954cc095be23566bf7 in / 
# Wed, 12 May 2021 01:10:16 GMT
CMD ["bash"]
# Wed, 12 May 2021 02:02:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 02:02:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 02:03:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 02:06:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:02e79e4ee7225612ac3aad55b918cb4257f8e4ea2821e093d61ce58205474706`  
		Last Modified: Wed, 12 May 2021 01:17:23 GMT  
		Size: 53.2 MB (53155797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e0b63156a44114e717b4b43275afc2af76c4643abc5ccd5f74eb95f7154772c`  
		Last Modified: Wed, 12 May 2021 02:13:13 GMT  
		Size: 5.1 MB (5128666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b331baf926199e9584576eb92ab16ebc86d42b9f2840844dfe1a47f4a77ca98`  
		Last Modified: Wed, 12 May 2021 02:13:15 GMT  
		Size: 10.9 MB (10872527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93031818e73d166b608909a1fcf1b8b480819e3a82e95a798eba9f81cdd9c345`  
		Last Modified: Wed, 12 May 2021 02:14:06 GMT  
		Size: 53.6 MB (53582263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a68877c328d050e165170fe777d35d30fcf45aa8853ef2c14154270e9d11aa7`  
		Last Modified: Wed, 12 May 2021 02:16:14 GMT  
		Size: 178.8 MB (178847692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d8ba29379864e2e1098d77199f3c8d9854a8e59b95108e3933b9b0d65aaf228c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.6 MB (330627533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96a51a742f5b007303cb3342189c8c9f609209bc3f391ea3eb6be5144756d103`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 01:27:11 GMT
ADD file:a41b62f9bc6147a0ab13a91e4ce5169739d220f716dc3752d7c872c9bf22748b in / 
# Sat, 10 Apr 2021 01:27:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:47:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 02:48:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 02:50:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 03:00:09 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:907e6a464bad63c32df38aaa0e848e3e09634237527afb1f8728bda2038576ed`  
		Last Modified: Sat, 10 Apr 2021 01:34:23 GMT  
		Size: 58.8 MB (58777775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d1d0df065cb2c84ba66e763425b139d7dc18eb050bf8cc5cb8dca7e25ac80b`  
		Last Modified: Sat, 10 Apr 2021 03:06:05 GMT  
		Size: 5.4 MB (5420160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebdfc94479ccc35bbc35f2da43ced87239a8ca75ef23ce43d8dd981eab17c3a`  
		Last Modified: Sat, 10 Apr 2021 03:06:05 GMT  
		Size: 11.6 MB (11621184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06204118184dc1ec0a05e69ba94ad3152a6c5fa8e3733a6d1313099c5e2d273d`  
		Last Modified: Sat, 10 Apr 2021 03:06:28 GMT  
		Size: 59.1 MB (59138557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2b97ca8796491eb99ef9274a70264dbc885bdf756788698b902aebcff5c121`  
		Last Modified: Sat, 10 Apr 2021 03:07:21 GMT  
		Size: 195.7 MB (195669857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:687fa2d40fd3a1e56ffcc40838204c9497463fb147d121a93053a5c5c2cb77fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.7 MB (295727886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:835b56e12cede9c4690b3f44837f2139302aac233b4a5d0cba0dae67fa5274cf`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 May 2021 00:43:58 GMT
ADD file:22b27fbf0808244bac39e39b8239caa784e78a6b5682c7978c1cb4fac0813a67 in / 
# Wed, 12 May 2021 00:44:06 GMT
CMD ["bash"]
# Wed, 12 May 2021 02:28:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 02:28:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 02:29:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 02:31:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:55e7e62594640e8831f8e39a7fe34cbb94c1ebfb345106b49c32b7d6c7e81eae`  
		Last Modified: Wed, 12 May 2021 00:48:17 GMT  
		Size: 53.2 MB (53183650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8529932d914624dabe07c03bc600a762580bed8457dbe8571680979ad85b69`  
		Last Modified: Wed, 12 May 2021 02:35:38 GMT  
		Size: 5.2 MB (5151016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3a75f6cba4036a878c0379562599e814a8859cb2041c9de51c09b79bbed27a0`  
		Last Modified: Wed, 12 May 2021 02:35:39 GMT  
		Size: 10.8 MB (10762861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f8dfb3a9c93915d107f4d14aeeb1484619028b66e5156f4237fa32fdaeec3e`  
		Last Modified: Wed, 12 May 2021 02:35:55 GMT  
		Size: 54.3 MB (54252972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36701b7af32efe51b09db5495efeba1fbb32d02ab6ee6f51748c7631991d269`  
		Last Modified: Wed, 12 May 2021 02:36:30 GMT  
		Size: 172.4 MB (172377387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
