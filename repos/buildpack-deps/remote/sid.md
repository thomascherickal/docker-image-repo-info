## `buildpack-deps:sid`

```console
$ docker pull buildpack-deps@sha256:21b91fb6e822f0ccb629778913eae139423dae9e78dabc8f7bf0c5f6cc6411c9
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
$ docker pull buildpack-deps@sha256:826b7f49bc9a72a20279db6c676aaf1f19ff402cc633bbbf904c251b7d4e5b41
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.1 MB (322078647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b41bb8c2c06896a0a16fc0921b0f55d9b4b0b01ec0d4811dee0afdd37b76e54`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:57 GMT
ADD file:97b8c276224b2b9407a1635d61780b968f86726642a00f3d49298ab19e9ea714 in / 
# Sat, 10 Apr 2021 01:20:57 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:55:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:55:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 01:56:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:57:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9097f35530b77dcae85a27364a3301e3362adb2860367422ed06b99fabe94b8b`  
		Last Modified: Sat, 10 Apr 2021 01:26:23 GMT  
		Size: 54.9 MB (54881626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cef4657bb2202fe6d13371845dabecbb1843dc3e9ab3d45afba017280a24f40`  
		Last Modified: Sat, 10 Apr 2021 02:03:17 GMT  
		Size: 5.2 MB (5169536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a456d1fa6a4d732964fc57896f119a9e85d6cae028f4deffc62729e23624641c`  
		Last Modified: Sat, 10 Apr 2021 02:03:18 GMT  
		Size: 10.9 MB (10868840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815ce4c9e511158bf858d6ebdb7862400e9c296a85eeccce737045c8e04145ff`  
		Last Modified: Sat, 10 Apr 2021 02:03:38 GMT  
		Size: 54.8 MB (54798810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce986c96c05b40a3246a50f4ed1397b3a8933e666eb453c9829290f006450814`  
		Last Modified: Sat, 10 Apr 2021 02:04:17 GMT  
		Size: 196.4 MB (196359835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:eae6cbaf20141aecfced2e5c51526d7d23846eb386a99f9cd4fcf791cf3be30c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.1 MB (295144721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7f5e1196dd3b711e7a01a4f21ac18f304f2ad73daef766bec8e5de21df97183`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 00:52:44 GMT
ADD file:9bdb85e8b11f9d011901b496376920ceaf2a43e4dd9f7dce303f362c5cd9847b in / 
# Sat, 10 Apr 2021 00:52:52 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:07:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 02:08:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 02:09:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 02:11:21 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:84ee0e585c798c84e07ba41f87e072c0fb43795cb12e325a126f9026f876059c`  
		Last Modified: Sat, 10 Apr 2021 01:00:27 GMT  
		Size: 52.4 MB (52414024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f91ce0c40daeff87428c76fc2b11803ad6153af50d86ab3e84d37fb8ad8ca7`  
		Last Modified: Sat, 10 Apr 2021 02:20:41 GMT  
		Size: 5.1 MB (5074282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a126b0b2e172136e012642af22312fd73d761d735f0990caf91f35b6f294fb88`  
		Last Modified: Sat, 10 Apr 2021 02:20:39 GMT  
		Size: 10.6 MB (10570471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d442e399c5e6a8d0ac5b10309719b78c3f28f95043726252343efa4387a92288`  
		Last Modified: Sat, 10 Apr 2021 02:21:05 GMT  
		Size: 52.5 MB (52498471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134a9d706d7bfb467b998041cdae5a80b507c2059ef13d990f31e13f45f2e876`  
		Last Modified: Sat, 10 Apr 2021 02:21:59 GMT  
		Size: 174.6 MB (174587473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:c1baf6d0bfe9dae2bcada6e693febdda0d8c91f0aeac6bc25e7a52de1f746529
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.6 MB (282570422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02afe6a325f0cb8fe7cbfebf971c41ba7059bf6c6ac19ea91855bfa9ae1a9dbc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 23:09:57 GMT
ADD file:3c49310ff7c2a9c21073b7ca0884f4b8e783606a6653a2d74d1aa04196a3ed8f in / 
# Tue, 30 Mar 2021 23:10:01 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 01:25:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 01:26:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 01:26:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 01:28:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f41ab33290e85402afe03e9a82d0262689d71eccbba0d79246595731d24f2688`  
		Last Modified: Tue, 30 Mar 2021 23:17:34 GMT  
		Size: 50.1 MB (50070962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d173ac9612777e7e6d56bd74819357eb0a74fdd29dd54af742a5652ae5ac6d`  
		Last Modified: Wed, 31 Mar 2021 01:38:18 GMT  
		Size: 4.9 MB (4934354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b41bd459aeb849bf22b88bf2563aeffb2527f25a09c92049467c43605bdc30`  
		Last Modified: Wed, 31 Mar 2021 01:38:16 GMT  
		Size: 10.2 MB (10218235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac4b6fcf9d7014405b480814f8a95c15f4f875f267145cf47283fb0315a7ec4`  
		Last Modified: Wed, 31 Mar 2021 01:38:41 GMT  
		Size: 50.5 MB (50514433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d236d27cc2a6699f4661433efbf6be31904da6b7b220e81a1a977f9063106e0`  
		Last Modified: Wed, 31 Mar 2021 01:39:33 GMT  
		Size: 166.8 MB (166832438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d46ed71c122fff936e5c78a8e146ad724e4d250304ada1a0cb89ae46562050d7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.8 MB (313768605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6516cc551c567d1a47efb9687399d22b4bc99767e3fe89c0eac5cfd738e5edfc`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:30 GMT
ADD file:6bd461aca61a6c4468971e152cdd2158ba47c56a30fedd2560ab69bc0d5429d0 in / 
# Sat, 10 Apr 2021 00:42:34 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:49:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:50:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 01:50:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:53:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e4d191ad9b976ffe4d9719cf4d8241d751e0870f7abf4ded747f4258cce757b2`  
		Last Modified: Sat, 10 Apr 2021 00:48:46 GMT  
		Size: 53.6 MB (53568143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5779dd445520bcb3f8ff73ed0cfdf91d218d8c0272557c8e2959626d83c1e6cb`  
		Last Modified: Sat, 10 Apr 2021 02:02:23 GMT  
		Size: 5.2 MB (5157782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef3c386828fc4d261064c2034ef6ea283e4de5534b6dc52e8f7dd4d4cb671677`  
		Last Modified: Sat, 10 Apr 2021 02:02:24 GMT  
		Size: 10.9 MB (10868647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f51a5dcfdd30750f476f52ea0e183b37054c17682ecbd66f52636582ad051c41`  
		Last Modified: Sat, 10 Apr 2021 02:02:46 GMT  
		Size: 54.9 MB (54920818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c48769838a9abb7c058dca4fa32400e26d68739d5fd7e303e2ec2f8b8a37ec`  
		Last Modified: Sat, 10 Apr 2021 02:03:35 GMT  
		Size: 189.3 MB (189253215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; 386

```console
$ docker pull buildpack-deps@sha256:75f47e98cf0af3bc3395ced1d036d2bbea5839049e1950e69167824cd439a59a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.9 MB (327938952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae24a23b3a3687e83fbe37d9854b71827bcb85d0f7ba08cb54f68e1475763aab`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:40:35 GMT
ADD file:1f041945ff890476db13a1209d904306e018db9cc0c3ddd68afde8ba20721441 in / 
# Tue, 30 Mar 2021 21:40:35 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:59:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:59:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 30 Mar 2021 23:59:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:01:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c1abc0a07df2794b8c01aadbeeb9293997b8a54aaa313f435b4d2d676f888235`  
		Last Modified: Tue, 30 Mar 2021 21:47:59 GMT  
		Size: 55.9 MB (55881675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc5ab305c1c154665b02986b2328de2fd181084b0c296c4d76f131107ddef04`  
		Last Modified: Wed, 31 Mar 2021 00:09:46 GMT  
		Size: 5.3 MB (5298115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95df009a7c979f03789affbb069b0972638a182a6594760beb04e5d621ca33b`  
		Last Modified: Wed, 31 Mar 2021 00:09:47 GMT  
		Size: 11.2 MB (11249054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e2268237c64ae5a91b7f0d8e740b5f590a7da88c2ae88e6e9356441350ab351`  
		Last Modified: Wed, 31 Mar 2021 00:10:17 GMT  
		Size: 56.2 MB (56194937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3610a79bdcdc0adf7228d3861a0cc861f7be9f315dc880fd1fc27bb0401ebc3`  
		Last Modified: Wed, 31 Mar 2021 00:11:30 GMT  
		Size: 199.3 MB (199315171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:ff73022f677b789c980c2de3e155df99d85e4fe026becf5c7a69a13fb055e3de
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.6 MB (301563351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a393ff6b5c68205031539b18f4cadca564d3b5a46cb657f358123dc7b5440fe2`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 01:10:06 GMT
ADD file:a0cb4c0af6dee6c99c3739fc2b27a4d60df79591342d18fd79bb4e38a25d28d5 in / 
# Sat, 10 Apr 2021 01:10:07 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:11:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 02:11:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 02:12:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 02:14:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6eda60e328d687e0091fed92ed18129ac8eeed03d72dd92f7941c847f05a6dfa`  
		Last Modified: Sat, 10 Apr 2021 01:17:00 GMT  
		Size: 53.1 MB (53138256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b35bc44f5e1748a146c217ae7f8eeb19f129f8171afdfb72f50c2e672425aa`  
		Last Modified: Sat, 10 Apr 2021 02:22:09 GMT  
		Size: 5.1 MB (5128904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9290332c458e552d3d40e8db4b52e91c80f460edf5da9ee4bd9e86668fe97738`  
		Last Modified: Sat, 10 Apr 2021 02:22:12 GMT  
		Size: 10.9 MB (10870902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0c1430cb8920e76053cbffc8ab83c10ecb5c076f046396b396d747c42e2d2b`  
		Last Modified: Sat, 10 Apr 2021 02:23:01 GMT  
		Size: 53.6 MB (53589224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c25459c6df1e5ba51d6ed513c9d939e2a6ed612bfa8375a6e6a419db8a35e37`  
		Last Modified: Sat, 10 Apr 2021 02:25:09 GMT  
		Size: 178.8 MB (178836065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; ppc64le

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

### `buildpack-deps:sid` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:88959a2e39a2e87711e39a570e5232c172a0720e4e39fa4ee1f0cd4f2fc33e32
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.7 MB (295694757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3e91000c7cfe8ecfeddb072a9511e59705f18031653402ae7dc3f909821c979`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:33 GMT
ADD file:95fd1353430dde759ab86e64384180601d2eec1359d5a81ebeb58e17b8998353 in / 
# Sat, 10 Apr 2021 00:42:36 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:29:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:29:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 10 Apr 2021 01:30:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:30:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1b22aeeaee0a7589a5b67e1a3571ce4d1a0942461ff2075b104514fa1967711d`  
		Last Modified: Sat, 10 Apr 2021 00:46:02 GMT  
		Size: 53.2 MB (53155408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a9ca0514c5f0614720863667ddd96ff334dce5555e8ae2112bed88bfa4c6711`  
		Last Modified: Sat, 10 Apr 2021 01:34:29 GMT  
		Size: 5.2 MB (5151136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe0daca911ede51529950150d6623adb8cf7f5d56b37a6dcb3e07ee55232054`  
		Last Modified: Sat, 10 Apr 2021 01:34:29 GMT  
		Size: 10.8 MB (10758740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f202156cce94de4434decbe56b2df6c30d6939cd5413272e421aa0edb064219e`  
		Last Modified: Sat, 10 Apr 2021 01:34:42 GMT  
		Size: 54.3 MB (54256990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afd2e43891e8d13519a0b8b4f80950dcb9584a442fce2f7f44e0333c603e212`  
		Last Modified: Sat, 10 Apr 2021 01:35:08 GMT  
		Size: 172.4 MB (172372483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
