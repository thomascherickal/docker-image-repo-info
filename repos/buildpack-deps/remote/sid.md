## `buildpack-deps:sid`

```console
$ docker pull buildpack-deps@sha256:c120bde67445affc29d73a69cdcb3a8e45245ddc5d8b9ddccb9639c68b225d2d
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

### `buildpack-deps:sid` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:6f5930f8c78bc124b26f4cbbf87e406fd8f5ae02bfdc3247286064429cda9af8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **382.9 MB (382859831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:564710380fc61bb72df6db961109159640d2c288e5722535ae2e90a47bc213bb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:22:27 GMT
ADD file:69815228666696b3cd3b2799492e3d9cdf4f513ccca5c1cc9282f6c569cc8730 in / 
# Wed, 01 Nov 2023 00:22:28 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:57:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 00:57:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 00:58:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bf371b8152e5df155015cbda7e76bcf445a8be262f7017a9c2cd27a64c3bd875`  
		Last Modified: Wed, 01 Nov 2023 00:28:24 GMT  
		Size: 49.5 MB (49534303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfdee5573ddff91e45c81d11193d3d33f964fe89aa56549950a84c64303f6c2f`  
		Last Modified: Wed, 01 Nov 2023 01:05:03 GMT  
		Size: 24.4 MB (24354415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ee245293502f2c719e3e2302ae5289fe69631d1c3bc58055166bf026f0a28a`  
		Last Modified: Wed, 01 Nov 2023 01:05:21 GMT  
		Size: 65.5 MB (65516786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3597d89d4867151946406aa63662fcdd669fe5dcc674c1e313be40e869926509`  
		Last Modified: Wed, 01 Nov 2023 01:05:59 GMT  
		Size: 243.5 MB (243454327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:be7474ba6810b160f581c83961a59c4e1ed617f41af3a1ef6ef43c934530b6ac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.8 MB (348777511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:112e381ec75b7310c8d79ed0b9d36a9ffa5d88ba0fbe6057b74ff806da63b28f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:38:22 GMT
ADD file:32bc859b55e9b4aada411b379418b1cd95da1e1f72e89ade7698d0132f8edafd in / 
# Wed, 11 Oct 2023 17:38:22 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:09:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:09:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:11:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2f4ea7fe7b8690c3ca25a1b3c670c2f82209d55ff6d955af872eb0ab8df5ff97`  
		Last Modified: Wed, 11 Oct 2023 17:42:28 GMT  
		Size: 47.2 MB (47164847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f544479290fab5feada5ea10b06b543b11d0716abc190b0d608b218fa5128b85`  
		Last Modified: Wed, 11 Oct 2023 18:16:56 GMT  
		Size: 23.0 MB (22993030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c941934e31a404779530c5e75e27d66e4e8c42e849ac2f650b72bf46c0f1796d`  
		Last Modified: Wed, 11 Oct 2023 18:17:15 GMT  
		Size: 63.0 MB (62997933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37f7bce4a3cc44aa542fcd3d30e1975249dd3d046c7e166d81625955228fad08`  
		Last Modified: Wed, 11 Oct 2023 18:17:56 GMT  
		Size: 215.6 MB (215621701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:543ae562deebc7444609c4410c14f9d9e98ebeaa075597ec324dae79e52777bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.7 MB (329670912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a90b032efcd128c9f497b9f4f124e2b3086e8b0c68684771458a83418a208fd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:43:32 GMT
ADD file:e83473ecad5aa9a153d02c535c6e40e22679b973268fdd74a0f5bd86b004222a in / 
# Wed, 11 Oct 2023 17:43:33 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:50:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:51:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:52:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b724b570b5800a7c354a5dac64a4fa673c71f6df8cbf449ab4ce5efd684dd911`  
		Last Modified: Wed, 11 Oct 2023 17:49:18 GMT  
		Size: 45.0 MB (44953579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9525e6d91de2d1165a43ec12ba22c9f291c7d260542aec1bb8f5ffe58d6dd1c6`  
		Last Modified: Thu, 12 Oct 2023 03:59:24 GMT  
		Size: 22.2 MB (22214800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1125f5d06321662f68a43b031f5a38e65b2f62c0728741c6bf3b55cf2c66fde2`  
		Last Modified: Thu, 12 Oct 2023 03:59:44 GMT  
		Size: 60.6 MB (60612153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f54942f68e668fd310d82c3681b4454e9a8ded88988fab1a788df177af06a9`  
		Last Modified: Thu, 12 Oct 2023 04:00:23 GMT  
		Size: 201.9 MB (201890380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d78929fb082b2ed1a977fcc01db1683bd434a6665e75ee2b23dde931377eab58
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **371.3 MB (371319355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e52a91ddd7922782ee4305bf34208d8d13028296c994f57afeefaacc6fe9d69`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:56 GMT
ADD file:c18e09bd64c99d045a504c333efaa05322c76b488039b206edcf75aa2a1a3812 in / 
# Wed, 11 Oct 2023 18:25:57 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:49:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:49:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:51:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d2c869ca968be69328dfec29874eb48a467a69cd422adc8efeb8becda0764bd`  
		Last Modified: Wed, 11 Oct 2023 18:31:12 GMT  
		Size: 49.5 MB (49505948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c237c6272beac4c07d1304257bf58d3b820f2122bcbcab4b1b528ef058cb4c81`  
		Last Modified: Wed, 11 Oct 2023 19:56:46 GMT  
		Size: 23.9 MB (23885868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:371f902523aeade9aa8fc3b19ce94a0e511fc0c9643616c1d93df922a8fabc1c`  
		Last Modified: Wed, 11 Oct 2023 19:57:02 GMT  
		Size: 65.6 MB (65585945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b37145945987b659002a316e849d45b95d3575102362f6ad2895e80603ac1278`  
		Last Modified: Wed, 11 Oct 2023 19:57:34 GMT  
		Size: 232.3 MB (232341594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; 386

```console
$ docker pull buildpack-deps@sha256:bfc36bead83b9287c71c8c41b8475d821d296d321e55886db84a21ff160e0f44
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.7 MB (385692684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:561a6f221b8fdd6e25e51018b04bdfe4b7ad43a0c5faf48692c5493d1de91344`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:19 GMT
ADD file:e8e1c13db04ddce5a6b3f4e29283e75eeecf85f213c2433ccb342a253457abc1 in / 
# Wed, 11 Oct 2023 17:42:20 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:16:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:17:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:19:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b15be2fd60b9adae282f32076fd2c71211d17ebbacfcd05f447fd925da0b81a7`  
		Last Modified: Wed, 11 Oct 2023 17:49:04 GMT  
		Size: 50.5 MB (50485267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:723c0728b8af72632afafd3935c3ba7ea6efc560054e0c90b0e9ac50ffb83d95`  
		Last Modified: Wed, 11 Oct 2023 18:26:25 GMT  
		Size: 25.2 MB (25160503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b827bfd5c1ab262e6257af597a15e6fc633a0ea1ea51c3903247b98e8892a97`  
		Last Modified: Wed, 11 Oct 2023 18:26:49 GMT  
		Size: 67.3 MB (67266446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03d152adaa0d915e84e2a84bfff0791f8ded2f3d6fd5db77ca3e08be7415c89f`  
		Last Modified: Wed, 11 Oct 2023 18:27:43 GMT  
		Size: 242.8 MB (242780468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:3d85d33226b2a8f3a920644a0647de8468ad5c2ea69bf77363b191f03775b89a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **356.9 MB (356898195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49d8c8588e6753fd51937342e65ee98ea4d642c9b48de9365834c8eb300b9655`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:52:38 GMT
ADD file:b80f07fa17341655abce58a1824ae94b2623d66b3f37a58194b8a738cf645945 in / 
# Wed, 11 Oct 2023 17:52:44 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:36:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:38:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:45:32 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f19fff78c927722277ff3254b811f343062ed8e219c72e6938e3662c09994cc3`  
		Last Modified: Wed, 11 Oct 2023 18:04:05 GMT  
		Size: 49.3 MB (49300361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15bac615908c95055b5313c63aafda011d597eca6630f640261a9fcb21dbf24`  
		Last Modified: Thu, 12 Oct 2023 00:01:50 GMT  
		Size: 23.9 MB (23888866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cd7c4ef998d1377d5f93a0a39cb5883535c8632bd1aa9bde6b889d7aaa211fd`  
		Last Modified: Thu, 12 Oct 2023 00:02:42 GMT  
		Size: 64.3 MB (64312786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363e88245300dd295bebfcfd7dc0187ca47f0a41d16ce1a06e966ca253573ddf`  
		Last Modified: Thu, 12 Oct 2023 00:05:09 GMT  
		Size: 219.4 MB (219396182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:4763324c2f7ebc16d1fbca409fb87278ae1f872e10749bf51785d95e27ea379a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **392.8 MB (392805756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aec605cf98188e10c02f1acca308c4196ca2b7646da54f643fc012649f988e6f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:45:44 GMT
ADD file:5f062baf648f8cba61d84347ebedbe11eca129a318a8146b4c7c30586cbf0436 in / 
# Wed, 11 Oct 2023 17:45:47 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:25:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:26:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:30:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ba8528ad854acf64973cba0749a6cf58ce475318878f99dccc45c01a8b19dafc`  
		Last Modified: Wed, 11 Oct 2023 17:52:11 GMT  
		Size: 53.4 MB (53418284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271e36b4d4e036584f3b2cdbde2fbfbc08b9134b8b07ed792b7e85266c0094e2`  
		Last Modified: Wed, 11 Oct 2023 18:39:33 GMT  
		Size: 26.0 MB (25976148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae5a58cfdcc6571603f1108fcb3b5e7462aae879c92f07ae4940c5808065856`  
		Last Modified: Wed, 11 Oct 2023 18:40:01 GMT  
		Size: 70.9 MB (70916924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e1eb59507ba99adede33a09aee8d430e21375cc7abcb407bc2d23cb9708cfec`  
		Last Modified: Wed, 11 Oct 2023 18:41:07 GMT  
		Size: 242.5 MB (242494400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:0150bb87b97db7106a8883b1971dae5b87fbd5391ec9118cf15f6932d83b0f8d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **584.9 MB (584935368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77126be424a00a29f764cd8e7f8da503eebb4c14608d89dd3edd5a2278ccba0d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:09:51 GMT
ADD file:fdcff160dcad587bb28b0cba721c24193be4ab5de90a2d503cba3d329b78797b in / 
# Thu, 27 Jul 2023 23:09:54 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:32:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jul 2023 23:35:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 27 Jul 2023 23:45:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f8b93f818da821e670e126126d6da395bdf2888315b8baa1a6912378c2f4e02c`  
		Last Modified: Thu, 27 Jul 2023 23:12:55 GMT  
		Size: 45.7 MB (45656956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdc8d46a9f89f9d06db33ee07cddd8aa1a54e242cd6463179064bb8e0711848`  
		Last Modified: Thu, 27 Jul 2023 23:45:49 GMT  
		Size: 23.4 MB (23350890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a627ecd6eb80659b2ec0c3464124a436336a8496c101d36a4e46180fdb32a2`  
		Last Modified: Thu, 27 Jul 2023 23:47:12 GMT  
		Size: 60.4 MB (60386385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d8d3e46d641c1277be46ab521cccf04aeac468f053836ff4e0626b3a862cb7d`  
		Last Modified: Thu, 27 Jul 2023 23:57:35 GMT  
		Size: 455.5 MB (455541137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:c98442cc0487cc0d6670b6012ecfcd2cdee07cfb3a075b787e46fcabad15f3fc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **353.3 MB (353300737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87b5f5260c823bc2f6a79c5aca377076720e92bc961cdf80d266c3265c856074`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:51:43 GMT
ADD file:66653f97d007e397b8dbcdca1bbb32bd8039456ae5b2cae3e049382489afb265 in / 
# Wed, 11 Oct 2023 17:51:47 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 00:05:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 00:07:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 00:22:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1c682795de2323b695b3a151f23480c972ce25be65bcc04708dd6eb7250c65b8`  
		Last Modified: Wed, 11 Oct 2023 17:59:19 GMT  
		Size: 48.9 MB (48923705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c5035b89544b06f157cc1fcccda207a6403d5570c3f7b39d2148ffeb92933b0`  
		Last Modified: Thu, 12 Oct 2023 00:36:45 GMT  
		Size: 24.6 MB (24578298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d73bd759805634b041aa9d93b37a142261e1a8bf4ecb0b621c18e8e42879943`  
		Last Modified: Thu, 12 Oct 2023 00:37:14 GMT  
		Size: 66.4 MB (66391135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b4adade00d365c65b646f468a7fbc9243ecff927cdae416e6896e80abe1cfa`  
		Last Modified: Thu, 12 Oct 2023 00:37:59 GMT  
		Size: 213.4 MB (213407599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
