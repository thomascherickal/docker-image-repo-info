## `buildpack-deps:latest`

```console
$ docker pull buildpack-deps@sha256:5a3f9038371117b13503676a1980ad3cc90e2981e8fb300c61d11204ffadcb0a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:latest` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:5d56c9a108dcfc845daf1d1b5d892873bd19727992914ea7a37aa8fe4d1abad9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.2 MB (312188133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:088b3d4cbdb274e6431764087e072e272399be107cd2cf4c30e761af38713e49`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 03:22:03 GMT
ADD file:a0c8e81c4c7fa85b43d4a9daaed7ba25964a0bf494711b6911cd4b7f5201a17f in / 
# Thu, 16 Apr 2020 03:22:03 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:00:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 04:00:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 04:00:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 04:01:59 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7e2b2a5af8f65687add6d864d5841067e23bd435eb1a051be6fe1ea2384946b4`  
		Last Modified: Thu, 16 Apr 2020 03:31:27 GMT  
		Size: 50.4 MB (50382957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b6f03ffac4cb4e42f8ab0bfc480bd3a3fa20e1ddee37784db63bc886b0cbb3`  
		Last Modified: Thu, 16 Apr 2020 04:16:01 GMT  
		Size: 7.8 MB (7812113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3f0c679f0f4c39597721c1df5cdb4f9685b26bd789a44eeb406835a1800d5f`  
		Last Modified: Thu, 16 Apr 2020 04:16:01 GMT  
		Size: 10.0 MB (9996327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4b47407fc30b8206971ec60f280b107b00df8007da2fb912ebb8656b53695e`  
		Last Modified: Thu, 16 Apr 2020 04:16:23 GMT  
		Size: 51.8 MB (51826807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b32f6bf7d96d26a22dc62da6522f384dcdc936c30c88b233d378e06cf127346d`  
		Last Modified: Thu, 16 Apr 2020 04:17:13 GMT  
		Size: 192.2 MB (192169929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:6ee39d5ee9e79364b2cacb6d057485844355e53d9f20bb8e070da98692057212
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.8 MB (285808053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b2014abcb2de789ac6f9671596056a446c71ad4ced462b0b5c82360d43ae830`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:24:32 GMT
ADD file:a72a8728037d512b79dddab73bd0df9cd4ac56f51fb9f5f8f92cd0814ab43c5f in / 
# Tue, 31 Mar 2020 01:24:35 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 03:23:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 03:24:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Mar 2020 03:24:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 03:27:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c37639eaa7e0ad121e7d329798e6c27a345dbc864d59dec4f04446a2c40e819e`  
		Last Modified: Tue, 31 Mar 2020 01:32:42 GMT  
		Size: 48.1 MB (48095724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f87c19604cd8bfe32a8092d64433839a11077e2602dfd6e6f5dbd9d1f8f2d8a`  
		Last Modified: Tue, 31 Mar 2020 03:47:12 GMT  
		Size: 7.4 MB (7358987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf4e7c27f7acd110a2d7b7ab9f59d4f00ec1be6f6901751dac4ce0f170bc1244`  
		Last Modified: Tue, 31 Mar 2020 03:47:12 GMT  
		Size: 9.7 MB (9687046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d074bdc44f55deaca5b5a75768bbf484abf4a9c2be35396a1a775d8f06901644`  
		Last Modified: Tue, 31 Mar 2020 03:47:37 GMT  
		Size: 49.5 MB (49533381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863b0c2b4c4d24558b7d068e41cc08b38dddc433c5bdacad5d8a0f823030bbeb`  
		Last Modified: Tue, 31 Mar 2020 03:48:40 GMT  
		Size: 171.1 MB (171132915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f9127ff1d4295fe753046cc4714fbee205126c70e787b6a4a97a08a439cde72b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.0 MB (278034909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89fe66f5fdbbd1f52e69c2d8240bf6939e637583a0ddfa8392e839e885e6e024`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:59:14 GMT
ADD file:c2369e5669e570f90abaa1fd4fcea4ae1e6654bbd81e8fa070a5b2484c03ee74 in / 
# Thu, 16 Apr 2020 00:59:15 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 01:38:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 01:38:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 01:39:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 01:42:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:020b29c91094d59c5eb128b7bc2b0b835e2ba4414358664e467428fe8b95bf52`  
		Last Modified: Thu, 16 Apr 2020 01:08:38 GMT  
		Size: 45.9 MB (45864371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f878eece65f73163f26e0755d7bf2d0280b635e9354ee5ac677dd0e1c3b9f485`  
		Last Modified: Thu, 16 Apr 2020 01:56:53 GMT  
		Size: 7.1 MB (7096553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070c5585774beab3cf31d2f66df886bd4295763a00c5f013aab32f261a9559fb`  
		Last Modified: Thu, 16 Apr 2020 01:56:53 GMT  
		Size: 9.3 MB (9343267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e454adb17af2402de86f3b7834eb2d85a7ab8d1199be3963a7ddf802e25a5480`  
		Last Modified: Thu, 16 Apr 2020 01:57:17 GMT  
		Size: 47.3 MB (47343806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4738ef48ef8e257a70acb1ee91104ca66fe43781630b6fe4ed8ce6dc244c918a`  
		Last Modified: Thu, 16 Apr 2020 01:58:08 GMT  
		Size: 168.4 MB (168386912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:1d423f9064fe50e1c9cbcb1b4a20c378e35e89cb44606ecc31373986924c66fe
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.7 MB (302701056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38764b0959657a6bad4b830aa0ee790612f0c295b663a558db8ef301fa90748f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 02:41:20 GMT
ADD file:02afb66e938cbc67271aaf8cbee75def87458a21d961d02e86383e0ed36b0c71 in / 
# Thu, 16 Apr 2020 02:41:24 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 03:13:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 03:13:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 03:14:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 03:16:52 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d080dad46627d4103daddf54c89f2ef0a0b72ba8270066c50e95ffbf4a79362e`  
		Last Modified: Thu, 16 Apr 2020 02:48:36 GMT  
		Size: 49.2 MB (49169521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8c76f347939ef96b2815e45f9fa43995940a8d4a01525012b2bce1adcbfc3a`  
		Last Modified: Thu, 16 Apr 2020 03:27:53 GMT  
		Size: 7.7 MB (7681332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454b6b37aa5fec6dcadc18e45dc6d58e4cf4b967540152c4f44030737e2f5351`  
		Last Modified: Thu, 16 Apr 2020 03:27:53 GMT  
		Size: 10.0 MB (9983908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0caa3b2294305ed3cf1d91d1fe2e2dbf3e294a694a4f636dea6bf733975e237a`  
		Last Modified: Thu, 16 Apr 2020 03:28:16 GMT  
		Size: 52.2 MB (52155917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781c72d22e41051b6112fcf26da1ff478afa45e9da91b07bad2dfd425666c2b4`  
		Last Modified: Thu, 16 Apr 2020 03:29:13 GMT  
		Size: 183.7 MB (183710378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; 386

```console
$ docker pull buildpack-deps@sha256:c4b6abfad742c78e3b65707948ae533f02ee37a7af1f74aa9f213a196ad63ca1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.6 MB (321604090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70e471c3d2f0504027dab61690e5579d8b650f2dfe59b7384b1004befe1ba943`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:39:37 GMT
ADD file:9a9b9c1d98dfe76e20b3ed67b866e2bdbc1095e26de13b892d07f2a3ee062c83 in / 
# Thu, 16 Apr 2020 01:39:37 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 02:18:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:19:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 02:19:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:20:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6a29df432ebf22a237e5e0940a65a1f908be66a5204c5ef240ead7315c27335f`  
		Last Modified: Thu, 16 Apr 2020 01:46:01 GMT  
		Size: 51.1 MB (51147069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec62877ba52bb13d1e47ca6d0c47e1e0d1c61598a0ff5c3590b28c93b2718c3`  
		Last Modified: Thu, 16 Apr 2020 02:37:17 GMT  
		Size: 8.0 MB (7981604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baab3373b511919f98b91c8b654596e531ed2f4612bf5b9d63614e0aa420ee01`  
		Last Modified: Thu, 16 Apr 2020 02:37:18 GMT  
		Size: 10.3 MB (10338497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80102fc76b236a12f5fdd11396159f29e8b9567c8c5a159b09b8dc46fc9c003`  
		Last Modified: Thu, 16 Apr 2020 02:37:39 GMT  
		Size: 53.4 MB (53423402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4915342deee38d6426d697e2a977d4e9b96fbded288158decdc92d0f577d09c9`  
		Last Modified: Thu, 16 Apr 2020 02:38:30 GMT  
		Size: 198.7 MB (198713518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:73f0df53a2af47b2ea4caa21981bb116a76acabb2a554d0ab19b3d8adffd2f75
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.5 MB (333492129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e86bbcda35096f636a208ac9224fb17c81cc101874ee204ad8fc4afe4a429da`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Mar 2020 01:32:00 GMT
ADD file:ccb86d1c4380ce5c6d0f26560ca6d637d15f7a9dd5a3e56977bcf80edcac69ac in / 
# Tue, 31 Mar 2020 01:32:04 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 03:17:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 03:18:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Mar 2020 03:20:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 03:30:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2ee2adf89ee904a62d0e8993a1c564c340ff8a0d3ae152066c13e15fbae902ea`  
		Last Modified: Tue, 31 Mar 2020 01:44:47 GMT  
		Size: 54.1 MB (54138582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7915606b477e202ed2b21747b3be7759d7149f3196e41b5fb1cf369c4de0be`  
		Last Modified: Tue, 31 Mar 2020 04:01:16 GMT  
		Size: 8.3 MB (8252489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2bbb0da6a42dc57d1f7b6790ad807eb7769963d865a7fbc93c11ad41ec9aa16`  
		Last Modified: Tue, 31 Mar 2020 04:01:15 GMT  
		Size: 10.7 MB (10727214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c4349e78867844cdb6b83633fcdacb72c4290b5d7124f9e8e94ea8c947dccb`  
		Last Modified: Tue, 31 Mar 2020 04:02:06 GMT  
		Size: 57.4 MB (57391063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7c69814cc6706127d225dbc647fe9eec3f4ce2278144090bc5d32d7b0ea53a`  
		Last Modified: Tue, 31 Mar 2020 04:03:54 GMT  
		Size: 203.0 MB (202982781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:8b7a97154b5bc7fea050988357e2b1ec9400227e7f75ee8185997deb2db85bfd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.3 MB (294322282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1884094e36848822f02b581eb8db7ea99f23d08fb81dcee8001d8848c0998b8`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:42:03 GMT
ADD file:26367817216af13dc3ba9f495303f7bee8fe138fc8fb728289781563308ce0bd in / 
# Thu, 16 Apr 2020 00:42:05 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 01:58:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 01:58:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 01:59:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:00:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:54e2fb160a5d4a95ec7efe70c0045923ee557e87ee68ce03f2150b8366f26729`  
		Last Modified: Thu, 16 Apr 2020 00:46:03 GMT  
		Size: 49.0 MB (48960213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0f0f1e0f91312a55967b48addc24054fb2e7fb63926a621dd6e86ea62aff2b4`  
		Last Modified: Thu, 16 Apr 2020 02:06:25 GMT  
		Size: 7.4 MB (7382082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c7ce4aae52f7ba529ea00a3a1bfe7656e52dc1d8b0168a3d70b4e0a4392989f`  
		Last Modified: Thu, 16 Apr 2020 02:06:25 GMT  
		Size: 9.9 MB (9882086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d5250b872c2e5d6fcb26d734d43c62187b594e1ce80d34f0cf57fd5e3666b8f`  
		Last Modified: Thu, 16 Apr 2020 02:06:39 GMT  
		Size: 51.4 MB (51370893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914c4ce682a07636bc6fe18e529eac69219759dcae2709cd678c638142bb5c84`  
		Last Modified: Thu, 16 Apr 2020 02:07:07 GMT  
		Size: 176.7 MB (176727008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
