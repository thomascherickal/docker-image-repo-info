## `buildpack-deps:jessie`

```console
$ docker pull buildpack-deps@sha256:db851117f7339bd46c5814f7770dafd99c7c0a2e1d971481ad773c7dfd8bad99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; 386

### `buildpack-deps:jessie` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:a852b431ac946df5b9ee22e5cfe6a0634d64d6fc80af0787b7b90fca5f6221c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.2 MB (247182848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c4e2243285ab5c1128de18b0d86c056da72986b9d3dd6f79f32c0ace2c51c9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:33 GMT
ADD file:a6871f73455488933c1b46ec3a892d3db537f631c01e75573369c7c45b41d017 in / 
# Tue, 17 Nov 2020 20:21:33 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 00:34:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 00:34:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 Nov 2020 00:36:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 00:39:32 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dbcd895dc67d5ce0b25d47678d747226ed725a22e31901fc021fd23879b1ccfe`  
		Last Modified: Tue, 17 Nov 2020 20:27:44 GMT  
		Size: 54.4 MB (54388442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74c5e680cac4523e977d5f2e4e08afec0feb025fba9c24c0c340d4b5ec0d414`  
		Last Modified: Wed, 18 Nov 2020 00:51:29 GMT  
		Size: 17.5 MB (17545974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80d9c23dcbcf37c06d7a291d64c888a36610efee07985b4224774f93bd1ff85e`  
		Last Modified: Wed, 18 Nov 2020 00:51:50 GMT  
		Size: 43.3 MB (43334641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ecde76706f85e86e66f896e76527f5720a364bb7a7ca8db1d1ee88a4d2e919`  
		Last Modified: Wed, 18 Nov 2020 00:52:27 GMT  
		Size: 131.9 MB (131913791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jessie` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:58d94fafd36d36c4b07e7bbe7f578c1553394d82ce15e88bf2158d8a5477cf24
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.2 MB (227156326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b9c23617c0f9df850555113995047eb78f26c31409a76ae9a3324f4035cfa56`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:09 GMT
ADD file:06d0d96a3590043e004bbd651614b8c1b4b048df6ce8706542c12613e2ef83f3 in / 
# Tue, 17 Nov 2020 20:21:10 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 21:47:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:47:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Nov 2020 21:48:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:53:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2950e78c0ac6ca79b0455caabb98b5d25fa715881ced046fe07f25029b96bd01`  
		Last Modified: Tue, 17 Nov 2020 20:30:58 GMT  
		Size: 52.6 MB (52582709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d215fc87b1798e34927476d1004914e87fa45af53379310422e62443ed2654`  
		Last Modified: Tue, 17 Nov 2020 22:10:02 GMT  
		Size: 17.0 MB (17037302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af54c82019f8f5925604f7d31a5b391f3abbddce89539670db949eb979855c82`  
		Last Modified: Tue, 17 Nov 2020 22:10:29 GMT  
		Size: 41.2 MB (41156827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d883b2b6632347781ef239b69b3566e14f83515d89658a8c8e61c10d5b8c2cc`  
		Last Modified: Tue, 17 Nov 2020 22:11:09 GMT  
		Size: 116.4 MB (116379488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jessie` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:0ae8906dd38f6f6661b7c24aaa631e235db9edf89bb89bf65a30d288d3ee4d8d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.4 MB (221441463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:774fc33699998edf53f8d31537d952b4d28fc05d4ee30a7342e8b2e177173e26`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:34 GMT
ADD file:b2545152b2d5298539a3587be3ec1f7ecfececebb4ee80eaff97f66143feac5e in / 
# Tue, 17 Nov 2020 20:21:35 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 21:46:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:46:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Nov 2020 21:48:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:51:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d4af4a46f2c554db32c2423a35e7d1fd96ec1a41633404963392957596e60a5b`  
		Last Modified: Tue, 17 Nov 2020 20:32:10 GMT  
		Size: 50.3 MB (50305387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc5e67e7f7b7f724bbb49fbc0795a7c5d76ac00b944870eb1d2ea3a69994caa`  
		Last Modified: Tue, 17 Nov 2020 22:08:52 GMT  
		Size: 16.7 MB (16723254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39ae13d33a579507fdea6e1eec1193840d5da4b64759da63d75f2a9836acac9`  
		Last Modified: Tue, 17 Nov 2020 22:09:16 GMT  
		Size: 39.8 MB (39779853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed093686662704579944f5ed0aaf54c8b69c31e75b807f4d76edb19f072f6e57`  
		Last Modified: Tue, 17 Nov 2020 22:09:56 GMT  
		Size: 114.6 MB (114632969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jessie` - linux; 386

```console
$ docker pull buildpack-deps@sha256:e6f9b3387310eec820aea3e48a7c78375fa76ba9c6c29dd18419ec6c4efeb928
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.3 MB (254343044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bdf82f0db18ce835eafa31cf92aeb320d9e201fcfaaf9efb57dcd24e0de8da4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:20:16 GMT
ADD file:843de10973ffdcb28448f75b968c0f3f47adc33e3bb0fa5adf1c488c8fbbf5f1 in / 
# Tue, 17 Nov 2020 20:20:16 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 21:09:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:09:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Nov 2020 21:12:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:17:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b79b7651073e6b6c71d7e4168850a7ded5ca4e7d948a7035975a0e83ad6703c6`  
		Last Modified: Tue, 17 Nov 2020 20:27:07 GMT  
		Size: 54.6 MB (54608823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c14b2d754487de7f15aff3e85e50a59c7af0d8f0fcd3ce1c40e8ec436e5fb2d`  
		Last Modified: Tue, 17 Nov 2020 21:25:19 GMT  
		Size: 19.9 MB (19855902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c28c8c47874c59fc4e54207d922f4c54d51d7a37a316b580d7d35b07d690749`  
		Last Modified: Tue, 17 Nov 2020 21:25:38 GMT  
		Size: 44.0 MB (43991143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2585c35068181468900e9ad3aea7e9c7e386f29889eedd04b2488c2da685fe3`  
		Last Modified: Tue, 17 Nov 2020 21:26:11 GMT  
		Size: 135.9 MB (135887176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
