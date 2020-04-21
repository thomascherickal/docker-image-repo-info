## `buildpack-deps:unstable`

```console
$ docker pull buildpack-deps@sha256:98436cfaa93fa2152337eb520e5b170ff3b722e5f44661a8004688253be11d0b
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
$ docker pull buildpack-deps@sha256:156c4624280900031c17fb6642ab8dcaab00623c1ac81ec82d310e22f0c93641
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.1 MB (324121143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b89c8c30e9e4891107500d580d04f1f7b030a59eeb6ad3cd7c7afa8df7e1cdb3`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 03:25:32 GMT
ADD file:2496494632885054452c6f15317aaeace67145465fe0f719da9d3b5c95e6c8ed in / 
# Thu, 16 Apr 2020 03:25:32 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:09:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 04:09:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 04:10:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Apr 2020 01:32:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e4396830990ba6684412015e660aecabd027170dd4336124dd128865a6a81898`  
		Last Modified: Thu, 16 Apr 2020 03:33:46 GMT  
		Size: 52.0 MB (51976212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:819e4b8dc00ccde83638bcdc38c48e437757b1891ffbc63bba9e3fe11cd2f70d`  
		Last Modified: Thu, 16 Apr 2020 04:18:37 GMT  
		Size: 7.9 MB (7933282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1945a2e225e1c6c7667997f238da1810114a7c8260dfd32f9fe4281719b17c6`  
		Last Modified: Thu, 16 Apr 2020 04:18:37 GMT  
		Size: 10.3 MB (10298119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b97794719e7218495589ddaa99735f4c9a7a87113187a3e00ec3cf7d29784c`  
		Last Modified: Thu, 16 Apr 2020 04:18:56 GMT  
		Size: 55.7 MB (55706282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbb643cc37d9b42dc98ad1465ccc1bffb8d80e4120dfbf8594159580f673c78`  
		Last Modified: Tue, 21 Apr 2020 01:40:29 GMT  
		Size: 198.2 MB (198207248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:759345087abea1fee212187261a8b408da0f6135eabdc88bf12e70a1821b7409
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.5 MB (295451182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68fdb6a3e175480478b244741af18b17273e01009dd3cf9a7ac54723785a747a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:52:56 GMT
ADD file:bd1d9af70dc12dc4f17f2b7768c241504faf686b41fc7a690e618f93048fde8e in / 
# Thu, 16 Apr 2020 00:53:01 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 07:53:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 07:54:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 07:54:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Apr 2020 02:03:40 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c1a8f9f50766a877cfcad4d61e0db97b4f5cc37823b5af730a9b1e2a867d6410`  
		Last Modified: Thu, 16 Apr 2020 01:00:47 GMT  
		Size: 49.9 MB (49930750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0560a304aa773636ff4d2d0b589147c30f28a9f3a9eb74d4cec04316bcddef9e`  
		Last Modified: Thu, 16 Apr 2020 08:08:19 GMT  
		Size: 7.5 MB (7514769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d0b1b12f45fe7e95157fac9261c9861a14d708d1a418158b4cf1e4707779d9`  
		Last Modified: Thu, 16 Apr 2020 08:08:19 GMT  
		Size: 10.0 MB (10008673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91d8d715f62c3edfb9a0578335f92a722eb8c560e795e8788cbb8cd7a8746e7`  
		Last Modified: Thu, 16 Apr 2020 08:08:49 GMT  
		Size: 53.3 MB (53286784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793ddf3a8ea224674e93f51c4e26237d2368267bc486fa07d4116a5f950e953a`  
		Last Modified: Tue, 21 Apr 2020 02:11:19 GMT  
		Size: 174.7 MB (174710206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:8793765004bae0e22782d4c5490fe5d7372e7270ad620c04a75a88de863b8e41
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.7 MB (289683681 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19fee37a16c58bcb22ef03346df45fb4aebf49f45196167f56fc666cb1b5ff16`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:02:49 GMT
ADD file:5de6dfe62ae35545ab2dc195cdc7ed6211867d4583f721d08acfff371bc7cecd in / 
# Thu, 16 Apr 2020 01:02:51 GMT
CMD ["bash"]
# Fri, 17 Apr 2020 02:09:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 17 Apr 2020 02:09:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 17 Apr 2020 02:10:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Apr 2020 01:16:22 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d58ce8574bee4c2429ae80f47b2650443254f3f9a0dd9fc1c8d64277895520c`  
		Last Modified: Thu, 16 Apr 2020 01:11:11 GMT  
		Size: 47.7 MB (47655417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49d113a28808faa8fe3cf110ffbf1d3f61e1734b4bf5bc389129f31b164756c`  
		Last Modified: Fri, 17 Apr 2020 02:13:40 GMT  
		Size: 7.3 MB (7255893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cdd02f3a35cf68582a2a9020525ec2a2db6792c7abd94d1eed23a0c585b6be`  
		Last Modified: Fri, 17 Apr 2020 02:13:40 GMT  
		Size: 9.7 MB (9672981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:207f8e898223cc175d4799cfe51f6bb1eec0c1047d38a0f3e1399fc009e8a5a5`  
		Last Modified: Fri, 17 Apr 2020 02:14:03 GMT  
		Size: 51.0 MB (50978414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77aa65612c23ae8e1c0bae0f93ee2daa1d58a40f725cac7fbae435000a3d3002`  
		Last Modified: Tue, 21 Apr 2020 01:26:42 GMT  
		Size: 174.1 MB (174120976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c07c6cbbfbf71cc146926f69bd492df4b026af24befc80ec842853b3e5d29f92
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.0 MB (315979084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78ff3578de55f126cc5674fb8d91331e7428a3df4ccd4544dd19965aa42214ba`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 02:43:10 GMT
ADD file:ff8b5c2517d26b49a4c8114e515f5413a0c64b28ff1e5d3fa1bd70603aaadff6 in / 
# Thu, 16 Apr 2020 02:43:13 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 03:17:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 03:18:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 03:18:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Apr 2020 01:56:18 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2f361d4eae096128866baf55f9d19448df20331f319ad8df0f05397bfd2fe7fc`  
		Last Modified: Thu, 16 Apr 2020 02:49:55 GMT  
		Size: 50.9 MB (50910038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c3a136011851aa29f08165cf962f4b5df6865a2236b90a5fc6d0f1c01ded33`  
		Last Modified: Thu, 16 Apr 2020 03:29:25 GMT  
		Size: 7.8 MB (7808061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0d0c43c17c0157ca9f4cd6b676d7a8e76ef248c724901495c897b950e8ff1b`  
		Last Modified: Thu, 16 Apr 2020 03:29:25 GMT  
		Size: 10.3 MB (10294341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a324e1cc769adafc8b7660201edefbc372e565378179fb1de4f142725a42842`  
		Last Modified: Thu, 16 Apr 2020 03:29:48 GMT  
		Size: 55.8 MB (55809319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c110d5695500bcea07a976fb7f38cb2434752621c2a74d6178d9535e29f2894`  
		Last Modified: Tue, 21 Apr 2020 02:08:36 GMT  
		Size: 191.2 MB (191157325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:29dab517b85e9035e3ed3cfbc907ec771ed53ccac76cc337af6583a18c7c7210
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.0 MB (333975622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31c2e896399e5ef9698313a83f1a9dec4cd7094e8373761bebed23410405e532`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:41:56 GMT
ADD file:af11f81927371cc0ed957aa36f4036c71c73a0b79ab27523cf0d49d8e0260041 in / 
# Thu, 16 Apr 2020 01:41:57 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 02:31:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:31:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 02:31:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Apr 2020 01:51:54 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1cf4ce40baf558f42709af03658907805f477c72b1b1a39869aef429cd35cd3c`  
		Last Modified: Thu, 16 Apr 2020 01:48:16 GMT  
		Size: 53.1 MB (53130042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dcc2dce5f80bcf713e09688ddce4e707509747c60ac5dcb21b50ba63fa26bf6`  
		Last Modified: Thu, 16 Apr 2020 02:39:42 GMT  
		Size: 8.1 MB (8110058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b96fa002b78190463928c6db889856164ede953e0bbc48a860d1856d448dd69`  
		Last Modified: Thu, 16 Apr 2020 02:39:43 GMT  
		Size: 10.7 MB (10657287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7351fce1761580c1a90469f6a39ce4b504f9c1b1c46ac9de64a36b5067846200`  
		Last Modified: Thu, 16 Apr 2020 02:40:03 GMT  
		Size: 57.6 MB (57552290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e38930c81235d00bef91f73bcf1b4529bcbfa85cbc7b862fbb97180dadb9f3`  
		Last Modified: Tue, 21 Apr 2020 02:02:06 GMT  
		Size: 204.5 MB (204525945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:ccd701b5906b93bf8f1fc702939ffbcfd04f97b1130bcbd7f30a93979d9a74bc
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.3 MB (306334693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c53a3edb68b6a0b16068bafa132be6cca9f3da2010b002a42e5431eae9db26c`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 03:31:58 GMT
ADD file:4c8da98109a760f1d6fe331f6b242401bd519a727c19c13f3f490f0bcb3158db in / 
# Thu, 16 Apr 2020 03:32:00 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:19:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 04:19:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 04:20:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Apr 2020 01:16:30 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6757dff0382d5411b1004ff5edeb85cdd1f3776f5d3176d7d12e44563a4577ab`  
		Last Modified: Thu, 16 Apr 2020 03:58:56 GMT  
		Size: 50.7 MB (50691556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d36c2768c5b8693d65638ec047a971f014d1bbc98bfc09ce530b37a44c150b`  
		Last Modified: Thu, 16 Apr 2020 04:43:09 GMT  
		Size: 7.5 MB (7460540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f85fba4b2539f3e581194e8e5bd60f526b459fd2de0bfca983c44dda1df3d02`  
		Last Modified: Thu, 16 Apr 2020 04:43:10 GMT  
		Size: 10.3 MB (10324511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d06feb02a41d4bc159332669937d6dff1c06a6abb82e40834ef1e85a7002a42`  
		Last Modified: Thu, 16 Apr 2020 04:44:35 GMT  
		Size: 54.6 MB (54640945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2638595ba9143c2b2ca40b0753423598962fb83a2f61336d9d7c32ce5d482fa6`  
		Last Modified: Tue, 21 Apr 2020 01:27:50 GMT  
		Size: 183.2 MB (183217141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:2d236e58e4535e5fddb0654e68f34a29156778457eb3d7a3e0f2c7b80ab12793
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **342.5 MB (342492974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:496610804144ace711a4e1d46cee0dbfae0ad6260494e92ab78567137c5b1a90`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:40:28 GMT
ADD file:68afd6d0e23ee44127b8e1f922e1a6977efc12c46c7aa7afff807e146187d870 in / 
# Thu, 16 Apr 2020 01:40:38 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 05:51:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 05:51:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 05:53:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 06:01:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2b17b1afa1bd62e539e75bfdf0ac70297d76a76fc7df9fcbbc67ef6c31717636`  
		Last Modified: Thu, 16 Apr 2020 01:58:42 GMT  
		Size: 55.9 MB (55860496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f930d34b8f1d3792eb6eb828ce6a77754290b38b418d7578625e5b4eb10f66`  
		Last Modified: Thu, 16 Apr 2020 06:23:28 GMT  
		Size: 8.4 MB (8356254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d760269fe892aae3c468a162893981cdd2303cdef6cd9b9f91904b4af14ac395`  
		Last Modified: Thu, 16 Apr 2020 06:23:28 GMT  
		Size: 11.0 MB (10975936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe2bf753cab2c284c76e43577e864c921733f03c9fa3ce1fd63f1d264ac21f2`  
		Last Modified: Thu, 16 Apr 2020 06:24:20 GMT  
		Size: 61.1 MB (61057967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4521bb75e1a1bf4c5c6726ce811526cd631cd426e5551a1a3037ab897e1532e`  
		Last Modified: Thu, 16 Apr 2020 06:26:59 GMT  
		Size: 206.2 MB (206242321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:46e56ee20a6842a54ad2029af9844e8f533fdbfe5acc9aee20a1e8fd303cb2c2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.8 MB (304812073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b482611fb4977ac6f7d953ac28a4685f77dc60ec809c0da9538664f2d49a619`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:42:56 GMT
ADD file:1d96a73c9c03d31b0a60aa6b4e0215085afcdee6dc39954655798110c12c223f in / 
# Thu, 16 Apr 2020 00:42:59 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 02:01:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:01:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 02:01:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Apr 2020 01:48:51 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3633d30b569d7f8e4addec62b3bb5c460572eb82d6568a9bc40a9f189dc4bdcb`  
		Last Modified: Thu, 16 Apr 2020 00:47:02 GMT  
		Size: 50.6 MB (50576543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275dfe1709bf7bfd1a7e225a7b974994148dca503ef21f837a74970529f9eb01`  
		Last Modified: Thu, 16 Apr 2020 02:07:15 GMT  
		Size: 7.6 MB (7600071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae5ff7d1251f85fd4f476599f4408381f4e029ec36f4f1b66a96e89b921e7a0`  
		Last Modified: Thu, 16 Apr 2020 02:07:16 GMT  
		Size: 10.2 MB (10183857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:686e996ff9bb08017109e59fc8068db8d4300aea3359952891468365b7d82d4d`  
		Last Modified: Thu, 16 Apr 2020 02:07:29 GMT  
		Size: 54.9 MB (54938818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:202e61d671146ab08ed175699f2d544b62652cf0afde5edbcb5bc7ea33e3c73c`  
		Last Modified: Tue, 21 Apr 2020 01:54:25 GMT  
		Size: 181.5 MB (181512784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
