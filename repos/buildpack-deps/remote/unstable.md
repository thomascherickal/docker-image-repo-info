## `buildpack-deps:unstable`

```console
$ docker pull buildpack-deps@sha256:dd99d7995b4908e577c5151fead90f5849e7a7385febdb97437240c3040b6474
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

### `buildpack-deps:unstable` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:9c3a9865a0eaca802969ddae636a9889fbd28ece6e5807eb5655efea4dc20873
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.9 MB (336890013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d95eae509306665ba4babf9dc330df9aee24de14269b45a8a66098a35f8b891`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 15:44:34 GMT
ADD file:7b4df5810238cdff80845df3de1b017b9646e41ae4981a0dc81447c9e63b2e43 in / 
# Tue, 04 Aug 2020 15:44:35 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 23:34:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 23:34:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 23:34:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 00:26:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:eb43504b07c3311fd407398c6de1b3b659cd4413087291e081d599040a320054`  
		Last Modified: Tue, 04 Aug 2020 15:51:13 GMT  
		Size: 52.4 MB (52403508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54da343b269771dbf23c5981583739bf4bd61a501a182b83e04658803eda3d19`  
		Last Modified: Tue, 04 Aug 2020 23:41:17 GMT  
		Size: 7.9 MB (7921868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fd0e91d8a06079fba129e4b4a489c0ebd206ec45a25cf7916c8b7ab789c48d7`  
		Last Modified: Tue, 04 Aug 2020 23:41:17 GMT  
		Size: 10.6 MB (10580741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0511f36f89e95042414306efb1e65ac63d57f7d5c4947f3de90f837e2fdbfc`  
		Last Modified: Tue, 04 Aug 2020 23:41:33 GMT  
		Size: 58.9 MB (58930036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed4cd24b6e3f2ca77ae8abd6e10436ed9c03273e6fb7c8d9f512d981811b0c3`  
		Last Modified: Tue, 01 Sep 2020 00:33:04 GMT  
		Size: 207.1 MB (207053860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:e9da338c0676adc6b8873130cd154aa9acbbd7ebd879dce17b4a7256b121fd47
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.1 MB (313098002 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75dbd2b5af6445005598c4a1397dc99e5c176d4461161539f6406beaaf06a9a5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:19:33 GMT
ADD file:966adedb56b8840e71e14255f1e10c11506897b861f32a0c8c84c32338edea04 in / 
# Tue, 04 Aug 2020 03:19:44 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 06:24:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 06:24:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 06:25:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 00:31:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70fc41871a830209ccc29805b1bb08b4058beb41df471ae13bc23555229a9623`  
		Last Modified: Tue, 04 Aug 2020 03:37:01 GMT  
		Size: 50.3 MB (50310118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c042826fa49924c4933b5f443c67da73885272c029983f30a8e5a154ae5b2ba7`  
		Last Modified: Tue, 04 Aug 2020 06:39:59 GMT  
		Size: 7.5 MB (7501462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:647f2d1c9e043d778892369b2ac4ba55c261e45346581518d8e9c0923f580979`  
		Last Modified: Tue, 04 Aug 2020 06:39:59 GMT  
		Size: 10.3 MB (10267096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1e363591d4c61017b4adf9fc9d4b3da3938064ff6fbb809e08a84bf5049cec`  
		Last Modified: Tue, 04 Aug 2020 06:40:32 GMT  
		Size: 56.3 MB (56302538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6517245410291733f18920d2ae1b1ca99a5504740a6a59db72ef3f719227ca5d`  
		Last Modified: Tue, 01 Sep 2020 00:40:53 GMT  
		Size: 188.7 MB (188716788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:3f99e2e10104678a51da2e2e6e890235e3ea8a73b0f8594e28ef61e2189ad9a8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.0 MB (298961222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e7df2111e904a5cf7b0e84003fa66bd5e5b4c04bc87ce94ae235644c97e74d5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 04:59:26 GMT
ADD file:5793438e4679788bcbcd7ff2adcfe8f0c31bb4ceca63088d7c74a20cac1e87b8 in / 
# Tue, 04 Aug 2020 04:59:32 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 08:08:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 08:09:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 08:10:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 00:24:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7ebc2f87ea858cf67ec5ea8f8fcd77fa8fefcd9b35b71d1b3efa355f8289ce59`  
		Last Modified: Tue, 04 Aug 2020 05:07:30 GMT  
		Size: 48.1 MB (48082910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e76657e19ac1e0b31daaf79a3e351dad82e57e1e9714d8bcb5ca885c77b1150d`  
		Last Modified: Tue, 04 Aug 2020 08:29:01 GMT  
		Size: 7.2 MB (7243562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:227bb50b47817c708c54d7d565ccfc1a6a7f89fdf3edf9cb85c81453f41011e2`  
		Last Modified: Tue, 04 Aug 2020 08:29:01 GMT  
		Size: 9.9 MB (9915847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f083ffc50f274a9b7bab4204c81cb5d08c3488fdec1a235c7acd3d6293a1702a`  
		Last Modified: Tue, 04 Aug 2020 08:29:29 GMT  
		Size: 53.9 MB (53874244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc0898ff03f73b908adb4e53cb91661d15186f3c7c54d302890743431001d74`  
		Last Modified: Tue, 01 Sep 2020 00:36:14 GMT  
		Size: 179.8 MB (179844659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm64 variant v8

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

### `buildpack-deps:unstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:9b17ec7c08f2630c0c0510cae61aff53b2dcd5219b5e54980c3f986366b100d8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.2 MB (346240325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4fb150369a8c95ec59f0576ef12693f3a3e673baafe417c4336736ffa046fd6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:39:04 GMT
ADD file:545a4c28d2d65f9f31d6deed3b22ae80dcdf0f0ba234b36acb715ebf6da67f3f in / 
# Tue, 04 Aug 2020 03:39:05 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 08:19:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 08:19:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 08:19:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Aug 2020 23:46:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5671e8963d62284adafd28133509ee2239373c96d0091ce2b4491327cac9724f`  
		Last Modified: Tue, 04 Aug 2020 03:44:13 GMT  
		Size: 53.5 MB (53490363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58173079354050a764e0b7ab86cb86890a027949b6c49f2f6e431042520f5793`  
		Last Modified: Tue, 04 Aug 2020 08:28:46 GMT  
		Size: 8.1 MB (8099063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5b5148c590d93c505260dbab5cecf462a0afd80a0aead458ebbc0ca4cbf438`  
		Last Modified: Tue, 04 Aug 2020 08:28:46 GMT  
		Size: 11.0 MB (10960412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0958f5cb4e332f3b1109c6672be060a7766e25652f77917b2bd99d249c2dc27e`  
		Last Modified: Tue, 04 Aug 2020 08:29:08 GMT  
		Size: 60.9 MB (60900835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3c3d6426d138c7d26564edba2b648e659a0f4d45a8969ff1c86f48cbff91aa8`  
		Last Modified: Mon, 31 Aug 2020 23:51:29 GMT  
		Size: 212.8 MB (212789652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; mips64le

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

### `buildpack-deps:unstable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:8bb262a5e00edb528b5e333a869914a4a227bc7bfd3f1f9915605c198a21930a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **353.4 MB (353368468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2af2775f2be9b589a82dc68eaddc42352fb9b71dfdefe24ff8338b2ec5f1fdf1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 04:45:56 GMT
ADD file:4f9206295fed0198f64e3e8588d30592afb355ad315b7f02a90d92274b37766a in / 
# Tue, 04 Aug 2020 04:46:03 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 07:25:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 07:26:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 07:28:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 01:08:48 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:54ff323e52b64530253b6d180607b58565d781a9b132031a9baec3e1577690ab`  
		Last Modified: Tue, 04 Aug 2020 04:53:50 GMT  
		Size: 56.2 MB (56196736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b6163322bc0beea20fbb00969be62fd8e2c8790b205e246ff0b8d2a3b72ed82`  
		Last Modified: Tue, 04 Aug 2020 07:46:38 GMT  
		Size: 8.3 MB (8347727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae8dbc9e7891e1d54106baaa34d375e35b66be62a672cd47f7d6388f7ed7797`  
		Last Modified: Tue, 04 Aug 2020 07:46:39 GMT  
		Size: 11.3 MB (11327086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123657860e3a0579d09f7f5f2bed55b40d18ab151ca05653ce1c874ea4be1b9a`  
		Last Modified: Tue, 04 Aug 2020 07:47:10 GMT  
		Size: 64.6 MB (64613910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6809a964c8553898cba72387207733f41637a2513d8acd09a0850125fb282c72`  
		Last Modified: Tue, 01 Sep 2020 01:15:22 GMT  
		Size: 212.9 MB (212883009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; s390x

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
