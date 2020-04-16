## `buildpack-deps:oldoldstable`

```console
$ docker pull buildpack-deps@sha256:c54f80b7f3e744d000087720325b44c695676934fff728187f22daf72ccbf2a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; 386

### `buildpack-deps:oldoldstable` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:13b358eadd210eccd79001ae371fb26cec4f599407614ee6f3325a7363830c8a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.2 MB (247170089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:538e0eb1cc979771115adb0d18df7dc170f2b47f9eb3e86e9e3f9729b10b055d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 03:23:07 GMT
ADD file:06c434cd627b8970a4f3d8d76b36955fbf53b74db3f0ce29f1fc3b269c81f2eb in / 
# Thu, 16 Apr 2020 03:23:08 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:04:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 04:04:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 04:06:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 04:09:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3707da5d661028328ae23959ded4ecbb1e5ddbe2a4e8551cd5b6f90e90e6cbd5`  
		Last Modified: Thu, 16 Apr 2020 03:32:06 GMT  
		Size: 54.4 MB (54390842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a013c08ba606e93a8e6efa446e68ae82873c251f8d211d99fb2c3896cd7df989`  
		Last Modified: Thu, 16 Apr 2020 04:17:25 GMT  
		Size: 17.5 MB (17545810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc3dd2434033ea5efd099d5168eee7856f41fbd7d636fe85dfb2a6af4bef6e2a`  
		Last Modified: Thu, 16 Apr 2020 04:17:58 GMT  
		Size: 43.3 MB (43338655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea538f8c33b75bd7ee86a9e1bd88e3fd92b682c9f6484c8fddb9431cf800d98`  
		Last Modified: Thu, 16 Apr 2020 04:18:29 GMT  
		Size: 131.9 MB (131894782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:c702e637ef4204ef2f3da553876c25d24441b5786eb6338154603015bd9b1ddf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.1 MB (227142558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40cdc6b4254529083c6c008dee03f98ee365377a69ba7dca6d43f09b9a4465f8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:25:13 GMT
ADD file:631f76030613657eb3d82228323e5a3860b5141b58858b628bee342bd47d427d in / 
# Tue, 31 Mar 2020 01:25:17 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 03:29:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 03:29:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Mar 2020 03:31:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 03:35:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3ebddd0cca47bf5452de875b55a7b0a10e182a550196df63972f211a03e9f7cd`  
		Last Modified: Tue, 31 Mar 2020 01:33:28 GMT  
		Size: 52.6 MB (52580205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e80167505cea44898f4dce8e6007acae3e6ccf8b0b3b62d514cb4d769474d4`  
		Last Modified: Tue, 31 Mar 2020 03:48:54 GMT  
		Size: 17.0 MB (17037090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7962f7d2575522a8a0df557e93a9845753c76833c794b332df26816e3213f676`  
		Last Modified: Tue, 31 Mar 2020 03:49:15 GMT  
		Size: 41.2 MB (41159943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd4b8d411f9744bb3e6e4c8707228ecd533bdeecea6dad8285163abcbca29f0`  
		Last Modified: Tue, 31 Mar 2020 03:49:58 GMT  
		Size: 116.4 MB (116365320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:3d20b0c635abb73c0d320b6d0404e04cf480c2b652381eb78b372810af63ef27
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.4 MB (221425259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31916f43d7db1d7cc81a5efba5715fa8d14325ccfd731af1f26df59b9650e6de`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:00:13 GMT
ADD file:0b08b600835a16058b725946cb7ae338fea6a14cf6998584f9728d2c62324f1e in / 
# Thu, 16 Apr 2020 01:00:16 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 01:44:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 01:44:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 01:45:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 01:48:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cc084eacfbe394e053f99559ca63f9d660d60dad0b70a31347e5088af534b2e9`  
		Last Modified: Thu, 16 Apr 2020 01:09:20 GMT  
		Size: 50.3 MB (50304312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2753eba5d276059ffd460d19c6e651040079c4a18c7d6a93682bef3e285c0b9`  
		Last Modified: Thu, 16 Apr 2020 01:58:21 GMT  
		Size: 16.7 MB (16723352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aff41b20f0ffb69690b5b8efa517a6db82e30df6bbb8a1ba31dda7369f437c9a`  
		Last Modified: Thu, 16 Apr 2020 01:58:41 GMT  
		Size: 39.8 MB (39777408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead15096fd044e35c9129cdaa284dd871825323849b5ca80a56d9994411a00a4`  
		Last Modified: Thu, 16 Apr 2020 01:59:18 GMT  
		Size: 114.6 MB (114620187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:67b6c2a1f9055ebb1ba55aa65f3184dc40bc054da417c458510197ccf643c2d7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.3 MB (254319130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87ab958b27fb48226f8be91f5d242e35aae8ec0b0a926090b7821153668ffa05`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:40:13 GMT
ADD file:fc5ade2a561dca01c2a4d4035601db636d098801b5655a1bf239e8b706395f87 in / 
# Thu, 16 Apr 2020 01:40:14 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 02:23:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:23:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 02:26:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:30:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:582c227f31bedb5a1092c02e624ef551c8659052150d9e9368da891fffd1528c`  
		Last Modified: Thu, 16 Apr 2020 01:46:40 GMT  
		Size: 54.6 MB (54607914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c1866a4665d6ee342c90adf77b23d7002ec3ef1fc701d3c2df2ca95ab860994`  
		Last Modified: Thu, 16 Apr 2020 02:38:43 GMT  
		Size: 19.9 MB (19855771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e614c5ad0e7f598900eb10a2560d248d97421d118be8b34cc663827e5e9b0f2b`  
		Last Modified: Thu, 16 Apr 2020 02:39:00 GMT  
		Size: 44.0 MB (43980201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814dbe23f02c4c3590f1f159f1465504efb745f04e66c7d483e5de10425c5789`  
		Last Modified: Thu, 16 Apr 2020 02:39:36 GMT  
		Size: 135.9 MB (135875244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
