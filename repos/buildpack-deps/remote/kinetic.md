## `buildpack-deps:kinetic`

```console
$ docker pull buildpack-deps@sha256:dc6dfd8eb7484f1478517233d5a4254087445dbf06188812644803f51c579a8e
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
$ docker pull buildpack-deps@sha256:81cbd1992c9c44903c6f4e35cd275f15d81c2010d6c83c6c6b4458212c24fde5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **253.3 MB (253328299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:629591b3c411109b5908b2cfa5fce077a1b66f91a13b857dd779c9655b66d4dd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:29 GMT
ADD file:2496d47197031551828443c95a5e1dc6bb6dc7855695a8470f3ec96e8441e76b in / 
# Wed, 05 Oct 2022 00:02:30 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:32:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:32:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:33:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:34:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9a768b6c77af7a723d25d349fe4a633e82e8ad41fae270b2bbee8849bb840009`  
		Last Modified: Wed, 05 Oct 2022 00:04:31 GMT  
		Size: 26.7 MB (26690398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56476b006a508648b853d25af5afc829804e3d75931022c7583240f09d0c1b06`  
		Last Modified: Wed, 05 Oct 2022 00:43:58 GMT  
		Size: 6.6 MB (6608273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e10cd4bede843113d9336d39042872604d754220f3cebb42d6f4d05652dd7d`  
		Last Modified: Wed, 05 Oct 2022 00:43:58 GMT  
		Size: 3.4 MB (3389726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8841f74546971e6dc2a63f25ac58478259dab7f54f7f714c4d97bb22457ced0`  
		Last Modified: Wed, 05 Oct 2022 00:44:16 GMT  
		Size: 39.5 MB (39494012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e116ec4db443c64e87f9234aa4e61bce8bae057ef6ac2fe619ffb830fa07c08a`  
		Last Modified: Wed, 05 Oct 2022 00:44:52 GMT  
		Size: 177.1 MB (177145890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:aacd2841a1e442fc1a51300cf1624bb6f38dffcdff3c27fa7a1e7f942d4a3ebf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.3 MB (282251775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:015622ad1f917fcedd420ed628aa2356b7b6306b47a5885e9a81b47e602f7868`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:50:26 GMT
ADD file:79183abf8a1f4a6d4d04d73bcbe47e66f08bea9796acebd37d515855a459d132 in / 
# Thu, 01 Sep 2022 23:50:28 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:46:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:47:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 03:48:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:51:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ff717d18c49d9ec97ec3efef7dd73fe40829e1902f57d95a91516a42f69a091a`  
		Last Modified: Thu, 01 Sep 2022 23:53:03 GMT  
		Size: 32.1 MB (32082633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e76c734e70f580a1e1db27a87020a89cba5ca648c7e9c85068bd42b1e3126ebe`  
		Last Modified: Fri, 02 Sep 2022 03:58:49 GMT  
		Size: 7.8 MB (7750570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09098d7e8658181028c27fff2df2b67293550987d175c5fab78075ddec7dd8ac`  
		Last Modified: Fri, 02 Sep 2022 03:58:48 GMT  
		Size: 4.4 MB (4361359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc897ebe25a803a066f6b1910e20dec6fc0162253745894a729850d1d32c57c8`  
		Last Modified: Fri, 02 Sep 2022 03:59:13 GMT  
		Size: 44.2 MB (44161167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b502c070e035bff4190a1869e54d6a3382719ec5513be9900a64d748b181aaad`  
		Last Modified: Fri, 02 Sep 2022 04:00:12 GMT  
		Size: 193.9 MB (193896046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:73bf7abfabd3ce3f80d631c8b4246bfb77cc7865a6ea4a088e1f1bcd8e898b00
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.8 MB (280785501 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86d3e3d306e8b6f9c7a24e537c8ca6080ef2a051ad1d85eeb998da9e2c4ff0b1`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:14:23 GMT
ADD file:7c2ab85ecb4dc221c58ed92c05acad8d0b2ad90e46ec34c0a45fd5a5c3a9f7e2 in / 
# Fri, 02 Sep 2022 00:14:25 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 01:16:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 01:17:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 01:20:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 01:27:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:26010bd634bfca42373b6c36c189031dcce89570ea1226e9462a48d7a684240c`  
		Last Modified: Fri, 02 Sep 2022 00:32:57 GMT  
		Size: 25.6 MB (25594334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0826196a5d14cf0f019090771814dce885e1420c992b36ab31bfed7b28d86cf5`  
		Last Modified: Fri, 02 Sep 2022 02:00:23 GMT  
		Size: 5.9 MB (5930253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add19389e79fd75d5e3421d12568767855677a99cc4cfe5d50d5590034851237`  
		Last Modified: Fri, 02 Sep 2022 02:00:18 GMT  
		Size: 3.9 MB (3881273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f04e7e633bdcb9ab785ebbaa03714ef1fb30b6e9341369572e7eb655916151`  
		Last Modified: Fri, 02 Sep 2022 02:02:44 GMT  
		Size: 42.9 MB (42853430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67eaacb0aa78a362fe9ee225ee0e3ca057354904b8418793e4b7a1511e7aab3`  
		Last Modified: Fri, 02 Sep 2022 02:09:59 GMT  
		Size: 202.5 MB (202526211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:fe214606ef506ef1183c74248e883bf2d5b6b03ca030c2acbb7521a8661dde6f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.7 MB (234719614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6074c9f0b34efe7f2115c2ed8407a44a6e79ccabcb0b702f37164e15f51ea975`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:53:10 GMT
ADD file:4b04232627e4ab4441752376c6d51dbcdf07b65cadc7027da4c4cc79d37824cc in / 
# Tue, 04 Oct 2022 23:53:13 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:26:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:26:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 00:26:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:28:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:756b9b94f7ea9eda3168c766dd8c30136a2409b90d55b16cb335507dcc5e055f`  
		Last Modified: Tue, 04 Oct 2022 23:54:50 GMT  
		Size: 26.0 MB (26029724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777e01a92aac9f6f68b883738330b61f5dd370112f6443f44898ba567cbb938c`  
		Last Modified: Wed, 05 Oct 2022 00:36:17 GMT  
		Size: 6.5 MB (6475463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918aa0d020e12cbe864a35fb042a07a6069bd7e8dd270eed48961e8d5625b6ea`  
		Last Modified: Wed, 05 Oct 2022 00:36:16 GMT  
		Size: 3.6 MB (3625655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5628cde4bbda67e815888cf5a1d62f8a40e0b37be66e0725366f9129ad88da83`  
		Last Modified: Wed, 05 Oct 2022 00:36:29 GMT  
		Size: 39.5 MB (39548273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bba3b606b882054aa0640558298fcc15f609522f6950fdc1107d05376815a47`  
		Last Modified: Wed, 05 Oct 2022 00:36:55 GMT  
		Size: 159.0 MB (159040499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
