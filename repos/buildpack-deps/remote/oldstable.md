## `buildpack-deps:oldstable`

```console
$ docker pull buildpack-deps@sha256:1a294d3d404e40e584d4d424ed487fd8691f95c84658f7b8641f601db1914cec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:oldstable` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:e5b39fe0f583451250fadb67733c6d8a9c946ac57311eb29e32f2ef2fe4738d8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.3 MB (322297709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:337d5c3296dbe61598d78522d56582f1893dbf23ecf8b2a563411e498bdbf0c7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:59 GMT
ADD file:da3938f00f114fa8f5948fb7182da39c43e5ce57a334ba528681cb29aff0d2f6 in / 
# Wed, 01 Nov 2023 00:21:00 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:53:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 00:54:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 00:55:16 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2f088d622efd8dbaa13d01eafd0aac8f9f33bb335edd3be897ae8059338c7bf7`  
		Last Modified: Wed, 01 Nov 2023 00:25:49 GMT  
		Size: 55.1 MB (55058052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de448b80f06437f3025dcaa9285d40c9c81e4be00df1b04bd5a26fd6b9447fc8`  
		Last Modified: Wed, 01 Nov 2023 01:03:07 GMT  
		Size: 15.8 MB (15764212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24e5da9a0e1f93fa4f1a07ca9a691e0d941bab6927f80157ffc14b478815f95b`  
		Last Modified: Wed, 01 Nov 2023 01:03:23 GMT  
		Size: 54.6 MB (54595619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d61681290435197504d4cdaa3724700bd66544d064d068e837f70e5abede255`  
		Last Modified: Wed, 01 Nov 2023 01:03:55 GMT  
		Size: 196.9 MB (196879826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:04535164c424cb704b73bb1a19096a7e575863c4dbc9adb873d833e366628ccd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.4 MB (295372008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a5f995269b01b9f80a154b38cb65347aa8df4e33c664107279723056ea8c8e9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:37:51 GMT
ADD file:dd011733a11e4681328b2d45bbfc478e1dab88a95554fe817e238ef27b1865c2 in / 
# Wed, 11 Oct 2023 17:37:51 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:06:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:07:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:08:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d310e2405531cf391481a06c9f4d0fc75165ad8e3025e4035c6be5245b6cc754`  
		Last Modified: Wed, 11 Oct 2023 17:41:07 GMT  
		Size: 52.6 MB (52563098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c07441895e6cb16dc8222813db91b971828ec10cafdde9634c13ad69f7723b`  
		Last Modified: Wed, 11 Oct 2023 18:15:51 GMT  
		Size: 15.4 MB (15374683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36086464e7a231c171f28068f405baccff6fe849ecc79fba7ed52c6ebfdba6f9`  
		Last Modified: Wed, 11 Oct 2023 18:16:08 GMT  
		Size: 52.3 MB (52331039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcfedfb2a62724677848265f66d1519ef423f3440998f0a2ce6a01dc498f2b22`  
		Last Modified: Wed, 11 Oct 2023 18:16:43 GMT  
		Size: 175.1 MB (175103188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:e4e482d959b44f9fe93c58da44f823f57a6c75f8f1ac90b76f88d71420aae7a9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.8 MB (282800401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5067c84592299d066e5e61cdeca7db4d8ddd0cfd8d1012de6c767b147e0af26`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:19 GMT
ADD file:684f3634c6b747a4caad8f9f820cc02b53a2122591fe215935c5497ec234c3ad in / 
# Wed, 11 Oct 2023 17:42:20 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:47:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:47:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:48:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:33d0c7672db93e653471872c639cd6129ec25c168942e15a008c4920cafe62d7`  
		Last Modified: Wed, 11 Oct 2023 17:46:42 GMT  
		Size: 50.2 MB (50215704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe33e05af9470f2356c8047560fded363dda4990bb2d70e9194f0dca496bb82`  
		Last Modified: Thu, 12 Oct 2023 03:57:11 GMT  
		Size: 14.9 MB (14879720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0953bb94dc6fcb1dee741e8bfc886a0671f4516a04fbf1a92527c2bb1598e1dd`  
		Last Modified: Thu, 12 Oct 2023 03:57:33 GMT  
		Size: 50.4 MB (50353136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783a8cf6b572fdf6838ef5ecf60b5713b7139f7f8e554b1ccd61d56a597e3cf7`  
		Last Modified: Thu, 12 Oct 2023 03:58:11 GMT  
		Size: 167.4 MB (167351841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:00ffaa1775df7aa605c2ced1697ead01a9b21693aae4289cfe39e23f12001037
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.0 MB (313959291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62c1e77e85cc31b53ae5fb1cf23802ccb5e6e8394bc753361cf259672e530e5b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:58 GMT
ADD file:e1a6c6c976e5e7c53eb2a7343a7a763b46e56828588535f4c79e63d6ec08198d in / 
# Wed, 11 Oct 2023 18:24:58 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:46:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:46:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:47:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dd0dc10f921f4b3b65b17f20d367374079e6cb4e26531624ee64caaaf4adcc28`  
		Last Modified: Wed, 11 Oct 2023 18:28:45 GMT  
		Size: 53.7 MB (53707810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7a630df11a812111dd2b7f5b819a692f2350ad055fab0cd3e60b322c2eead5`  
		Last Modified: Wed, 11 Oct 2023 19:54:57 GMT  
		Size: 15.7 MB (15749899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9c8e3bce435b9fb78d2fd6a8f0ce18ddecff51902c10074a9da4287cb35963b`  
		Last Modified: Wed, 11 Oct 2023 19:55:14 GMT  
		Size: 54.7 MB (54700074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda70d4f1c4310da8eb56a83b481a5bda9d57efa32a6ef6d7915a7cf487c8ba6`  
		Last Modified: Wed, 11 Oct 2023 19:55:43 GMT  
		Size: 189.8 MB (189801508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:027c2ac7b7fa9f7c2154a9a29054feac38fc193959a31cf73c35f363d04ef38a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.0 MB (328045308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:384002c0f12bf18ca0f3797b1f0a18d7a84a7ed8720b3688b2b735b291d8ce4e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:40:52 GMT
ADD file:a3c1e94bb116d940a614a5275c69bacbac46e00da2070b5c7a561e64b975acc6 in / 
# Wed, 11 Oct 2023 17:40:53 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:12:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:13:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:081c634ff059d5636b4292d84d0b49429030b3dca70ca56828543b295adb9d47`  
		Last Modified: Wed, 11 Oct 2023 17:45:55 GMT  
		Size: 56.0 MB (56046358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c55d0c1747845e146fb76750b201af94d841ddeee081fcbdefcc5353c17f2e`  
		Last Modified: Wed, 11 Oct 2023 18:23:38 GMT  
		Size: 16.3 MB (16268212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:049e1171db56ce9d453ea26b1abcc12e301ef98dda47be8250cb0ced74ec097a`  
		Last Modified: Wed, 11 Oct 2023 18:24:01 GMT  
		Size: 55.9 MB (55936762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e77fa153db9b2a24390633ef303b38a33f84bbe4d12c7490cfcc8e12554868d`  
		Last Modified: Wed, 11 Oct 2023 18:24:50 GMT  
		Size: 199.8 MB (199793976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:e5f03b8a3612aa16737fb4f085988cd8bba30d0a048cb95c65b85fedf27c9418
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.1 MB (301123558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f13213c1ead0656fc3dcddc0a9823684c244f11c9e87c31973becaccd971048`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:50:06 GMT
ADD file:c4be7fca661f2a8181ee1e05fda057c18a2d7c1ae0e08ab63b2c5567ef9cc0a7 in / 
# Wed, 11 Oct 2023 17:50:12 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:27:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:29:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:34:59 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d237f50a9f05adf465246bef37e194e1d7a226224c7f90ae7b55925c5b509d15`  
		Last Modified: Wed, 11 Oct 2023 18:01:27 GMT  
		Size: 53.3 MB (53289043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a8381daee3205699bef24f6e7ee0bd6b3621924baae8f1b0b0026007cfe3b4`  
		Last Modified: Wed, 11 Oct 2023 23:58:42 GMT  
		Size: 15.5 MB (15529612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9e6da5ca3b34590abe253ac60b2000d9724ff3d9572311ded53ba9d66e58de`  
		Last Modified: Wed, 11 Oct 2023 23:59:27 GMT  
		Size: 53.3 MB (53302304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2632af27ef8e60c2473640fa869c1560b9bc160073d3db4db8c120329ad58ba3`  
		Last Modified: Thu, 12 Oct 2023 00:01:26 GMT  
		Size: 179.0 MB (179002599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:958d63f118f9541a5d8261b37e6ea3047bb2c96deb9af2464690bec55b58dcbb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.8 MB (330810785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1f7cd93d79e43a628cbf38352b5a20938139f8968c227d5a0b718d6b34fc765`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:44:35 GMT
ADD file:d59326770edede2ba1d2005697bf41540a3d76a4bae883b91fede9b68018630c in / 
# Wed, 11 Oct 2023 17:44:38 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:20:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:21:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:24:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6613fa9f09034273d2b35a47386f8d53c77953a73e561b9f189ffa43ea17bd54`  
		Last Modified: Wed, 11 Oct 2023 17:50:25 GMT  
		Size: 58.9 MB (58929717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565fd5d2ec4119e0cef3217e4496512c36e4adc4e98567f565f105e684e80c4e`  
		Last Modified: Wed, 11 Oct 2023 18:38:00 GMT  
		Size: 16.8 MB (16765485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac6ae11620e817afc07c304ae67f21276148cc99a42e4ac56d481faceb27146`  
		Last Modified: Wed, 11 Oct 2023 18:38:24 GMT  
		Size: 58.9 MB (58866926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e868ed372aa88cb7b1880038e68bff4def65e8692014745f7a779d67797a8527`  
		Last Modified: Wed, 11 Oct 2023 18:39:18 GMT  
		Size: 196.2 MB (196248657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:c508b62b26cf4c3e78a3a679727268f9c89cf031809913639114575bed3387f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.9 MB (295893977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2030b0af1fd8ca97341a629b714304bddce2ff9594cb68f4483fdcccafced6d4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:50:40 GMT
ADD file:bb3ee20a7ddf364b23163c517132146872491e85ef2f1465bf7fd2ed33f94827 in / 
# Wed, 11 Oct 2023 17:50:44 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:58:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:59:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 00:03:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e651436ffb848f56da62cd2c80f206a288b94da8113c4c23a7e5502fb597ce23`  
		Last Modified: Wed, 11 Oct 2023 17:56:38 GMT  
		Size: 53.3 MB (53296378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a52fe3127c9c85c0c5e50b52a035e6bcee230e0c38db795abfee4b60522f157`  
		Last Modified: Thu, 12 Oct 2023 00:35:16 GMT  
		Size: 15.6 MB (15640232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58e9fa5eede43b49ed76d5e09e5c978ac8b2296773dad3161eae081bba447e45`  
		Last Modified: Thu, 12 Oct 2023 00:35:44 GMT  
		Size: 54.1 MB (54066239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d404a1f00add5fb24f6224adfac012cf688caba0fb9eb52c82c499b84498b414`  
		Last Modified: Thu, 12 Oct 2023 00:36:17 GMT  
		Size: 172.9 MB (172891128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
