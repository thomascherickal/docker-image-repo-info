## `buildpack-deps:impish`

```console
$ docker pull buildpack-deps@sha256:546da64e56fd044fabeef1295a1af1161ee024c31b505661c62d34b1267db511
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:impish` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:9af39729d3d63f5797c785605e9c26effbfb09444ef91f5bd0099e5827edd880
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **406.9 MB (406868171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa7f2e7a9355bb02a5478b27f15892dda84f9277790d6bf142f99d5982080d53`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:21:12 GMT
ADD file:355a5f56bf0136597bcd90b01ff73fc517b6bf7e76f45b65bf1af1136f434462 in / 
# Tue, 31 Aug 2021 01:21:12 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 03:02:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:03:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 03:03:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 03:05:48 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:25907b3add375d4f44a3bf4bfc3544b51ff9f4a23fe8c186f3b20e54b37d19ae`  
		Last Modified: Tue, 31 Aug 2021 01:22:53 GMT  
		Size: 30.6 MB (30602781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ef40c83a42d65ce37ce8bc08e06a0c4b994512527cad13196aca51586d9bd7`  
		Last Modified: Tue, 31 Aug 2021 03:14:51 GMT  
		Size: 3.7 MB (3692694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a871edcbb988433606f5a8d03efc8f0d9d49a4cd78a5d506401ec3b7854a2162`  
		Last Modified: Tue, 31 Aug 2021 03:14:51 GMT  
		Size: 3.6 MB (3552016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59778cb761facf0aaa7ff7cab370d47bdee8a1c0764186ec8286f50fb911a78b`  
		Last Modified: Tue, 31 Aug 2021 03:15:08 GMT  
		Size: 38.1 MB (38114895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ffa26f12ed647c5e1c9898915298f9e7389c733e2825bad35dac65a6b529755`  
		Last Modified: Tue, 31 Aug 2021 03:16:00 GMT  
		Size: 330.9 MB (330905785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f6678c935da21dcc51c2272f514ae95e68946b6e94206470cfa7e0d3c84f3f33
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **371.1 MB (371066555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f07948a9b90cd3d03abd58a6ebacbaa26c4f20e9a3ce2cd987bd465f4ed3965`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 02 Oct 2021 05:59:55 GMT
ADD file:6ac61c944ca4bc7b903b037816e21005acf3338af57e5732f38b396acbbefef6 in / 
# Sat, 02 Oct 2021 05:59:56 GMT
CMD ["bash"]
# Sat, 02 Oct 2021 22:27:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:28:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 02 Oct 2021 22:28:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 22:30:43 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:85bc3e6b05f0f487b1f8903c51a8bf098a931ac723c2ff30726c9b4f42e7d8be`  
		Last Modified: Sat, 02 Oct 2021 06:04:07 GMT  
		Size: 26.9 MB (26916992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfcf1a9d4fbdb8bcdea8da245690e0e7b0d7f42cd7b7480dd3f9866881a1da2c`  
		Last Modified: Sat, 02 Oct 2021 22:43:19 GMT  
		Size: 3.4 MB (3448048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dfa76bdfd39c414c299c1e02cf75c9b579b3aa69ca8e1abf9eb876765fcc9ab`  
		Last Modified: Sat, 02 Oct 2021 22:43:18 GMT  
		Size: 3.7 MB (3742516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360154fa07ad953713f7e71f7feffabf9f868fa69562aeb598e60ebd881ede16`  
		Last Modified: Sat, 02 Oct 2021 22:43:59 GMT  
		Size: 40.3 MB (40285193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80eb0c2a0ca1287f5644704ab6ae1dbfd650eeae5b8ce48ee335e46a1a2bd068`  
		Last Modified: Sat, 02 Oct 2021 22:46:58 GMT  
		Size: 296.7 MB (296673806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:173282a68ed3c7d434e0a049630d7ee47e5ff9b0937c87e24de80c41032b44f8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **399.8 MB (399753642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c681f790e2c9ad75fe348a46f94492c9e4e2a4cf1c6e08b36b18048884d41020`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 02:44:16 GMT
ADD file:55c9fc8bcadd5ae136c0fd0e7bc6b97490ad9f02d9fe707ffda0ab5ba6208a63 in / 
# Fri, 01 Oct 2021 02:44:16 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 03:20:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:20:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 03:20:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 03:21:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d6840eb3b14e719af003eb60b9616929459d959673d9a13237691e5be0928545`  
		Last Modified: Fri, 01 Oct 2021 02:46:30 GMT  
		Size: 29.0 MB (29047978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50e1bb6cc21d9aa99ea2365d91ca737ff33423cf8eef3ac6d444f9264ecf62c`  
		Last Modified: Fri, 01 Oct 2021 03:27:33 GMT  
		Size: 3.7 MB (3680866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44384e90f77381715996a06f1aef553b1ffe6e32cd9f467350b914746ba678eb`  
		Last Modified: Fri, 01 Oct 2021 03:27:33 GMT  
		Size: 3.5 MB (3533741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15dc1cb90f475d191407aa41ee7d90ffd845371c604e65fedf778556ba48612f`  
		Last Modified: Fri, 01 Oct 2021 03:27:51 GMT  
		Size: 38.0 MB (38028253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41fd4f9a27c5ce4d91f6bfc6770ad8a8b894911d0d94e7e683e9c34844be1c22`  
		Last Modified: Fri, 01 Oct 2021 03:28:51 GMT  
		Size: 325.5 MB (325462804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:9cbc0b25eb1059a2344688a05c44515a8ba8a519851d59da84420c3d28ff2280
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **414.1 MB (414117401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d6e8a9a92bf6c2666f62184bc67b5754d4d946e9b3cf4957015311ff4edf39f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Oct 2021 11:08:44 GMT
ADD file:336f6c173990c33ed817c24e2640c594320911a456647acdd356ff4dfd6c2d3e in / 
# Tue, 05 Oct 2021 11:08:51 GMT
CMD ["bash"]
# Tue, 05 Oct 2021 15:23:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Oct 2021 15:23:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 05 Oct 2021 15:25:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 05 Oct 2021 15:33:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:364d4546a8bf6fc0df00b576bfd4c074f52c0bd19474259ab96c4c6a58140d0f`  
		Last Modified: Tue, 05 Oct 2021 11:11:40 GMT  
		Size: 36.2 MB (36159197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08941d10301446e3b9f95eb93793958be04db53bfcedd63800802197446f3ec6`  
		Last Modified: Tue, 05 Oct 2021 15:54:28 GMT  
		Size: 4.1 MB (4129253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6916b52ad6f9ca46fb53c02f0f6025d866e6855850ceeef9a213c9021ef24132`  
		Last Modified: Tue, 05 Oct 2021 15:54:26 GMT  
		Size: 4.2 MB (4241645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e54bd8b9982b0cbabe2313153156a1cbe061d95abe7ed46b02f29992ffb8b851`  
		Last Modified: Tue, 05 Oct 2021 15:55:01 GMT  
		Size: 42.6 MB (42633497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd8664edd50c4e10be42fd89d3e3ef7e051ced233847b35efe6557d6456f280`  
		Last Modified: Tue, 05 Oct 2021 15:57:18 GMT  
		Size: 327.0 MB (326953809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:4b22a884a0b2e518316ae5bca5a1d25a68152cbcd931d8334e80136baac33ec5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.5 MB (266483053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ad71d8370638795c9aa2a2d157409cd2ca60b36e0d78e0577c61ffd4d3c3dbd`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 01 Oct 2021 01:18:45 GMT
ADD file:e18a9f741d10c7c0a74f1cb7527ca233ce7d1b16b4b8ce47c97acf8d6a561bc6 in / 
# Fri, 01 Oct 2021 01:18:47 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 02:22:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:23:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 02:26:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 02:33:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:834bf9f8a8e81cd7ddae19382f75e69f5f13259008681b25aa70aca6da903e07`  
		Last Modified: Fri, 01 Oct 2021 01:42:59 GMT  
		Size: 27.2 MB (27210170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70e1ff9e0960442ac8e0ed27318b8f50e84d12cbedd17b4f36bfa157115adc7`  
		Last Modified: Fri, 01 Oct 2021 02:59:17 GMT  
		Size: 3.5 MB (3490761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2050b829842e591df4469c3681081a8cf61654b45f11d26e6953e514d6869b93`  
		Last Modified: Fri, 01 Oct 2021 02:59:17 GMT  
		Size: 3.8 MB (3803189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c488cbe594d2cf170d43a86c8cde4efc13bd529cf61fd3b9acb9ff640aa8b617`  
		Last Modified: Fri, 01 Oct 2021 03:01:12 GMT  
		Size: 40.8 MB (40766562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72f040e257abcc701d46bbbbe741df280b9aad1f553176cb2cffa3942dcd9f8`  
		Last Modified: Fri, 01 Oct 2021 03:06:53 GMT  
		Size: 191.2 MB (191212371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:289c4e33490a29a0c4d1e91ff90ba687e49e4d9bfce3cffb5ac1bbcbf8eb91af
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **367.9 MB (367897006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e42552a4cc5f56b542c98c8f021e4f0397b5897c83e276e4edaa0e79d5471db`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 16 Oct 2021 00:42:02 GMT
ADD file:e3ac42c4b4650e7d57adf242fb9b7137898397121142c4fd47afb661024e0b00 in / 
# Sat, 16 Oct 2021 00:42:03 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 01:11:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:11:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 01:11:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 01:12:19 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7101024e2e65688584ff7a7aa5f503fe9e8165ebcc5fb924b1304bbdd0d4256e`  
		Last Modified: Sat, 16 Oct 2021 00:43:14 GMT  
		Size: 30.5 MB (30527974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c893f3d07db208a09670ca2a61f5af4e83488249bea3ec02f9de57eb0e6c1f`  
		Last Modified: Sat, 16 Oct 2021 01:15:57 GMT  
		Size: 3.8 MB (3771530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3328cbd7261ef1a0a50687cdd7d7c486ab672569fbd2f169f94fdb4d20618a`  
		Last Modified: Sat, 16 Oct 2021 01:15:57 GMT  
		Size: 4.0 MB (3962629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba43f37a0fd565fd1fbb24c6e2586d0d7a7bad8eda0d92d2407d12fa7ee680a`  
		Last Modified: Sat, 16 Oct 2021 01:16:10 GMT  
		Size: 38.3 MB (38324342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d6471533ad95df35c90efa28ac34a550430001d0c9a7c71ffb036ea4bfa034`  
		Last Modified: Sat, 16 Oct 2021 01:16:49 GMT  
		Size: 291.3 MB (291310531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
