## `buildpack-deps:unstable`

```console
$ docker pull buildpack-deps@sha256:1ee25a250e74463901b71bfb4d6b4dbee803365d3bf291b5f074627ba27ed740
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

### `buildpack-deps:unstable` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:5f70cb77ecceabd13b47c72a297febd2d3784528065df5c4aff21b3a80725748
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.1 MB (333083929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e5de3cebbf3b808c5f0f779cddaa8c2fb4cf34d59fe079739bf2215155a80a5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:14:59 GMT
ADD file:62b7e1deca7e12cf507f0b06446a94bfbaff1760c4333fb3f8f92392b57d50b9 in / 
# Tue, 01 Mar 2022 02:15:00 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 06:29:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 06:29:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 01 Mar 2022 06:30:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 06:31:17 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:740da9cc2bb63315fd21f4469ac9e44b2f6efbfd32f98a83c863fa9c1a145714`  
		Last Modified: Tue, 01 Mar 2022 02:21:38 GMT  
		Size: 56.0 MB (55974168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0280ba50ca2de993dcb64a6b9609cf934e39abda112acfcbab8f17a1f5874075`  
		Last Modified: Tue, 01 Mar 2022 06:38:49 GMT  
		Size: 5.3 MB (5275205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04148c21dcbdebe02df7619b1d768334fddc8ac9b581eea2f0dfea8e0a08664f`  
		Last Modified: Tue, 01 Mar 2022 06:38:50 GMT  
		Size: 10.9 MB (10927898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b4ca56fdb263c3de262d59dc9b2ba426e3ef8aa77a2fc23b05601de0aa16bc6`  
		Last Modified: Tue, 01 Mar 2022 06:39:11 GMT  
		Size: 57.2 MB (57188199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec3113631084316a1b852361c2a5edb4bf541795421164361f866978cbef7775`  
		Last Modified: Tue, 01 Mar 2022 06:39:53 GMT  
		Size: 203.7 MB (203718459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:d8844919e8850317227458c1d8f9efac4a2bebcf5f8f74da75dd81ef3854a833
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.0 MB (303976398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:569becd1e01a27104c04f49a719659cf8b39ad2a703cbaa7c28878fa65af919b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:06:24 GMT
ADD file:ac39701f9a18e3289cda9df4afa1e6d52cc3d78e450fe0f6c8eeca44fcfbc1f8 in / 
# Tue, 01 Mar 2022 02:06:25 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:10:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 03:10:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 01 Mar 2022 03:11:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 03:13:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:63235811a46a23f0266af9da0adeda5035210e9743bc381224f6094ba385018a`  
		Last Modified: Tue, 01 Mar 2022 02:23:10 GMT  
		Size: 53.4 MB (53368459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6001fc0f1458be1cd71edddcfc4c80e694e97390d00c3d9321a55c350435e3d`  
		Last Modified: Tue, 01 Mar 2022 03:30:47 GMT  
		Size: 5.2 MB (5175117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:980544d5a86961e1d8ee36922ff866b49151ba29c6e9147204d209098f94070c`  
		Last Modified: Tue, 01 Mar 2022 03:30:49 GMT  
		Size: 10.6 MB (10594892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8726f5abedda8b2a181508f2dc523f0eaf4bd531588cd8ce42312aa018200f9`  
		Last Modified: Tue, 01 Mar 2022 03:31:41 GMT  
		Size: 54.8 MB (54812998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c62bb80dc6b88ce41e3143e437e63ec6baafb7614209cb68e6858a28ef608860`  
		Last Modified: Tue, 01 Mar 2022 03:33:40 GMT  
		Size: 180.0 MB (180024932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:513ab6ae0b39885dc0ff8dc85de19457da4665ba9e2d23c4120e5dd6057fd0ff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.2 MB (294228993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d854a52c90bb9302953775ef435d4ee07735e1b833c2e337634ec1d42513ef62`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:45:42 GMT
ADD file:25bd7c90ec9cba9155b5f5e4b8ba10eee0a84413efe182bfd8e270eec1783ca2 in / 
# Wed, 26 Jan 2022 01:45:43 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 16:45:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 16:45:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 16:46:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 16:48:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8beb160c955a6211ac47cc7f90ad3b37999d7da6c9b2f0d32e82d6ac9bb4e6a3`  
		Last Modified: Wed, 26 Jan 2022 02:02:50 GMT  
		Size: 50.9 MB (50897789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5033ef8051fa00849de7e1029124d977fce14e2255ef3ea2e9a0aa226e20a793`  
		Last Modified: Wed, 26 Jan 2022 17:09:44 GMT  
		Size: 5.0 MB (5035338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2221dacf46091a2f23a799af18530570a3c4d219f9d87d052eb48e5982c95d9`  
		Last Modified: Wed, 26 Jan 2022 17:09:46 GMT  
		Size: 10.2 MB (10241510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1f76ba35e51e63fcba8c49e3f3d26df6cf84550a69e9a8be7657bff2df3d43`  
		Last Modified: Wed, 26 Jan 2022 17:10:35 GMT  
		Size: 52.3 MB (52316409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be847485a9a04e36e5c1fb9b34bf8785f81b78f959f0e907dc63dda6e9927e0`  
		Last Modified: Wed, 26 Jan 2022 17:12:25 GMT  
		Size: 175.7 MB (175737947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d6517f223d5612ca6817c62ba7f8db23864b3b2c3d4571893d9456fe6cc81202
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.1 MB (329108336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98ac843f3264c288d5f92cb2cff90603b7a72602d042a06748cbf35638f625bf`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:43:52 GMT
ADD file:b374f2870285b974edf3ed21e9bcab7b86f3d5f58f504052e4ef7507affd730e in / 
# Wed, 26 Jan 2022 01:43:54 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:16:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:16:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:16:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:17:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3c162c40f334c8be5b3a873f3af9fdbb3e46d36b02232496f08adc78fd0d1197`  
		Last Modified: Wed, 26 Jan 2022 01:51:38 GMT  
		Size: 54.8 MB (54776771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e5527738d1213690712a506bdfb6a4e4e53f00abc3a857f27e46783342a012`  
		Last Modified: Wed, 26 Jan 2022 02:26:12 GMT  
		Size: 5.3 MB (5263075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb344bcecb1f1e4eb7e0b7d7ceb695b290ff4e82c3967bc1c646a8c98de6d21`  
		Last Modified: Wed, 26 Jan 2022 02:26:13 GMT  
		Size: 10.7 MB (10676867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3064c5c0474d687b691ad542db19a5af822c25a6bb02dcbdc584dcf2f73154a5`  
		Last Modified: Wed, 26 Jan 2022 02:26:33 GMT  
		Size: 56.8 MB (56834268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1f652c20e06c8948683dbc64b6032f4dae6fa84dde6693f9e21e7c14d941e3`  
		Last Modified: Wed, 26 Jan 2022 02:27:11 GMT  
		Size: 201.6 MB (201557355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:6b6cac50f5f17a1e51a2373d63b7667c2ac7b39c2ec0eea6584a86b6f42a1268
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.4 MB (336392823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea7966145d171c49e63a64a8b44cd70ba7e698a3996411b4f464c77a11c5f944`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:09:17 GMT
ADD file:cc05e2e409ddf6094d6143fb5d4b47dfb3390bc7281658217d6456c28a94c208 in / 
# Tue, 01 Mar 2022 02:09:17 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 05:44:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 05:44:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 01 Mar 2022 05:45:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 05:45:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fe6e66c27ed7931bded2ff21e1416e6590e3576bb223676ce7abc704e1326545`  
		Last Modified: Tue, 01 Mar 2022 02:18:48 GMT  
		Size: 57.0 MB (57009099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7111e6839c4aa2db70f0f1ec148e3436b2b0964e461965e85327ded44355cb32`  
		Last Modified: Tue, 01 Mar 2022 05:55:11 GMT  
		Size: 5.4 MB (5407372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ee5a5a98edeffbc2270186d55a9d2f1ea5dea3a894a3a0b2cf2ed8cf132b99`  
		Last Modified: Tue, 01 Mar 2022 05:55:12 GMT  
		Size: 11.3 MB (11320306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99c8e04d5ae04e8c6407881aa6a67cfd912e7af562b22fdcfa31ebab1ec3a29`  
		Last Modified: Tue, 01 Mar 2022 05:55:38 GMT  
		Size: 58.6 MB (58606019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6de03d54945bd7a4f2b060c5473083ee8418203cc1fac431dc3b8d3ed00f020`  
		Last Modified: Tue, 01 Mar 2022 05:56:34 GMT  
		Size: 204.1 MB (204050027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:2886d736125239ab9e65fd3ff38f1ed42f9409294275c8733509e2a4dc259750
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.3 MB (313325887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:806e1ac150be048bd76735f53ad7e319409c5080bb77d2f56ec4075fc42d880a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:05:25 GMT
ADD file:203c31666290b4e65e608aeb6cf875bc54d17e55d10989248bc2e2de001c76ab in / 
# Tue, 01 Mar 2022 02:05:26 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:13:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 03:13:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 01 Mar 2022 03:14:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 03:17:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b2b0d222db40c7856984c24ac798f37a235dcde0335158adc8c39139ae52f7cf`  
		Last Modified: Tue, 01 Mar 2022 02:15:36 GMT  
		Size: 54.6 MB (54567600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d562f6b968b46a3de6e09307afbb7cfa6dde77f9fcf6233afe17a922240c64e1`  
		Last Modified: Tue, 01 Mar 2022 03:27:17 GMT  
		Size: 5.2 MB (5232082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be770772e21b5a1d959feb0ae9f1caf8620cfa788e9a77787add844ecb690498`  
		Last Modified: Tue, 01 Mar 2022 03:27:19 GMT  
		Size: 10.9 MB (10887924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e54ea87e9fccbf370c19f94a57e6458cedb8f904f3b3ffb18a86a40d3ab9b06d`  
		Last Modified: Tue, 01 Mar 2022 03:28:06 GMT  
		Size: 55.9 MB (55941329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8059748185653885e38f86639aa31311ddd44bc51e51535bede6f48fe626567e`  
		Last Modified: Tue, 01 Mar 2022 03:30:06 GMT  
		Size: 186.7 MB (186696952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:299430777465940626afb0cd679d087a5509f775c29ea0bddff23139970edb44
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **342.0 MB (342049379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d3fe1ddc87779531aada5ac25cc0f77018bd1e8e537510879ce691103aa6065`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:48:50 GMT
ADD file:00619ac2b9b09af1ef0989fac7a97e811d92f85cef55887a843850c6edd6397d in / 
# Wed, 26 Jan 2022 01:48:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:58:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:59:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 03:00:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 03:09:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:207334870a9e08012db59a768343c68c9297e1123cfd3f49c878d325443196c9`  
		Last Modified: Wed, 26 Jan 2022 02:01:42 GMT  
		Size: 60.2 MB (60197594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e44ef395f05a799994decb77ffb1782c89a4c0282be793f404418d1a7f1d81a`  
		Last Modified: Wed, 26 Jan 2022 03:25:17 GMT  
		Size: 5.5 MB (5540064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f233b52a0118c53ec4e4fcbf2d80e0f1a054746b47ff133ba2e3c92eb1246992`  
		Last Modified: Wed, 26 Jan 2022 03:25:16 GMT  
		Size: 11.7 MB (11693400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f445939acd54056bc3389536f9954772ff534bdffa069800f03bfe155736b47`  
		Last Modified: Wed, 26 Jan 2022 03:26:24 GMT  
		Size: 61.5 MB (61473244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc87e4865f8d2b814bd32992f41e2bf6850e5013631d6be1450a6764281f904d`  
		Last Modified: Wed, 26 Jan 2022 03:28:41 GMT  
		Size: 203.1 MB (203145077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:8eba6bd76e364d31f470138d12d10a3c1604ee5a3cef225f1a3f478f5abfc74c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **342.7 MB (342740508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62a6357ff1e99d258d501d195f32663948044cc626d7fe2fa1ec67b1a910baae`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:14:08 GMT
ADD file:1dc8a81ea9c954e594eb32623a82cdfb528586b569a915ba8f70a49f68a6f7fd in / 
# Tue, 21 Dec 2021 02:14:10 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:56:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:57:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 03:02:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 03:10:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f6b741955e06623f1924320507da1630323c4cf1d6489febc99917464e765860`  
		Last Modified: Tue, 21 Dec 2021 02:30:31 GMT  
		Size: 51.5 MB (51541457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91689f9aadadd96fe4e4ad4ed92ff1cb6a48034aedc9f41e14d54cf85bcdd039`  
		Last Modified: Tue, 21 Dec 2021 03:34:04 GMT  
		Size: 5.1 MB (5089016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a290be0dbc2a1d1f5f12db96d9dc0949f33b55d33712a23f37c71cb89606a3`  
		Last Modified: Tue, 21 Dec 2021 03:34:07 GMT  
		Size: 10.3 MB (10320854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44222df82131b4d925c2f594e50c018b1fb6d67154b22de79d99eb4cd4a356c9`  
		Last Modified: Tue, 21 Dec 2021 03:36:17 GMT  
		Size: 52.8 MB (52817006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f71e08edf3534b3a52b84e74759377bd253863a9cf43fa9dde36a31debd1990a`  
		Last Modified: Tue, 21 Dec 2021 03:42:27 GMT  
		Size: 223.0 MB (222972175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:2ba97f7a267aacf9c56b8a2463b6427b084e28e414b67a64e6e1c54aecfa6026
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.2 MB (305233885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4c1b3564de893443cd394bcfa42e8ef0e21e60818821327cd8efd68337b154f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:03:07 GMT
ADD file:2f65c3757aaa4675484ab3662d157fea03e752f3e5c0b584a7d05649e2599f2e in / 
# Tue, 01 Mar 2022 02:03:10 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:54:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 03:54:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 01 Mar 2022 03:55:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 03:55:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b3073d0c9abbb315a4b9ae0014cf38bf506aea211bf49fa8a5cc18e3c3f8e282`  
		Last Modified: Tue, 01 Mar 2022 02:08:44 GMT  
		Size: 54.2 MB (54226570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cce01958dc2b82af4149cffed8f513336e35311876a55434ce123fbf4ab7f28`  
		Last Modified: Tue, 01 Mar 2022 04:01:38 GMT  
		Size: 5.3 MB (5256919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56a31c0ef8012cb8ef744bce50c47373eeee13a4d42a2fb45572f73067f0115`  
		Last Modified: Tue, 01 Mar 2022 04:01:38 GMT  
		Size: 10.8 MB (10822176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a9637fd788d743da931947073736b89e6109c9a28b73c90479c258875d7398`  
		Last Modified: Tue, 01 Mar 2022 04:01:51 GMT  
		Size: 56.6 MB (56564387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d32537c33a930ec1995edea113b417e8008acdb9b9b0524ebb289773ef805f`  
		Last Modified: Tue, 01 Mar 2022 04:02:16 GMT  
		Size: 178.4 MB (178363833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
