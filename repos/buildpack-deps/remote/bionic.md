## `buildpack-deps:bionic`

```console
$ docker pull buildpack-deps@sha256:7306ebbeebc1183e2005cd1fbbf1c94a70fa7d237202936d84a14e744bb26432
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:bionic` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:60599545f660f32d83b38e1bc604c83a724adbe132c28226cd1c04db1c22b940
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.3 MB (221261555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:720c9b13204794a9cbe61d130d4bbd0dc5834d6e062fef2874741bac2ffd3df7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 22:59:58 GMT
ADD file:5131314b62b7386e388b173018be7058491e96459344f78e6a2220771a65a2cd in / 
# Thu, 21 Apr 2022 22:59:58 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 01:27:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 01:27:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 22 Apr 2022 01:27:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 01:29:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:88736512a147458c580cd28c969698561f236abba2ef04dbf0d7940cb3d7375e`  
		Last Modified: Tue, 19 Apr 2022 13:10:00 GMT  
		Size: 26.7 MB (26709883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40d74cdf65aa24870bf2345d9c4fa42388a09f5388e94469f3e6f08644a35dba`  
		Last Modified: Fri, 22 Apr 2022 01:43:43 GMT  
		Size: 6.6 MB (6641787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29dc3910681266625514ae173ec9b5aad8bd2bcc5b5ed7ce0e668a4f43e1a93c`  
		Last Modified: Fri, 22 Apr 2022 01:43:42 GMT  
		Size: 3.0 MB (3022435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeeabe337490f3baa39daf3ec713767aea729f5abf9f3f763910203571419504`  
		Last Modified: Fri, 22 Apr 2022 01:44:00 GMT  
		Size: 45.5 MB (45486492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f2b261bf5b4e0f56b81c33068f45ffaba82d86ef45f1df23cbb827b80c173a`  
		Last Modified: Fri, 22 Apr 2022 01:44:29 GMT  
		Size: 139.4 MB (139400958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:0177867e809f0c0b76ee4a76a630c86ccf40d9a2eb9889a5983861afbd87ab13
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.5 MB (189453093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24c5648d51a53675ea925a4a5616b02f5dadfcca5012cd47b0b6a1bea155a9c4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 06 Apr 2022 03:25:38 GMT
ADD file:3230d8a499e37ff816595cbac3892a80005afccf8a55053c28e24989d52de08b in / 
# Wed, 06 Apr 2022 03:25:38 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 05:03:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 05:03:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 06 Apr 2022 05:04:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 05:06:24 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:419a71fa3c92c7dd0e8cfbfdf694362de1c27dafed508aeb2e5bc9ff8376fc98`  
		Last Modified: Tue, 05 Apr 2022 13:12:06 GMT  
		Size: 22.3 MB (22301415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da9b34da99841919b0af9f447099b7d6b004654e1f27cb9822534950a1f44bc`  
		Last Modified: Wed, 06 Apr 2022 05:23:44 GMT  
		Size: 5.7 MB (5711821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b36893f5a19e981da33035ae9e385a11b6213d3c677e36b6da86f20b55b167`  
		Last Modified: Wed, 06 Apr 2022 05:23:42 GMT  
		Size: 2.6 MB (2584515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa75840a85e1cccff64ce7108a91815978c6e514231ea0effcaa49c218259bd5`  
		Last Modified: Wed, 06 Apr 2022 05:24:23 GMT  
		Size: 40.7 MB (40677577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eeee81d87d123cabae7ee71905c92d4b1b37c96823c56e533fa4b183d89ae26`  
		Last Modified: Wed, 06 Apr 2022 05:25:47 GMT  
		Size: 118.2 MB (118177765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3f7ad893336946b4d93804e90116d6f07b03f0770d257a41ba57a8f56223d355
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.4 MB (205390933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:739aa6cbb04c5dd793b7ae063862b6477255762be17a71ceeefe6599b44eeabc`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:54:01 GMT
ADD file:5c0ff944739f8966900c55d6a77ba4ba6031b585962994b1684845dcd411c2fb in / 
# Fri, 22 Apr 2022 00:54:02 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 04:29:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:29:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 22 Apr 2022 04:30:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 04:31:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:945d527fe80d536e4da70ea808f70d90bc97d7930c7ae2c61b5dabd1dba19e07`  
		Last Modified: Tue, 19 Apr 2022 13:10:40 GMT  
		Size: 23.7 MB (23734459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31dd4f068bf0b02d321355a3f8fb2eaaecdb976b6c1e065e3316599c0ccf8dd5`  
		Last Modified: Fri, 22 Apr 2022 04:38:56 GMT  
		Size: 6.1 MB (6082554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f02ffc7642bf1096d5f4511822ad6d8e2c6a6da8a483abdc1b95902454ae8fe`  
		Last Modified: Fri, 22 Apr 2022 04:38:55 GMT  
		Size: 2.6 MB (2570164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b35cad735bb5ee52e0db045775ead9ac2da3682386e82c32e4a5d7832794979`  
		Last Modified: Fri, 22 Apr 2022 04:39:14 GMT  
		Size: 43.3 MB (43288371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1cd4e5834d5d47bd2412717b2612fd5e64b29dac87650a7e45128c880111b8`  
		Last Modified: Fri, 22 Apr 2022 04:39:44 GMT  
		Size: 129.7 MB (129715385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; 386

```console
$ docker pull buildpack-deps@sha256:2f1f6e4d4c77a3ef85a7aa4c68817a22c7bfb342cd843cff3ff3038897010afa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.1 MB (218134402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b0940f238c2638e0b328a2854001cd0aceee57c59ad78a73d999569476af2ca`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:53:57 GMT
ADD file:164f0ee7842870b8f94ab2ee8f9151b49e08f461b99fdfa1b7586fa864d4a320 in / 
# Thu, 21 Apr 2022 23:53:57 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 00:16:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 00:16:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 22 Apr 2022 00:17:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 00:19:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:57fda0d035c311017871931fe2f2a2c241e46b4bc95d2a87dbf533afd8e72668`  
		Last Modified: Tue, 19 Apr 2022 13:11:34 GMT  
		Size: 27.2 MB (27163453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80020c29fe6d0575254dda040fc655dfaa84bca26136ce9b29f390d4fbb29b6`  
		Last Modified: Fri, 22 Apr 2022 00:22:15 GMT  
		Size: 6.9 MB (6929643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91cdf0da60441cb8fc028c8ef1f25bf94a0e154a9fe189221f99d9d7e17e0579`  
		Last Modified: Fri, 22 Apr 2022 00:22:14 GMT  
		Size: 3.0 MB (3038571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e7e0cc8bbbca0f6e3c427507a389d0fa1ede6bdc4b6510939e3a64d6efa643`  
		Last Modified: Fri, 22 Apr 2022 00:22:35 GMT  
		Size: 47.1 MB (47084276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c475941d0d1a577edd87a4d5a0c38144f268dfae6f23559cf99bccd33a7d7f5c`  
		Last Modified: Fri, 22 Apr 2022 00:23:04 GMT  
		Size: 133.9 MB (133918459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:3ca98d5cec6b57ba054629c460764dbb4dc8ecdbdf4ebf2919ff23317984f883
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.3 MB (246252570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c66a5941019bdf772bf81d62ef51f42e037508bf3adbdd73b7e8746567291c8b`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 08:07:45 GMT
ADD file:d5447cb8fcc4a12030e43cda74f87e1bec09c6d1093307e25164127500f5e0d9 in / 
# Fri, 22 Apr 2022 08:07:52 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 09:06:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 09:07:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 22 Apr 2022 09:09:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 09:15:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:00422cde8b22ee0ff419263739625132280d08ffe78075ad3fb44dd003fab8e2`  
		Last Modified: Tue, 19 Apr 2022 13:12:05 GMT  
		Size: 30.4 MB (30442273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d587db8c583825f01547d10158ffcd670b22090b1d7e22c4cc5e38a8d66de0`  
		Last Modified: Fri, 22 Apr 2022 09:40:32 GMT  
		Size: 7.1 MB (7056674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9dc57e211ce75e162542827ed82b7296b4e38b40d85577df3c9df74cc13ae0`  
		Last Modified: Fri, 22 Apr 2022 09:40:31 GMT  
		Size: 3.7 MB (3719458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f3d85745514e470e8c7feb12770beffb279852e12e73b52443c36b69c39fc4`  
		Last Modified: Fri, 22 Apr 2022 09:40:56 GMT  
		Size: 53.7 MB (53729622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c8e6619e0a40ac93bca6305785776fc1dd3bacba430fd75bdfe8305ed8f8f4`  
		Last Modified: Fri, 22 Apr 2022 09:41:36 GMT  
		Size: 151.3 MB (151304543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:e55162539da3be3c12f9ed56473b4ce9cd77125f3d24798569be2bf12017404a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.4 MB (205449389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de4d150b61ea4da45a81a3a39435fe8655d412c9b8988d975e39840a23cb94fc`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 22 Apr 2022 00:39:17 GMT
ADD file:bc2c78cc62a5e94931f8bd76f2fa050b19598c050fc18aa56bbd202826ec784b in / 
# Fri, 22 Apr 2022 00:39:19 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 01:30:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 01:31:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 22 Apr 2022 01:31:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 01:34:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:18c1f746bcbccc4e7599497df0d1d562571c9ecd9effcfb7bee0bbe17d1156b5`  
		Last Modified: Tue, 19 Apr 2022 13:12:34 GMT  
		Size: 25.4 MB (25365079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8405e5ec3de7029a8d9e579e70b8ad1e1c0c54178d2bceeddbddd9891f208caf`  
		Last Modified: Fri, 22 Apr 2022 01:50:36 GMT  
		Size: 6.3 MB (6332722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75f8f2095b8a73b68dac155f8b672164e44e681428870a909eb95d1bbadfd2d`  
		Last Modified: Fri, 22 Apr 2022 01:50:36 GMT  
		Size: 3.0 MB (2975175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef53d077886666b6b48b25300b869d8cf8d6cdbaf6ce678b6e3eb7cbaf4f6f2b`  
		Last Modified: Fri, 22 Apr 2022 01:50:52 GMT  
		Size: 45.0 MB (45029759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc59c864ceb06976ef97deb5f42391efe562e50e6abe62f40345ed18b8391425`  
		Last Modified: Fri, 22 Apr 2022 01:51:19 GMT  
		Size: 125.7 MB (125746654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
