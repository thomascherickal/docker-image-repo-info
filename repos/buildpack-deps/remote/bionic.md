## `buildpack-deps:bionic`

```console
$ docker pull buildpack-deps@sha256:9ac27efda917198bf27efc5793d8149435ee00736bba49926fc8a654f5c356a3
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
$ docker pull buildpack-deps@sha256:e528083f16c11b7887692e4e3c95c3a6870518320b2f58540dd7bbe969c6d1b8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.4 MB (221392214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5aed41ef81bfee2777d4de5e91ad756fef93503d0700fc0dacc473d761971818`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 19:38:36 GMT
ADD file:8733c7e8faf03d53cb2143ff6ac405362944cfa07422fccd21a3066cc2f42c83 in / 
# Tue, 06 Sep 2022 19:38:37 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:56:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:56:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Sep 2022 19:56:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:59:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:726b8a513d66e3585eb57389171d97fcd348e4914a415891e1da135b85ffa6c3`  
		Last Modified: Fri, 02 Sep 2022 15:41:13 GMT  
		Size: 26.7 MB (26710833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7dbb4551b9c872b2053c38cdd5dd7e02c06107e648b950551a585e5e88394c7`  
		Last Modified: Tue, 06 Sep 2022 20:00:54 GMT  
		Size: 6.6 MB (6630965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79cc7a6dc37d1b46bb3edb182f0a133c77f677de31779964db5569d6137a99d`  
		Last Modified: Tue, 06 Sep 2022 20:00:54 GMT  
		Size: 3.0 MB (3023688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5b4b52eebf079a3d5e1a1decad6af97acccd018f5d50a4c0e9533a54a3cdbc`  
		Last Modified: Tue, 06 Sep 2022 20:01:11 GMT  
		Size: 45.5 MB (45498322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4c3ab92be332905d30314f7e4fc0775d75a34044a859f49564b40fe4e7cffc`  
		Last Modified: Tue, 06 Sep 2022 20:01:40 GMT  
		Size: 139.5 MB (139528406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:0fce3a21c1614e61a642bf5a439ac1770eb692c003e2ae3e08a76e619291b0d0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.6 MB (189556723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e2da3dee6e14720f0c8cb851fba01ac825f58712778a0f763864eeaa456d206`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 19:33:23 GMT
ADD file:45c82fca220161f3905a06e276f12ec0cb3be5c099cca70bb6d495da10088f7d in / 
# Tue, 06 Sep 2022 19:33:24 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:51:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:52:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Sep 2022 19:52:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:53:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:074d633b5bde02245e333b110dde5850e06ea4ebefe4283af6e4dfd8d462b170`  
		Last Modified: Tue, 06 Sep 2022 19:35:07 GMT  
		Size: 22.3 MB (22305954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:594729c31c2cb7f63b20f449c44c215064e068c94731174e4b57603ce032fd82`  
		Last Modified: Tue, 06 Sep 2022 19:57:06 GMT  
		Size: 5.7 MB (5698254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da759356c74e12ad90a263cb412b2ea0620a103ffedbdb492aac5586d59cdb83`  
		Last Modified: Tue, 06 Sep 2022 19:57:05 GMT  
		Size: 2.6 MB (2585972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31889323a628fc6a5d5b97236ff7b9500b05e2cafa958463ef4094646c8f3603`  
		Last Modified: Tue, 06 Sep 2022 19:57:25 GMT  
		Size: 40.7 MB (40691568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7cff271266119a86a51033715e0198a3b8755f84d2c5cca74c523f8225cc280`  
		Last Modified: Tue, 06 Sep 2022 19:57:53 GMT  
		Size: 118.3 MB (118274975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3ebaa3c12382c2516c8728bafd1ee97a069548dc91e3dc74d6867d591d5a17ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.5 MB (205513212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:931d6758b74219c522750ad62e920c8098f22702e137a5eed6754217c4556dd8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 18:49:02 GMT
ADD file:26cb5ace98a4462b36211bf28f1e73781dd6d8984350d9bd53243dbe50ae180c in / 
# Tue, 06 Sep 2022 18:49:02 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:12:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:12:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Sep 2022 19:13:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:13:59 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d30cf2a6a25aea48a115837d149468c8de7df7fb51f210b9fa1173c065f7b34c`  
		Last Modified: Tue, 06 Sep 2022 18:50:34 GMT  
		Size: 23.7 MB (23734076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79317661c5fe6a8a22ce652c9fb0999eb96ed08b735a16224e9a795c877780d`  
		Last Modified: Tue, 06 Sep 2022 19:16:57 GMT  
		Size: 6.1 MB (6072017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:737382e506f963b99b1453e20a2fcbb6bc4328a0c68bfc3530b2082a5f3da14f`  
		Last Modified: Tue, 06 Sep 2022 19:16:56 GMT  
		Size: 2.6 MB (2571091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160f71044c4c89d05d500625b4eda19add7227d613b991017a9850f2945440d2`  
		Last Modified: Tue, 06 Sep 2022 19:17:14 GMT  
		Size: 43.3 MB (43296151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ec4cd1624a82a57e6cd377e4126b4e69c04991aca1f9dd6b9380b4a351e588`  
		Last Modified: Tue, 06 Sep 2022 19:17:44 GMT  
		Size: 129.8 MB (129839877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; 386

```console
$ docker pull buildpack-deps@sha256:1e08f63aabe1e3e0539b94fb88d71d70045de1b2a09c1cb0678ae765d602281d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.2 MB (218228400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:523091bbe3ef5b646de02652ba174944425c430cba9e8d570d61d6936e640f7c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 18:40:06 GMT
ADD file:31701667cc90b9f4ce7d6ede94bf7dae4d63c49e62d3725094d547f9601e1165 in / 
# Tue, 06 Sep 2022 18:40:07 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:02:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:02:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Sep 2022 19:02:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:04:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:10d3032d1995d3163c20a7f2f197299fae258c2ad020a8fd586fd6b7dd1b0e1d`  
		Last Modified: Tue, 06 Sep 2022 18:40:53 GMT  
		Size: 27.2 MB (27164710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360b65e679bf1db70d92b45a6d39c882e074d441412548705adf35d49a12c70a`  
		Last Modified: Tue, 06 Sep 2022 19:06:33 GMT  
		Size: 6.9 MB (6919740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8820513ab0577fe6133989b66cdc2a5a0b1a97af5280746721af55657c0897d7`  
		Last Modified: Tue, 06 Sep 2022 19:06:32 GMT  
		Size: 3.0 MB (3039943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ad90e9fc8930485dc12eedaf8101fe62b983d943986b7325ff502b9d424d75`  
		Last Modified: Tue, 06 Sep 2022 19:06:52 GMT  
		Size: 47.1 MB (47083595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bdffbbc9ce11b7acde16175dcc810b3cd9c5e5f850cac91cfcd033e2c2bcf9`  
		Last Modified: Tue, 06 Sep 2022 19:07:20 GMT  
		Size: 134.0 MB (134020412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:ac71ffe284d77165ccbfe8e4f10276653fde3026f002fc1e2a5557fba36cdfe1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.4 MB (246400050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddcce9c6043a6417a17152dbbefebdc2086e1240454861f17bfdd701a73c7c6f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 19:38:57 GMT
ADD file:1b76d0a41921afefb92711c44ceb312c16828d433b689a951d65c238faa9ac50 in / 
# Tue, 06 Sep 2022 19:38:59 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 20:06:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 20:06:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Sep 2022 20:07:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 20:09:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4abf8f40556a940861bc7fc313acefb89c775273ed06b7d41cfb222ccf8a1438`  
		Last Modified: Tue, 06 Sep 2022 19:40:56 GMT  
		Size: 30.4 MB (30441623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7afd3028934ff054bca1d0bb218e690d2cdb60f7754ad3bb6426c3744e730f`  
		Last Modified: Tue, 06 Sep 2022 20:12:44 GMT  
		Size: 7.1 MB (7050146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33850c25587eb4418b5e6aeccf1c9e6fa5b0baac624020bc56b4d4db8c2742c5`  
		Last Modified: Tue, 06 Sep 2022 20:12:43 GMT  
		Size: 3.7 MB (3720231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677c4d750793a0cab4cd23689261d167383d4e03f7fce03417017fcfd5497d21`  
		Last Modified: Tue, 06 Sep 2022 20:13:12 GMT  
		Size: 53.7 MB (53744408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2548f24520c161a34a9b39bc85562ec79da91528e4742bfafd4dc333ae3b0489`  
		Last Modified: Tue, 06 Sep 2022 20:14:01 GMT  
		Size: 151.4 MB (151443642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:00d5ff189772c956744ca48d4cb80e449ce51e844a304eb5336ed8ff5a1c96d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.7 MB (205748449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d78f4436f2d6ebf559f756716d8782d1472e28502b39ffdd40c045b74f4ea2f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Sep 2022 18:43:36 GMT
ADD file:dbe2a8e3943129e654ee29c636cab2bb10dd7eb0ac27d51e6954af2ccbe22807 in / 
# Tue, 06 Sep 2022 18:43:37 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 19:11:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:11:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Sep 2022 19:12:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 06 Sep 2022 19:13:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be6761156800c616810cb8aeb5b3ae71b9a2082f1c1221210befe119f082e879`  
		Last Modified: Tue, 06 Sep 2022 18:45:00 GMT  
		Size: 25.4 MB (25370130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae409e724954611ea7731639a0dab7c4c59fdb64deb51dba5327bc8c5a085c5f`  
		Last Modified: Tue, 06 Sep 2022 19:17:11 GMT  
		Size: 6.3 MB (6324234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aca3edc7c631417c9e3dbbcb30698aed6531dc2482e10dd41ee221de2d450ca5`  
		Last Modified: Tue, 06 Sep 2022 19:17:11 GMT  
		Size: 3.0 MB (2977166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee7b8f6dba5690621ef3c6a174a056a9b68be9f2c37eeb155bc990d0284bcf0`  
		Last Modified: Tue, 06 Sep 2022 19:17:26 GMT  
		Size: 45.0 MB (45043901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:654a99a01d5150ba8cc8996260cf51a2b5c4a95e746908bcf7f69f1a719549ac`  
		Last Modified: Tue, 06 Sep 2022 19:17:50 GMT  
		Size: 126.0 MB (126033018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
