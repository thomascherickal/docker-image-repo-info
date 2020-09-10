## `buildpack-deps:testing`

```console
$ docker pull buildpack-deps@sha256:986eee1095e3587b6e26745baef96407bdca2c509db25662218e6901d34f4e04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:testing` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:974ec0e20190521375a9bfdb4664d1b604c035d8f931e507d56d3d973441ac84
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.5 MB (327468962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1299eb4e60a4ccb47277649259e36bd27e336cf06fa67b5bb4778d79a289c257`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 10 Sep 2020 00:20:54 GMT
ADD file:375c01cd4aba0ddf77202decfeed5df5e3119ce460fcbf1f3b47f540a70b3864 in / 
# Thu, 10 Sep 2020 00:20:55 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:57:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:57:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 00:57:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:58:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:08d7334100fee80149028a0d0df44589b68e0c31592157808d18b68e6a572fd3`  
		Last Modified: Thu, 10 Sep 2020 00:33:04 GMT  
		Size: 51.9 MB (51906528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e2cbaa6fb6571d6e6f88e645061abb7c64ad18e76e900e6cfd8b80c5b36e84`  
		Last Modified: Thu, 10 Sep 2020 01:14:04 GMT  
		Size: 7.9 MB (7866624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70f330112cba767d415d7e4179b0dd52578b7685d2984ac61d9c3ba0884843a`  
		Last Modified: Thu, 10 Sep 2020 01:14:05 GMT  
		Size: 10.6 MB (10628764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a512e8a3ad92fa17f1debc71fe57ac4b49e1ffd4b1b80b5b847f6d5e48df83`  
		Last Modified: Thu, 10 Sep 2020 01:14:22 GMT  
		Size: 59.0 MB (59022579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab576645e0af6e13ec22468374b13f52110c182d9b622b69dc0b26559cb8b35`  
		Last Modified: Thu, 10 Sep 2020 01:15:12 GMT  
		Size: 198.0 MB (198044467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:0c49f98a38da35f9170dd61c401ce016cd4e6a7bf22dae1df1f77a792ba1323a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.8 MB (304792764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dc1a9c0bc89acefffd8355057f5dbff9abf2178c7bfa8aa035757ebfacf861a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:52:26 GMT
ADD file:f71e0d87d6d096130aa8dce14ce4db75b3a50725e9ba2aaab46f722a444291c9 in / 
# Wed, 09 Sep 2020 23:52:28 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:26:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:27:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 00:28:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:31:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:23e3aed2d466532e16ed7a54a2dc8d1ab497d8cd849573a7aa149e39f499eb77`  
		Last Modified: Thu, 10 Sep 2020 00:01:42 GMT  
		Size: 49.9 MB (49868299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57296d1a05acc9b2b6a146828bc5cd73f18a33087981038e29d2911236360b77`  
		Last Modified: Thu, 10 Sep 2020 00:51:46 GMT  
		Size: 7.4 MB (7444028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf329ff0c0ac4aa69298e3dae2a5539c0c7f11957ec83f3ae34b781fe1af258`  
		Last Modified: Thu, 10 Sep 2020 00:51:47 GMT  
		Size: 10.3 MB (10315041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3cadd83d92f88a8a5feb6e4917c4c36841c9e067f1bb16dd55109f787f57cc`  
		Last Modified: Thu, 10 Sep 2020 00:52:12 GMT  
		Size: 56.4 MB (56367974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb728b39421fa23655f111e5d3712042a92b0717645b6f502f2bc26ab56ef742`  
		Last Modified: Thu, 10 Sep 2020 00:53:09 GMT  
		Size: 180.8 MB (180797422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:ccdb8c27201aa03ee055107202fb3569aeb086ca6a9c3a63bb49ff6f1fee4902
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **291.1 MB (291064530 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2418cd5db3846c2314b2620b518a1b4390807ef2a05d535117dcf7793a4a7240`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 10 Sep 2020 00:06:19 GMT
ADD file:1cf6aad11149d2248c2d64e694eea8993365bc92e69acb766de8eed5ff5ea516 in / 
# Thu, 10 Sep 2020 00:06:24 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 01:34:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 01:34:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 01:35:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 01:38:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d74d0dbf37b1422ef3ad4850d0d2337a00c1b3b940052b8328d43b006d7cac98`  
		Last Modified: Thu, 10 Sep 2020 00:16:52 GMT  
		Size: 47.6 MB (47622633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39be7872e432bb84dd6799e4f7aea36b8e63f90690ab9a44e04241ca2c86b8cd`  
		Last Modified: Thu, 10 Sep 2020 02:00:02 GMT  
		Size: 7.2 MB (7184503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba87750aacaf06d58ec51afa56e4906f26eb6e094675669d666733b31b9313be`  
		Last Modified: Thu, 10 Sep 2020 02:00:03 GMT  
		Size: 10.0 MB (9959100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b151654e46e69be96bffc92ab40bf87d534d6125cea216288fc9486abd79d2`  
		Last Modified: Thu, 10 Sep 2020 02:00:29 GMT  
		Size: 53.9 MB (53939558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cdbbffb4a24fd4dee74f8fa7f3f09eb6b091acc8ec1bbbc8436d9adbd28b03d`  
		Last Modified: Thu, 10 Sep 2020 02:01:27 GMT  
		Size: 172.4 MB (172358736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:fcfdafa95417d6dc7ab6def1685cc483a19edb4d44a96dd1cf9ed6bb275db6a8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.1 MB (318142077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1024db947d7cf271f5f0339c00c1722483211eb259c6b0e78500f96060c3435d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:49:11 GMT
ADD file:82c33a26fb9be3ddaf17956539af2b205bdb6e28fe5ff1c7304ae8f294fe9581 in / 
# Wed, 09 Sep 2020 23:49:14 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:24:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:24:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 00:25:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:28:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5a65667356fa05b061c6733c879afab36ec44c6877341c2527e321b7206a26b2`  
		Last Modified: Wed, 09 Sep 2020 23:58:05 GMT  
		Size: 50.8 MB (50825395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:730279b4ebb859065c90bbf90b3ac77059bd7d1e6cdc143106e0994dca9f4c59`  
		Last Modified: Thu, 10 Sep 2020 00:40:35 GMT  
		Size: 7.7 MB (7743447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a2c8b657c8d1b22dc8f6d15821f7035a315a0900f84b26ef36c86803feb02c`  
		Last Modified: Thu, 10 Sep 2020 00:40:35 GMT  
		Size: 10.6 MB (10635675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c8357b95e1bce3c0d061d88bd56a0cbc03afe5af4f86cdd0057650adee23ef`  
		Last Modified: Thu, 10 Sep 2020 00:41:30 GMT  
		Size: 59.3 MB (59260366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25c09ac3d1e1ab5b6669b347445ae0a7a219b9cd0553332077f30aeec31137bc`  
		Last Modified: Thu, 10 Sep 2020 00:42:25 GMT  
		Size: 189.7 MB (189677194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; 386

```console
$ docker pull buildpack-deps@sha256:b6fd0a7f88e05afd3058a17e8243aca7b8cce37ac43e79eaaf92c1ae09165905
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.0 MB (336984462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e9cc1d46ca51d5fdac1c5a4636bf3948d4ea449a9784aa83f8315cf0592ac60`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:39:17 GMT
ADD file:f37f3bb35b6cca1cef993e4f39f48aab88ed76e0c47d97d61b4329fd8c5c5d03 in / 
# Wed, 09 Sep 2020 23:39:17 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 01:47:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 01:47:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 01:48:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 01:49:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4e5adf65093f5c6d699308a44f2173fac564be9f4e4daf24d82204c617b438d5`  
		Last Modified: Wed, 09 Sep 2020 23:45:45 GMT  
		Size: 53.0 MB (52969189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6830211bac3c1325ba53a3a4581992aa1d1916adf979c416833a3e9c0e9f24`  
		Last Modified: Thu, 10 Sep 2020 02:10:09 GMT  
		Size: 8.0 MB (8040370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf7dd281614cde829dde09a35d83f8a4fa325cab69fafac8dba60a7b8950cae3`  
		Last Modified: Thu, 10 Sep 2020 02:10:09 GMT  
		Size: 11.0 MB (11013589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08863d0a092f025c74c2a9e8e76db66b3097078722465f8c26eebaa59a4772bb`  
		Last Modified: Thu, 10 Sep 2020 02:10:43 GMT  
		Size: 61.0 MB (60997607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4efeba3e86781b301d25a0ca0ffdc29e78eacc14c9eec2461102d1ef994bd378`  
		Last Modified: Thu, 10 Sep 2020 02:12:00 GMT  
		Size: 204.0 MB (203963707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:232a65d9c6fd7d07101e6470c9f5d3ada8dee186cbca6a31deec7cd62cdc37b9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.3 MB (328329968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f040f641ccdddad298e18338ba80ff60c0d442cc7bc49ce07fee9fef24b5b8d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 06:41:13 GMT
ADD file:9e3d31545fae8b44e8aa3ad24629d2336276c01e23dfbdde9885d01e61a54298 in / 
# Tue, 04 Aug 2020 06:41:14 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 10:33:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 10:34:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 10:35:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 00:10:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:249c58d6beef4ec2d380f0e2adf7ea99a80c295cddcf6f6bc3d6b463dfe44a05`  
		Last Modified: Tue, 04 Aug 2020 06:46:35 GMT  
		Size: 50.6 MB (50550783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:049f809de28cc8d8e169ab9ee5721613f58fafdc670bbe6d66a1058fe998ee06`  
		Last Modified: Tue, 04 Aug 2020 10:47:30 GMT  
		Size: 7.5 MB (7450522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d557e2093dc94091a8f931745b728c83f35ad977f14de65f1ec5db00bedf8580`  
		Last Modified: Tue, 04 Aug 2020 10:47:30 GMT  
		Size: 10.6 MB (10599039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748d597a52166ec3c0e83e53c0b933c57f9230d87fbc629e0c1fb4c68970dec8`  
		Last Modified: Tue, 04 Aug 2020 10:48:22 GMT  
		Size: 56.0 MB (55973336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfc999e7d7fd4c3ced516367f51379b9dace7c2210c5fe087d53d0b39673608`  
		Last Modified: Tue, 01 Sep 2020 00:18:21 GMT  
		Size: 203.8 MB (203756288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:0a0573021f5de12c129e6debf246f40aeb2e2b81830127638eb5e8f7cae65d18
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **342.8 MB (342750136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c7279f49363261b6a8327ac4bc6c150aa38b84e940650cb233208f079e0c97e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 10 Sep 2020 00:54:23 GMT
ADD file:4529de4df0d9d1d1c2fc4ea683021e7ff678a24ca45c21d9dfaeb7c4dc1da51f in / 
# Thu, 10 Sep 2020 00:54:39 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 02:03:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 02:05:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 02:12:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 02:53:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6146fe38f8409e50a43aec229f36623c0f8c195d2cdf9bad02573a9d952a31a1`  
		Last Modified: Thu, 10 Sep 2020 01:23:23 GMT  
		Size: 55.8 MB (55774504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be50b08123b1849db4a42098bf6c8ac1fa2b4b66f3529542c22e6ebd32daaf8`  
		Last Modified: Thu, 10 Sep 2020 04:03:25 GMT  
		Size: 8.3 MB (8295948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc42e2c525916d192694c8773ed6f0bf7a72f3fa13d751e4087189acf6827c6`  
		Last Modified: Thu, 10 Sep 2020 04:03:24 GMT  
		Size: 11.4 MB (11389924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9ab50161d442dcd0b65170374cda4a3a14daffa715865256250897962df11df`  
		Last Modified: Thu, 10 Sep 2020 04:05:25 GMT  
		Size: 64.7 MB (64690217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab7be67f7424cb87215dc5c7560cb309e1a8ace688b3b3109f2cba899dde4d2`  
		Last Modified: Thu, 10 Sep 2020 04:09:36 GMT  
		Size: 202.6 MB (202599543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:a5cd08af63b87b0c0b469701744746d92cb51d9780b0387e9f9d2cdd9f0d5c8f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.5 MB (305477181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1b0b7fb20e7a7e6d8f01ff31ed867645dc63dbde2c07d3a4542884cb31bc1bf`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:41:38 GMT
ADD file:d30705fcc57734260b517d32c4d610f1fe18e7d5faa78a22754774f5bf15eb9a in / 
# Wed, 09 Sep 2020 23:41:41 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:03:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:04:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 00:04:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:06:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b7fac0c9089d6ff39f6a7de3af657a8d580a7b074b45118b115539fd90213654`  
		Last Modified: Wed, 09 Sep 2020 23:45:45 GMT  
		Size: 50.5 MB (50468550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e4abf36c400373c14e1dc03dc7d41c9bb01249ef118a39b67294471b0cea9d`  
		Last Modified: Thu, 10 Sep 2020 00:11:24 GMT  
		Size: 7.5 MB (7537717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c291ff634945f7dc165f540d95c5d3958483aba31d45fbae0ee30d37ef13ca7`  
		Last Modified: Thu, 10 Sep 2020 00:11:25 GMT  
		Size: 10.5 MB (10504927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6369fe3859abc7090769cdf547264b790f6a68071ae32f9e9cc6ae6002948f10`  
		Last Modified: Thu, 10 Sep 2020 00:11:39 GMT  
		Size: 58.2 MB (58230238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d366617311fb83c07081328602eaff47174c41add63c01aef83ebcd87843eb6e`  
		Last Modified: Thu, 10 Sep 2020 00:12:06 GMT  
		Size: 178.7 MB (178735749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
