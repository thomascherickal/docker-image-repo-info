## `buildpack-deps:kinetic`

```console
$ docker pull buildpack-deps@sha256:4bb8f04c36a68d87bb5d569f8ef15acf77df7d6d27bb36b3b935211fddc8acd2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:kinetic` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:b33788a433b2f998ebd368f99762872a3c6c6009abe173f62fb4e1e94c9ae7a8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **265.8 MB (265793471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:622366e2d78507bc25ad39ba5e3b6c6a4b43d982571e1a8250ba68d37223db3e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:28 GMT
ADD file:3384549425c94b92a7d7be15958e3ec7494bdf83242deb465d9059d4362d34d6 in / 
# Tue, 04 Oct 2022 23:35:28 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 01:13:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:13:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 01:14:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 01:16:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5887826a0d8b4c403d9bfaf57279fd8b585d272c3f450d374349365dc22cd8ef`  
		Last Modified: Tue, 04 Oct 2022 23:36:56 GMT  
		Size: 27.5 MB (27455077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b7fd9cb5adf6a195c3c2162caa409d926d4342598cad09f7fa4691e9ddd25f`  
		Last Modified: Wed, 05 Oct 2022 01:25:38 GMT  
		Size: 6.8 MB (6780586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9023f9ecbe71ceaba400cb934168d975ecabc157d85fe246f71d3d684947742d`  
		Last Modified: Wed, 05 Oct 2022 01:25:37 GMT  
		Size: 3.6 MB (3633909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d44eedd822ec1ffd1b32f87638bae3694f27cf99e85f8d3d8f6d1f2857fdc1`  
		Last Modified: Wed, 05 Oct 2022 01:25:54 GMT  
		Size: 39.7 MB (39713928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46cfc3a166e18ca21a45cacaeec49e724ff39c9215001117796bd74cb3b40410`  
		Last Modified: Wed, 05 Oct 2022 01:26:30 GMT  
		Size: 188.2 MB (188209971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:d55d7353e6aa732cad00a73a6c198a481ba08a5afd55721ac086a1017b1559ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.1 MB (228118532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10bca3a5fa8bf85ff72ac75e507466eacf465294389c059f87eb1ceaa37efa93`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:14:09 GMT
ADD file:4b538f2c7b46aa601d747159ce9e8c2c7a99b2b6e09e4efe1073ca58e47fbeed in / 
# Wed, 05 Oct 2022 00:14:09 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:47:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:47:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:48:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:49:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:788f7bb1e1d719f6a9a9b3b1530cc5bbe5b808a2ad77a65f23e2c6d15b8ae546`  
		Last Modified: Wed, 05 Oct 2022 00:16:28 GMT  
		Size: 25.9 MB (25873193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31aeed2022326b456329596b112851c2e027ba5773dab33fcd717efb1a016274`  
		Last Modified: Wed, 05 Oct 2022 01:01:56 GMT  
		Size: 6.0 MB (5955685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b8a4829745394c3402e5970b4558ef9fe23515f895e7f8a99fe24ae33a7c4f3`  
		Last Modified: Wed, 05 Oct 2022 01:01:55 GMT  
		Size: 3.8 MB (3801708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199fb45c30ad58843e78384afd22f7dec65ac55a285086da2083dea2426fd37e`  
		Last Modified: Wed, 05 Oct 2022 01:02:19 GMT  
		Size: 42.6 MB (42596389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd5d37220a8883d442a1686f49907c73299d8c1df3d5f6cc9a9d1b8c9012583`  
		Last Modified: Wed, 05 Oct 2022 01:03:07 GMT  
		Size: 149.9 MB (149891557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:7f591bb67e4190e35105756af84f44d4bdd7c020d451632335a530a83e8e299a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.6 MB (246644046 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:418c243a099dd8aadaf491de0633949554b9e17b02bb3dbecaeba22314be0c60`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 05:55:06 GMT
ADD file:30361063c284df6e20a85ff95b9c7b93648fe9e04ac935c9ff888e5c5f3af7ea in / 
# Tue, 25 Oct 2022 05:55:06 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 08:19:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:19:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 08:20:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 08:23:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a2e58a4bc1e52e3ab8904706a68a79146364ec32d8caf1bd106c3c9966a38fc`  
		Last Modified: Tue, 25 Oct 2022 05:56:30 GMT  
		Size: 26.7 MB (26676995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208c8913a9c66f64a1f5ca1349c8a8b9923f9eb9c8aed25bf3ec160a33e5a796`  
		Last Modified: Tue, 25 Oct 2022 08:36:03 GMT  
		Size: 6.6 MB (6607031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8491d7cc7a42af61771e26652e91532db813e380fa19339f7279420206df0290`  
		Last Modified: Tue, 25 Oct 2022 08:36:03 GMT  
		Size: 3.6 MB (3602476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2cf60ff33717c4a17f0ca2f77473b69d8d357e4dc81ef8bb8a5e24382aa106`  
		Last Modified: Tue, 25 Oct 2022 08:36:17 GMT  
		Size: 39.5 MB (39486568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2297c22e5e80de066ab641f5f47a060831dda9dbda728c9ffc0333ffd65aec38`  
		Last Modified: Tue, 25 Oct 2022 08:36:45 GMT  
		Size: 170.3 MB (170270976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:b85564067cd24e7645a51fcc5b5ee66f50498a7a4cad4db8f8e748271b4cbfe0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.3 MB (281263738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:402a9d4fffb8624f6fa449162bbd5c6ef48031ba4a3813d392416260f6ab5055`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 03:26:14 GMT
ADD file:60dd11bbfa9f1e2bc613c7f05cbbb83bca9e4b81550b6a0540a5d1d39f870cdd in / 
# Tue, 25 Oct 2022 03:26:16 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 06:40:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:40:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 06:41:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 06:44:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6d37bc653a986baef621c195bf8def80ca65133b8a3917bbd3a148b31bc1704f`  
		Last Modified: Tue, 25 Oct 2022 03:28:34 GMT  
		Size: 32.1 MB (32099941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc18decfda3085820c97e73c59dba18c534c4455c2eafc5812d29975ad7a9292`  
		Last Modified: Tue, 25 Oct 2022 06:57:12 GMT  
		Size: 7.8 MB (7752006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a931134d9aa21913f6400e3083b4c6955008f9fab7eae04019249a1d912c279`  
		Last Modified: Tue, 25 Oct 2022 06:57:10 GMT  
		Size: 4.4 MB (4361351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33eb213c2d45440f6da62e4c97dcc2936c1a9881896421d53a86927e2618b29`  
		Last Modified: Tue, 25 Oct 2022 06:57:35 GMT  
		Size: 44.1 MB (44120965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77829c624efe1a2e9a13f40cb1d0c0f4d7fe497125dbf87d40699e87a907c260`  
		Last Modified: Tue, 25 Oct 2022 06:58:34 GMT  
		Size: 192.9 MB (192929475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:5670cbeec0868228f4cbe82cc9abb1f3c09d621ebbf85c7bf0369b24642df074
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.6 MB (285585964 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f98764f075d571c93930c9fbb0965fe3cfd34f36ad2840deac11698e7d1b51d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:16:49 GMT
ADD file:2d01ff45e6105658cf6791d4ade5cc3168c7d455422fc973a54a795907023c4e in / 
# Wed, 05 Oct 2022 00:16:51 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:00:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:01:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 03:04:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:11:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:69c33ccbf3d1b09c78fae3f88deb756ae33a9e4610a01fc9ab8b457ee6107d7f`  
		Last Modified: Wed, 05 Oct 2022 00:35:11 GMT  
		Size: 25.6 MB (25618700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6742bf73589f8dd7c6c3ba8c0c07b6783a8c31c40b8e815941b550d904b49030`  
		Last Modified: Wed, 05 Oct 2022 03:54:22 GMT  
		Size: 5.9 MB (5938180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039b60e6247434b31a05dcae8802e410a92a3e9e6f9f6472455a58d4c1d5e1b6`  
		Last Modified: Wed, 05 Oct 2022 03:54:18 GMT  
		Size: 3.9 MB (3881311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde1ee2ce8c7376ef3e85ac490d31dcdf52bf954c3186472c53f3404c2421078`  
		Last Modified: Wed, 05 Oct 2022 03:56:41 GMT  
		Size: 42.8 MB (42832698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5e3cc23193e77d3695c7e56f6e60082abbcf0e11af954a30dda857279c355b`  
		Last Modified: Wed, 05 Oct 2022 04:03:57 GMT  
		Size: 207.3 MB (207315075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:10403bdb366987e6b3d1e90233130b79cd5e6931553eebe344edb75b787b74d6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.6 MB (228553552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e5108db95c124c6268c561f7f0b5c01f26b48f3801c253310534a9736f474fd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:23:31 GMT
ADD file:9c0c4172b14f0d37b0b074729a4738aeb165efe5c83e2d9bfefc5b39e4a4fe0b in / 
# Tue, 25 Oct 2022 01:23:32 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 02:44:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:44:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 25 Oct 2022 02:44:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 02:46:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cf61a33f110308ce64c1dd7a5dddf2a5587ee1c8ab2351219b925428957cbc10`  
		Last Modified: Tue, 25 Oct 2022 01:25:01 GMT  
		Size: 26.0 MB (26022178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df11273ce2e4ff8fbfe44b4708e1c3b2323d38c23cc29bfb9935c1788807165`  
		Last Modified: Tue, 25 Oct 2022 02:53:37 GMT  
		Size: 6.5 MB (6473357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36f51f919c9bd6bce882afd5ce69c1de2f32276ae54369c26ae41702ff241ce`  
		Last Modified: Tue, 25 Oct 2022 02:53:35 GMT  
		Size: 3.6 MB (3625569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69ad44ec319ab50167d51a4bd01dd344bd736541842217bc94d0c6da1960b16c`  
		Last Modified: Tue, 25 Oct 2022 02:53:49 GMT  
		Size: 39.5 MB (39548002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed2d65b37ea7643db5c4a31a4261ef32fbaa397af4762b1b8e36a5f997c79998`  
		Last Modified: Tue, 25 Oct 2022 02:54:14 GMT  
		Size: 152.9 MB (152884446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
