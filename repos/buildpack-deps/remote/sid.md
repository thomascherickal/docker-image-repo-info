## `buildpack-deps:sid`

```console
$ docker pull buildpack-deps@sha256:c7c9993bab4cef62c53c1d969b713cd603aadcd5eec65e391ca4f6072b64689f
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

### `buildpack-deps:sid` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:5bd6ee6e0a24f8ebdca210719df40a3862bb7bbcda99c914ac927f79e32b4392
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **393.2 MB (393208481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f8a39e4cda8e50c9e1dbe7d792e4ac22070c57584931cdca0dd5e5fdde56da5`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:22:27 GMT
ADD file:bd8ad5ff1bfae3fed182d348486f9719820be43c8b6b13ad4385f6cc6a15ce87 in / 
# Thu, 07 Sep 2023 00:22:28 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 03:00:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:01:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 03:02:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6c36f0cb17f99a82a25600b41f67d97eba8474b1cc58f325f0d1307303171b68`  
		Last Modified: Thu, 07 Sep 2023 00:28:36 GMT  
		Size: 49.5 MB (49492324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706b764f7b6e030a499bf8ef09bc0ce09547c7bcbd95b0454538450c65a9adb1`  
		Last Modified: Thu, 07 Sep 2023 03:07:53 GMT  
		Size: 25.0 MB (25003720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0383dddb5ef2d2b7f853291557ef1e8af6166b53bfd59d8bfd946cbe3d236bb`  
		Last Modified: Thu, 07 Sep 2023 03:08:11 GMT  
		Size: 64.7 MB (64676113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1977c69eafea9ef2c08c786e1b68e9f402c4057c72607d76141e5335a10b8de7`  
		Last Modified: Thu, 07 Sep 2023 03:08:50 GMT  
		Size: 254.0 MB (254036324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:842bc94d439dcd23e0f35e0ec6c73ee18b5dadc47b86ada629cb6701f13d0aee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.6 MB (362576307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e89732fa37d6bff0477ed251dd82dc5c68f6e869eacb5543c59c42d0ff0b3168`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:49:09 GMT
ADD file:65d133984adb1710a633ac35df6dab81e453734fdf5cabf6936e9a60011fc410 in / 
# Thu, 07 Sep 2023 00:49:10 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:19:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 06:20:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 06:22:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:501694e1228126374bf3e18e7ce91920d16f560440d860976cd128b459e62654`  
		Last Modified: Thu, 07 Sep 2023 00:53:15 GMT  
		Size: 47.2 MB (47191094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf1e8fde0a23e63f1853d8dcb4c7a8585aa8b9c8391f01712b567ce1ea29f44`  
		Last Modified: Thu, 07 Sep 2023 06:26:59 GMT  
		Size: 23.6 MB (23645705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318d821d91da4851762eafb4cc38bfc7d350acc025b7a6e1000c9b77ff93d8e0`  
		Last Modified: Thu, 07 Sep 2023 06:27:19 GMT  
		Size: 62.3 MB (62274982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbaa74b712fda7389e53823f4ce6f40f81ca2289c3605611dce90efde0e78327`  
		Last Modified: Thu, 07 Sep 2023 06:28:00 GMT  
		Size: 229.5 MB (229464526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:525bf95e230eeb47123196c7f9724013efab2c5af512f889132b32815b8d9b2e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.8 MB (343769402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25e62edce6be3ec20b38c0e21137a5bc016907aa9010f035dc4ef20c2cbe161c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:59:28 GMT
ADD file:48b9003b5f16cca577ade266eaa0f16a82c1470540f591ca5b3478846402f252 in / 
# Thu, 07 Sep 2023 00:59:28 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:39:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:40:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:41:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d85f55a7a6c774695f75c1a7ec0bc0caeb915349d9250d2f4e6737e12fcc92fc`  
		Last Modified: Thu, 07 Sep 2023 01:05:21 GMT  
		Size: 45.0 MB (44983245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b914bb1a1428c8af17f4b5fe2002cd56706f2764ffe325bc5a8693a2d5885cd`  
		Last Modified: Thu, 07 Sep 2023 01:48:19 GMT  
		Size: 22.9 MB (22863094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39cce762d527587259cc24735a7095b0706f16c46d1015868fffe9995eb694b6`  
		Last Modified: Thu, 07 Sep 2023 01:48:38 GMT  
		Size: 59.9 MB (59887601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1ff0f182ec867b8b013cf5e11054554a02f8de6c932f6556378cb6b8c44afa`  
		Last Modified: Thu, 07 Sep 2023 01:49:14 GMT  
		Size: 216.0 MB (216035462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:b387b1fd19a2f662585f16bd18586f3a0100d74dfd341da5d98c43aedb56f942
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **384.1 MB (384064102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca178a5ee94eb78894ba6e716be5f6cca66fdbc2444a12cdb158c9538ac8b9a2`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:41 GMT
ADD file:3fad0766985d4815384b52dbb02c3f23c3f0c6e9b05ae96cdb2f60692ebe3c47 in / 
# Thu, 07 Sep 2023 00:40:42 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 06:55:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 06:55:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 06:56:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:352986db96f4040761867c771dd7419bd03916c5a2f552680219ad48902eec34`  
		Last Modified: Thu, 07 Sep 2023 00:45:36 GMT  
		Size: 49.4 MB (49413074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a48ca0dfa7863c95cd7f5922e7ec0194090cd24c969b9936d768cd01354881a4`  
		Last Modified: Thu, 07 Sep 2023 07:01:59 GMT  
		Size: 24.5 MB (24531894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee8b08339dcbbaf894091d82da68954334103340d1d2952574feaeff7a2ffd4a`  
		Last Modified: Thu, 07 Sep 2023 07:02:16 GMT  
		Size: 64.7 MB (64650030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ca8caabac9147a02c589cab964eb49a8b3255f251123caa510d8f250c4e6cf`  
		Last Modified: Thu, 07 Sep 2023 07:02:48 GMT  
		Size: 245.5 MB (245469104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; 386

```console
$ docker pull buildpack-deps@sha256:790d032ce26d7fa9f74f42872855f6d1749c588cb66147e7f6b8eda92524644b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **398.9 MB (398894892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:319d04ebf1e81162e44851efe7c955cf095c1acd3a7cb0f437a2dfcaa57b9853`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:40:40 GMT
ADD file:ff611322e6674f9fde9d60d146cd9f1206176a7ad0bffa135200bb5ce18ef6fb in / 
# Thu, 07 Sep 2023 00:40:41 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 05:32:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 05:33:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 05:34:48 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e341a6bda5bb8b3c55cc00b75f2a70088193c4ac06611dc91b32f6ca7c58df58`  
		Last Modified: Thu, 07 Sep 2023 00:47:07 GMT  
		Size: 50.5 MB (50501474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199c1deb7fa20bc9fa5f1c71efb48e77dbb9169e65a80ee76e1af76eb11ef7bb`  
		Last Modified: Thu, 07 Sep 2023 05:41:15 GMT  
		Size: 25.9 MB (25854651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41bdb07681e939562c846b9666284e56c74395ac42f0c90225a11e7174a6a41e`  
		Last Modified: Thu, 07 Sep 2023 05:41:38 GMT  
		Size: 66.5 MB (66485654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e5705124676d0db75afec641f15936fe277fb8422fee742d014d7f49bfa737`  
		Last Modified: Thu, 07 Sep 2023 05:42:33 GMT  
		Size: 256.1 MB (256053113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:a77d6c2fa92a2c0fa1a642be1ef111baf6ace13f4432da0633bbefe3293b65c1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **371.6 MB (371613137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11f3499b2e9a3e7a54b44bcc97b35ccf50ce350b7d1069942a7cd10a779c1829`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 01:12:16 GMT
ADD file:a0f62fb4629026abfbc8955434580788fb6798315ec2cbb9fff3b490cae4ae5f in / 
# Thu, 07 Sep 2023 01:12:22 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 04:01:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 04:03:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 04:10:17 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fbf3aa413814601f6b34fe509eeee19b8570d10547318d9e50b786a1305da8f5`  
		Last Modified: Thu, 07 Sep 2023 01:23:38 GMT  
		Size: 49.3 MB (49337937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c57139e98311e15a5beb5188d286eb35893fd7b66379668ca38afc3c3926810`  
		Last Modified: Thu, 07 Sep 2023 04:26:24 GMT  
		Size: 24.6 MB (24560622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfe5e62077ec632bacdfa13759bc11189801d913e3ad23d63f1a3c430854c2b`  
		Last Modified: Thu, 07 Sep 2023 04:27:16 GMT  
		Size: 63.6 MB (63613201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d42f260a00a794f4603d66d1aaaf987c17cd8f6257dea59ce1c533e0dd7614e6`  
		Last Modified: Thu, 07 Sep 2023 04:29:49 GMT  
		Size: 234.1 MB (234101377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:3ef564eae232269e9b8cdb85ca989ed7364d8f9fa147d61f18250fae882b9c4c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **405.7 MB (405715664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f01f8af7b56455a36abd14cbb31e20d1bc7cd3853d02cbee247ef464866750e7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:19:03 GMT
ADD file:0a03052b027b835521a56eb544f68d37afd082caf6b0f2a86d36ba3a4df23574 in / 
# Thu, 07 Sep 2023 00:19:07 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 09:32:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 09:33:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 09:37:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:61513ad4f292fbcfceaab5e01ed63b82ba881a99736b2ffd97579f96947c0829`  
		Last Modified: Thu, 07 Sep 2023 00:25:38 GMT  
		Size: 53.4 MB (53429824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af30e0c1afcc76f65c4a2143f30e1403d1ff2bff1ecc5e0fee30d5f20906d81b`  
		Last Modified: Thu, 07 Sep 2023 09:46:15 GMT  
		Size: 26.7 MB (26685074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40404ef47fcfffb836201c5b1dd0e820e464c6b2a6a7467a3d61e3b2beb302d8`  
		Last Modified: Thu, 07 Sep 2023 09:46:43 GMT  
		Size: 70.1 MB (70133231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00735a792dece50d37c617ab19442746b45a20f4addf4058670069e8e6d3889`  
		Last Modified: Thu, 07 Sep 2023 09:47:50 GMT  
		Size: 255.5 MB (255467535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:0150bb87b97db7106a8883b1971dae5b87fbd5391ec9118cf15f6932d83b0f8d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **584.9 MB (584935368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77126be424a00a29f764cd8e7f8da503eebb4c14608d89dd3edd5a2278ccba0d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:09:51 GMT
ADD file:fdcff160dcad587bb28b0cba721c24193be4ab5de90a2d503cba3d329b78797b in / 
# Thu, 27 Jul 2023 23:09:54 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:32:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jul 2023 23:35:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 27 Jul 2023 23:45:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f8b93f818da821e670e126126d6da395bdf2888315b8baa1a6912378c2f4e02c`  
		Last Modified: Thu, 27 Jul 2023 23:12:55 GMT  
		Size: 45.7 MB (45656956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdc8d46a9f89f9d06db33ee07cddd8aa1a54e242cd6463179064bb8e0711848`  
		Last Modified: Thu, 27 Jul 2023 23:45:49 GMT  
		Size: 23.4 MB (23350890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a627ecd6eb80659b2ec0c3464124a436336a8496c101d36a4e46180fdb32a2`  
		Last Modified: Thu, 27 Jul 2023 23:47:12 GMT  
		Size: 60.4 MB (60386385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d8d3e46d641c1277be46ab521cccf04aeac468f053836ff4e0626b3a862cb7d`  
		Last Modified: Thu, 27 Jul 2023 23:57:35 GMT  
		Size: 455.5 MB (455541137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:e895e750e326e8586e14c679ce855b30977543286cabb2a1faf0c3d351ab820f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **365.0 MB (365046205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00b9498ab42633f099c424e23d398bcfcec3d909429f641d0f82fe5395e8b29c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:45:36 GMT
ADD file:bd3fde5e3038704806827aa08d23e09a06b39ae915868b757132819f9c65e50e in / 
# Thu, 07 Sep 2023 00:45:43 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:13:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:14:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:15:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ee0f0030591cd1c61bb2bb7366cf7acef7874305f79e676bf8fcb8d10698613c`  
		Last Modified: Thu, 07 Sep 2023 00:50:52 GMT  
		Size: 48.7 MB (48730438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e552f7737ff7ce568b8ed95d29640fc89a141d02eb8ae1ff41a15b8e8305a3b`  
		Last Modified: Thu, 07 Sep 2023 01:23:57 GMT  
		Size: 25.3 MB (25267434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5438a4ee4569f4cfcd590fac3b9d0967f9e05e28ee9229c56cff8f039d32de`  
		Last Modified: Thu, 07 Sep 2023 01:24:13 GMT  
		Size: 64.3 MB (64277143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b13d80e18060b1f76d7d53f77baed863066e16d6d0813e78edf0c0ede273e6`  
		Last Modified: Thu, 07 Sep 2023 01:24:47 GMT  
		Size: 226.8 MB (226771190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
