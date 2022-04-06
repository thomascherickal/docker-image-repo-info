## `buildpack-deps:impish`

```console
$ docker pull buildpack-deps@sha256:f4eac776ee824772adbb0b49b81e4c6a056e2ad59ee7db16a29fe45097fb4745
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:impish` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:6e8526c3af4df1c23fca7a2f14a7bccb0a018e91150bd1c95870d2d2656c58a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **406.7 MB (406675011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea1f21f1559035305c29412b36d8f23df57b95d497e5928816e80ddc37423865`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:20:58 GMT
ADD file:eec4cf20bda495a93a4e4c816abd77f5a14cb3fd6ebf56e6b8d7c9f37651edc6 in / 
# Tue, 05 Apr 2022 22:20:59 GMT
CMD ["bash"]
# Tue, 05 Apr 2022 22:47:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 22:47:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 05 Apr 2022 22:48:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 22:51:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:34031c10e7d284f922b3f277e18997db8f3250fd9777be60a86b59e25b2bb155`  
		Last Modified: Tue, 05 Apr 2022 13:19:26 GMT  
		Size: 30.4 MB (30386032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b620199073d87654cb09ef591c8be4e7778d489c08d0f2d33d1e6ca0da3052b`  
		Last Modified: Tue, 05 Apr 2022 22:59:03 GMT  
		Size: 3.7 MB (3692650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a5bf4be237bfb6e07b3c2d8940770141c9cc787c140d50f46e9e4badf20a206`  
		Last Modified: Tue, 05 Apr 2022 22:59:03 GMT  
		Size: 3.6 MB (3552186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e385b6e8171f1f9bc9ae119f11c7e09a53831403999f569bfa63b833c0a30c2`  
		Last Modified: Tue, 05 Apr 2022 22:59:18 GMT  
		Size: 38.1 MB (38085338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1cebfe0e56ac26b375dfa6ded5a1b96423abf90d83d89a250b5c1b2fcd0453d`  
		Last Modified: Tue, 05 Apr 2022 23:00:10 GMT  
		Size: 331.0 MB (330958805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:5a75937fb3add510c6703b0505eed435280fb553891531a4aa375d87136433fb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **371.1 MB (371090239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfe6a76f529619d8d949f4e424a76f1ff2336ca7ab7f55fe1d55765a67b49762`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 07:33:05 GMT
ADD file:380138b8388e9dab10885559d020801299e8a053731bc61eeac23044d83317c6 in / 
# Fri, 18 Mar 2022 07:33:06 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 03:14:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 03:14:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 03:15:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 03:17:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fbf944519806fa77357b54f48091ca8c7ccaea62ebbb79761a15cc513dbcb20f`  
		Last Modified: Fri, 18 Mar 2022 07:36:56 GMT  
		Size: 26.9 MB (26921466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a10b93b08ad29a35f3e5c193f2bfe6b9f9e7d502ebd11b72f4aa644268f77f99`  
		Last Modified: Sat, 19 Mar 2022 03:45:36 GMT  
		Size: 3.4 MB (3443108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5e15c098c0600535f00359aaa245c8a9bbe723d52157f0a5df1dbe5fcba6d6b`  
		Last Modified: Sat, 19 Mar 2022 03:45:35 GMT  
		Size: 3.7 MB (3742619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:887aea08d6ae55f9a1408735ea11709c157a49cafae9637ea0f94abb79b667ab`  
		Last Modified: Sat, 19 Mar 2022 03:46:16 GMT  
		Size: 40.3 MB (40286145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c5089eebc8f352e98caa04d67863156d0c76cf4d120c89db1deff3895ca1b3`  
		Last Modified: Sat, 19 Mar 2022 03:49:18 GMT  
		Size: 296.7 MB (296696901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:93bb779ba86b424f7428ee05b5c2cf6a003dff3798dfdfb13341322a9f834617
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **399.3 MB (399342282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a13f9ada36793b44c976b5bcd4ba566bcfe962579c34c10ce7db589f4d8a34ed`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:41:09 GMT
ADD file:6291956a2e3fe9eea698936c2110257f655f85ef5fde2a71623e0625141cef5f in / 
# Tue, 05 Apr 2022 22:41:10 GMT
CMD ["bash"]
# Tue, 05 Apr 2022 23:08:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:09:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 05 Apr 2022 23:09:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:10:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f91b2ec0e6ea0b2df920d20005a7fd4f57f359296c67e8f7dc8210a85a5a5b41`  
		Last Modified: Tue, 05 Apr 2022 13:20:30 GMT  
		Size: 29.0 MB (29031824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2e6701d71f01758a7fe34633a9bebcc4523c8af74e634139d1dae91ada413b`  
		Last Modified: Tue, 05 Apr 2022 23:16:51 GMT  
		Size: 3.7 MB (3676915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb277949f9898a4ae702c5215a79664e8d0f8874d2fc0a578acacd75f3dfcb1f`  
		Last Modified: Tue, 05 Apr 2022 23:16:50 GMT  
		Size: 3.3 MB (3327618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d8d88abcaf38126a7f82f112b780bec79a8fe5c48d4510b8a319e5937c3700`  
		Last Modified: Tue, 05 Apr 2022 23:17:08 GMT  
		Size: 38.0 MB (38033387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c9cff0aead51230bf5dc2f7532467dde20a8ec540a912f543270d875454ef0c`  
		Last Modified: Tue, 05 Apr 2022 23:18:02 GMT  
		Size: 325.3 MB (325272538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:bd0e217723e7915a78fe9747b690d657b322a83d247ba7563ce97204dbf5cd06
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **414.3 MB (414284649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26219ca2da0822587b0dd6dd704fe9ffa34c8f7406a7f3139dfe6406764a4bec`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 06 Apr 2022 03:35:59 GMT
ADD file:12ad43f11dfcb52c536f049db16e0355dd0eb94d8fa80bc5b0cd7cee083bd07f in / 
# Wed, 06 Apr 2022 03:36:03 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 04:36:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 04:36:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 06 Apr 2022 04:38:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 04:45:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d7170978615332f0cc77a33a016a1fe353d81871a63f50b984b0dac7a1fcabd0`  
		Last Modified: Tue, 05 Apr 2022 13:21:57 GMT  
		Size: 36.2 MB (36176423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a001bd2aababd21010b68132cf219c881a583ea786aae051c1d24233dbff6f`  
		Last Modified: Wed, 06 Apr 2022 04:51:16 GMT  
		Size: 4.1 MB (4146450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e952ac3aad57a80fbcf05e6e6e9a441633123d2befa88f8ed59cb111ddd87518`  
		Last Modified: Wed, 06 Apr 2022 04:51:16 GMT  
		Size: 4.2 MB (4242388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d8053497042759fc4429cf0e72add80e817a741e8d3a370c1d8c6fc60ac789`  
		Last Modified: Wed, 06 Apr 2022 04:51:42 GMT  
		Size: 42.7 MB (42723365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec4801aaede9d15aff6c17f49938d7e3ca65e597e9d65ca4715383dada07e13`  
		Last Modified: Wed, 06 Apr 2022 04:52:49 GMT  
		Size: 327.0 MB (326996023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:429dc372f9cd5e60cd4d58485f2d76a44589e67ccc139a9821d081a7429f17a5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.4 MB (266354638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8249f7618279f6e83532d04588fd62d1812604904a79edcea4be0259735ead5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Apr 2022 23:16:31 GMT
ADD file:68ec34fd3adbb39c77004745e0c6c740c02017efc5274ed14a79e417c54c00bc in / 
# Tue, 05 Apr 2022 23:16:33 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 00:09:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:10:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 06 Apr 2022 00:14:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:20:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:141a3fe0a236e81d09c7406bb701e9ffa4cd6df5c814a6c137c9071355c53920`  
		Last Modified: Tue, 05 Apr 2022 13:22:31 GMT  
		Size: 27.2 MB (27215296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ee819ad05fd79c3b98a1361272f08ada186ca41388b51cd377c360a59de8f26`  
		Last Modified: Wed, 06 Apr 2022 00:51:05 GMT  
		Size: 3.5 MB (3490448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f43a55d5058967c982b5d0ce14e52b6789ac432bab595cf90d32c7973f78dbc`  
		Last Modified: Wed, 06 Apr 2022 00:51:04 GMT  
		Size: 3.8 MB (3804330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4a2d9aa83703456f8af4f7924f19f487a6976624af3c12d2d138c1c604212b`  
		Last Modified: Wed, 06 Apr 2022 00:53:15 GMT  
		Size: 40.8 MB (40768705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569ed4a005b02847b5d724bcd8b4cf27658a875dc2c7c51edd7b813b48ae5214`  
		Last Modified: Wed, 06 Apr 2022 00:59:05 GMT  
		Size: 191.1 MB (191075859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:1669134436dd55a11ce0afdd722c81b7561b187d693670e093f963d0090e2262
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **367.8 MB (367805508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52544d44da539d5f4d85134ce487fc13d781aa913ffa8f889f385328174c6066`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:42:16 GMT
ADD file:93fccbbeddbddb4c4631654eb89c174aa404957f9ba48e6eb738d040c2124b71 in / 
# Tue, 05 Apr 2022 22:42:17 GMT
CMD ["bash"]
# Tue, 05 Apr 2022 23:21:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:21:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 05 Apr 2022 23:21:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:22:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:71116f092cb4d97e181bbee9672334a28730486450b1c615aa5b7956b5a32eec`  
		Last Modified: Tue, 05 Apr 2022 13:23:06 GMT  
		Size: 30.5 MB (30524447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc484e5cf466200eaf92e0a58b88b7b5d7be1d3b5dfb8e8bd029fa6c63aff9c`  
		Last Modified: Tue, 05 Apr 2022 23:28:26 GMT  
		Size: 3.8 MB (3762182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977057d0394b24c9cc6fc05ee89b59244dec00dac84caaa805e6b74c158899c3`  
		Last Modified: Tue, 05 Apr 2022 23:28:26 GMT  
		Size: 4.0 MB (3963382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637eaa514348ba94ae6761e4486bdc41e9f79bc21c5990e40b39f21aff00e011`  
		Last Modified: Tue, 05 Apr 2022 23:28:38 GMT  
		Size: 38.3 MB (38327856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c09492c5e3cf0d7a935aaef4e3d6f76b0eb8c4258f91ca70641bd3ab52f699`  
		Last Modified: Tue, 05 Apr 2022 23:29:17 GMT  
		Size: 291.2 MB (291227641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
