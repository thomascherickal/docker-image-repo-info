## `buildpack-deps:trixie`

```console
$ docker pull buildpack-deps@sha256:e1a1af9997b0a0b3209f6efdd1ac32967e59abb80b8f121269b5afd4423b18f1
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

### `buildpack-deps:trixie` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:76eb5e32172570da1b6bda61e11f0cbee6572c35b8a7eeabe5b484ea2d802352
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.6 MB (385631216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3c533569935244fa74af768bb5f93b0f8da2205a8ad7d9f42536d17e9af7086`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:23:31 GMT
ADD file:00d06a447c9580e05c2514d623a6906f35419629a74e8f29f8627b620df970f3 in / 
# Wed, 01 Nov 2023 00:23:32 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 05:08:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 05:09:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 05:10:21 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9f30dcdc5629f1d2f740d6a704db5e6f29ed782df4486ef49cdbddb30250312f`  
		Last Modified: Wed, 01 Nov 2023 00:30:07 GMT  
		Size: 49.5 MB (49486885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b00fcc62737a4287ca8fcd27724545f3a9669ead301dbede869f8af73f94159`  
		Last Modified: Wed, 15 Nov 2023 05:17:53 GMT  
		Size: 26.3 MB (26255430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ccab398df14d3fc8ad70c0ac91181d737fba7720072d703f9b4cd4776dd5a54`  
		Last Modified: Wed, 15 Nov 2023 05:18:10 GMT  
		Size: 65.5 MB (65508665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d8e7265592a80bc6680099d6e4ebc6438f12eb4409b2ba9c29c9e1cd6192615`  
		Last Modified: Wed, 15 Nov 2023 05:18:47 GMT  
		Size: 244.4 MB (244380236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:c4dd02b720a78446828274ab2cc6528fa2c312793ed7452b372b8bd885afc039
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **354.2 MB (354181507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd6c57d4fbb357e2da385c326cf859f23bcbb94acf5c4d2a75da642ad8a76c3e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:49:55 GMT
ADD file:c8135c4f5f4b7815dc29bb93d73adb514649c5dfb72bfc1c072a7a9ae53653f1 in / 
# Wed, 01 Nov 2023 00:49:55 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 04:19:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 04:19:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 04:22:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:136f2fd3e12dd347dbdab54d5a79402eda3c65de7050120b6c1d86345bcc99da`  
		Last Modified: Wed, 01 Nov 2023 00:54:48 GMT  
		Size: 47.1 MB (47142117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76630daa19e4462e67c7427306ed19109a580c7c1d8e740a83a167e409d9cabc`  
		Last Modified: Wed, 15 Nov 2023 04:22:58 GMT  
		Size: 24.8 MB (24757320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20938e88d9c5a89a0f108e782b84fd782c481cd62c2b806cf84d1ec9e42be3fb`  
		Last Modified: Wed, 15 Nov 2023 04:23:17 GMT  
		Size: 63.0 MB (63026865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b34524d0ae9b6222d63fb5f12bcd3ba14069504b977deaddf1ff76f5e2f5add3`  
		Last Modified: Wed, 15 Nov 2023 04:24:00 GMT  
		Size: 219.3 MB (219255205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1fd4efca28447d364730072aaf05453d9dbce242854e327d14f86a31410de3e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.0 MB (334031743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ac2ec93c94487daa3001f353568b804e94ad3dafadb27880a05040daad71603`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:00:07 GMT
ADD file:035b362840f9210e5a7bfde4a95079958d9f57f5b5a556d22b48ad6abcdf2134 in / 
# Wed, 01 Nov 2023 01:00:07 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 02:00:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 02:01:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 02:03:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b403287e0cd0f39bef349bb68bed383fd0582cc2ae9137aac1969a41c84e30db`  
		Last Modified: Wed, 01 Nov 2023 01:06:58 GMT  
		Size: 44.9 MB (44936197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d95ccb30a9e3ceec487ec02756f65216d24abc33ca03c71393ac6e54f4e82b2`  
		Last Modified: Wed, 15 Nov 2023 02:10:23 GMT  
		Size: 23.9 MB (23949923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a902151f0ab2df8ae45f89c290b155db85a2180a36075c89127fdbbdbccb5431`  
		Last Modified: Wed, 15 Nov 2023 02:10:46 GMT  
		Size: 60.6 MB (60620862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15cd9a864ac37ceaebcb654bdbe09fa0bf0e29cb8d0748ee7f70f1dee480df63`  
		Last Modified: Wed, 15 Nov 2023 02:11:29 GMT  
		Size: 204.5 MB (204524761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3688319b9c516e88d24c8592d6f88fa17216ed884e10e81f6fb8c67ab2266bc8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **364.1 MB (364078462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ebd82260ec2e6d7eaf8c5e1a4fe85b1b86ad077d536c2d55d19661bc0babff5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:41:27 GMT
ADD file:d0c94454bffd347b60b86607fe3aea27f4afc57648c812d80575bc9d7d71a1fc in / 
# Wed, 01 Nov 2023 00:41:28 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:11:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:11:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:12:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6bbd151733a83c3c4e1747562a07b8dc0d6b9a1a38140e050fec86a0e73e1f0e`  
		Last Modified: Wed, 01 Nov 2023 00:47:15 GMT  
		Size: 49.5 MB (49495227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aaa14e94a2e8ffb5faf3100c888245cbc9a4eaaf9d6edea6ed3aef228b6b1f1`  
		Last Modified: Wed, 01 Nov 2023 02:17:28 GMT  
		Size: 20.1 MB (20141380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94bd9c6d088804a732d5962844e6cf83a29d1b30528f3b5ec7ff6e67e742a132`  
		Last Modified: Wed, 01 Nov 2023 02:17:45 GMT  
		Size: 65.6 MB (65600134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c397bd2bdea2862ea763227f6eda962a2798527c478e64bd500bdad5239cdbd9`  
		Last Modified: Wed, 01 Nov 2023 02:18:16 GMT  
		Size: 228.8 MB (228841721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie` - linux; 386

```console
$ docker pull buildpack-deps@sha256:1255020c439389d597eaa2b16dee9c7aa1536b2b4aa224dfbc210a3756402d3e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **378.1 MB (378083228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27c3defb0da7e8349b162012f087f54867d2c18aad1f3b129d672e18ae6a787f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:41:31 GMT
ADD file:99d6a1f205a46734ffc61c992b3c9029eb83aceaab7b9777a94552ae226a209f in / 
# Wed, 01 Nov 2023 00:41:32 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 13:53:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:53:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:54:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7778791eeb3e7444e84c2d682795ca0f756d9e1d87e924e2739660a8ed9134ad`  
		Last Modified: Wed, 01 Nov 2023 00:48:34 GMT  
		Size: 50.5 MB (50466373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d80422353ec8a9a13b994d878c456b9feb2c3711191dccf08d7957979acd368`  
		Last Modified: Wed, 01 Nov 2023 14:01:24 GMT  
		Size: 20.9 MB (20909176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be46fd0a3e04a3c48fa349f6b3baa84f402e8ec4ed841491191fa80991567c8`  
		Last Modified: Wed, 01 Nov 2023 14:01:50 GMT  
		Size: 67.3 MB (67264025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f58267d46c1a5f0b0d20f45e86d4a01dbce5ad96ec0ea36ee8de24679e7fc63`  
		Last Modified: Wed, 01 Nov 2023 14:02:44 GMT  
		Size: 239.4 MB (239443654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:d9a456d77bdcd7c232974a87886dd2bbb590b9cf95313c9f1f0fdffa407dfca2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **361.9 MB (361931070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6647c63058a006d3eb26ee45646b020d6a4bd9871013d88648b3668a910bd6bb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:15:37 GMT
ADD file:fcddbc3f0c0456097a49c255590801b884727d47f9ceac6afe8463117d63a70e in / 
# Wed, 01 Nov 2023 01:15:43 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 02:09:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 02:11:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 02:18:52 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:434392845279581746e8cecd769b536845c39fb214d29012afa566896853392c`  
		Last Modified: Wed, 01 Nov 2023 01:26:47 GMT  
		Size: 49.3 MB (49278627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ede9f97c171cbb8a558528bdc51f6a5dd9e805644cae6cc9891cb76258eb9d`  
		Last Modified: Wed, 15 Nov 2023 02:19:46 GMT  
		Size: 26.1 MB (26073841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7717e39a49a836fc0908b857bdee9522fd3c967c00400172afac7d1498f8b2`  
		Last Modified: Wed, 15 Nov 2023 02:20:37 GMT  
		Size: 64.3 MB (64324993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6b9044ec2fd759757a7d3da51aebd64910bbea1f92e2ab8c2074ed1c4023fb`  
		Last Modified: Wed, 15 Nov 2023 02:23:00 GMT  
		Size: 222.3 MB (222253609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:6f399110e0e0cf3dcce653b18ab632e351a9b0b44822bda406fb7ec996027af3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **398.7 MB (398685762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6faa4d627a08f8d90cb01d865c1011c663ea79b5a68f992797a5e15914ff8fae`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:24:06 GMT
ADD file:d45c9f62cb1fd4297a5ee2026bc6abb62f25a456f3a44a8ab6d115eb1d59ce39 in / 
# Wed, 01 Nov 2023 00:24:09 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 02:17:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 02:17:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 02:20:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a86485f1d263f9f0955a85f3d3707fcc2bc7bb4d598df11d02b766bd3da90ad3`  
		Last Modified: Wed, 01 Nov 2023 00:29:48 GMT  
		Size: 53.4 MB (53390698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4809c26c5fbcf46e724e97753b831c03c2021ac2def13026b528fb114d6989f`  
		Last Modified: Wed, 15 Nov 2023 02:28:19 GMT  
		Size: 28.8 MB (28814600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01dd59a7c5494927ca7f0a3267579f63aea083a036ffa58f2bdba9773f3f058`  
		Last Modified: Wed, 15 Nov 2023 02:28:39 GMT  
		Size: 70.9 MB (70934394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187103a4b58ffe18a1ab1eb4ebd7272365c8a7b0c6d3c3a47de357e5293439b8`  
		Last Modified: Wed, 15 Nov 2023 02:29:23 GMT  
		Size: 245.5 MB (245546070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:0aea1b61a3cc9258f80eb9afd15b4d43a1fec3dc78a985dcee84a17ffb7d8abc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.5 MB (346493962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8528bad8c02e35e6fc9861a3f1e072a52eae0d62f97c014affc16af978eb160a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:45:36 GMT
ADD file:b451624b6214da7e4871235da21071d55a6c21b9ed56fe301e78beebaa9c034d in / 
# Wed, 01 Nov 2023 00:45:40 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:01:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:01:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:02:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:37319c2577b55a62447a947186364b13c616c3448bd2c4aeb444733fc58dfb64`  
		Last Modified: Wed, 01 Nov 2023 00:50:43 GMT  
		Size: 48.9 MB (48900178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10e593352eeadc1fa34f624da16ec4d5ffc03e962de8e47f9fd30d101863f83`  
		Last Modified: Wed, 01 Nov 2023 02:07:56 GMT  
		Size: 20.1 MB (20059774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b780353fcf3645d3b82950a80a107c5134cb03e7e2514a5a84924d066df64f80`  
		Last Modified: Wed, 01 Nov 2023 02:08:13 GMT  
		Size: 66.5 MB (66470254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfd3c0b27e6f490c7f70213d49854c77842e63e87abe059666a4a45282b64bf`  
		Last Modified: Wed, 01 Nov 2023 02:08:45 GMT  
		Size: 211.1 MB (211063756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
