## `buildpack-deps:lunar`

```console
$ docker pull buildpack-deps@sha256:707ef74b248f53517c08807e9a732b770bdc79d450a8ec52ff945c12c48b8e8b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:lunar` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:1a5c5e7cb1d0b8121f6af03e5d81b2903f193eff7d9d8680767bfd31587cc9a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.6 MB (268569702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddcddba17812f7b0067d772977bf987dba5a1298b2cf5249d50ea340bc08ec0d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 04:28:31 GMT
ARG RELEASE
# Wed, 16 Aug 2023 04:28:31 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 04:28:31 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 04:28:31 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 16 Aug 2023 04:28:32 GMT
ADD file:7392bed4dbab9fb7c9ad5bde6f3bfcde3bcbf1885c336af9c231af6defaa31e1 in / 
# Wed, 16 Aug 2023 04:28:33 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 00:03:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:04:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:07:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:05cdbc478740a42a5ebb092eefd6fc221933f796ee343c49cb920ee60025bab8`  
		Last Modified: Sat, 02 Sep 2023 00:12:48 GMT  
		Size: 27.7 MB (27651898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ea73fe152c7c1b43c8962bdf8054f83c720b0d6251821ccf461eef843531c42`  
		Last Modified: Sat, 02 Sep 2023 00:12:47 GMT  
		Size: 13.7 MB (13744690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e8d218b3d1561b5d122cd9db4c10b2fa28d00a9d62a5fa468005767a3c57ad`  
		Last Modified: Sat, 02 Sep 2023 00:13:03 GMT  
		Size: 44.4 MB (44386354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1579db9ae1a076a64156b02ae82feb2f9ce83e2e9b3b34ac15a03af76804c4fb`  
		Last Modified: Sat, 02 Sep 2023 00:13:36 GMT  
		Size: 182.8 MB (182786760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:d10e6715b29dbd0ef1f2ad8e5abf94556ec18422adecbd8bab056d3fc58649b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.4 MB (232441827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c5bfe8d3346fa65b2a65490f89c9d157d50669df53d95f446c6ee5fe8d1690f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:25:21 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:25:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:25:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:25:22 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:25:24 GMT
ADD file:b92305119eab5dd3dfb00f4d83cd84e00c8ae57143739329da5a19aeda55be4e in / 
# Wed, 04 Oct 2023 12:25:24 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 01:05:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 01:06:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 01:10:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0055151e5ef44f81f2355e8073f34f53cc16494749dbc5ba14445ce5edf3d3b6`  
		Last Modified: Fri, 13 Oct 2023 01:13:54 GMT  
		Size: 25.4 MB (25432981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e866c11041f7a46cb12551f8e93dea44f566d63d4fe5e9771fba148287d761c3`  
		Last Modified: Fri, 13 Oct 2023 01:13:51 GMT  
		Size: 12.7 MB (12665364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f378438bc51fcd6e34f3bded8ebdf10b2f56f47951e89908cd028fb60f9d763`  
		Last Modified: Fri, 13 Oct 2023 01:14:13 GMT  
		Size: 48.7 MB (48674522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a87bb08d55e31d0d5845bac5b3d441c3142141dd75d4c02bbf6b036fdc6be30`  
		Last Modified: Fri, 13 Oct 2023 01:14:48 GMT  
		Size: 145.7 MB (145668960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c1669c3bfc03aa349cc7266907fa3c34faeaaf68a9aa3bf7a888b0c4cb59b797
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.1 MB (258146485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:622129654f3cd970d2cb1ad360340c236ca504db8e4dca2544956acc6a1422e0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:23:52 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:23:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:23:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:23:52 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:23:53 GMT
ADD file:c9b1098bc90ac9b887c3bffdffbcff0c32f32e48df9a673041e3aa796296e69b in / 
# Wed, 04 Oct 2023 12:23:54 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 02:37:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 02:38:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 02:41:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6bd86e5a51fe562347e4392a584c2c048e2caf3c855ee2b39d193782482989d0`  
		Last Modified: Fri, 13 Oct 2023 02:45:03 GMT  
		Size: 27.0 MB (27009502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72b644e1b04fb1dbe3643839ab4b6c1c7562eed7fec98b56653bc7526d1f21b8`  
		Last Modified: Fri, 13 Oct 2023 02:45:00 GMT  
		Size: 13.3 MB (13334915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7195734b83041efa5c9550d35f558288d4c59268de32267217d78d00f7cd0dbb`  
		Last Modified: Fri, 13 Oct 2023 02:45:18 GMT  
		Size: 44.2 MB (44238877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73bddc9768e169e64876fcaec439a948c34e36801d337869e2bf980d6c6417a`  
		Last Modified: Fri, 13 Oct 2023 02:45:44 GMT  
		Size: 173.6 MB (173563191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:211af056d6206cb0c054c6574399551ddb83a5aefee80159536d3f16682d1b6f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.9 MB (292938985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c019c888201adff9c93262404f25da2ecdf4a7eb3676b3029a6fda522ea2219c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 04:16:31 GMT
ARG RELEASE
# Wed, 16 Aug 2023 04:16:31 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 04:16:31 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 04:16:31 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 16 Aug 2023 04:16:34 GMT
ADD file:a9d35b320d969ee1ae8a7bc83aba49da30d93724befb5948c680066ad4f1acdf in / 
# Wed, 16 Aug 2023 04:16:35 GMT
CMD ["/bin/bash"]
# Sat, 02 Sep 2023 00:52:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 00:54:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 02 Sep 2023 01:01:59 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7726bd9db2470633f663befac95b40c8e232237cc11c665bf1475ea520873afa`  
		Last Modified: Sat, 02 Sep 2023 01:14:06 GMT  
		Size: 31.9 MB (31887072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb47e875735b54909bb26c51f415b01486b244104962761fb0b086e0ba7adc81`  
		Last Modified: Sat, 02 Sep 2023 01:14:03 GMT  
		Size: 15.8 MB (15842384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e0eb0d3a3bb8011cff8a14f8ab7ca63d45cafb31bcca77da48df64a6de6930`  
		Last Modified: Sat, 02 Sep 2023 01:14:31 GMT  
		Size: 49.1 MB (49086244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcfdb80569e9bbc6c768f87bc629d4d1c70584a568e035b365f404305b830776`  
		Last Modified: Sat, 02 Sep 2023 01:15:29 GMT  
		Size: 196.1 MB (196123285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b03c2d5655663b83f6a221f35784d8902b4af4751413f0a874d38b81c25573ad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.2 MB (240157223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df5b35e4a07ed4da761b7644d6c49ad1a8694b981e74aaff067b260dec6c54a8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 04:29:27 GMT
ARG RELEASE
# Wed, 16 Aug 2023 04:29:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 04:29:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 04:29:28 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 16 Aug 2023 04:29:29 GMT
ADD file:14fcf0756fb29b609af54412c31e2ff9acbf4634984ce95bf204c67668706cb5 in / 
# Wed, 16 Aug 2023 04:29:30 GMT
CMD ["/bin/bash"]
# Fri, 01 Sep 2023 23:16:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Sep 2023 23:16:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Sep 2023 23:19:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e9a6157a42893e6f99bd42ba05c70c5313add95c69f61f12e51517c0100470b8`  
		Last Modified: Fri, 01 Sep 2023 23:24:13 GMT  
		Size: 26.2 MB (26223925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f88ef015543162519d8e086a0bb86351d03f27b98218ff39b27f3b8b7bc2cd`  
		Last Modified: Fri, 01 Sep 2023 23:24:12 GMT  
		Size: 14.0 MB (14005753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ad80a5cffb7414f3bd06d5dafc212e2f5a767d3312bead7347e2ba8fae5be35`  
		Last Modified: Fri, 01 Sep 2023 23:24:25 GMT  
		Size: 44.3 MB (44275476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f495142834cd7cf92ea01d1b100c2b74a416627d5613eefc2c858d2b4c774d2`  
		Last Modified: Fri, 01 Sep 2023 23:24:50 GMT  
		Size: 155.7 MB (155652069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
