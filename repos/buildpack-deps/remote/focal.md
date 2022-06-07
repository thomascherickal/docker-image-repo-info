## `buildpack-deps:focal`

```console
$ docker pull buildpack-deps@sha256:adc1b7d86465b59a76d2f46b39c4d30b7fd723fa137c61bd3e0951f8d6860aee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:focal` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:b08dce8dedf46e22ffda2e9efbf3cdbea220cbb8db0b3597992137aca8fcb40a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.6 MB (245647506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cfc6f9e82c5502d43d3c2ad2131c353dea2b28e0a65f63a013aede798a739f6`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 02:07:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 02:07:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 07 Jun 2022 02:08:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 02:11:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0b6a9c72470ff5d8860f27875472d3ad0d4b19051144f27660ad480b70c73c`  
		Last Modified: Tue, 07 Jun 2022 02:24:50 GMT  
		Size: 7.8 MB (7768843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27bf6512b10b479ce26a5fccce481830b0b356e00838901ed5d1d051119e3f6`  
		Last Modified: Tue, 07 Jun 2022 02:24:50 GMT  
		Size: 3.6 MB (3624431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc5331f186f0258321175753c071842d764a2bb5d9ebfcfd39cbfb6b96bc9bd`  
		Last Modified: Tue, 07 Jun 2022 02:25:10 GMT  
		Size: 60.7 MB (60730246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac023281c303d2b9aa51404a2813e3dca32b4812908455a6167e7bc9d1146a8`  
		Last Modified: Tue, 07 Jun 2022 02:25:41 GMT  
		Size: 145.0 MB (144951354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1e5cbc62964ca1a9bf0515ae836b1692131f953e653af8f4c2e85584c5995f21
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.5 MB (211491770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a99ef08236c5538fa41d1a35c83c71128687bc5946e6909d4b2022b9ef317958`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:58:46 GMT
ADD file:5f12bea85a1ebe365907ca3979b0e31e6043dccfcb9a3cdf62be46e054494147 in / 
# Fri, 29 Apr 2022 22:58:47 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:27:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:27:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 29 Apr 2022 23:28:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:30:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b20724a4297c7ca8b89f31d6ad53e7ead0c17c7908a4592871cdc97332193580`  
		Last Modified: Fri, 29 Apr 2022 23:03:00 GMT  
		Size: 24.1 MB (24073650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a1563a0a8b5e832769a2de291e460a7fcacd9bee37ad7a2d8a73b14a0f0ddfc`  
		Last Modified: Fri, 29 Apr 2022 23:46:30 GMT  
		Size: 6.8 MB (6762469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493cef317c1c6766357569ceb016cc5074fdef707c8caf5a67a543cd3f49f167`  
		Last Modified: Fri, 29 Apr 2022 23:46:27 GMT  
		Size: 3.1 MB (3104192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aaaed45380a5a8e10619db9bee81a02afc8c18a5b05750eb6b438db9b180461`  
		Last Modified: Fri, 29 Apr 2022 23:47:21 GMT  
		Size: 55.4 MB (55446990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a1b8aaf8cacb29bf277d07f2810a418fab5edf5daf9a7b0541da9e23bd620e`  
		Last Modified: Fri, 29 Apr 2022 23:48:47 GMT  
		Size: 122.1 MB (122104469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:efc7f7cd386595ba3c57309b563442d62672082250954ee7e129fe34ab626a89
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.7 MB (235650477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bb1cc7e13e937312936da088712575c354615da23bdf240a29471ee554e94ba`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:34 GMT
ADD file:ccdde790bb849fe101367f2b541f1062b3544d21f99a5acc535bf2b0884cc0eb in / 
# Fri, 29 Apr 2022 22:49:35 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:16:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:16:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 29 Apr 2022 23:16:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:17:43 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d4ba87bb7858f0dd4a60003f011338f3a58b87d0add985652856007fe5ca5034`  
		Last Modified: Fri, 29 Apr 2022 22:51:32 GMT  
		Size: 27.2 MB (27169388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7feebf8b53c2ab8397b63406bbd6ed34bc670367c3fa74c734bf99c6a2e8ec4`  
		Last Modified: Fri, 29 Apr 2022 23:24:40 GMT  
		Size: 7.6 MB (7634266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8adbae9f42bff04c79875d37944fa1587613ef0de5f7bca85a0b429d4e8d83b`  
		Last Modified: Fri, 29 Apr 2022 23:24:39 GMT  
		Size: 3.4 MB (3386282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b7412064586b1ab2a3ac7b334961d6862b1ce933411b8fd3b75cda3f82b02b`  
		Last Modified: Fri, 29 Apr 2022 23:25:01 GMT  
		Size: 60.8 MB (60774560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce509fb2df8c01e8476ea6d4c6974d3c932abbbedac3c1727ddc4f981ce3597d`  
		Last Modified: Fri, 29 Apr 2022 23:25:33 GMT  
		Size: 136.7 MB (136685981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:c3f0e30e610175b602019b9d1e592d8ca905927b4ed532345c2540c8d5b523c8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.7 MB (269728693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5588b42e4884808f561342644fc2b4b978545186694f2c79a03e473f4ac0dc90`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:28 GMT
ADD file:55691ac7d76af0fcfafc39ebd1e5a4f2d7018147d6db6f89812db33fbaffc2f9 in / 
# Fri, 29 Apr 2022 23:22:33 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:03:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:03:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 30 Apr 2022 00:05:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:13:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e9c0a77cb9f0f7330e3fc62254e4c8ae89ed4bba21209fdc1088195250f950b9`  
		Last Modified: Fri, 29 Apr 2022 23:25:23 GMT  
		Size: 33.3 MB (33290661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52152a0de6e46d74b97d1c4aa354df39f45b928545e3b3cfd5562aec916b61a2`  
		Last Modified: Sat, 30 Apr 2022 00:26:15 GMT  
		Size: 8.7 MB (8722859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7e0fa1464e2cd697c14ed00b03cfae9577e44abba441afa9930519b611d1da`  
		Last Modified: Sat, 30 Apr 2022 00:26:13 GMT  
		Size: 4.5 MB (4456217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af186f438c091a97a62b0923300630e559cef87a617df0381966dc2178cde764`  
		Last Modified: Sat, 30 Apr 2022 00:26:41 GMT  
		Size: 69.4 MB (69419397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e4da36c21569e4140cd7573e1caa9ad05e1b26ce0a58a7018542a1d153a5cb`  
		Last Modified: Sat, 30 Apr 2022 00:27:24 GMT  
		Size: 153.8 MB (153839559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:eb36b4132690733c26db0f2068917e638d60c1e773470db20079068c58451ead
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.7 MB (226716900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a125fdb502d2c22366653c248ba95d1cb89186cfc2918c9db98f4bb54cb334f`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:05 GMT
ADD file:fdc1835c7f7eae641bd78a4c938c3d94746b95a0c151498d332a2b9878fd99d8 in / 
# Fri, 29 Apr 2022 22:50:07 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:11:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:11:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 29 Apr 2022 23:11:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:12:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e0f1090807e81093e3637ffe3d350f58816de907201055908c3506a30c68993`  
		Last Modified: Fri, 29 Apr 2022 22:52:01 GMT  
		Size: 27.1 MB (27065417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad05d33c3457ff71f921fd9c69734064bb89a93c55c748e7c2b83b0aa4b6237`  
		Last Modified: Fri, 29 Apr 2022 23:19:20 GMT  
		Size: 7.4 MB (7422981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa203495428900214c5ff3ea85c5b6134947347f9c1dfda07e1576ab83bf1f9`  
		Last Modified: Fri, 29 Apr 2022 23:19:19 GMT  
		Size: 3.5 MB (3542183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f815ebe8abf75b277a16ac4bc87b6aa8e7db92f1993dbbe8240dcc3d1359c14c`  
		Last Modified: Fri, 29 Apr 2022 23:19:36 GMT  
		Size: 60.0 MB (60010783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b384470b3360a8904f551bdcbee6132718cacafafd1c02ffa61efcdf7b4929`  
		Last Modified: Fri, 29 Apr 2022 23:19:59 GMT  
		Size: 128.7 MB (128675536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
