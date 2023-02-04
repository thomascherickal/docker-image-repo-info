## `buildpack-deps:bookworm`

```console
$ docker pull buildpack-deps@sha256:0a415d8ed73d5cc8252ad598585c310dc63bd0fb9d71373091ee8f8855cc280e
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

### `buildpack-deps:bookworm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:7d3febecfaee0066c271d56cf4d9ff4db2d11c84bee903e59dd77998d2559fad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.6 MB (344648174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fc869086722fb708453e59e77c90910944a91b539d4da0d5c8f43fad4786035`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:50:57 GMT
ADD file:59c477049f0246331c6723687b7f8995e7a8946172b967d10fb8b67146220c33 in / 
# Sat, 04 Feb 2023 06:50:58 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:20:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:20:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Feb 2023 07:20:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:22:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:20aeb9ca89f41415a92cd1a5e9ff6c0280e09a250e0f950c9df57d97b0d3efb5`  
		Last Modified: Sat, 04 Feb 2023 06:55:19 GMT  
		Size: 49.0 MB (49043016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd16dee5feec7a2da71bdef1f07b5a546389f1554d69d474530b8f847d0c1890`  
		Last Modified: Sat, 04 Feb 2023 07:28:22 GMT  
		Size: 9.0 MB (9033132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba40466925cfd251e3c9b97a519794ed3580ca83f2135be0ccea17e5b2d6f99`  
		Last Modified: Sat, 04 Feb 2023 07:28:23 GMT  
		Size: 11.4 MB (11354722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e5912b196c98527faa75de1f03b026f5c2740634e4a9498c536214352bbd910`  
		Last Modified: Sat, 04 Feb 2023 07:28:40 GMT  
		Size: 64.4 MB (64444820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ef8ca27ca4b3d886b88f1478d0aaf27aa1a473c66efce2cc36dc72160b423e`  
		Last Modified: Sat, 04 Feb 2023 07:29:16 GMT  
		Size: 210.8 MB (210772484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:911d51edac0adedf0e794af3776caf33a212603429d431318ab404b352f2c58b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.9 MB (313906409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25bd69faabfb49684f497e14c34b369d080e3c187499ddfc5fa5f933f38d88b6`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 02:45:51 GMT
ADD file:6283625dd02e5a15e67c45fb0ce9fec384c9086563a64fbd85ef7eec12283466 in / 
# Sat, 04 Feb 2023 02:45:52 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 03:13:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 03:13:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Feb 2023 03:13:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 03:16:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8a4b4311a2a6055167419fac8cc987d97e7a797e53f6176ee2b5d0e6edbde230`  
		Last Modified: Sat, 04 Feb 2023 02:50:25 GMT  
		Size: 48.0 MB (47993284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35559dda00a93e84323ff0a3cd944fd9cebe193cb866743b2bf5d33ac8f7ecd7`  
		Last Modified: Sat, 04 Feb 2023 03:21:50 GMT  
		Size: 8.5 MB (8481336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69dbad85bdc4db8aa9aaa97d1620037878a7830e27a0a13e6913172f0885cba0`  
		Last Modified: Sat, 04 Feb 2023 03:21:50 GMT  
		Size: 11.0 MB (11001821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b85ad8323370f7fbfbc955cee459d994385944146584314db17353d54e588b16`  
		Last Modified: Sat, 04 Feb 2023 03:22:13 GMT  
		Size: 62.0 MB (61978188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e9c0f54ea5320afaad6fac2f4c85b31f181810998dbb3f67fdb0396b69ce0b`  
		Last Modified: Sat, 04 Feb 2023 03:22:57 GMT  
		Size: 184.5 MB (184451780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:53065a53ac011f6d06a448dbc9e404895a21baccff51516c5928a6a263f4753c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **298.3 MB (298252189 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a0f790e1bb138420d3864592880463b870513a42c1729c8554b27736616d175`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 03:59:43 GMT
ADD file:b6a187b9130cac841492cfd6fca00af190439f4343e640b8bf9a62de450ba611 in / 
# Wed, 11 Jan 2023 03:59:45 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 04:30:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 04:30:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 Jan 2023 04:31:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 04:32:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:702c5cffc9db6e776f7684c8b275c47d1706fe0c1c6ae97ecbca1158b5344ce9`  
		Last Modified: Wed, 11 Jan 2023 04:06:34 GMT  
		Size: 46.9 MB (46896199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5bc10aae9d9ca78937a14c74d77038319d33368c9eb41b80d9f5931c62c9efd`  
		Last Modified: Wed, 11 Jan 2023 04:42:44 GMT  
		Size: 8.1 MB (8133411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5241b3a60c9e1048ba06ff64a109707b8e25f445184957a0c680152e95eabc`  
		Last Modified: Wed, 11 Jan 2023 04:42:44 GMT  
		Size: 10.6 MB (10633267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b45a71ccf9d081155bfef6ab2ab05af9ca87f9c343ad39cdbbf80e9adb02b0`  
		Last Modified: Wed, 11 Jan 2023 04:43:06 GMT  
		Size: 56.1 MB (56062222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3bda083baf690aceab8ee8e8983cb571c1978947e76ada07fa8280bac5c5a2`  
		Last Modified: Wed, 11 Jan 2023 04:43:44 GMT  
		Size: 176.5 MB (176527090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:88cc2b989fa72d56437d6c5cc80d27eedabfff5568a8c129d65da94bf075cf8a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.8 MB (335793973 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e15efaf3ff558b8e656be9c3b5ea2af453ced4461ab10c7667c735af9d65b76`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:08 GMT
ADD file:b40ad920bd7dd081e20adf36435db50381b9998a1de3d2eac6b2c45734ce60b3 in / 
# Sat, 04 Feb 2023 06:17:09 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:43:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 06:43:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Feb 2023 06:43:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 06:45:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a43b5d5927a7651097e784be4430a6ade09951f5b6879cd06b0f51fc7c4812af`  
		Last Modified: Sat, 04 Feb 2023 06:20:30 GMT  
		Size: 49.1 MB (49081538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f6dd523027aa16778d661d27e72bbe882cc841d9a40bcf7ba993f9653c66e5`  
		Last Modified: Sat, 04 Feb 2023 06:51:08 GMT  
		Size: 8.9 MB (8865599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef33a1f8ffdb43ea2d51e44c388d4de6bedede50060c1397f6ae0eff23cd307`  
		Last Modified: Sat, 04 Feb 2023 06:51:09 GMT  
		Size: 11.3 MB (11319794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f81f9fe3edb2827f590b523951ed4c6d26f17d9aa521c3b4da9f99c21d74bb`  
		Last Modified: Sat, 04 Feb 2023 06:51:25 GMT  
		Size: 64.3 MB (64337322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e60ca384af68da7f39c9a4d38819036b92341935e4eb94617faede0e25f6e5d`  
		Last Modified: Sat, 04 Feb 2023 06:51:54 GMT  
		Size: 202.2 MB (202189720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:4f003c11513c0b6ab61af9bbb9228e0858525f53ca1dfeb08d8b24535a9e0f7a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.9 MB (346853795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b31150f5b93bfee2f1531241c9e358a19a708605dbd0f4e8867112441a85d494`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 07:48:40 GMT
ADD file:71f93fd08314b2207fb2e5840185c4db4279fa8f008742cf35eaf4daf925d475 in / 
# Sat, 04 Feb 2023 07:48:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 08:17:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:17:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Feb 2023 08:17:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 08:19:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0b6e1871a6864b2026696c7ffe48da3030a97146a6a0f3ca18f87c19b1ed6e05`  
		Last Modified: Sat, 04 Feb 2023 07:53:55 GMT  
		Size: 50.1 MB (50093420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd7274669ca31ae25c99ffbeb62b7bf63cf6e70c0afea787b6483e8e1e233d5`  
		Last Modified: Sat, 04 Feb 2023 08:25:56 GMT  
		Size: 9.2 MB (9211501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:222e731d14a700e618d6e7298602f00a0ac9884fbe12a867349d9a13ae14bb4a`  
		Last Modified: Sat, 04 Feb 2023 08:25:56 GMT  
		Size: 11.6 MB (11557630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e9553d1e75be1e95f064cd22c826152b2da62a778c20ddc098b2c20f0575749`  
		Last Modified: Sat, 04 Feb 2023 08:26:15 GMT  
		Size: 66.3 MB (66316077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea46a0242002669ddfb4948fc0ce1d00941d8e3fa2de8699c0aea1d605498232`  
		Last Modified: Sat, 04 Feb 2023 08:26:50 GMT  
		Size: 209.7 MB (209675167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:47b65885fbe9dc9d1483a43a949d82ced569be69af8de0bd15ac5b317ff0074f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **320.3 MB (320292058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:162542698152a9a53b5ee686bcd0066a07e3565fc1417b84664dcbc8e864c505`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 16:32:17 GMT
ADD file:aa37d39fc83f9cce3f1f8522cce22a9c3f9734fea6996431d00a2921079da343 in / 
# Wed, 11 Jan 2023 16:32:22 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 17:11:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 17:12:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 Jan 2023 17:13:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 17:20:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:951f9db918ae0d2bc2c008522e4d5801e026653a12e21d76a02a48b96faaaabf`  
		Last Modified: Wed, 11 Jan 2023 16:41:22 GMT  
		Size: 50.1 MB (50120566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f5f91f049142f1806ecb72912bae28f718b88cdfc593aeaf7a39f089532f66`  
		Last Modified: Wed, 11 Jan 2023 17:39:47 GMT  
		Size: 8.4 MB (8398591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cee1eb44d9967c2535c5377493c304e9066c347f97119b605462ed59745bcfa`  
		Last Modified: Wed, 11 Jan 2023 17:39:47 GMT  
		Size: 11.1 MB (11104095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3efd79671fe172dfdbace9a335d8792f6cae970d99d15077cf26e204ebb898`  
		Last Modified: Wed, 11 Jan 2023 17:40:37 GMT  
		Size: 59.7 MB (59681015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e0ff5fb90935407c9586ba85dd96b12953468351269b7fa95a4b6ec367f1105`  
		Last Modified: Wed, 11 Jan 2023 17:42:48 GMT  
		Size: 191.0 MB (190987791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:bf73003533d9b48c91a35b48daea9a5816b78f0c9d75034dcc139d0ef56866f9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.5 MB (357470016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:424fa9081972646c8b5ba2b43399bf4eb18f37ebf175cde49470776aee24aa50`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 03:48:20 GMT
ADD file:be85aca9c16cf896fbced9508d29913a52fd69f8b2fd24c49efca520a37eeb1e in / 
# Wed, 11 Jan 2023 03:48:23 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 07:09:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 07:09:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 Jan 2023 07:10:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 07:13:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:752672804a573b7cec5745cda59b6068007db5af1aef95a3e7929331c20247e1`  
		Last Modified: Wed, 11 Jan 2023 03:54:09 GMT  
		Size: 54.1 MB (54143855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750945def87bc453cd91c327bab81f39d93adb5ab86cdb4c913921aff512e2df`  
		Last Modified: Wed, 11 Jan 2023 07:24:14 GMT  
		Size: 9.6 MB (9612460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51845b4a51b4708da56bb53781c3d9bab20bd3820ac919ab7598b33948797a8`  
		Last Modified: Wed, 11 Jan 2023 07:24:14 GMT  
		Size: 12.1 MB (12114275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cce18c9a581eda32c9677a56ce48754f33c6fce961d31ad0e8990173c2b6421`  
		Last Modified: Wed, 11 Jan 2023 07:24:42 GMT  
		Size: 66.3 MB (66314568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af4665dcf20e3e8528e2cef81e6aaeb306b7119d42ab34220a3a1ba5cc164e9`  
		Last Modified: Wed, 11 Jan 2023 07:25:43 GMT  
		Size: 215.3 MB (215284858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:d43d58048dc72bbf79a62da9c29384f7d80b3417899c2c6ef67c8c7a07cb0df7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.6 MB (313623657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daa45557df4039ea181329faf4cf1746d95e1c5f1093b34b86b9631888bb5b33`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 04 Feb 2023 04:05:23 GMT
ADD file:cac3f762206c0f8ad807211cb73145ac093d8917f5b8cf3a79eea3ef1fd14eea in / 
# Sat, 04 Feb 2023 04:05:26 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 04:30:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 04:30:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Feb 2023 04:30:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 04:31:48 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5788bb4f4cdc5bb0c03495b0d17914750f0dffcbdc053321669358a95967dbed`  
		Last Modified: Sat, 04 Feb 2023 04:09:43 GMT  
		Size: 47.4 MB (47429742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1e84e5465158af09efec27ef891007b9bd6994985807b81f054e6b39a0cdf0`  
		Last Modified: Sat, 04 Feb 2023 04:38:50 GMT  
		Size: 8.7 MB (8666425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a1fe479ceec98fa274b9f162d0d9d0a555e7ecadb9aaa64ad94b2423e5d22a1`  
		Last Modified: Sat, 04 Feb 2023 04:38:49 GMT  
		Size: 11.2 MB (11218182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b390826d9588a3304d3449fb7e5d2594d77558be4387e3fb22b9188f1bc4c4`  
		Last Modified: Sat, 04 Feb 2023 04:39:04 GMT  
		Size: 63.4 MB (63413204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f173695e8b20910d073734310e8db6aed8b8704417cdcacd4fb5c9fd9e69637`  
		Last Modified: Sat, 04 Feb 2023 04:39:31 GMT  
		Size: 182.9 MB (182896104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
