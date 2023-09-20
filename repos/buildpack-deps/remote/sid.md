## `buildpack-deps:sid`

```console
$ docker pull buildpack-deps@sha256:62df8299455902395d1af737ec3eec65d40c20305fed95b04e2b6a258df768c0
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
$ docker pull buildpack-deps@sha256:996010cc001e51825acb2b265c7ac7d964ba92c984bf4b348638b6d3ff86a096
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **374.9 MB (374936161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:800ac6808232cd7cb3edfd542e208f50a580fab05a28f65ac42f7548bebe996e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 04:57:17 GMT
ADD file:bc0b5b71ee53adf6297821668404ace4f79c4256461b99497849721dbd8e86ae in / 
# Wed, 20 Sep 2023 04:57:18 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:25:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:26:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:27:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d036181e87bed9eb2432498f0ccbf7baa06719a2d8360c3bc9c496bd9f853a7c`  
		Last Modified: Wed, 20 Sep 2023 05:03:10 GMT  
		Size: 49.5 MB (49482728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a1e6c60efbe0c0012665a19f7b4b47dbdad105e96128f40794e9aa23e0da2c`  
		Last Modified: Wed, 20 Sep 2023 09:33:06 GMT  
		Size: 24.3 MB (24333156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28922a0c46a328800d30ba9ed43a2347d3d2859f84e5f14eb9a375ca7a20e3bb`  
		Last Modified: Wed, 20 Sep 2023 09:33:23 GMT  
		Size: 64.7 MB (64694699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c606031c2ccc331b560972a847afa50740100483f8d48472dc718f9ed3d99dc1`  
		Last Modified: Wed, 20 Sep 2023 09:34:00 GMT  
		Size: 236.4 MB (236425578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:9fa0ad460d7d90afdc44e040ac09770bf8375ee5af8938909e2a7e62db044a23
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.3 MB (344293353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:144eea0a10e2580078922cef01fb34d4248bcc8930f986d8b7203aa3c2e411da`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 00:51:01 GMT
ADD file:4c775ca1c9a8c87b9e1d380ae08f73f13d6c554601a5b87aef7f73b399316a50 in / 
# Wed, 20 Sep 2023 00:51:02 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:59:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 10:00:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 10:02:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:af64b4d6568f99d4aba6c0cd1799711a18174e7c92ab564f1783b1b859742070`  
		Last Modified: Wed, 20 Sep 2023 00:56:46 GMT  
		Size: 47.2 MB (47165885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a6ad399a5730010d73ad40e178b7766f2f23d621da8fcbfeaa0d9b45877a92`  
		Last Modified: Wed, 20 Sep 2023 10:07:36 GMT  
		Size: 23.0 MB (22966714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d774b6481cfa6a90dbdb4c1195266ca5258843ac16be4271bc6b26b545c6a023`  
		Last Modified: Wed, 20 Sep 2023 10:07:58 GMT  
		Size: 62.4 MB (62412206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd0865ebb7693f94985b2d2945f01b383d5fdb15de2902c64e865216c731ad6`  
		Last Modified: Wed, 20 Sep 2023 10:08:38 GMT  
		Size: 211.7 MB (211748548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:6469b7469fa7ea2e01640994e6a4ac52e95d28d450200f3909775dc426442732
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.5 MB (325528553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f07967692c9e6e5a9532b51f834f9de682e86c49b077d193b7e9af3bd7776f2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 04:58:39 GMT
ADD file:bcf56497ef1c60145d8d33d6611db5afce8122c3b654e448011714e12ab569e2 in / 
# Wed, 20 Sep 2023 04:58:39 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 15:30:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 15:30:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 15:32:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d3df769ad992dc9a8483f18e8dddf99140307545a5d1930bf5937f68b3c1589`  
		Last Modified: Wed, 20 Sep 2023 05:04:05 GMT  
		Size: 45.0 MB (44956764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d705d8b764c841b69aecadbfac5375ae37ed8e88fc3d6fc44d1d1cf476578a50`  
		Last Modified: Wed, 20 Sep 2023 15:38:27 GMT  
		Size: 22.2 MB (22190999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b72d13bc4a97358a6693133378961b04032ee4e87b23fade95386ab3231e5dd0`  
		Last Modified: Wed, 20 Sep 2023 15:38:45 GMT  
		Size: 60.0 MB (60033958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96065202e8d18c615a35a3f8fdf01822b6fcfb46a3f90d70113a4142fff7640e`  
		Last Modified: Wed, 20 Sep 2023 15:39:22 GMT  
		Size: 198.3 MB (198346832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:9998858ca64d290b9f9f5fb1e92fab84933c1212424031f02d564c8d72a3324e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **366.0 MB (366029961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1619f9ec19750248503f889545f9e7a9d5afe7818a26975e9c3e2004fc1a30e3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 02:45:16 GMT
ADD file:3493f4ad2710629ee9ad4c981682b2afcc1d9964cb5034de77189556f0c0e810 in / 
# Wed, 20 Sep 2023 02:45:17 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:28:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:28:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:29:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d83e3b52cf7f7a250777a05d8d2d7960fd6dba8a6438beed3879ff3c389bb01b`  
		Last Modified: Wed, 20 Sep 2023 02:50:04 GMT  
		Size: 49.5 MB (49450488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3c1d25120e8f2e9e343e08182a50d4c8702fe0c41bd340742c6b29f86d2bd7`  
		Last Modified: Wed, 20 Sep 2023 09:34:51 GMT  
		Size: 23.9 MB (23885219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de9a4b96724b03d813d1d7221957e9975fae576e911ef75a702924957cd7ef59`  
		Last Modified: Wed, 20 Sep 2023 09:35:07 GMT  
		Size: 64.8 MB (64833249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62e35813b56db50b9682f6107a6bb2e31a0e3a04f015477c9b0dd4e4d4eed09b`  
		Last Modified: Wed, 20 Sep 2023 09:35:37 GMT  
		Size: 227.9 MB (227861005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; 386

```console
$ docker pull buildpack-deps@sha256:2478b7a0fb85abe26894953263cac492886a848e294edb45ac05286213e7bd4e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **380.5 MB (380549415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7058feae282aebd4417c9bb8007624b6063c381005138d458214666b5a4f6a7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 00:43:36 GMT
ADD file:89a1cfdf26e23095cc168a8c054aaa8afe0cb7f1b748f0dbca755e9aad935ce8 in / 
# Wed, 20 Sep 2023 00:43:37 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 11:31:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 11:32:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 11:34:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a77a25e288eca9c35f0aeada81ba65e2f4beb3d0b739a139eb41bdd87309a97b`  
		Last Modified: Wed, 20 Sep 2023 00:50:06 GMT  
		Size: 50.5 MB (50483129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f9d0828fee9f05991f2163329e3ca3eedfe9d48281cece36f1e558396ef057`  
		Last Modified: Wed, 20 Sep 2023 11:41:02 GMT  
		Size: 25.2 MB (25160739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b802bd7b1ded8bd6d43b0b0a6249842e2b4aa05bbbb74de605231953d5ed682f`  
		Last Modified: Wed, 20 Sep 2023 11:41:26 GMT  
		Size: 66.5 MB (66509608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060110af2fbbfaff90f7fd838fe6351e5b1d88e09b9c7cd95388d2938268bca0`  
		Last Modified: Wed, 20 Sep 2023 11:42:22 GMT  
		Size: 238.4 MB (238395939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:e32da8582ebda8c1044c89d09cb5dd00aa5d5e9e2731f6240f9bf267246a752b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **352.8 MB (352828117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0313d31e66e417288d80962f65486d474d036ed259beda21b51ffdaa21363ac0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 03:13:05 GMT
ADD file:d3d484dbfd0f0dc6ecff269124b80444453666776b40afc16452523a3cc9dd00 in / 
# Wed, 20 Sep 2023 03:13:11 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 22:02:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 22:04:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 22:10:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3d916b18191c13bb0519a1e7808ab4f18b1becaa8745ab10fbd22162e95dd7c8`  
		Last Modified: Wed, 20 Sep 2023 03:24:25 GMT  
		Size: 49.3 MB (49295906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37dac64b63353ff1a16ae4fc5513c18b3d2c448042a7486b231cf5bf73a658b`  
		Last Modified: Wed, 20 Sep 2023 22:27:05 GMT  
		Size: 23.9 MB (23888740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e0025b063efa676d7e72e9f70b2c32a9cd37e5731a20d54ac90a7b8671d602`  
		Last Modified: Wed, 20 Sep 2023 22:27:57 GMT  
		Size: 63.8 MB (63772353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea5544b9b9753e1446b8a7e54b2143e1cc3759c863c00be94245e1bfbaa3478`  
		Last Modified: Wed, 20 Sep 2023 22:30:21 GMT  
		Size: 215.9 MB (215871118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:b97da0c563bdf286c776324ce007ef56ca5a587c0c147cc8ed3e540dd12b1a5c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **387.5 MB (387532229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2986aee4bded1765a1b68fd813dcb0b38c27376797fdcd4b96428709c2c2ac6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 07:54:20 GMT
ADD file:cdb28efb46a4441fb0c394ab6cc1dc2932b94e5af87d436319c9c1f7be36c739 in / 
# Wed, 20 Sep 2023 07:54:23 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 10:00:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 10:01:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 10:08:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fe32f2ba77f5d8b224f7db94357a292203e69ae2f9a815b5aecb41517006d3ab`  
		Last Modified: Wed, 20 Sep 2023 08:51:55 GMT  
		Size: 53.4 MB (53397269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:371cfd6d9bde7f492d0557b8056722af99aeec7719a46f7523e196af4a49e416`  
		Last Modified: Wed, 20 Sep 2023 10:23:48 GMT  
		Size: 26.0 MB (25976696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52d4b968457b19c383bfe9ecb0826c6b5224b515e8f8b8632474ee77c61b2454`  
		Last Modified: Wed, 20 Sep 2023 10:24:14 GMT  
		Size: 70.3 MB (70311387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673bb1f3d867961bf411a5844d2bf7811e32d3b29532612d966d0cd2415954a0`  
		Last Modified: Wed, 20 Sep 2023 10:25:18 GMT  
		Size: 237.8 MB (237846877 bytes)  
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
$ docker pull buildpack-deps@sha256:7b527f8e22a2a2ea04126b0b20f9434b2c93cb53c43051559d6a4c2f125392bc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **347.1 MB (347109478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c9027782a40cf42c298be85c617c0cd33762e893d81af95edebf7033a2cad11`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 02:55:43 GMT
ADD file:aeb19ed2c9b92cbe76bb1e733b04de5bcb32489c00c1c06504aef79cd36c3c3f in / 
# Wed, 20 Sep 2023 02:55:50 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:52:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:53:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:54:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b1b4950b21705690e4b15e5257a0efcf7d334776307aaa893216166a5c37f2c0`  
		Last Modified: Wed, 20 Sep 2023 03:01:02 GMT  
		Size: 48.9 MB (48852678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bea1485478ab1093cd60cf0d37627157771e79e9a675510ea1e4233d2499a85`  
		Last Modified: Wed, 20 Sep 2023 10:00:18 GMT  
		Size: 24.6 MB (24576163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:248968c69731e8439bb01eea6789e1dd63c573a1c9e2be9c33d19b9a4411e465`  
		Last Modified: Wed, 20 Sep 2023 10:00:34 GMT  
		Size: 64.5 MB (64464214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1216d62557bc01680a4114e354b2870f938d7b7d419fdd564e12aaaafc2d8f2`  
		Last Modified: Wed, 20 Sep 2023 10:01:05 GMT  
		Size: 209.2 MB (209216423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
