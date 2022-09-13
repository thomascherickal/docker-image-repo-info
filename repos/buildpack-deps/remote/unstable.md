## `buildpack-deps:unstable`

```console
$ docker pull buildpack-deps@sha256:7278bfdc58a72bde77a78885b8e9dade8349caeb172318ad50d20d7453b6fbce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:unstable` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:db6bbe1b47461494b07e4ccf08863f7920f995babcf8b79a06d2d33940614b66
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.5 MB (344536691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ced5c01daf393dc64fd1bc7067bc47f053da4f30f88cfb32b6f2de8fd17bf75`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:57:16 GMT
ADD file:7b7161ef988532de9a1ae3caee50f4337a445cd5d88bfe1da455ad45111e2a4f in / 
# Tue, 13 Sep 2022 00:57:17 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 03:46:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:46:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 03:46:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:47:24 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fbb5199f866b772d7999f8d0fead2c513b95972d6d32ec2c8e29311458f0855f`  
		Last Modified: Tue, 13 Sep 2022 01:02:12 GMT  
		Size: 52.6 MB (52643556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5abee259a1d9101a0890f49e244222094315b4c017c58d8cb8a6cc0cd43e833`  
		Last Modified: Tue, 13 Sep 2022 03:52:28 GMT  
		Size: 9.3 MB (9298049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a8698192cb686ddacc8322753abf5c95c28d7cca2e06243ec755c2044f89760`  
		Last Modified: Tue, 13 Sep 2022 03:52:27 GMT  
		Size: 11.4 MB (11380792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a113e2744da1b277bfdaa7b2eb0ce67a02441dae47ae08b93fc8cade18fed1`  
		Last Modified: Tue, 13 Sep 2022 03:52:47 GMT  
		Size: 58.1 MB (58067914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cacfc029773ae889d3d70c7c7a697f979aca0586699838016d7647e998071dab`  
		Last Modified: Tue, 13 Sep 2022 03:53:26 GMT  
		Size: 213.1 MB (213146380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:ae6debf772cd416d3418020d444b526e6dbb85caf44ec3d847d6ece14fdddbd5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.9 MB (313920314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:346d312be574d74cdc36cf1bba138bd96a787ab9df0c21436f66850af54f9485`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:17:35 GMT
ADD file:dd3257a03b58fae4238ad4fccb1c79ff49c76b1294f5fb6f57ecee4bb748c9ca in / 
# Tue, 23 Aug 2022 01:17:35 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 06:21:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 06:21:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 06:22:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 06:23:24 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4cd09bc891cabc28c38273b3b8e22a810888bfc449c6fd4ec5610c27492b2603`  
		Last Modified: Tue, 23 Aug 2022 01:23:14 GMT  
		Size: 51.9 MB (51911406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f224d9458f88dbd5a7ba922c9cb4a7116b314d234615e7981e233157663a02`  
		Last Modified: Tue, 23 Aug 2022 06:28:49 GMT  
		Size: 9.7 MB (9741837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f3836f63f5d9bf55c4350c9f89c9a7b420aa71f6408278b53d58e61634cb3fa`  
		Last Modified: Tue, 23 Aug 2022 06:28:49 GMT  
		Size: 10.9 MB (10949073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c127ba25c98f2eef6419ecfbb5bb63c8da103c1ea0298e7e61e2103424e530a`  
		Last Modified: Tue, 23 Aug 2022 06:29:16 GMT  
		Size: 55.7 MB (55747826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e249ad29978f097d481f4bfe9ce42ca0c44552bf26944aea2b847496fd0838`  
		Last Modified: Tue, 23 Aug 2022 06:30:09 GMT  
		Size: 185.6 MB (185570172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:bc91dc378f70148cbcc97cbad3f64cf843806fd1c0646f19238db6080b94a4cc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.0 MB (298991295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:671f185210ae0119c498b99bc311b791bceaf84950a530029f4219db28085d62`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 03:44:03 GMT
ADD file:6c202b99cd5c91b3c2b2bc39ddaf5738d4def8520e18a716d249d62881657e5e in / 
# Tue, 13 Sep 2022 03:44:03 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 07:37:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 07:37:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 07:37:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 07:38:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:261cac8f52f598a2e1428463187e026d01259f7076e6ca3adf9b13c1414ba47c`  
		Last Modified: Tue, 13 Sep 2022 03:52:11 GMT  
		Size: 49.5 MB (49523940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69e346b65163965ce437753259a3a5635ac1fdc3d48b6735d5be0f1dc103653`  
		Last Modified: Tue, 13 Sep 2022 07:47:06 GMT  
		Size: 8.4 MB (8397051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c75620166463dd3a4557387e6591fccb3f2196f7d3af1c7d033dd15cc6cc0cd`  
		Last Modified: Tue, 13 Sep 2022 07:47:06 GMT  
		Size: 10.7 MB (10659656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd2c4f9d78247385adc3f52a5344d1ca72d43e2ab8f373b72acb1de956dcce4`  
		Last Modified: Tue, 13 Sep 2022 07:47:29 GMT  
		Size: 53.7 MB (53724765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0659a194bbeaef3eac1a8c6bf276474271aa26a4286c7deff7e89cefccf611`  
		Last Modified: Tue, 13 Sep 2022 07:48:17 GMT  
		Size: 176.7 MB (176685883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:807335b9281318f0ee1e55e5a1202e1d0058eb21b424eea8009a033ecb4e6938
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.2 MB (335201621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d0f9616e841cadc1dd77c1e3e671d95c499fb72f7a565d4e28dc6fab9c6b06a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 02:11:54 GMT
ADD file:13af7384e2c4f0c81e2c22e39e5d930dc4524d300c5f3d92ab3288096c308777 in / 
# Tue, 13 Sep 2022 02:11:55 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 05:04:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 05:04:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 05:05:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 05:05:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:113c8010a5d8650dba62a6df118557cb9b270a562e4a0537563cf79291f65ab0`  
		Last Modified: Tue, 13 Sep 2022 02:18:11 GMT  
		Size: 53.1 MB (53103634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f00ceb8508161cf15d9580001f11e56a6e5eb7d0293d831a4d3bb4932e1050`  
		Last Modified: Tue, 13 Sep 2022 05:12:22 GMT  
		Size: 9.1 MB (9127731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ac595041e810cadc49116d5630a0f49b2e0bb6084756143d92c87a24e9c24f`  
		Last Modified: Tue, 13 Sep 2022 05:12:22 GMT  
		Size: 11.1 MB (11133512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d53dea7bf1a209edbd8cd322893334f5833b0fe4fc7f12f48fe6b6efe11e6f`  
		Last Modified: Tue, 13 Sep 2022 05:12:43 GMT  
		Size: 57.9 MB (57932408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b337306ffcf9d968cd0c9711095e28c4edc9bf8ea9990417811135e09839c9`  
		Last Modified: Tue, 13 Sep 2022 05:13:21 GMT  
		Size: 203.9 MB (203904336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:740100b3b3a1ea66d2289fb83e923656ef22f6c41211a391ccc9f34179aa8c63
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **347.7 MB (347662446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1052d1934ae195d477519a00225a48065fff55c479a2350f86dc8e988be299e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 01:40:48 GMT
ADD file:6c1d0f31b3527c2c240577c73b2476b1c6bcb8fa8d10fea614680e40f1c15858 in / 
# Tue, 13 Sep 2022 01:40:49 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 04:52:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 04:52:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 04:53:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 04:54:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6d4ab670272048731963c87509c528d8f874ef24e7e5eb410c2b800aea0d16cb`  
		Last Modified: Tue, 13 Sep 2022 01:47:14 GMT  
		Size: 54.0 MB (54012005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c04187b376672562963fd175ddeca1b7d946a1a8549cfced79b8ad15f14bfe`  
		Last Modified: Tue, 13 Sep 2022 04:59:31 GMT  
		Size: 9.5 MB (9473423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab613e1d69d3fd1948062b98b955ccac19ca917e8a3dcc8e71abdc22b83e9897`  
		Last Modified: Tue, 13 Sep 2022 04:59:31 GMT  
		Size: 11.6 MB (11576535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81e07ced1faf9475820e62de73f3541fea07b3862a0dbccfeac8685967d00dd`  
		Last Modified: Tue, 13 Sep 2022 04:59:51 GMT  
		Size: 59.7 MB (59675489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a04388509af3380a3df541b6aa7d74328bd5e9b415e222cf388541d3c567976`  
		Last Modified: Tue, 13 Sep 2022 05:00:26 GMT  
		Size: 212.9 MB (212924994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:44932d5ac5c7c5b4769849503ca026630ef64ad261f181908e37e315f4a6a562
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.8 MB (321764495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aaf48cd27b846d1c74c094bed63d9fc6bdcad9711050ce213db2592c1f435d3f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:11:52 GMT
ADD file:372730632835dde60a084d1dc5d1d8d7840a118d3aa6413f1568d2a939e39e05 in / 
# Tue, 23 Aug 2022 00:11:58 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 22:34:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 22:34:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 22:36:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 22:42:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f6fdf476c348ab651944f6f008015e5c5184fa9f5620904fc65599b044dd5761`  
		Last Modified: Tue, 23 Aug 2022 00:20:20 GMT  
		Size: 53.2 MB (53216630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f889c0bad3c21c23d5613d840cb6194f047e7bd8b0ab913aa4c3aeb3f22ff6aa`  
		Last Modified: Tue, 23 Aug 2022 22:52:22 GMT  
		Size: 8.7 MB (8666700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e682c1b586301933075fc1a74ded2cb91e71a70eb9e075ab5291aec1d56e833`  
		Last Modified: Tue, 23 Aug 2022 22:52:22 GMT  
		Size: 11.0 MB (11041861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec7b75657e271145b112803a3b136f6eba775667758887ede8d7bf5eea806dd`  
		Last Modified: Tue, 23 Aug 2022 22:53:13 GMT  
		Size: 56.9 MB (56881826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ccde40f554bb70ef53d85d915e58944b5bde8dea04124f47de1cc710a908bde`  
		Last Modified: Tue, 23 Aug 2022 22:55:22 GMT  
		Size: 192.0 MB (191957478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:ad9e07723d3d250ec9067d3f3a7891a5a34c9b1f9b6bc084e8f3f3c627e0947f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **356.6 MB (356579180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:076ad0287576c809d28ca1e66232493b078eae16018a2473ee625b85da1ad96d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 02:08:14 GMT
ADD file:7d9f6a3f8ad433abf431bcad8e6116e9904ba35fc9bce2c28a606c6e697eb4ad in / 
# Tue, 13 Sep 2022 02:08:17 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 05:17:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 05:17:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 05:18:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 05:20:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a14f00c47c74a23076b6e04f2c1edb527d3e4b88249c3395ff38af7d4a745799`  
		Last Modified: Tue, 13 Sep 2022 02:14:11 GMT  
		Size: 57.2 MB (57189582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:735886547a07f8548c5997c489b42bc8ee28201c1944154a2d51099b3431a97e`  
		Last Modified: Tue, 13 Sep 2022 05:26:48 GMT  
		Size: 9.9 MB (9884481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94b4869677af77dc3f19d87e03cfd23841b6b7b0c65fed4be462f2bc786a3b67`  
		Last Modified: Tue, 13 Sep 2022 05:26:48 GMT  
		Size: 12.1 MB (12142712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7ce98afb4b4ec55ce30ea48aa7da9329b7619f43b0bcd31f96e1e3766b19ee`  
		Last Modified: Tue, 13 Sep 2022 05:27:16 GMT  
		Size: 62.9 MB (62850919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac08115c80e42ccdeeedf9297f9be78390b36441b7cae443e744e1c71eb7a27e`  
		Last Modified: Tue, 13 Sep 2022 05:28:18 GMT  
		Size: 214.5 MB (214511486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:0b603f88c28fb8429fd05206b79945930b5fa5ce8d8d9427b2652d28e5f11ad6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **361.4 MB (361359664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49edae0a85c7897d7dd6a29945939bd7d3f18568d25701d3e7853f7d0cf9d594`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 01:11:44 GMT
ADD file:cf4408ac501f6e39f1a9c7abb24ec07a6bc62afa97f48fd63879c903abfaaf4c in / 
# Tue, 13 Sep 2022 01:11:46 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 01:57:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 01:58:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 02:03:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 02:13:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d8cced8b0f3f30b0928735c74d8208eae12a348b798bd4253f1b4acb6d9d6728`  
		Last Modified: Tue, 13 Sep 2022 01:29:57 GMT  
		Size: 49.3 MB (49268300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cdf2efe1eb61fd0bbcf2b293d4e031b05f13a19f3ee4f9691262666970b15c1`  
		Last Modified: Tue, 13 Sep 2022 02:42:01 GMT  
		Size: 8.4 MB (8401065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f281e9cb277bf50237e9e04b09169648d24499c56aa01f94bedcadcb173d0a3`  
		Last Modified: Tue, 13 Sep 2022 02:42:02 GMT  
		Size: 11.4 MB (11435697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f5ac0089cbc5e6a2fd5b2e4f0a87d121dfc9b18f21dfa4cbfa5fc80eea4dfb`  
		Last Modified: Tue, 13 Sep 2022 02:44:33 GMT  
		Size: 54.0 MB (54030810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ef7a6f28e22ddd1f3cc453a92dfebf08b8c3f176ed1b1d213b66b076a2c7b1`  
		Last Modified: Tue, 13 Sep 2022 02:52:05 GMT  
		Size: 238.2 MB (238223792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:3380f5eb469b98e12046ee103b120a9bc84afb65a17f38812751e1b32fd6da22
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **499.2 MB (499173410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76a19518653a77d77c1c607b119f24c614cdd67c4fdc9f27f4385f192cc0ed7a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:54:14 GMT
ADD file:fb4926c73b650f18bc1eb6b58287dc0872251073fd0bc72bcd007f74315f89a5 in / 
# Tue, 23 Aug 2022 00:54:17 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 09:53:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 09:53:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 09:53:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 09:55:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0aaf3bb8cf1626ddbd85331fa1967c48ccf9d314270b99a2a506e53979592f79`  
		Last Modified: Tue, 23 Aug 2022 01:06:53 GMT  
		Size: 51.6 MB (51581993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b9f9f1f0cb3b7d4b45cdcacf5c7c93102c09bc71207f7dcc091136f732a622`  
		Last Modified: Tue, 23 Aug 2022 10:01:01 GMT  
		Size: 8.9 MB (8943771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06f6fca0053787f32630628512d8ae3f948e6ae085840b8a4083d3ac745fa220`  
		Last Modified: Tue, 23 Aug 2022 10:01:01 GMT  
		Size: 11.2 MB (11168320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e0960b87cafae9e1bf612df6c73bfb7680cbb0139fd149d5c6e367e797b282`  
		Last Modified: Tue, 23 Aug 2022 10:01:16 GMT  
		Size: 57.2 MB (57210664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886ef7d8187dc34f74cbea7c999fbf59f6940f6f469d36dc12cf47527ef36d7a`  
		Last Modified: Tue, 23 Aug 2022 10:02:03 GMT  
		Size: 370.3 MB (370268662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
