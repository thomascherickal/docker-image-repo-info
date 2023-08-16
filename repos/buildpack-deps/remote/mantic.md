## `buildpack-deps:mantic`

```console
$ docker pull buildpack-deps@sha256:889d740fe04ac8069b368651b191c3dff372e77d75f6ee4c3ba79b72eb1fe50a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:mantic` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:15a9c82e91f6055ea56f7093ab3352b638354992022653c97d07bddafde2b927
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **467.9 MB (467936388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d443c7c75624e3e4d1d108e4ce75ef982f23faf61c6cb56002986ceb62509cb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 05:32:47 GMT
ARG RELEASE
# Tue, 01 Aug 2023 05:32:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 05:32:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 05:32:47 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 01 Aug 2023 05:32:49 GMT
ADD file:7d5373d4ccc5f70f68afa885a495329e33f2bf9f97a437251cfc79e7b85a1a88 in / 
# Tue, 01 Aug 2023 05:32:49 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:33:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 03:34:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 03:36:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:316675922a661ce4c35389bdeea6e9ec8d4708e41f08671b586c7aaea469b2c1`  
		Last Modified: Thu, 03 Aug 2023 03:40:24 GMT  
		Size: 27.9 MB (27857084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a7def12313ae9d69537ed1d4ea003f137f16c5789329735bfd447f8c86cfca`  
		Last Modified: Thu, 03 Aug 2023 03:40:22 GMT  
		Size: 13.8 MB (13783649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476103e20eaed817175054747eac1aeb5b843e57c0d9a11994cdf770c7fba77d`  
		Last Modified: Thu, 03 Aug 2023 03:40:39 GMT  
		Size: 44.8 MB (44785477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f019394434fbbf1dc0322c09dce1c54606b0a0995f99872a492c3de4219eb6b9`  
		Last Modified: Thu, 03 Aug 2023 03:41:32 GMT  
		Size: 381.5 MB (381510178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:d2d3d8a109f9aee3a8a84b5db4b7a4ee8968e36ddc3b5444d516ff9a29e82fd7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **421.6 MB (421628972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad28e1633eea717ac4e3c294c3565d98ce72353358c4847cf40b1f7a874824fa`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 16:43:12 GMT
ARG RELEASE
# Mon, 07 Aug 2023 16:43:12 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 07 Aug 2023 16:43:12 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 07 Aug 2023 16:43:12 GMT
LABEL org.opencontainers.image.version=23.10
# Mon, 07 Aug 2023 16:43:20 GMT
ADD file:443a623a513d24fb17f92fecba92ab4b48c5cd58f4c71a4d1017f68cb28ed803 in / 
# Mon, 07 Aug 2023 16:43:20 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 05:42:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:43:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:46:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9a882830b71793138cc20048eb0866464a2a925cea19f5d96e75bef586f07b01`  
		Last Modified: Wed, 16 Aug 2023 05:52:57 GMT  
		Size: 25.5 MB (25451971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69c48a8564dd51e9033d498988912470fd0761ce0f5546103b27b81cf550ee6`  
		Last Modified: Wed, 16 Aug 2023 05:52:54 GMT  
		Size: 12.7 MB (12696492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59849160634729b9bd9592e9a03ab989ba30317f88c213629a7f24a45111cf44`  
		Last Modified: Wed, 16 Aug 2023 05:53:13 GMT  
		Size: 48.9 MB (48938888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780d3e51aaa28824d8d5f1bec7531f98d5db35b9a576d6c08419ade5b0935f37`  
		Last Modified: Wed, 16 Aug 2023 05:54:09 GMT  
		Size: 334.5 MB (334541621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:2b275e20b8b5fe54ce2809db704d194f38a8c16840cb8233af7f972b5e721af4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **450.9 MB (450948418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:055f72bc14865f7b7ad19033e21241a2fc102800f09200345be0c66e6359bace`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 16:59:38 GMT
ARG RELEASE
# Mon, 07 Aug 2023 16:59:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 07 Aug 2023 16:59:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 07 Aug 2023 16:59:39 GMT
LABEL org.opencontainers.image.version=23.10
# Mon, 07 Aug 2023 16:59:47 GMT
ADD file:a621d5a90b1c5e05eb41dfa44616425f9e9c474acc76e148c36a525e99ff2bac in / 
# Mon, 07 Aug 2023 16:59:48 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 01:33:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:34:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:37:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4b4647be7125cb643de6d0a75158905d697da4afc1e9edcd35dbb27a43edf604`  
		Last Modified: Wed, 16 Aug 2023 01:42:51 GMT  
		Size: 27.3 MB (27266349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f74bc0fb029a079dcd558844cc26c5973e7ec9efc2db4555c60ab536a1a11f`  
		Last Modified: Wed, 16 Aug 2023 01:42:49 GMT  
		Size: 13.4 MB (13369802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7156641b60d58d063ba957dec8ada8f9f2a4052eae760ec0c791b84480868de1`  
		Last Modified: Wed, 16 Aug 2023 01:43:05 GMT  
		Size: 44.6 MB (44630963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940201d34510d57ca35e81b1408d0a6893688d7001f16225853e3ad50c4ec0fa`  
		Last Modified: Wed, 16 Aug 2023 01:43:48 GMT  
		Size: 365.7 MB (365681304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:3f0f104171eb5c17a8352d60506ca6b3fc243aa9f21f00276f864bb351d26963
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **461.8 MB (461771891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b4706d0db06585683cffa47739535f887ddcf98fc2bb6a0361061044183ae11`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 16:57:20 GMT
ARG RELEASE
# Mon, 07 Aug 2023 16:57:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 07 Aug 2023 16:57:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 07 Aug 2023 16:57:20 GMT
LABEL org.opencontainers.image.version=23.10
# Mon, 07 Aug 2023 16:57:23 GMT
ADD file:4cb180718bb451f8c264f3c3ca17e21c2f353537e1350e7285186274e7c13aa1 in / 
# Mon, 07 Aug 2023 16:57:23 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 02:01:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 02:02:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 02:08:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fdf3d625c5c62f16c8647b6f71fb3627aa49027d553c24dfb5bb5fe384576e06`  
		Last Modified: Wed, 16 Aug 2023 02:16:46 GMT  
		Size: 32.2 MB (32220285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4266d044f5749871179995f4d16bfab0f930c8a7fc456be89d9dde4ff53c9a04`  
		Last Modified: Wed, 16 Aug 2023 02:16:42 GMT  
		Size: 15.9 MB (15897836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a546e021bdd3317f25b6399220a698c011a5ef8050a924b3d8d5e67bdc99f46a`  
		Last Modified: Wed, 16 Aug 2023 02:17:11 GMT  
		Size: 49.6 MB (49552401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e76da498d1d6703121456f54c7ec9587100db812456959db12ee2efca2da463b`  
		Last Modified: Wed, 16 Aug 2023 02:18:44 GMT  
		Size: 364.1 MB (364101369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:24d5d1fca2335cafda10036afa67a1e2b2f8015352f51db269db56f4173c0918
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **415.5 MB (415542447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2315269bf260a2bfd983eea1e176a1b3df29ef2b983f6369a8a789c53d3cc0b7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 16:41:40 GMT
ARG RELEASE
# Mon, 07 Aug 2023 16:41:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 07 Aug 2023 16:41:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 07 Aug 2023 16:41:40 GMT
LABEL org.opencontainers.image.version=23.10
# Mon, 07 Aug 2023 16:41:42 GMT
ADD file:7038e8b287279d65872808b33572bb449a981ceacdc4533e8e1047544044f524 in / 
# Mon, 07 Aug 2023 16:41:42 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 04:32:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:32:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:35:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e4b480e7bad6fd35ac328034bc72b280c0019028bc95dd0dbf78d168750430e`  
		Last Modified: Wed, 16 Aug 2023 04:39:53 GMT  
		Size: 26.9 MB (26884397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44867c9f8a414f35f7e550468ffda8aadf82a61ad02779247fe2d748d28e5390`  
		Last Modified: Wed, 16 Aug 2023 04:39:51 GMT  
		Size: 14.2 MB (14158805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e837d29076d6daa1f70750605bd3c0d36bced4e25e6e7f34c8bc4360af79e30`  
		Last Modified: Wed, 16 Aug 2023 04:40:06 GMT  
		Size: 44.8 MB (44814597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1f743134a60cbf024185cb1ef08197ade21d0e304f5d3f6915df0822b32e9f`  
		Last Modified: Wed, 16 Aug 2023 04:40:51 GMT  
		Size: 329.7 MB (329684648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
