## `buildpack-deps:sid`

```console
$ docker pull buildpack-deps@sha256:c37b773d0c403308f293df6836b176931fa7c0d3e6b3cbde5797881ac72176b4
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
$ docker pull buildpack-deps@sha256:ae72104fd0ce6c8ffaefcd004872bc5d66bf9b2f482601b05496389b26e4188d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.1 MB (328106414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:261d0a86b8da00e4ea11caf1e538e5f2c8495a54101f4ad28ba1897c5687b7e2`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 10 Sep 2020 00:28:02 GMT
ADD file:d09d72986a18210fc325abfbe18d3d35fef6de8ede47304410bea7528e5ab5e6 in / 
# Thu, 10 Sep 2020 00:28:02 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 01:08:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 01:09:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 01:09:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 01:10:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5da2bf34dd483faff62b98f29a31447619812af8afb0cdee07c188e866571393`  
		Last Modified: Thu, 10 Sep 2020 00:35:58 GMT  
		Size: 52.5 MB (52488092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c931b35f2563d7d9db709f3ab5b56a2f0281308f452acc51620919959073a9e4`  
		Last Modified: Thu, 10 Sep 2020 01:17:58 GMT  
		Size: 7.9 MB (7870622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8964fa9112bd6ffcd1be08e066d6e3aade5cbc082a4e29ed533274a85381328`  
		Last Modified: Thu, 10 Sep 2020 01:17:58 GMT  
		Size: 10.6 MB (10628636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc1f746f15e2336dd645ac66e83aa772659a1179d7b3effd2f3610981e957ba`  
		Last Modified: Thu, 10 Sep 2020 01:18:18 GMT  
		Size: 59.0 MB (59023664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f79ed0f2fd45aa5c2ce14ab5658b44854775c614505cb555257eb5ab197bdd`  
		Last Modified: Thu, 10 Sep 2020 01:19:08 GMT  
		Size: 198.1 MB (198095400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:45b1cd06ce0c6546379fe4f25d2bca5cd6c11b1c6e44b2931775500c0e286a23
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.4 MB (305413672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d8d2d8ca64cc70626c6e0498cd01624f4e7b347dd80c6e7d9e4fafcf959b9da`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:56:41 GMT
ADD file:9c8616d4fabe6861a7f03ec7c1849957393374004adaf865fad27fc7e91057dc in / 
# Wed, 09 Sep 2020 23:56:44 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:42:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:43:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 00:43:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:46:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dd8dd816178223393e19e5b2cd1f62df2d94bc6d5c9c393d8da9f901c96e3f93`  
		Last Modified: Thu, 10 Sep 2020 00:05:28 GMT  
		Size: 50.4 MB (50413542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b2d13ac158f55a44a68ac2d72292b51ad657a5202b688ec68c8cf3d7b42c7d1`  
		Last Modified: Thu, 10 Sep 2020 00:56:35 GMT  
		Size: 7.4 MB (7444216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c022e48ce06ce9a71076c5494577357f81ef67fdb3da661d48226f9f774c37d`  
		Last Modified: Thu, 10 Sep 2020 00:56:36 GMT  
		Size: 10.3 MB (10314983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37810e689b38ee68a82a6e11e092cb03c3b43af079aaac26e44b1719e537bc8a`  
		Last Modified: Thu, 10 Sep 2020 00:57:05 GMT  
		Size: 56.4 MB (56368366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057e250425fcb110848648061de5c9d8386baf377d891398e3f50d4610d08aa1`  
		Last Modified: Thu, 10 Sep 2020 00:58:10 GMT  
		Size: 180.9 MB (180872565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:7076f02eb891d5e2b711f2edc7cbdf4efae233382dc121f92886d2543b000997
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.7 MB (291659963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9b3f4c7da6f4d49d99d977707cb7324a9cb2dd6f62174b0182063d9f240afde`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 10 Sep 2020 00:11:28 GMT
ADD file:23fbc90316c23c82a8b8da300c8a5623fc3db73c430d1cbdbfab09ab920a25cf in / 
# Thu, 10 Sep 2020 00:11:29 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 01:51:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 01:51:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 01:52:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 01:54:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d4d2daf5b278e6cc19610d2a52a8745b441acb4d3e087f6cc35aff05d6ce2a0d`  
		Last Modified: Thu, 10 Sep 2020 00:20:05 GMT  
		Size: 48.2 MB (48156817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a6077d1cb3cebb93b8c52f5ee67a1e8892b694f688bf524f487683dd6d73ae`  
		Last Modified: Thu, 10 Sep 2020 02:04:24 GMT  
		Size: 7.2 MB (7183991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68290485256667f0290c0c36ddfaa24ac0efa67a798c296d2394e992241c37f`  
		Last Modified: Thu, 10 Sep 2020 02:04:24 GMT  
		Size: 10.0 MB (9958902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6243d9066fe23d908d1940b8e53b4e697b444414574a36cb7036b971ad2fac4`  
		Last Modified: Thu, 10 Sep 2020 02:04:50 GMT  
		Size: 53.9 MB (53939644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cbc3d9d502aa2db90b0b7e210db0b20a933489b6670fd1006a590c95618294f`  
		Last Modified: Thu, 10 Sep 2020 02:05:43 GMT  
		Size: 172.4 MB (172420609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:821bfedb2ae9b56ef224f54990ee251673fa4173db03f68b390143c0c40721d9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.2 MB (318195683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de3cba83f25f0d69ea7c5e30bc6d6342448948130748124bd95732596700737c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:52:18 GMT
ADD file:0b10d18375e8cd004468a07659e73e4afcd826f2808314dcc8fbb6b773c3ed6a in / 
# Wed, 09 Sep 2020 23:52:28 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:32:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:32:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 00:33:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:34:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:21fc4451f3aee8da37deddc4046fa3dd8ea41b5a39481b93c43bc5dd385277d5`  
		Last Modified: Thu, 10 Sep 2020 00:00:09 GMT  
		Size: 50.8 MB (50845252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a512823677991a1ec2c1f7550a8c3a6487f162cd565b6dd962c3aa9b66dc8e4`  
		Last Modified: Thu, 10 Sep 2020 00:44:13 GMT  
		Size: 7.7 MB (7742930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd8c9bf36c9423fe3a0d5d41b5d9036503bf5255e2c101307b378c250acebbe3`  
		Last Modified: Thu, 10 Sep 2020 00:44:12 GMT  
		Size: 10.6 MB (10635615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73d6346b9916616b4076b9aff9d017cdd90e7fb012d0b3d204e9b370267adb5`  
		Last Modified: Thu, 10 Sep 2020 00:44:39 GMT  
		Size: 59.3 MB (59260282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0861a90b98a4661aea400e18b046429342bf9e549575d7d1712413f99b736b`  
		Last Modified: Thu, 10 Sep 2020 00:45:41 GMT  
		Size: 189.7 MB (189711604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; 386

```console
$ docker pull buildpack-deps@sha256:180053af122f191be7ba247c82c956ce4ddac3dd81087a3ab9d7224acf2608d9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.6 MB (337610655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9066a0ccbe8b21a198b2def1603a85b436fc785e5903c3e59ddb086dcdceb0ef`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:42:20 GMT
ADD file:0f16119ad5399bd128cd02055185b1f534348a2ea02757438ace9e8b088822c2 in / 
# Wed, 09 Sep 2020 23:42:21 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 02:03:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 02:03:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 02:04:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 02:05:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9cf7fbf089a5c33a8981bcf78f935777e9a0e1340c0526fbe21a102ede6f5a74`  
		Last Modified: Wed, 09 Sep 2020 23:48:07 GMT  
		Size: 53.6 MB (53574966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f36d7641398c875328b89518c4c6818380e424e9aebcaa4eeefd60ae4fbcb51`  
		Last Modified: Thu, 10 Sep 2020 02:16:09 GMT  
		Size: 8.0 MB (8045826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5a56cc39855fb74a0eddc89ad1e907b97eedb1bd547082944b5873578db6bc`  
		Last Modified: Thu, 10 Sep 2020 02:16:09 GMT  
		Size: 11.0 MB (11013609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679898d9f857b002e401c706fa59cb54cf5d63db800bee6dde22629123036033`  
		Last Modified: Thu, 10 Sep 2020 02:16:32 GMT  
		Size: 61.0 MB (60997616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb0bb5b624ff7ea839a0a7c05b54a9e546bc836739d935e954721a0b919482cb`  
		Last Modified: Thu, 10 Sep 2020 02:17:29 GMT  
		Size: 204.0 MB (203978638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:db2b51af724b5d7d1677dbd1ecef2d8c0315d18ca7480b2fd6ddac0781565c45
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.8 MB (323762363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e276f205f5d781f48ccf9fe4eed1fb731450d83cdcaa4ca98b285b4fa559e77`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 06:42:49 GMT
ADD file:c8977e04a216367623fcae06b950449d648b73fe2ebfeea8ac4d43b825fd9072 in / 
# Tue, 04 Aug 2020 06:42:50 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 10:43:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 10:43:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 10:44:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 00:15:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d1b4f7d45a45e5da796e6015b373bab6d97853967e128d506ed0b95683b889a2`  
		Last Modified: Tue, 04 Aug 2020 06:49:31 GMT  
		Size: 51.1 MB (51146678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a299ca8f90646201e10c46e3299d7cb736e87e65cf92c7bc2363c5f7d61a0985`  
		Last Modified: Tue, 04 Aug 2020 10:54:08 GMT  
		Size: 7.5 MB (7450327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0eab5aef0c2a963011fc5090931d6499bfdbcfbfa1b05f6c2134d7eec1353f3`  
		Last Modified: Tue, 04 Aug 2020 10:54:09 GMT  
		Size: 10.6 MB (10599009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bcde08b2db228c5f62bc2c132c08a80d4bb091d3fbbd8918d0bd2307cf756a4`  
		Last Modified: Tue, 04 Aug 2020 10:55:01 GMT  
		Size: 57.8 MB (57828805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16b113c1b04e9dcdd245386909bd2fbe30cf44703f3f876052a7eb3482f23e2`  
		Last Modified: Tue, 01 Sep 2020 00:24:24 GMT  
		Size: 196.7 MB (196737544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:aa1a3efb8e895dd7a52b080f30baae656dc7af495547b984309e3bac59f368d6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.4 MB (343409142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:440164e3689e6f0090001a13580dc54e3f692d4810a8f57ef84f78e7936d3599`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 10 Sep 2020 01:06:51 GMT
ADD file:6525cb187fc85a4741e9d9de398149d93f43e196e99a20d48f165a25a1a8f36e in / 
# Thu, 10 Sep 2020 01:07:08 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 03:30:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 03:31:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 03:34:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 04:00:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:184155505be08ee96b6e64926098f03c472ad33bae3d34b8f683480960d7b5d6`  
		Last Modified: Thu, 10 Sep 2020 01:30:22 GMT  
		Size: 56.3 MB (56336687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f84de13452ce499d161f512ceea2535494fd124e4903980cc88297c393465b`  
		Last Modified: Thu, 10 Sep 2020 04:18:28 GMT  
		Size: 8.3 MB (8307371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62889fb00d8e6d8533f5a3ae0d38209c3a2e220aefda427a5f00b595e3862e8f`  
		Last Modified: Thu, 10 Sep 2020 04:18:24 GMT  
		Size: 11.4 MB (11389809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d0d792fd0c71e7d5a634580e82d16f64ab3485e3ec0591357c0572795f9bfe`  
		Last Modified: Thu, 10 Sep 2020 04:20:32 GMT  
		Size: 64.7 MB (64690200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad3b07475357d385dc65b22fb55b0c2efdeb798c5a12428c78dd1322adb5c30`  
		Last Modified: Thu, 10 Sep 2020 04:25:56 GMT  
		Size: 202.7 MB (202685075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:9bd95fe32cb8a57baed91471c61ba22b2b5bbef26326c0d2c1261d980941ed43
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.1 MB (306116171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5b5cd0c9c518c6806de33a4bd99fa77f56a99399e9a654a627669eece70f0e4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:42:52 GMT
ADD file:8cf459b787b06e517199d5538d4a79b845b7b7d72ccf10fffdee5a385c0895bd in / 
# Wed, 09 Sep 2020 23:42:57 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:08:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:08:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 00:09:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:09:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0777a1517003dde2e616b494a11a7867f55924ffac710d8d2c15b7b50fbeea1d`  
		Last Modified: Wed, 09 Sep 2020 23:46:42 GMT  
		Size: 51.1 MB (51060992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8333de3e2208d03a2b8282fff302f01069c5055fcb9e04e30943bfacf9e32d01`  
		Last Modified: Thu, 10 Sep 2020 00:13:13 GMT  
		Size: 7.5 MB (7541388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5f6b6e21fb8e9c70b582f6590d13e44a04a2d8a32abce90cbd029989466129d`  
		Last Modified: Thu, 10 Sep 2020 00:13:13 GMT  
		Size: 10.5 MB (10504798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc4641be68cc7431e368872e2c3c9c8325d04514cd9438c155d8f8e071d0b023`  
		Last Modified: Thu, 10 Sep 2020 00:13:28 GMT  
		Size: 58.2 MB (58230561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb0f160ae6f7086ea9f81a8b2d097e55b243d5175a3c74c9d72b5be2d5803d1`  
		Last Modified: Thu, 10 Sep 2020 00:13:54 GMT  
		Size: 178.8 MB (178778432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
