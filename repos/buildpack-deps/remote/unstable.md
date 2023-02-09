## `buildpack-deps:unstable`

```console
$ docker pull buildpack-deps@sha256:f40d3111f99008c51c9639e873bfaa41bd4cb0265ca5a7d5ab4409feb65d97ce
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

### `buildpack-deps:unstable` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:530aa2b48a2edb36394752b44168228f433560d8025cee067dc827fced2ff080
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **345.0 MB (345049456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a360f005a534aaa48677cfef0730ac1d149d9fbed32dc8e53a240aa4ee7a6a98`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 03:21:29 GMT
ADD file:b3a4ee0f0fbf2d8fbbab0aefd91aa4d658c41b09c8a2beea1024bfce5e7d3fca in / 
# Thu, 09 Feb 2023 03:21:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:14:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:14:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 09:14:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:15:24 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ca2c7deeb5af7aa8a0aa3358218901c07b10bb98573151782e5e7af0ab03009c`  
		Last Modified: Thu, 09 Feb 2023 03:26:46 GMT  
		Size: 49.2 MB (49234515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f93cb2a3ee7c65cae5b96772e26d36982fbb6f591036fc399794173b26a5be`  
		Last Modified: Thu, 09 Feb 2023 09:20:03 GMT  
		Size: 9.0 MB (9049525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550c07c3dce5647c4605a0f377d103211b5f499343e022eb8a7ca1fec0e6146c`  
		Last Modified: Thu, 09 Feb 2023 09:20:03 GMT  
		Size: 11.4 MB (11405779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c13917382022dd673297c082131550c1d9119b80b9149559b5ae6be503ee324`  
		Last Modified: Thu, 09 Feb 2023 09:20:22 GMT  
		Size: 64.7 MB (64654750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03ca5f4971b69d313ded5e37be68b6110e3af42674aa52c9fe6280498b6a0fca`  
		Last Modified: Thu, 09 Feb 2023 09:20:58 GMT  
		Size: 210.7 MB (210704887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:467dc0c8577d09b8d8c46d25087bb1fc5041ee5c57cab2671c4d549edf1a7e1b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.9 MB (313850616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4b3caaddb529259b5e04b9cc5a1b02d122a0545dd26195991a2bf43963769fd`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:00:45 GMT
ADD file:dc28e6a68656b2258d74ca814eedc70f45b8b6c604f68add2cf2f5f7bca2b675 in / 
# Thu, 09 Feb 2023 02:00:46 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 02:33:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 02:33:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 02:33:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 02:35:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cfc3c8b7a8637963e4e7c58d3159378d2dbbf0ac34f355b8781c04894e7b070c`  
		Last Modified: Thu, 09 Feb 2023 02:06:07 GMT  
		Size: 48.2 MB (48168655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b0465a62c889ae7f4e147e07d5d9bf9550c4429db66328d0b271ef3a102aadd`  
		Last Modified: Thu, 09 Feb 2023 02:38:57 GMT  
		Size: 8.5 MB (8494792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af07aa0cc01d6588de33c6d10e2165894401135ac335ab64e1eb43ae2718b707`  
		Last Modified: Thu, 09 Feb 2023 02:38:57 GMT  
		Size: 11.1 MB (11051457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8d98ee8d17ac4670826e17e1835b3837241b0308caf8c0db0c4c022d7a0cca`  
		Last Modified: Thu, 09 Feb 2023 02:39:20 GMT  
		Size: 61.9 MB (61913806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33ce4a8b93d8a6b03769fa649d930b8453d4da3b7cc0002e3f66ebeafadbfa85`  
		Last Modified: Thu, 09 Feb 2023 02:40:04 GMT  
		Size: 184.2 MB (184221906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:803196a373cae16bbc90262196f1750bb65dccf3007c59033cad85955b6c46e3
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.3 MB (299324000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d03bcca0c61e6bfe584ed320b3dc22485198b2beade97da312fab4430056f83`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 06:13:32 GMT
ADD file:fbab075e495bd9771e90704c5bfe9fb15c30193973e2bb5c45e75cd23af10cf3 in / 
# Thu, 09 Feb 2023 06:13:33 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 17:40:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 17:40:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 17:41:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 17:42:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a7ea7bdbf318551bbcc5dd17e61a023405583aed3de05afb9d0d7d7c69f7d9f1`  
		Last Modified: Thu, 09 Feb 2023 06:21:13 GMT  
		Size: 46.0 MB (45986881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cae37dac679959624898f1540e289e04f11094cac8e34e5a293d7b735010ab1`  
		Last Modified: Thu, 09 Feb 2023 17:49:39 GMT  
		Size: 8.1 MB (8140778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5340840f2ef04e80ad9c82beb3b4a9f0685e521d4da3bcd8a7a2b582fa331d`  
		Last Modified: Thu, 09 Feb 2023 17:49:39 GMT  
		Size: 10.7 MB (10687604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc4c568e22aed5e461cc11486e5372ec33f00c28da96d57e6d52a3969885726`  
		Last Modified: Thu, 09 Feb 2023 17:50:01 GMT  
		Size: 59.7 MB (59737446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f84d4a7ae460f65650f5aacb56658d1f3206bd83af4f639559ce998e4f1514b`  
		Last Modified: Thu, 09 Feb 2023 17:50:40 GMT  
		Size: 174.8 MB (174771291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:4481d1a1e5e8419669bca300ed0da3e5fce2840dc3ee213ba4479ecfa0f70269
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.1 MB (336128116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87d606b7d94172cfef488feda1efae7adc91b46988bc880981855c08a37b8de4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 03:59:27 GMT
ADD file:e092144c3667bd346dc4cb05da5a70ca9f7303d7160f9d5763af88fe51e02f66 in / 
# Thu, 09 Feb 2023 03:59:28 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:10:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:11:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 09:11:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:11:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:00f9d2ac5ed56c16a45852afb781f7257c58125a3b154fa75d18141566291f9f`  
		Last Modified: Thu, 09 Feb 2023 04:04:03 GMT  
		Size: 49.3 MB (49272262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4236d19f832b8139af289e6bc94d52514e6619bf7af68bf4e0d5486d078ab198`  
		Last Modified: Thu, 09 Feb 2023 09:16:12 GMT  
		Size: 8.9 MB (8881496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d593ddd7505c3c57f2e72480778f0c8b24fd4fc541502ac3315e74da1ece02`  
		Last Modified: Thu, 09 Feb 2023 09:16:12 GMT  
		Size: 11.4 MB (11371475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34a0f918de12021ca105f08f15048dca4f091a52ec82562e8ed161c20d6295be`  
		Last Modified: Thu, 09 Feb 2023 09:16:28 GMT  
		Size: 64.3 MB (64330786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e884eb398901dc2829b1495c14b982e938786dcf5ba0376fb78be3cfb3195e21`  
		Last Modified: Thu, 09 Feb 2023 09:16:57 GMT  
		Size: 202.3 MB (202272097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:a27de1357f62800bc5b75f241eea6c650c8328ec63e58580cae2aac6f5c413f7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **347.3 MB (347265875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47549e319edcb9175d4054cd9505206510ab2ec3bb8158830b24a2a09d1e246e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 05:14:01 GMT
ADD file:9ac1978405b6f0a95e33d1c34f01be82bbc11fcce2878747e4f688335279964c in / 
# Thu, 09 Feb 2023 05:14:02 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 12:21:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:21:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 12:21:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:22:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e58ae2871ac91256d220f3da2b9736b2afb1a06906579876546cfae103647f95`  
		Last Modified: Thu, 09 Feb 2023 05:20:31 GMT  
		Size: 50.3 MB (50285434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63157a71f0b70036d0f159943883d2dec99b34dd02078c1150493e56800b5e7a`  
		Last Modified: Thu, 09 Feb 2023 12:27:34 GMT  
		Size: 9.2 MB (9228126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a7be4264e22d81f1727f1d238e725bcec2452ff92a06d1353a114921801f911`  
		Last Modified: Thu, 09 Feb 2023 12:27:34 GMT  
		Size: 11.6 MB (11607645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4572df341089434d0f6aed05bf3344d403f26e9871bfc61f4520c2ab4eefbc`  
		Last Modified: Thu, 09 Feb 2023 12:27:54 GMT  
		Size: 66.5 MB (66527869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c9c73eaf745eed4672ad9ab4796ffd5a3c57f3feb5d6a216f22be09c4fa0e3`  
		Last Modified: Thu, 09 Feb 2023 12:28:29 GMT  
		Size: 209.6 MB (209616801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:a82507a1277c2124e09e887dfd7b4a31b0b1a1fc8bdec1f883b117f297e76d2c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.0 MB (324036580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d50a394cea62448159f423b39c3070b86d3314f1423d507654ecb0497d9c0d7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:46:00 GMT
ADD file:e14c7d6714484cc404ef7af2c7e0fcb17120cc8c1b631e9ac731a3be75da22b8 in / 
# Thu, 09 Feb 2023 02:46:04 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:48:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:48:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 07:50:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:55:48 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:84e1d5547cbc284ab87d41eaa50711a7148e6080522c4ba245d27048c9d0fe70`  
		Last Modified: Thu, 09 Feb 2023 02:54:32 GMT  
		Size: 49.1 MB (49094289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16034fc732dcaff117d4120f724155ad39c461a2791c8bc488000dd93d88467c`  
		Last Modified: Thu, 09 Feb 2023 08:03:01 GMT  
		Size: 8.4 MB (8414070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95cc8b6e8bd467b0d1e27bfaf0bf0138f2e690aa8dd7eeddcc636d65c4b0ac34`  
		Last Modified: Thu, 09 Feb 2023 08:03:01 GMT  
		Size: 11.2 MB (11153733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23789f2ae164d9a3f26a9a0663d938660993a4ba223713b5bde1aa34f68d35dc`  
		Last Modified: Thu, 09 Feb 2023 08:03:53 GMT  
		Size: 63.3 MB (63305330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd03ad3d3e89587274ed0844975c8ff2700fd1f95b056d7346b990bf970c894`  
		Last Modified: Thu, 09 Feb 2023 08:06:05 GMT  
		Size: 192.1 MB (192069158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:5be92ba5a3b017d2b78ebfb369785c115888e85e0cf5c0cc17d72b79e42ae0b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.0 MB (358966060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7af53061cbcc3dd1d8384071e81ad83d3562f09422c4bcedc969216810173fb`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 06:22:13 GMT
ADD file:2c626d6b2dc96ed4051ff24603784037a34ea2aca8a2555baab15ec102b1f250 in / 
# Thu, 09 Feb 2023 06:22:16 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 12:30:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:30:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 12:31:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 12:33:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bbf1522fb0b9e1d36e390546f20fa29b91e1fab7c915527df75f01bbcf172b2c`  
		Last Modified: Thu, 09 Feb 2023 06:28:56 GMT  
		Size: 53.2 MB (53247040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0635828bd5bfeb3b339b41770bdc09a23b92382a15dfbf2d52d458b6eb76ea09`  
		Last Modified: Thu, 09 Feb 2023 12:40:38 GMT  
		Size: 9.6 MB (9629627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc219ebf76efb77244a7b932cc029b1d8c0a8582447c1c83b5951dbd0300b5c9`  
		Last Modified: Thu, 09 Feb 2023 12:40:38 GMT  
		Size: 12.2 MB (12168333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:953c4fb72f302b1bb289286f1d3d5c20dd2e2c7a41f26f635e40d881218721e8`  
		Last Modified: Thu, 09 Feb 2023 12:41:08 GMT  
		Size: 70.0 MB (69988564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfa3cbad67be8f62db0d3946c3ecbdcaf700fdf297615751de439b5d5e4e017`  
		Last Modified: Thu, 09 Feb 2023 12:42:08 GMT  
		Size: 213.9 MB (213932496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:2d7a50da581b3dcea2f7a8c6a23d25dbbb2906e342446e79512b1b76cbde6e67
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.9 MB (313928587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d769cf3be472cb469b0cfd71f347e39b010ba850a804b249ee087d976cbe8070`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 09 Feb 2023 02:41:57 GMT
ADD file:2e666c175716fd02a858ff036fcece3fd5bc91959ad6e87ba5371f0e1c35eee8 in / 
# Thu, 09 Feb 2023 02:42:00 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:33:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:33:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 07:34:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:36:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3019a6e7de2300389d30ae5349430a715e5e0de8dee24a1c55adb1f7bf5c4133`  
		Last Modified: Thu, 09 Feb 2023 02:46:21 GMT  
		Size: 47.6 MB (47605532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe2bb0faf3ad6788e6ff9dc1a5f7979c08396fca0cc8a68674481cb53146b784`  
		Last Modified: Thu, 09 Feb 2023 07:41:24 GMT  
		Size: 8.7 MB (8681429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6878c76211620beede9a73a2e8ac2a5aecaefaf3857d40ddecc77e798a54c9`  
		Last Modified: Thu, 09 Feb 2023 07:41:24 GMT  
		Size: 11.3 MB (11269128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60bfa6a2fd1c7666b1f759c24592d944f1cac039fbe1f1feb9d7d1103426b1df`  
		Last Modified: Thu, 09 Feb 2023 07:41:39 GMT  
		Size: 63.4 MB (63407110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27fbcfa024c9102d27c271fd9457878bb5348d6c140cf7d2b6e027a439389b7b`  
		Last Modified: Thu, 09 Feb 2023 07:42:07 GMT  
		Size: 183.0 MB (182965388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
