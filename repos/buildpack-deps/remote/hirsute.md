## `buildpack-deps:hirsute`

```console
$ docker pull buildpack-deps@sha256:0763bfd59ca79835896bb02e6be807329761ba61f5cb9e6f3292f07d7f7242cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:hirsute` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:91e9acc792f026674dd45f446df640319265b7262c1005bde38528222773d568
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.9 MB (248920500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe66bef49b8843238f7319eab8d5305a356c059489e901289f25b7ea66d4e34c`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:54 GMT
ADD file:6ae44786caae9af1c6b70dc9cc244e7d4e06fffc0696f68877527d69aa3fc735 in / 
# Mon, 26 Jul 2021 21:21:54 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:54:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:55:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 26 Jul 2021 21:55:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:58:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4451f5c7eb7af74432585f5ebfbeb01bbfc87ec4a74dc93703bdd89330559cd1`  
		Last Modified: Mon, 26 Jul 2021 21:23:44 GMT  
		Size: 31.8 MB (31837572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0f50de6f11a7b6e208c43425014772ef0610d5f771979c6704e166be5c0499`  
		Last Modified: Mon, 26 Jul 2021 22:13:33 GMT  
		Size: 5.4 MB (5431174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bfd280fb76c1b9717ecd762750a8e603d628c6cffebe143f0b34966a47bae5`  
		Last Modified: Mon, 26 Jul 2021 22:13:32 GMT  
		Size: 3.7 MB (3661446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde9939f009cb8ebf9ee9b4f6b6f99c0a7ca437c96b046a6345f065cbfcc3dde`  
		Last Modified: Mon, 26 Jul 2021 22:13:53 GMT  
		Size: 43.5 MB (43540366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111c706438d96ec9682736266bade1a4ac6bc3b0a5c98d469c32eddc94a5acbc`  
		Last Modified: Mon, 26 Jul 2021 22:14:30 GMT  
		Size: 164.4 MB (164449942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:786b965a9d6a8aa7384f2db07ae95fa6fb61ce55efe86186d39ffca8a2ed1056
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.9 MB (208923584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f552a257abc3da22a3250ecfc6d93dec61196503231879dba0c59f3b55dea58b`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 22:52:32 GMT
ADD file:76353e48968f6c84802b150e577cc7fb1bc50985e78e1b499ecd8debfe50d8e5 in / 
# Mon, 26 Jul 2021 22:52:33 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:25:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:25:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 01:26:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 01:28:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:681a32f1cee4135c0497939e80766271e03a995a197d8293224e8f6bd470bfdd`  
		Last Modified: Mon, 26 Jul 2021 22:57:17 GMT  
		Size: 26.9 MB (26857313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b181d081ccdbe67f74ab6dab322dc6e8e84a9b56cb1909518f7d199a8fc8936d`  
		Last Modified: Tue, 27 Jul 2021 01:47:35 GMT  
		Size: 4.9 MB (4858897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9fb191db7ef79ad38fdcde76e18b9267b765696ecf8c500929ef80b649f800`  
		Last Modified: Tue, 27 Jul 2021 01:47:34 GMT  
		Size: 3.1 MB (3138386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b923df82160d2d4eea0012b206b82fae9ca16efd703aacc1069a7bb396b558`  
		Last Modified: Tue, 27 Jul 2021 01:48:15 GMT  
		Size: 40.0 MB (39956131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81972472b3986b3a6bbc0402e59a3d8f113ad7e7069d8918c442e57619255ef6`  
		Last Modified: Tue, 27 Jul 2021 01:49:48 GMT  
		Size: 134.1 MB (134112857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:7e5f6e0a00dda48a76aa17bdd9632efad49c2d5e958de1da097c4ba901fcab89
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.6 MB (239569400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd905178021460f6c7f78fa90eceb02ac097094f0e7b4fa0619328671c28a7f2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:40:53 GMT
ADD file:93dcfc1791d96861438a84bfd38f5c0520353febfcc59bde5510c9e85eab2cf8 in / 
# Tue, 31 Aug 2021 01:40:54 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:11:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:11:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:12:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:13:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4fbd1b15195364f20d4b603e346a2b5c64ae93e9de90f5c1bd82a61e92851632`  
		Last Modified: Tue, 31 Aug 2021 01:42:57 GMT  
		Size: 30.2 MB (30162874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d54fbc3de08027791a7280c6d2d7f821165cc126fd0e08c6cba66c1d6fc122`  
		Last Modified: Tue, 31 Aug 2021 02:20:51 GMT  
		Size: 5.4 MB (5401544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f7180cc8ab79571bbc48658748543060674d12cbbdf7683a598d89f6086677`  
		Last Modified: Tue, 31 Aug 2021 02:20:50 GMT  
		Size: 3.6 MB (3638240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826a66d619e21f0b3656bcd20cb8925d105fc0e444b4a72eb69d81408ecf67ed`  
		Last Modified: Tue, 31 Aug 2021 02:21:10 GMT  
		Size: 43.5 MB (43525534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0590f0535def702f02a4c077e4c3fe732c276f278986df7dc19c8a7c463603`  
		Last Modified: Tue, 31 Aug 2021 02:21:45 GMT  
		Size: 156.8 MB (156841208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:e912d8844618c3e84df88afdb02d2fcc5ed1713afcb23c067a3e0d469ab40951
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.2 MB (268194289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6428d43eec21252ab8aa929510a3955ba8fa3a1e59f0f8d49cbf487fc2abf9cd`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:13:18 GMT
ADD file:42c46f2fd1479c7d309139946c738ffe5c5379a9561b96a8d7511bdb0090481e in / 
# Mon, 26 Jul 2021 23:13:21 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 03:35:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 03:36:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 03:38:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 03:47:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:50f10986101895abb3160c75977e8e8eb7b79e82f78fa9dd1883692b644e4675`  
		Last Modified: Mon, 26 Jul 2021 23:16:36 GMT  
		Size: 37.4 MB (37352998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae72f19678043711c11465b507df75ce318af4bd2b392f685ca3841dbba055aa`  
		Last Modified: Tue, 27 Jul 2021 04:26:44 GMT  
		Size: 6.1 MB (6133314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a982650c2954b338afda90c5ba86d7603861d62a22b2e3800362985c59823f`  
		Last Modified: Tue, 27 Jul 2021 04:26:43 GMT  
		Size: 4.5 MB (4523551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a4da86ef0de66c418b38e81b81a9690c0e7b660053a2b63e8a7b090c8ffdd23`  
		Last Modified: Tue, 27 Jul 2021 04:27:06 GMT  
		Size: 49.5 MB (49482660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df05ea742cc84cf005f5b1fbce3aa2099c7974bbd0654675d0c0ff8c7dbab40f`  
		Last Modified: Tue, 27 Jul 2021 04:27:48 GMT  
		Size: 170.7 MB (170701766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:ac52edf6a4ea4ab1f8ee0096caf69ad869cac3a58b760bee7eb927b04a48d6a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.9 MB (257914485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8b02dfe5db83585a676ecaa8de2d87d02ca0e88a0eb635baf0a58f8a5a54119`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:17:33 GMT
ADD file:c9125fcbdad41a027e81c7fc0616e4698eefb4bf591e9c215748c44001492a71 in / 
# Tue, 31 Aug 2021 01:17:35 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:03:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:04:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:07:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:13:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:de98d6361415ec89b2135480af53817e96bf60ae2c78c53dad37c447f0f7b040`  
		Last Modified: Tue, 31 Aug 2021 01:33:15 GMT  
		Size: 27.1 MB (27143365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225134e3c31562a8c1d476ee61f8672ab2a39bc9f6dd1aa9d2334027bacf22c0`  
		Last Modified: Tue, 31 Aug 2021 02:44:14 GMT  
		Size: 4.9 MB (4945167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55ca77fa5925540bdc2a4cf61c8acfdf7fc0d169793ae57fd6e0b7a6465022d`  
		Last Modified: Tue, 31 Aug 2021 02:44:11 GMT  
		Size: 3.2 MB (3177763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98a854c5e99476d386d6334136c9b5839b261270f40552a56a5557336599fcd`  
		Last Modified: Tue, 31 Aug 2021 02:46:12 GMT  
		Size: 40.3 MB (40329103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c567f920ef8255eb4f50d24bf8b4329ffc4253128705dc547c32723ea2c15bec`  
		Last Modified: Tue, 31 Aug 2021 02:51:50 GMT  
		Size: 182.3 MB (182319087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:hirsute` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:16cbc9689a2459ec88062d9374e59c88dd2d38965300fa2f3d8afa87b6141c1c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.4 MB (241418909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b8f027f78486d0ae43707e9e3128407eb00ebf6a230cfd375abfca1a96e8690`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:38 GMT
ADD file:ba5c2c420b69d0c125e25122344e156fa468282be3e91af99f6941eb676f308d in / 
# Tue, 31 Aug 2021 01:42:41 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:37:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:37:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Aug 2021 02:38:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:39:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2e7ad6541ebda77ecfec574e1268bb944ba28f14ca69dab7bad1d63702975176`  
		Last Modified: Tue, 31 Aug 2021 01:44:29 GMT  
		Size: 32.5 MB (32491578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66e7ecd9588795e7cf09605e17fa940cd2b5566b310df2b484b60ba5faee036`  
		Last Modified: Tue, 31 Aug 2021 02:46:51 GMT  
		Size: 5.8 MB (5802191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36acc9b914fe8f7ad986a1869bcd54799c01524d5a43634c1cff6407f77d9a14`  
		Last Modified: Tue, 31 Aug 2021 02:46:51 GMT  
		Size: 4.2 MB (4185117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceeae36ed176d953e43f3ac748df4f3d272212947102e33987f59a8cecb55002`  
		Last Modified: Tue, 31 Aug 2021 02:47:06 GMT  
		Size: 47.4 MB (47400028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6beaf975b1e5ae8c6fbc46716b09e0482ee34d077a5e324a7cb39c58d7d7e096`  
		Last Modified: Tue, 31 Aug 2021 02:47:32 GMT  
		Size: 151.5 MB (151539995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
