## `buildpack-deps:bionic`

```console
$ docker pull buildpack-deps@sha256:0677881751de9ea7d1fb18df17c461ee433f120b7c0fb2b314b4a572865018b7
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
$ docker pull buildpack-deps@sha256:4c51af3fb20a774f5a7f1eb8cd8260b9d7fa97f616d957bdbaf773eb884b9e12
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.4 MB (221390946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a07bcdd37ddcf68ea25412fdfa297e57410684e473d121d7cc209afea4cddded`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:18 GMT
ADD file:8b379a8fd96e76d10db6f9ae4e9675de33d227db0431ca2a7ca799119e905e8f in / 
# Thu, 01 Sep 2022 23:46:18 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:19:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:19:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 02:20:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:22:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dad0f37c70a668d101c86b5c769d452ff29c6d51f811891384cc7da00fce192f`  
		Last Modified: Wed, 31 Aug 2022 06:57:55 GMT  
		Size: 26.7 MB (26710085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9fb6a221e5e93168fd6c2e8fc1f6ac2ffb76528d9054917643eac23ecd551de`  
		Last Modified: Fri, 02 Sep 2022 02:36:30 GMT  
		Size: 6.6 MB (6631015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:622831c8e90067ca6fdaa29a2de932500fe9d780882f88bf84f70ea805f1e07a`  
		Last Modified: Fri, 02 Sep 2022 02:36:29 GMT  
		Size: 3.0 MB (3023735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef5399f56ce76677a6f9640dca31defa9b9c4eff3349b86ab8b540065f95fb6`  
		Last Modified: Fri, 02 Sep 2022 02:36:46 GMT  
		Size: 45.5 MB (45497370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512a5d2eb89ef20e41cda278a1c40c2027e4c73b0fb02e83b031e758e368c73f`  
		Last Modified: Fri, 02 Sep 2022 02:37:14 GMT  
		Size: 139.5 MB (139528741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:42c68e0fd12354cc0c8ff238452dd5f4dc3b40facc7d74bf491a935a148a3371
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.6 MB (189561437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae9fd874dc667c861187dbe1149d6742144b1d0ec1f281759a6dcd6ec9a09ef7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:40:36 GMT
ADD file:c5ca169f034f6be72446c95b43cd8cc6001848067793f102e7a2b970dd21db54 in / 
# Tue, 02 Aug 2022 01:40:37 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:53:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:53:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 01:54:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:56:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a03a1d54dcfd6ce7007bfa41c40b1747d5553db7ee3404e88dd3ddc54ede514e`  
		Last Modified: Tue, 02 Aug 2022 01:42:53 GMT  
		Size: 22.3 MB (22305613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e447528136f6bae661b10431db78cb9ef7c19ab2955f91547ad42ab927ab0a0`  
		Last Modified: Tue, 02 Aug 2022 02:13:58 GMT  
		Size: 5.7 MB (5706380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:853e8366b770a1c9813eeefe7e724b6b8a31f9c0f568cbe9111d2175d9615ae5`  
		Last Modified: Tue, 02 Aug 2022 02:13:57 GMT  
		Size: 2.6 MB (2585832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7091c5a50797aff4651704a5191e217f82e2558a29faa50bc2b17b38c723dcf5`  
		Last Modified: Tue, 02 Aug 2022 02:14:20 GMT  
		Size: 40.7 MB (40691688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fe51894567720f873449b2e6a0eb5052cf1d462d414dd4aa0ebd3731d57981a`  
		Last Modified: Tue, 02 Aug 2022 02:15:00 GMT  
		Size: 118.3 MB (118271924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:5cd3a764a3a0c6fec38fe227dbf551044ebfbcb68f15c6dca87566bb4e314752
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.5 MB (205516616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:284100b2301796f64bf6b9680715286f26d882c61cf648a2ccb11f9bf677728c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:43 GMT
ADD file:7002810c3cfdef12d2e13c49037e759257e42f5972f300411294e0239f3bdfe9 in / 
# Tue, 02 Aug 2022 01:18:44 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:29:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:29:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 01:30:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:31:24 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d2f2687beb6dd5f04849c57d6d83cabdfa44ec5cc5062369416bff4844045533`  
		Last Modified: Tue, 02 Aug 2022 01:20:09 GMT  
		Size: 23.7 MB (23734714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5a8ce0030c4c3bf1c638b4471e5162eef4a430b61c537057f0f8ce51fc18444`  
		Last Modified: Tue, 02 Aug 2022 01:48:44 GMT  
		Size: 6.1 MB (6079418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b63b2c6b27d8a588f648165c46146db98c94f4640019d6d8caf00868911d4133`  
		Last Modified: Tue, 02 Aug 2022 01:48:43 GMT  
		Size: 2.6 MB (2571299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18f5b480d0ef29386fe0d6deafedbc802a712685a5e5d30297050c9b51966267`  
		Last Modified: Tue, 02 Aug 2022 01:49:02 GMT  
		Size: 43.3 MB (43294820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f9ffbca9a42c25693e08ae45121aafa9cea7ce511c75f4b59cb6c96f2e4f907`  
		Last Modified: Tue, 02 Aug 2022 01:49:32 GMT  
		Size: 129.8 MB (129836365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; 386

```console
$ docker pull buildpack-deps@sha256:fc92538a42246a19e9b6fe14d4b7c484434d83d3921f7a8fe246c6fac0e7e090
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.2 MB (218226012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db587a96f18b5d8b5406236f5bc8470285602383cefa89ada14319edb706e6a0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:53:52 GMT
ADD file:93fdf10efcfc26ed4b10659ddc78284113a38c500811d27ffc41de25e2c9b4ab in / 
# Thu, 01 Sep 2022 23:53:53 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:49:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:49:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 02:50:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:53:24 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e09c10b62acdd55abc0548e8b24a3f314d657a49d5b9e4714ae753238c982a61`  
		Last Modified: Thu, 01 Sep 2022 23:54:38 GMT  
		Size: 27.2 MB (27164218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d41b26fc7fe91e2ecf5ff70769343de752ef61a55319ca667f268a98cc810f6`  
		Last Modified: Fri, 02 Sep 2022 02:55:19 GMT  
		Size: 6.9 MB (6919767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d7fab530814537d9359e7280fa86174abd2e93c698749527eaaee9d9ddf4b77`  
		Last Modified: Fri, 02 Sep 2022 02:55:18 GMT  
		Size: 3.0 MB (3039990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb2373c56afc32235e195e037d785f8292bb0241c3f6868421583bc3dfda755`  
		Last Modified: Fri, 02 Sep 2022 02:55:37 GMT  
		Size: 47.1 MB (47082793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a181670a8ba0bac016282ddffd44da983f589cda6bdf0e0b5f446db705d8d52`  
		Last Modified: Fri, 02 Sep 2022 02:56:06 GMT  
		Size: 134.0 MB (134019244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:41a63bf7973f04ddbec814069a00f18ee0cb97202aaf7971d0c10360c0564083
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.4 MB (246401872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11d9a9223beb8fb80585f9d45f14913bc249952f620f183153c4845dee9d0173`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:50 GMT
ADD file:32fc7b9b5853c93c45b1a96054c30104fd200ac7d40d0388aff736c478f917cb in / 
# Tue, 02 Aug 2022 01:30:52 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:39:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 02:40:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 02:41:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 02:45:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1a9ff13e38cae7994b55e6db5c3d190d2b7a03043ae238a6f71a285376de46bb`  
		Last Modified: Tue, 02 Aug 2022 01:33:07 GMT  
		Size: 30.4 MB (30441470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64118351c6d44eaafb1d0d7269124dc78b3b33e148c24e6e74c4ceec8f193a5c`  
		Last Modified: Tue, 02 Aug 2022 03:19:51 GMT  
		Size: 7.1 MB (7056186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eef1999418600ed0a0609447fc56e75b3b7fa9da4cf9c794143e6e7bf5e4397a`  
		Last Modified: Tue, 02 Aug 2022 03:19:50 GMT  
		Size: 3.7 MB (3720105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33779d765b23b6ec593dbfa7277e0bf995bc1d1ef071983b91619f293a535ff4`  
		Last Modified: Tue, 02 Aug 2022 03:20:17 GMT  
		Size: 53.7 MB (53744456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf86869cb4503e4b9bdefd4f0c3727612e42919ca0205783fc1de2425e16d9d0`  
		Last Modified: Tue, 02 Aug 2022 03:21:06 GMT  
		Size: 151.4 MB (151439655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:36cbc7af0f26da3257ab199a3e47cf3a966752ad27d166f1e6b947cef3abd82e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.7 MB (205747929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d011dd5ab53e3e563c6d96002d937f78405e0104087e57ac73d6b6d3d6d9d954`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:02 GMT
ADD file:ee88f505cbf59825aed59486848971d1be33d8cc49f3a1df647a1486f310405f in / 
# Fri, 02 Sep 2022 01:03:04 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:00:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:00:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 02 Sep 2022 02:01:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:03:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f98934bea0e17bc3e47aa5c2cb45f3bbcf512fd6211b763c88da22fffe217709`  
		Last Modified: Fri, 02 Sep 2022 01:04:37 GMT  
		Size: 25.4 MB (25369467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c380fb10cb841412807796ed4eb2a04c1db2dfb865319b304c5fe5fb3c1b9c`  
		Last Modified: Fri, 02 Sep 2022 02:14:48 GMT  
		Size: 6.3 MB (6324340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb2f7f4ce09236ffef21b9c319d300db314d1a530955a50f2097828643dee8b3`  
		Last Modified: Fri, 02 Sep 2022 02:14:48 GMT  
		Size: 3.0 MB (2977303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df77d423dad6b62da1d1c3444af712c31aa09215ac05dadd44cae836fd5c9db`  
		Last Modified: Fri, 02 Sep 2022 02:15:01 GMT  
		Size: 45.0 MB (45043976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d180965de40e5c0adbf799aa1acbd0a5d61ad7003f3d6c70407e047d90ffe7e8`  
		Last Modified: Fri, 02 Sep 2022 02:15:23 GMT  
		Size: 126.0 MB (126032843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
