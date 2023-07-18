<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `buildpack-deps`

-	[`buildpack-deps:20.04`](#buildpack-deps2004)
-	[`buildpack-deps:20.04-curl`](#buildpack-deps2004-curl)
-	[`buildpack-deps:20.04-scm`](#buildpack-deps2004-scm)
-	[`buildpack-deps:22.04`](#buildpack-deps2204)
-	[`buildpack-deps:22.04-curl`](#buildpack-deps2204-curl)
-	[`buildpack-deps:22.04-scm`](#buildpack-deps2204-scm)
-	[`buildpack-deps:22.10`](#buildpack-deps2210)
-	[`buildpack-deps:22.10-curl`](#buildpack-deps2210-curl)
-	[`buildpack-deps:22.10-scm`](#buildpack-deps2210-scm)
-	[`buildpack-deps:23.04`](#buildpack-deps2304)
-	[`buildpack-deps:23.04-curl`](#buildpack-deps2304-curl)
-	[`buildpack-deps:23.04-scm`](#buildpack-deps2304-scm)
-	[`buildpack-deps:23.10`](#buildpack-deps2310)
-	[`buildpack-deps:23.10-curl`](#buildpack-deps2310-curl)
-	[`buildpack-deps:23.10-scm`](#buildpack-deps2310-scm)
-	[`buildpack-deps:bookworm`](#buildpack-depsbookworm)
-	[`buildpack-deps:bookworm-curl`](#buildpack-depsbookworm-curl)
-	[`buildpack-deps:bookworm-scm`](#buildpack-depsbookworm-scm)
-	[`buildpack-deps:bullseye`](#buildpack-depsbullseye)
-	[`buildpack-deps:bullseye-curl`](#buildpack-depsbullseye-curl)
-	[`buildpack-deps:bullseye-scm`](#buildpack-depsbullseye-scm)
-	[`buildpack-deps:buster`](#buildpack-depsbuster)
-	[`buildpack-deps:buster-curl`](#buildpack-depsbuster-curl)
-	[`buildpack-deps:buster-scm`](#buildpack-depsbuster-scm)
-	[`buildpack-deps:curl`](#buildpack-depscurl)
-	[`buildpack-deps:focal`](#buildpack-depsfocal)
-	[`buildpack-deps:focal-curl`](#buildpack-depsfocal-curl)
-	[`buildpack-deps:focal-scm`](#buildpack-depsfocal-scm)
-	[`buildpack-deps:jammy`](#buildpack-depsjammy)
-	[`buildpack-deps:jammy-curl`](#buildpack-depsjammy-curl)
-	[`buildpack-deps:jammy-scm`](#buildpack-depsjammy-scm)
-	[`buildpack-deps:kinetic`](#buildpack-depskinetic)
-	[`buildpack-deps:kinetic-curl`](#buildpack-depskinetic-curl)
-	[`buildpack-deps:kinetic-scm`](#buildpack-depskinetic-scm)
-	[`buildpack-deps:latest`](#buildpack-depslatest)
-	[`buildpack-deps:lunar`](#buildpack-depslunar)
-	[`buildpack-deps:lunar-curl`](#buildpack-depslunar-curl)
-	[`buildpack-deps:lunar-scm`](#buildpack-depslunar-scm)
-	[`buildpack-deps:mantic`](#buildpack-depsmantic)
-	[`buildpack-deps:mantic-curl`](#buildpack-depsmantic-curl)
-	[`buildpack-deps:mantic-scm`](#buildpack-depsmantic-scm)
-	[`buildpack-deps:oldoldstable`](#buildpack-depsoldoldstable)
-	[`buildpack-deps:oldoldstable-curl`](#buildpack-depsoldoldstable-curl)
-	[`buildpack-deps:oldoldstable-scm`](#buildpack-depsoldoldstable-scm)
-	[`buildpack-deps:oldstable`](#buildpack-depsoldstable)
-	[`buildpack-deps:oldstable-curl`](#buildpack-depsoldstable-curl)
-	[`buildpack-deps:oldstable-scm`](#buildpack-depsoldstable-scm)
-	[`buildpack-deps:scm`](#buildpack-depsscm)
-	[`buildpack-deps:sid`](#buildpack-depssid)
-	[`buildpack-deps:sid-curl`](#buildpack-depssid-curl)
-	[`buildpack-deps:sid-scm`](#buildpack-depssid-scm)
-	[`buildpack-deps:stable`](#buildpack-depsstable)
-	[`buildpack-deps:stable-curl`](#buildpack-depsstable-curl)
-	[`buildpack-deps:stable-scm`](#buildpack-depsstable-scm)
-	[`buildpack-deps:unstable`](#buildpack-depsunstable)
-	[`buildpack-deps:unstable-curl`](#buildpack-depsunstable-curl)
-	[`buildpack-deps:unstable-scm`](#buildpack-depsunstable-scm)

## `buildpack-deps:20.04`

```console
$ docker pull buildpack-deps@sha256:a185db68283db441b7051eb46a43aeb48529a876fa53a19aea0fc2eaf8adb22c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:20.04` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:c7c9e01f525b7b71c896947f93c1886f61cf600947fe9c6f52bb89306e9d837c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.7 MB (245713038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4fdc424c21a7faa2bb99b875d2ce47d52685d1f0692f07b0f4ae504cdab83c3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:59:08 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:59:08 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:59:10 GMT
ADD file:12f97b7b044d0d1166dd59408c67f5610a764127aa8a01bc57db23bee48911af in / 
# Wed, 28 Jun 2023 09:59:10 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 03:35:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:36:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:39:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0fb668748fc8bb961f4580895692ae741be788857ac2e8220adc2265ffb38e10`  
		Last Modified: Wed, 28 Jun 2023 18:43:28 GMT  
		Size: 28.6 MB (28580012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de25fa69197a0fe88312b7c08a3a8c96d4062222b035243751e6b307e1087e46`  
		Last Modified: Tue, 04 Jul 2023 03:54:52 GMT  
		Size: 11.1 MB (11129679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02e98539424ab3fee447b177cb642cceab5a0f5bcc7ac4658a3199d8a2efe22`  
		Last Modified: Tue, 04 Jul 2023 03:55:11 GMT  
		Size: 60.9 MB (60915116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10814cb888f2d0dc3b2fd0b1086cf83dffd5b89704534a791348878994befe3a`  
		Last Modified: Tue, 04 Jul 2023 03:55:39 GMT  
		Size: 145.1 MB (145088231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:93218030091d490ac3709f8ca1b26d36a56614c26e83306fce917bc01b3d5b9d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.9 MB (211948612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6217c3d30436343fdbea1735e914455a8eef4374a3879019fc7a6153849ebce`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:58:19 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:58:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:58:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:58:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:58:22 GMT
ADD file:8bedca16bf416520f5df29175a99b07585281465c459544b9f9679016f59762a in / 
# Wed, 28 Jun 2023 09:58:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 05:58:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:59:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:02:59 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:06e53fabee8df31622850c604f9242a52a466ec4eb75320019bdfdc8ec311692`  
		Last Modified: Tue, 04 Jul 2023 06:22:20 GMT  
		Size: 24.6 MB (24588135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7655bda15200da93eaa77218c915efbf215e822d3a7ef693f5fbc78a94b8e906`  
		Last Modified: Tue, 04 Jul 2023 06:22:17 GMT  
		Size: 9.6 MB (9599087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bf5309ca27fafde797ae93665faceb2bf2d10325336e4a2004fad3ea3a3928`  
		Last Modified: Tue, 04 Jul 2023 06:22:38 GMT  
		Size: 55.8 MB (55826315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60345e5479f7c8f72ad47b6401099a23948d09f83264bf4fbd7a1c5b8a8b120b`  
		Last Modified: Tue, 04 Jul 2023 06:23:07 GMT  
		Size: 121.9 MB (121935075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d643b544b4d5c4c222904b1995d0d52f516df830f01583a13eecaf761e02aadd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.0 MB (235966654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cf414eb726738eb2bed47de53bc51399a1a8044efc47ea93ff22a1feac978bf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:54:46 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:54:46 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:54:48 GMT
ADD file:a6db9f7789e57b7119f68e4e4ec9ec5aab8c3c8bd53fd932f3c59c54b1c20a26 in / 
# Wed, 28 Jun 2023 09:54:49 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 06:01:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:02:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:05:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1e77eb131c5c9032ce8e6e512f601714ce7ba48e296f5b7a5191703bdcbc904d`  
		Last Modified: Tue, 04 Jul 2023 04:05:23 GMT  
		Size: 27.2 MB (27198330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ae43f445a875bd258928e514043770667dbc9ab823c2a244e3c8d2fb4520ad`  
		Last Modified: Tue, 04 Jul 2023 06:24:04 GMT  
		Size: 11.0 MB (10982532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf4e8446ca8d143e3e482c4d70cf26e4702ff9b4e40c36c27fc3dd2a3c27c556`  
		Last Modified: Tue, 04 Jul 2023 06:24:19 GMT  
		Size: 61.0 MB (61006780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bc3cd52da7ce05900d047fd4cda3ce90636414f72af90486f6e969e2d2f6b0`  
		Last Modified: Tue, 04 Jul 2023 06:24:41 GMT  
		Size: 136.8 MB (136779012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:cc828381ce76a725b9d89f134a8d0cfa74d055174d4575477f34a423c98ea367
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.5 MB (269491158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbd8a25659464d102bb1ecbe6cc4007a51d569800d490f7ee98b20f4430850ac`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 10:04:43 GMT
ARG RELEASE
# Wed, 28 Jun 2023 10:04:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 10:04:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 10:04:43 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 10:04:46 GMT
ADD file:df651ead0b69eb261098e765354dbdf5ffca51275c037d8881fedcaa1c91c36d in / 
# Wed, 28 Jun 2023 10:04:46 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 03:40:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:42:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:52:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4e95615eadb7a0d90a47ca15a5c0693371494902f54d8d78a50d53e89e7a20de`  
		Last Modified: Tue, 04 Jul 2023 04:40:49 GMT  
		Size: 33.3 MB (33308759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276026532e2897addfb94053c99fabaff128631b0106992fca31995a4e07ee2f`  
		Last Modified: Tue, 04 Jul 2023 04:40:45 GMT  
		Size: 12.9 MB (12937997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f779e3d18cc00d1bfffc494a86c621971575cc7b49852f3e69213662057902`  
		Last Modified: Tue, 04 Jul 2023 04:41:19 GMT  
		Size: 69.6 MB (69626921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e13418b66e9f4c1f9d947e9d444eb0fb640256ac2ee6d0a41723d673cf1b16`  
		Last Modified: Tue, 04 Jul 2023 04:42:10 GMT  
		Size: 153.6 MB (153617481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:580cefb616a99fcf46bb964c69f12ed5649224e80a0008d94866de16639a35ea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.4 MB (226422472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cf7de8cb660b68cf94254f5b979338baf341742f41e919e60ccae14144fdd64`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 10:01:13 GMT
ARG RELEASE
# Wed, 28 Jun 2023 10:01:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 10:01:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 10:01:14 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 10:01:15 GMT
ADD file:777fd71e798b91bf768b21e1ca4403f388db9936ef55ef68b4b019cb167fa707 in / 
# Wed, 28 Jun 2023 10:01:15 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 12:51:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 12:52:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 12:54:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f5ebe8481b30a6d3b710b0efdec29843cca805811e3be1a4e375761725c40e5a`  
		Last Modified: Tue, 04 Jul 2023 13:07:41 GMT  
		Size: 27.0 MB (27013645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e76df5c29baf17b24cc9ec09debb6341e7d2b72276cb8ded9c6f9b91e2c3c457`  
		Last Modified: Tue, 04 Jul 2023 13:07:39 GMT  
		Size: 10.7 MB (10688202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d32cf23175b375841e6e543d986dd4143c7fffdb28041799bded0d024fec5d7`  
		Last Modified: Tue, 04 Jul 2023 13:07:56 GMT  
		Size: 60.3 MB (60306044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56679d2cc4435a4de5a03dc496c0e2a79d465112d7a7c30997f027f96e1154a`  
		Last Modified: Tue, 04 Jul 2023 13:08:19 GMT  
		Size: 128.4 MB (128414581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:20.04-curl`

```console
$ docker pull buildpack-deps@sha256:7ac75c83428eead00cdc790f512da48b07fc284c70f6dc20c1e8de6c094c5076
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:20.04-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:29349b0eaca1f8811a3d7d38a9846ab3314f69a804183b6e90a44aa3770e6fb2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.7 MB (39709691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb7221a59874eaac8926a513c75cfa4b39d8bf1d7d8e7c901e1896ef56bf7fbb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:59:08 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:59:08 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:59:10 GMT
ADD file:12f97b7b044d0d1166dd59408c67f5610a764127aa8a01bc57db23bee48911af in / 
# Wed, 28 Jun 2023 09:59:10 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 03:35:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0fb668748fc8bb961f4580895692ae741be788857ac2e8220adc2265ffb38e10`  
		Last Modified: Wed, 28 Jun 2023 18:43:28 GMT  
		Size: 28.6 MB (28580012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de25fa69197a0fe88312b7c08a3a8c96d4062222b035243751e6b307e1087e46`  
		Last Modified: Tue, 04 Jul 2023 03:54:52 GMT  
		Size: 11.1 MB (11129679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:0303a169ab81f1dd2dcd58af96b0874f72e751171dcd991e2d77d1e7e92b34bb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.2 MB (34187222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f37c50d81dcfa785320e75ef3b32c0ee9dae56393ee924c9005dd45710e8ddba`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:58:19 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:58:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:58:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:58:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:58:22 GMT
ADD file:8bedca16bf416520f5df29175a99b07585281465c459544b9f9679016f59762a in / 
# Wed, 28 Jun 2023 09:58:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 05:58:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:06e53fabee8df31622850c604f9242a52a466ec4eb75320019bdfdc8ec311692`  
		Last Modified: Tue, 04 Jul 2023 06:22:20 GMT  
		Size: 24.6 MB (24588135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7655bda15200da93eaa77218c915efbf215e822d3a7ef693f5fbc78a94b8e906`  
		Last Modified: Tue, 04 Jul 2023 06:22:17 GMT  
		Size: 9.6 MB (9599087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:2c0578c721a498af48cd9ef0884245d87b60ef60dd0a1f08d13b8ad59dfc24c2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38180862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05adb6402d4b50ffe9531fcbf9bc27b370c6736ee6bff914e4c2831eea2588c9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:54:46 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:54:46 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:54:48 GMT
ADD file:a6db9f7789e57b7119f68e4e4ec9ec5aab8c3c8bd53fd932f3c59c54b1c20a26 in / 
# Wed, 28 Jun 2023 09:54:49 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 06:01:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1e77eb131c5c9032ce8e6e512f601714ce7ba48e296f5b7a5191703bdcbc904d`  
		Last Modified: Tue, 04 Jul 2023 04:05:23 GMT  
		Size: 27.2 MB (27198330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ae43f445a875bd258928e514043770667dbc9ab823c2a244e3c8d2fb4520ad`  
		Last Modified: Tue, 04 Jul 2023 06:24:04 GMT  
		Size: 11.0 MB (10982532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:ebda49b806b5084f69baf79430dc3b5d2b8bb4631404e64e4c0f786e269e465c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.2 MB (46246756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fdf46f3154cdfb9e896f4ee40532dbbe0b2abd9fb58f55aff17d4b11dd6aebf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 10:04:43 GMT
ARG RELEASE
# Wed, 28 Jun 2023 10:04:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 10:04:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 10:04:43 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 10:04:46 GMT
ADD file:df651ead0b69eb261098e765354dbdf5ffca51275c037d8881fedcaa1c91c36d in / 
# Wed, 28 Jun 2023 10:04:46 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 03:40:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4e95615eadb7a0d90a47ca15a5c0693371494902f54d8d78a50d53e89e7a20de`  
		Last Modified: Tue, 04 Jul 2023 04:40:49 GMT  
		Size: 33.3 MB (33308759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276026532e2897addfb94053c99fabaff128631b0106992fca31995a4e07ee2f`  
		Last Modified: Tue, 04 Jul 2023 04:40:45 GMT  
		Size: 12.9 MB (12937997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:a1a74cd349bbde56ebcc8338244ffbe81f589de4017b9e4804563da5551adc4f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37701847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8de47ab95f94694c1633d536a99595b02886af13b8c51cc75b5f5afcc9b17e98`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 10:01:13 GMT
ARG RELEASE
# Wed, 28 Jun 2023 10:01:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 10:01:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 10:01:14 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 10:01:15 GMT
ADD file:777fd71e798b91bf768b21e1ca4403f388db9936ef55ef68b4b019cb167fa707 in / 
# Wed, 28 Jun 2023 10:01:15 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 12:51:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f5ebe8481b30a6d3b710b0efdec29843cca805811e3be1a4e375761725c40e5a`  
		Last Modified: Tue, 04 Jul 2023 13:07:41 GMT  
		Size: 27.0 MB (27013645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e76df5c29baf17b24cc9ec09debb6341e7d2b72276cb8ded9c6f9b91e2c3c457`  
		Last Modified: Tue, 04 Jul 2023 13:07:39 GMT  
		Size: 10.7 MB (10688202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:20.04-scm`

```console
$ docker pull buildpack-deps@sha256:cf75c25ab50018af643899159854d52e05aeeb25dc53c2728a16b5ea7ea40a4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:20.04-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:273eb870a63a22e195a285cb24188c8ed3a97fb62309d8a4f27b6027c040928f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.6 MB (100624807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87826ce481cf6aeaf241e717c398c87ff39180797900c7007e6808e03fab8921`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:59:08 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:59:08 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:59:10 GMT
ADD file:12f97b7b044d0d1166dd59408c67f5610a764127aa8a01bc57db23bee48911af in / 
# Wed, 28 Jun 2023 09:59:10 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 03:35:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:36:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0fb668748fc8bb961f4580895692ae741be788857ac2e8220adc2265ffb38e10`  
		Last Modified: Wed, 28 Jun 2023 18:43:28 GMT  
		Size: 28.6 MB (28580012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de25fa69197a0fe88312b7c08a3a8c96d4062222b035243751e6b307e1087e46`  
		Last Modified: Tue, 04 Jul 2023 03:54:52 GMT  
		Size: 11.1 MB (11129679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02e98539424ab3fee447b177cb642cceab5a0f5bcc7ac4658a3199d8a2efe22`  
		Last Modified: Tue, 04 Jul 2023 03:55:11 GMT  
		Size: 60.9 MB (60915116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:6375f2580b96022d4e2a789ebdb9260867c8f5ed0ecb27617d0f77093c37460d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.0 MB (90013537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d00851b856224282b6ead89b40dcd53b77538aec6d069855dea50a5297ceda2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:58:19 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:58:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:58:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:58:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:58:22 GMT
ADD file:8bedca16bf416520f5df29175a99b07585281465c459544b9f9679016f59762a in / 
# Wed, 28 Jun 2023 09:58:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 05:58:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:59:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:06e53fabee8df31622850c604f9242a52a466ec4eb75320019bdfdc8ec311692`  
		Last Modified: Tue, 04 Jul 2023 06:22:20 GMT  
		Size: 24.6 MB (24588135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7655bda15200da93eaa77218c915efbf215e822d3a7ef693f5fbc78a94b8e906`  
		Last Modified: Tue, 04 Jul 2023 06:22:17 GMT  
		Size: 9.6 MB (9599087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bf5309ca27fafde797ae93665faceb2bf2d10325336e4a2004fad3ea3a3928`  
		Last Modified: Tue, 04 Jul 2023 06:22:38 GMT  
		Size: 55.8 MB (55826315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:9e3ca944812a58a43d49c9389e13da1888d89316938b46ade73769204e83877c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99187642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf051e6d28b3c08f77351d519508701a4cc2b452556275a4ec5249d1dff91fb8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:54:46 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:54:46 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:54:48 GMT
ADD file:a6db9f7789e57b7119f68e4e4ec9ec5aab8c3c8bd53fd932f3c59c54b1c20a26 in / 
# Wed, 28 Jun 2023 09:54:49 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 06:01:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:02:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1e77eb131c5c9032ce8e6e512f601714ce7ba48e296f5b7a5191703bdcbc904d`  
		Last Modified: Tue, 04 Jul 2023 04:05:23 GMT  
		Size: 27.2 MB (27198330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ae43f445a875bd258928e514043770667dbc9ab823c2a244e3c8d2fb4520ad`  
		Last Modified: Tue, 04 Jul 2023 06:24:04 GMT  
		Size: 11.0 MB (10982532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf4e8446ca8d143e3e482c4d70cf26e4702ff9b4e40c36c27fc3dd2a3c27c556`  
		Last Modified: Tue, 04 Jul 2023 06:24:19 GMT  
		Size: 61.0 MB (61006780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:83bc9f99ef1a1d5eae5dc903bba37c760a0360920680682a5fafb3add76595c8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.9 MB (115873677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9a6dfad5115f5ece291290e14905952c3f87983f65565590978f5b4f04d59cb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 10:04:43 GMT
ARG RELEASE
# Wed, 28 Jun 2023 10:04:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 10:04:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 10:04:43 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 10:04:46 GMT
ADD file:df651ead0b69eb261098e765354dbdf5ffca51275c037d8881fedcaa1c91c36d in / 
# Wed, 28 Jun 2023 10:04:46 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 03:40:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:42:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4e95615eadb7a0d90a47ca15a5c0693371494902f54d8d78a50d53e89e7a20de`  
		Last Modified: Tue, 04 Jul 2023 04:40:49 GMT  
		Size: 33.3 MB (33308759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276026532e2897addfb94053c99fabaff128631b0106992fca31995a4e07ee2f`  
		Last Modified: Tue, 04 Jul 2023 04:40:45 GMT  
		Size: 12.9 MB (12937997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f779e3d18cc00d1bfffc494a86c621971575cc7b49852f3e69213662057902`  
		Last Modified: Tue, 04 Jul 2023 04:41:19 GMT  
		Size: 69.6 MB (69626921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:de8f76734b0c65cfa398d2ff4bbe8b0ffa917e8c1dff84edff6cf976da2bf84d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.0 MB (98007891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:771aca25ec8f105d9609f3e0abdbb6606b7b5f6217243c0ebf33378d8123b6a4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 10:01:13 GMT
ARG RELEASE
# Wed, 28 Jun 2023 10:01:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 10:01:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 10:01:14 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 10:01:15 GMT
ADD file:777fd71e798b91bf768b21e1ca4403f388db9936ef55ef68b4b019cb167fa707 in / 
# Wed, 28 Jun 2023 10:01:15 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 12:51:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 12:52:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f5ebe8481b30a6d3b710b0efdec29843cca805811e3be1a4e375761725c40e5a`  
		Last Modified: Tue, 04 Jul 2023 13:07:41 GMT  
		Size: 27.0 MB (27013645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e76df5c29baf17b24cc9ec09debb6341e7d2b72276cb8ded9c6f9b91e2c3c457`  
		Last Modified: Tue, 04 Jul 2023 13:07:39 GMT  
		Size: 10.7 MB (10688202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d32cf23175b375841e6e543d986dd4143c7fffdb28041799bded0d024fec5d7`  
		Last Modified: Tue, 04 Jul 2023 13:07:56 GMT  
		Size: 60.3 MB (60306044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.04`

```console
$ docker pull buildpack-deps@sha256:9b7ec77e64b6837e10968f9e2b0760af52fe7da4f66c1d008532f2bb80c0f1e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:22.04` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:8f28bd087741849791b564aea220968c88f2cace4063336681cd238858e05a79
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.8 MB (249847907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:442a35809fbea57170756e05e1a3bbb375ae8094fe1dbba784e092fd2935b0d5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 03:39:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:40:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:42:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97966f3f03442a3d645f8354f49cc622b4416879f6c59142fab244ca2663677b`  
		Last Modified: Tue, 04 Jul 2023 03:55:49 GMT  
		Size: 7.1 MB (7119871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e29c969f29843010dfda55528bfc810b4e577e4ba39fb2c788a8ea55bb92763`  
		Last Modified: Tue, 04 Jul 2023 03:56:05 GMT  
		Size: 39.4 MB (39428797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13d40b1da6010e8c9c1adb56fc6fb577c2db289f338cac71cc1c97fd28e6bdb`  
		Last Modified: Tue, 04 Jul 2023 03:56:35 GMT  
		Size: 172.9 MB (172868010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f84a66f57eb9a7526b7f1bb0427dd87c3672e42f677bb33bac7970d1c9ee6232
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.7 MB (216723569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2283fac8c756eddab693df3e3369926d3a93560b25cb7c61053ba83125fea69`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:41:15 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:41:15 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:41:15 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:41:15 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:41:18 GMT
ADD file:c13f43a31510c7a4eaa7e4ca90e4f973b19895658b1f9993cab5f93979d4e2dc in / 
# Wed, 28 Jun 2023 08:41:18 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 06:04:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:04:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:08:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:63b96265cfe95b9cec847027033d4226b783ecd042036f5c809a7386027f56b0`  
		Last Modified: Fri, 30 Jun 2023 02:08:02 GMT  
		Size: 27.0 MB (27026961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7ab0e6b76129c24867f4152f7c8da7289c6b5f4a0922ae184713f26945af72`  
		Last Modified: Tue, 04 Jul 2023 06:23:16 GMT  
		Size: 7.0 MB (7019201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78a55edb4070b31d77ce5a81d68e5d76539c587fdaf49d4e2a8b380e36371187`  
		Last Modified: Tue, 04 Jul 2023 06:23:36 GMT  
		Size: 42.2 MB (42222602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6038ce0ab4df67f1a1fb7fd041b97c4c222339ed93b979813ce2703dc8acbd9`  
		Last Modified: Tue, 04 Jul 2023 06:24:04 GMT  
		Size: 140.5 MB (140454805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:20528a086d9dc7bf09bc195454c032fa8d0576fd17267e5120c400ad0ab680e0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.2 MB (241179903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:761bc5ffd9cec06e5f9c4b6b62aac9f90e5db77fbf359088e2c3339804508de6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 06:06:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:07:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:10:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00483067c1437c60cceadf9b4d31783bc9e1adb93770b38287f24ef2943b3c0`  
		Last Modified: Tue, 04 Jul 2023 06:24:51 GMT  
		Size: 7.1 MB (7067072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c1fabd67ce9ecbf104292a6591b53f2a57503bf444faef66c672ca9017fc31`  
		Last Modified: Tue, 04 Jul 2023 06:25:03 GMT  
		Size: 39.3 MB (39345851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b86e59c87a49dd6808d4971ca94a4faea222b3461d58e99bbfb47b5505fd88`  
		Last Modified: Tue, 04 Jul 2023 06:25:28 GMT  
		Size: 166.4 MB (166375969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:36c2809c31013b604a1f6e752eb699bb2ed20f1ecad9ecba0ad16454e70315b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.7 MB (271695715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ed585ef780750325abbece0e460523e6e025223c2ca714512a7db9bd671b94f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:45:53 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:45:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:45:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:45:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:45:56 GMT
ADD file:8c2fc380378944326d602742fde0e30458cd3e82012847b0f7e09c7184bfd135 in / 
# Wed, 28 Jun 2023 08:45:57 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 03:54:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:57:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:07:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7faa46ce6b6f5c34485980029504c3995e38149d0bca67d8b976c5dbb3673644`  
		Last Modified: Tue, 04 Jul 2023 04:42:31 GMT  
		Size: 35.7 MB (35711469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5028dc76c028f10e8828b80e411d373e4db95e0d5232b4f5a0dde9146f46cf`  
		Last Modified: Tue, 04 Jul 2023 04:42:24 GMT  
		Size: 8.3 MB (8260592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e056faa463b64fc04b6eb21623bad5611901f025c629a92bcaf9337b98644f`  
		Last Modified: Tue, 04 Jul 2023 04:42:54 GMT  
		Size: 43.9 MB (43874959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496391575eedb44a7a5322b38c22ae05c7096680d5c21faa2f1793cd55852ac1`  
		Last Modified: Tue, 04 Jul 2023 04:43:51 GMT  
		Size: 183.8 MB (183848695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:df4cc2c63e69e5b07ee3466abb67396de15ed40b36e9e85e9cd80a17e7bf7bf6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.6 MB (223589120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0893b5590f1c90958e2f8a2b9b84d4a59ded9649b871d31c2014a5057e09d07f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:53:20 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:53:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:53:22 GMT
ADD file:fa0aef35be7808c8fd6751a52bdec4dd81057e2fcaa075c547a1db53640dae9a in / 
# Wed, 28 Jun 2023 08:53:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 12:55:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 12:55:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 12:57:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce02ee0330980398d6a84a50abfa1a8c4d1cba27cbd7442b79f4aa1b1a14020d`  
		Last Modified: Tue, 04 Jul 2023 13:08:30 GMT  
		Size: 28.6 MB (28645696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7aba4ce682de5293312667253fd0a7af53c579484786de09b36208aab9d22c`  
		Last Modified: Tue, 04 Jul 2023 13:08:26 GMT  
		Size: 7.0 MB (7033603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1c12ddc9521fd58bc71f4494c40a5c8889571901807762f83f2db5e8d7d6dc`  
		Last Modified: Tue, 04 Jul 2023 13:08:43 GMT  
		Size: 39.4 MB (39392616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6037f928a3a3f348ad27e66c8ef12e21545b65e48b071cbeeb2990c42fdcad97`  
		Last Modified: Tue, 04 Jul 2023 13:09:09 GMT  
		Size: 148.5 MB (148517205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.04-curl`

```console
$ docker pull buildpack-deps@sha256:1ec10719ed03e1ebeb0689d9af0543c4346cf37e8ba423bf4004b7dd3a350ba7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:22.04-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:483b82bc040102243b07bcbb2bb61e88294953b57782d2ee84dc0b81db449cc0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37551100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57a6f6f87887de69ba89a8eba29dd185ff073609b204037b4931d8322101cad3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 03:39:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97966f3f03442a3d645f8354f49cc622b4416879f6c59142fab244ca2663677b`  
		Last Modified: Tue, 04 Jul 2023 03:55:49 GMT  
		Size: 7.1 MB (7119871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:07e89f118c913b2585d650a226dc9954fc9951947e7926291adee70259dfd3f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34046162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c7a7f90ea62180724401b9d98d6cf69cdc58225b859ab44d433bc271d7e9560`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:41:15 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:41:15 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:41:15 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:41:15 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:41:18 GMT
ADD file:c13f43a31510c7a4eaa7e4ca90e4f973b19895658b1f9993cab5f93979d4e2dc in / 
# Wed, 28 Jun 2023 08:41:18 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 06:04:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:63b96265cfe95b9cec847027033d4226b783ecd042036f5c809a7386027f56b0`  
		Last Modified: Fri, 30 Jun 2023 02:08:02 GMT  
		Size: 27.0 MB (27026961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7ab0e6b76129c24867f4152f7c8da7289c6b5f4a0922ae184713f26945af72`  
		Last Modified: Tue, 04 Jul 2023 06:23:16 GMT  
		Size: 7.0 MB (7019201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:9a3b66500d95e556a3251f402d1a2cd06cf9a8d29812d76b179e6627d98c5a2f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 MB (35458083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:296393feca5c587e3328a58596b57de868f32b92cfbe7d8d3dd30578b8aa4e51`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 06:06:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00483067c1437c60cceadf9b4d31783bc9e1adb93770b38287f24ef2943b3c0`  
		Last Modified: Tue, 04 Jul 2023 06:24:51 GMT  
		Size: 7.1 MB (7067072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:a30f0fc4dd7363c101b3c0a6ddf8d05701c93d716bcfb3987a6440a256e02ef2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (43972061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66bb953f4cadc10c7aa36623450ee63de56159a9445d0ff555a886fd1cfa49ff`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:45:53 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:45:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:45:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:45:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:45:56 GMT
ADD file:8c2fc380378944326d602742fde0e30458cd3e82012847b0f7e09c7184bfd135 in / 
# Wed, 28 Jun 2023 08:45:57 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 03:54:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7faa46ce6b6f5c34485980029504c3995e38149d0bca67d8b976c5dbb3673644`  
		Last Modified: Tue, 04 Jul 2023 04:42:31 GMT  
		Size: 35.7 MB (35711469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5028dc76c028f10e8828b80e411d373e4db95e0d5232b4f5a0dde9146f46cf`  
		Last Modified: Tue, 04 Jul 2023 04:42:24 GMT  
		Size: 8.3 MB (8260592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:15dd98493e4ec64bad67c254e1518893e14856b6cc690172a22783584f2f914e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35679299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47ba8f5e175da4bc3069b45bf99ec082ea72d15c9e9924284125f1f00e92d24f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:53:20 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:53:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:53:22 GMT
ADD file:fa0aef35be7808c8fd6751a52bdec4dd81057e2fcaa075c547a1db53640dae9a in / 
# Wed, 28 Jun 2023 08:53:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 12:55:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce02ee0330980398d6a84a50abfa1a8c4d1cba27cbd7442b79f4aa1b1a14020d`  
		Last Modified: Tue, 04 Jul 2023 13:08:30 GMT  
		Size: 28.6 MB (28645696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7aba4ce682de5293312667253fd0a7af53c579484786de09b36208aab9d22c`  
		Last Modified: Tue, 04 Jul 2023 13:08:26 GMT  
		Size: 7.0 MB (7033603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.04-scm`

```console
$ docker pull buildpack-deps@sha256:f8d47bd7614fb9021e6e796abc17af03eabd4eb05bd18824ba436ff80c1acdfd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:22.04-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:c79e22f6262ffcc9eb5eee479f1728247ee7c37e1419034d7ef047a9cd8b649f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76979897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4da96a2a7c92bf335b49390e599ef90eeedbad15d69f1c2f3bac70574468ac75`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 03:39:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:40:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97966f3f03442a3d645f8354f49cc622b4416879f6c59142fab244ca2663677b`  
		Last Modified: Tue, 04 Jul 2023 03:55:49 GMT  
		Size: 7.1 MB (7119871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e29c969f29843010dfda55528bfc810b4e577e4ba39fb2c788a8ea55bb92763`  
		Last Modified: Tue, 04 Jul 2023 03:56:05 GMT  
		Size: 39.4 MB (39428797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:57bbae5325f47855ffd8c210e1d028f7d0b6100f91d555c8e12439d8b5eb447a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.3 MB (76268764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:733e20783ce4aabcb2e52abd12bf08f9433f8727787cdaccf590511d8a51f0b8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:41:15 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:41:15 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:41:15 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:41:15 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:41:18 GMT
ADD file:c13f43a31510c7a4eaa7e4ca90e4f973b19895658b1f9993cab5f93979d4e2dc in / 
# Wed, 28 Jun 2023 08:41:18 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 06:04:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:04:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:63b96265cfe95b9cec847027033d4226b783ecd042036f5c809a7386027f56b0`  
		Last Modified: Fri, 30 Jun 2023 02:08:02 GMT  
		Size: 27.0 MB (27026961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7ab0e6b76129c24867f4152f7c8da7289c6b5f4a0922ae184713f26945af72`  
		Last Modified: Tue, 04 Jul 2023 06:23:16 GMT  
		Size: 7.0 MB (7019201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78a55edb4070b31d77ce5a81d68e5d76539c587fdaf49d4e2a8b380e36371187`  
		Last Modified: Tue, 04 Jul 2023 06:23:36 GMT  
		Size: 42.2 MB (42222602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:e6eb6a297d3d042a39568d9807858287b9e33904800427dbc6cd381ca2fb5a18
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74803934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57426953690b8699e351256723056c42ba681320fd297019188c4e0e691a2c4a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 06:06:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:07:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00483067c1437c60cceadf9b4d31783bc9e1adb93770b38287f24ef2943b3c0`  
		Last Modified: Tue, 04 Jul 2023 06:24:51 GMT  
		Size: 7.1 MB (7067072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c1fabd67ce9ecbf104292a6591b53f2a57503bf444faef66c672ca9017fc31`  
		Last Modified: Tue, 04 Jul 2023 06:25:03 GMT  
		Size: 39.3 MB (39345851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d55364691bb1f9651472826186b92d4833f75b622cdbe27162c05407de6bf49f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87847020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b10e613256e8e7d422110f0c7e9c8b8862359fce3750e27a2181eda7e3baf12`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:45:53 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:45:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:45:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:45:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:45:56 GMT
ADD file:8c2fc380378944326d602742fde0e30458cd3e82012847b0f7e09c7184bfd135 in / 
# Wed, 28 Jun 2023 08:45:57 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 03:54:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:57:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7faa46ce6b6f5c34485980029504c3995e38149d0bca67d8b976c5dbb3673644`  
		Last Modified: Tue, 04 Jul 2023 04:42:31 GMT  
		Size: 35.7 MB (35711469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5028dc76c028f10e8828b80e411d373e4db95e0d5232b4f5a0dde9146f46cf`  
		Last Modified: Tue, 04 Jul 2023 04:42:24 GMT  
		Size: 8.3 MB (8260592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e056faa463b64fc04b6eb21623bad5611901f025c629a92bcaf9337b98644f`  
		Last Modified: Tue, 04 Jul 2023 04:42:54 GMT  
		Size: 43.9 MB (43874959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:3668467811030c710e7b4d32a58fa54ea53a8eb5e4d1150de312f66aff3c804b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75071915 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48d3bea1f433841c762ab73ba3e96579b91de4f23225f8ec515a383ab6cef371`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:53:20 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:53:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:53:22 GMT
ADD file:fa0aef35be7808c8fd6751a52bdec4dd81057e2fcaa075c547a1db53640dae9a in / 
# Wed, 28 Jun 2023 08:53:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 12:55:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 12:55:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce02ee0330980398d6a84a50abfa1a8c4d1cba27cbd7442b79f4aa1b1a14020d`  
		Last Modified: Tue, 04 Jul 2023 13:08:30 GMT  
		Size: 28.6 MB (28645696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7aba4ce682de5293312667253fd0a7af53c579484786de09b36208aab9d22c`  
		Last Modified: Tue, 04 Jul 2023 13:08:26 GMT  
		Size: 7.0 MB (7033603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1c12ddc9521fd58bc71f4494c40a5c8889571901807762f83f2db5e8d7d6dc`  
		Last Modified: Tue, 04 Jul 2023 13:08:43 GMT  
		Size: 39.4 MB (39392616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.10`

```console
$ docker pull buildpack-deps@sha256:c8182962268601e999685babfa78b460a948d4e6f8bebeaf9ac94dd7766a410c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:22.10` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:0b34490510c29fa74353ade9e5d90182d82346a3246992c1ae54ee125ccb8ed4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.7 MB (262660283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1957599663a9fb73a6c45227894308eee2990917cb02b30a6fa23a66f56f5b74`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:23:07 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:23:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:23:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:23:07 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 28 Jun 2023 08:23:09 GMT
ADD file:50094673f74cf3945ac21e23bb84d41d3516bc1ac90ebf7f17379288c33c17b2 in / 
# Wed, 28 Jun 2023 08:23:09 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 03:43:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:44:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:46:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e4ae0f456d5b5ed53c0d0f67cd1948207060810837f2b15dcdf5bd97bbceb300`  
		Last Modified: Tue, 04 Jul 2023 03:56:47 GMT  
		Size: 27.5 MB (27488903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f7fd2e9f809d0b31bf96fde0b09fb68493e5499b9a4dae5f3dfc0a0ed0b7ce`  
		Last Modified: Tue, 04 Jul 2023 03:56:46 GMT  
		Size: 14.2 MB (14189206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e60069d839c80c438523487b52eb9073ef4a8fd32af5b8a6dfe8480792c8a57`  
		Last Modified: Tue, 04 Jul 2023 03:57:02 GMT  
		Size: 39.8 MB (39825912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbc9753f2da447aadff4044bd763bb11c8f004fa9ab7cccc88048ddacb264aa`  
		Last Modified: Tue, 04 Jul 2023 03:57:35 GMT  
		Size: 181.2 MB (181156262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f78e0e5d6707a04956b352cf8fb6883cb9ce87a31fa7befcfb88144d5a452357
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.6 MB (225624695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3685089673bda68c20b3c886018604ff1e74c04bdd8989f7fca96ba999fab182`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:50:23 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:50:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:50:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:50:23 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 28 Jun 2023 08:50:29 GMT
ADD file:1c3ce20a4b19d1c7779aa47e9799d2887ac4d142bb495eb0bdca08ff1c8fd106 in / 
# Wed, 28 Jun 2023 08:50:30 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 06:09:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:09:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:12:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b2a8550df843bc39f9334e8b8d8524b0e0abe390674577c839e53aa1c6afb06`  
		Last Modified: Tue, 04 Jul 2023 06:24:17 GMT  
		Size: 25.9 MB (25912764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eef66710f99af0d044d772f07b2eaf0c9da9559b1b10f9da05b104e86fb12a7`  
		Last Modified: Tue, 04 Jul 2023 06:24:15 GMT  
		Size: 13.1 MB (13141364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f28d29b0c8e6083c797c1ed79183346245421c696c0b8365d1b4027561dc13e`  
		Last Modified: Tue, 04 Jul 2023 06:24:34 GMT  
		Size: 42.9 MB (42939065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f417099045b65e1689b25195d9a5ca52532043778ba15ae89200da7da00efea`  
		Last Modified: Tue, 04 Jul 2023 06:25:06 GMT  
		Size: 143.6 MB (143631502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:fe77e6e21c64105552429c5273332cc2e769d79bfbf74c26a92cb9cbec3d2d7a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.4 MB (250423813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b20fadd9a6936babea6d9dafc67064e118c913a7342ca0cfd0a522d03de2fd4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:16:50 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:16:51 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:16:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:16:51 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 28 Jun 2023 09:16:58 GMT
ADD file:a41ad4058e77a6f1ee9800af03cf13403d5d844e876246ba55c4ceb2106b6d5f in / 
# Wed, 28 Jun 2023 09:16:59 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 06:11:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:12:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:15:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c5528eed9908e3645e0eff6666ba300d135b6ff9801f5ae1cc49bb06a3f29fcf`  
		Last Modified: Tue, 04 Jul 2023 06:25:40 GMT  
		Size: 26.7 MB (26730941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8785a3c2b399ffc53927bd8e5eea56d2819ea053d0d78910ae32f88d2f9ec680`  
		Last Modified: Tue, 04 Jul 2023 06:25:37 GMT  
		Size: 13.7 MB (13727615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af381f44d3219c7eab50c1af5c7bf36233fa1a694569f8a29e1be2e7d55cd37`  
		Last Modified: Tue, 04 Jul 2023 06:25:53 GMT  
		Size: 39.6 MB (39636653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1160a4dcea08cb2cc3585710f41a7615c6d7bc8668f20d79b85391142f1910b`  
		Last Modified: Tue, 04 Jul 2023 06:26:18 GMT  
		Size: 170.3 MB (170328604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:015d6829eda0af44d4186f2cf2c0b6726a23f5b9574881a0b21e75e419f6f601
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.5 MB (285537534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41cee9ff03f244bfd65fcb2ce00a37aa729796de6aee6a06366fecbcef36eb6c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:04:09 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:04:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:04:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:04:09 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 28 Jun 2023 09:04:12 GMT
ADD file:8c5e727842a7ff4d34b93a1ee45f14532c9b03594ad53400240e6f0f4b99b390 in / 
# Wed, 28 Jun 2023 09:04:12 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 04:09:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:10:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:19:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c4c2a73576db8e1d5b385d67fe412db5e6cd146167f6c5fa6153b87f17abfc3d`  
		Last Modified: Tue, 04 Jul 2023 04:44:10 GMT  
		Size: 32.1 MB (32102426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:297facc34b9d65726d36999c1b9378836014f1dbb15725b2be4359b50bec9d21`  
		Last Modified: Tue, 04 Jul 2023 04:44:07 GMT  
		Size: 16.2 MB (16234063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9cb9fc38b5a1da1252223c33aa1381def6fb94284f39b6c1d6025d92bf99478`  
		Last Modified: Tue, 04 Jul 2023 04:44:34 GMT  
		Size: 44.2 MB (44231612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd62a63c22d9416c3b46dccf9da4cb3234f7549206282332be98c282450d9c7d`  
		Last Modified: Tue, 04 Jul 2023 04:45:31 GMT  
		Size: 193.0 MB (192969433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:5f93f187202e8c33d59f11df9460958e7bb82006e7f5c352aa3396e2f84c24ea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.1 MB (233054315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49759ff9442c254584b8c51244f18d3f1e16237357cf7762aae94572b5536be5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:31:17 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:31:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:31:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:31:17 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 28 Jun 2023 08:31:19 GMT
ADD file:e6e44f70accdecf50c8942a8e70c4d2c1d419d1d61696730d8aeda653da7216b in / 
# Wed, 28 Jun 2023 08:31:20 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 12:58:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 12:59:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 13:00:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:db47f8f6e4cba14e75b8de75cdb67df7e0da147a37a6d957e95b908f84f113c9`  
		Last Modified: Tue, 04 Jul 2023 13:09:19 GMT  
		Size: 26.0 MB (26034734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9685e4e083ab19eb76163b6e53eae847ce6aae92708ff92c594d59a98c7b4838`  
		Last Modified: Tue, 04 Jul 2023 13:09:17 GMT  
		Size: 14.3 MB (14344539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5066de6f57445c9a11aa5d720bdf2ef58d4105ba79b5f66be22ddfeb03e89d5`  
		Last Modified: Tue, 04 Jul 2023 13:09:32 GMT  
		Size: 39.7 MB (39678636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd20890008cbd35e672a467d9b7fe96a6dc49fcc4e9f24865edb1d639b3c2d82`  
		Last Modified: Tue, 04 Jul 2023 13:09:57 GMT  
		Size: 153.0 MB (152996406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.10-curl`

```console
$ docker pull buildpack-deps@sha256:10dc553ad4a9ec6df694b1bf115cd6fcb55239d60d0b42de46a26b1082fd45a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:22.10-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:9864a6a8920e10635a22be668dff1a9169c7e666efc7a51cf9cbd0fdacbd6a6d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41678109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6c7af30dd7e2311fbf3138dfcad631878055c64260ae8f409b8c95880e15e2c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:23:07 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:23:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:23:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:23:07 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 28 Jun 2023 08:23:09 GMT
ADD file:50094673f74cf3945ac21e23bb84d41d3516bc1ac90ebf7f17379288c33c17b2 in / 
# Wed, 28 Jun 2023 08:23:09 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 03:43:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e4ae0f456d5b5ed53c0d0f67cd1948207060810837f2b15dcdf5bd97bbceb300`  
		Last Modified: Tue, 04 Jul 2023 03:56:47 GMT  
		Size: 27.5 MB (27488903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f7fd2e9f809d0b31bf96fde0b09fb68493e5499b9a4dae5f3dfc0a0ed0b7ce`  
		Last Modified: Tue, 04 Jul 2023 03:56:46 GMT  
		Size: 14.2 MB (14189206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1f30c94b4bb67a6deaf734529e1d2c320e9c3f922b7b943f713c89b4f3ca87ac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39054128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75cd405b115352482c61020e337a99b4f2384b9fd08dced23ea846b4a6c434f2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:50:23 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:50:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:50:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:50:23 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 28 Jun 2023 08:50:29 GMT
ADD file:1c3ce20a4b19d1c7779aa47e9799d2887ac4d142bb495eb0bdca08ff1c8fd106 in / 
# Wed, 28 Jun 2023 08:50:30 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 06:09:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b2a8550df843bc39f9334e8b8d8524b0e0abe390674577c839e53aa1c6afb06`  
		Last Modified: Tue, 04 Jul 2023 06:24:17 GMT  
		Size: 25.9 MB (25912764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eef66710f99af0d044d772f07b2eaf0c9da9559b1b10f9da05b104e86fb12a7`  
		Last Modified: Tue, 04 Jul 2023 06:24:15 GMT  
		Size: 13.1 MB (13141364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:bb8b48791f089f579a9f0afb2d153d2446b2043976784a576a2f273109ffb37a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.5 MB (40458556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5284d33edbce56f17809d71b6dbbe0d5a70d631472e3c6d187c5e08e7f4ca3a4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:16:50 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:16:51 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:16:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:16:51 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 28 Jun 2023 09:16:58 GMT
ADD file:a41ad4058e77a6f1ee9800af03cf13403d5d844e876246ba55c4ceb2106b6d5f in / 
# Wed, 28 Jun 2023 09:16:59 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 06:11:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c5528eed9908e3645e0eff6666ba300d135b6ff9801f5ae1cc49bb06a3f29fcf`  
		Last Modified: Tue, 04 Jul 2023 06:25:40 GMT  
		Size: 26.7 MB (26730941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8785a3c2b399ffc53927bd8e5eea56d2819ea053d0d78910ae32f88d2f9ec680`  
		Last Modified: Tue, 04 Jul 2023 06:25:37 GMT  
		Size: 13.7 MB (13727615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:1a07aad2e6e2c52838bd9242961c6789330426428afb48c14562883694a9b122
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.3 MB (48336489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:679e8eb78bb21e03123228167c1acc8b09581ee954f76ba102155947e6cb639a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:04:09 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:04:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:04:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:04:09 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 28 Jun 2023 09:04:12 GMT
ADD file:8c5e727842a7ff4d34b93a1ee45f14532c9b03594ad53400240e6f0f4b99b390 in / 
# Wed, 28 Jun 2023 09:04:12 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 04:09:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c4c2a73576db8e1d5b385d67fe412db5e6cd146167f6c5fa6153b87f17abfc3d`  
		Last Modified: Tue, 04 Jul 2023 04:44:10 GMT  
		Size: 32.1 MB (32102426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:297facc34b9d65726d36999c1b9378836014f1dbb15725b2be4359b50bec9d21`  
		Last Modified: Tue, 04 Jul 2023 04:44:07 GMT  
		Size: 16.2 MB (16234063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:e908ca3d7bfcf4e6d6f2dc17aeca9c4457ff23e236f684e242b64d000694465c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.4 MB (40379273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2ccbd6c1f7c17aaac71be9909dcf08a4573fd11727adc6d75fadb51f36b2095`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:31:17 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:31:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:31:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:31:17 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 28 Jun 2023 08:31:19 GMT
ADD file:e6e44f70accdecf50c8942a8e70c4d2c1d419d1d61696730d8aeda653da7216b in / 
# Wed, 28 Jun 2023 08:31:20 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 12:58:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:db47f8f6e4cba14e75b8de75cdb67df7e0da147a37a6d957e95b908f84f113c9`  
		Last Modified: Tue, 04 Jul 2023 13:09:19 GMT  
		Size: 26.0 MB (26034734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9685e4e083ab19eb76163b6e53eae847ce6aae92708ff92c594d59a98c7b4838`  
		Last Modified: Tue, 04 Jul 2023 13:09:17 GMT  
		Size: 14.3 MB (14344539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.10-scm`

```console
$ docker pull buildpack-deps@sha256:1ca7f8e293e400892c469b069eae7e97b60cd0a1d2a6f58ffa6aafaf45bedda0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:22.10-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:d52ddd72ddd4f630e64370ad14d0ec6b99705784fc76f396c2d3d67230db3403
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.5 MB (81504021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ec8c6e4d643fed5a6197bd272d12574893b6727b71d0bddc0526d40019fb457`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:23:07 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:23:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:23:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:23:07 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 28 Jun 2023 08:23:09 GMT
ADD file:50094673f74cf3945ac21e23bb84d41d3516bc1ac90ebf7f17379288c33c17b2 in / 
# Wed, 28 Jun 2023 08:23:09 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 03:43:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:44:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e4ae0f456d5b5ed53c0d0f67cd1948207060810837f2b15dcdf5bd97bbceb300`  
		Last Modified: Tue, 04 Jul 2023 03:56:47 GMT  
		Size: 27.5 MB (27488903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f7fd2e9f809d0b31bf96fde0b09fb68493e5499b9a4dae5f3dfc0a0ed0b7ce`  
		Last Modified: Tue, 04 Jul 2023 03:56:46 GMT  
		Size: 14.2 MB (14189206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e60069d839c80c438523487b52eb9073ef4a8fd32af5b8a6dfe8480792c8a57`  
		Last Modified: Tue, 04 Jul 2023 03:57:02 GMT  
		Size: 39.8 MB (39825912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:44b7926bef25e86fda0ce933db0a51672dd4b6569f40fbde5413b85c40259d7b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.0 MB (81993193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1888d5faa20899d778ded8b8bc5a0d939c3c81a8d6ffeffa5669bf0f8dc8a9d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:50:23 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:50:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:50:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:50:23 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 28 Jun 2023 08:50:29 GMT
ADD file:1c3ce20a4b19d1c7779aa47e9799d2887ac4d142bb495eb0bdca08ff1c8fd106 in / 
# Wed, 28 Jun 2023 08:50:30 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 06:09:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:09:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b2a8550df843bc39f9334e8b8d8524b0e0abe390674577c839e53aa1c6afb06`  
		Last Modified: Tue, 04 Jul 2023 06:24:17 GMT  
		Size: 25.9 MB (25912764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eef66710f99af0d044d772f07b2eaf0c9da9559b1b10f9da05b104e86fb12a7`  
		Last Modified: Tue, 04 Jul 2023 06:24:15 GMT  
		Size: 13.1 MB (13141364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f28d29b0c8e6083c797c1ed79183346245421c696c0b8365d1b4027561dc13e`  
		Last Modified: Tue, 04 Jul 2023 06:24:34 GMT  
		Size: 42.9 MB (42939065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d82da2a7c889be494f08719c2be0bae60e0130d8f57987e9dbbefe8771bc942f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.1 MB (80095209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04eaa9e6f7cd4097cd50bf0de7c32b8d39d1c5d8ac59cf278e3defea8e03a703`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:16:50 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:16:51 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:16:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:16:51 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 28 Jun 2023 09:16:58 GMT
ADD file:a41ad4058e77a6f1ee9800af03cf13403d5d844e876246ba55c4ceb2106b6d5f in / 
# Wed, 28 Jun 2023 09:16:59 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 06:11:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:12:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c5528eed9908e3645e0eff6666ba300d135b6ff9801f5ae1cc49bb06a3f29fcf`  
		Last Modified: Tue, 04 Jul 2023 06:25:40 GMT  
		Size: 26.7 MB (26730941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8785a3c2b399ffc53927bd8e5eea56d2819ea053d0d78910ae32f88d2f9ec680`  
		Last Modified: Tue, 04 Jul 2023 06:25:37 GMT  
		Size: 13.7 MB (13727615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af381f44d3219c7eab50c1af5c7bf36233fa1a694569f8a29e1be2e7d55cd37`  
		Last Modified: Tue, 04 Jul 2023 06:25:53 GMT  
		Size: 39.6 MB (39636653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:264fc69c8de3193a7191aae5bb3f4c3db4fbf1a9f0e72d801c70971713aadbda
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92568101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6367bde1dbdeeadc100e3b50d95455d079ffc7c8f892d24e31742464e7e00931`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:04:09 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:04:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:04:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:04:09 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 28 Jun 2023 09:04:12 GMT
ADD file:8c5e727842a7ff4d34b93a1ee45f14532c9b03594ad53400240e6f0f4b99b390 in / 
# Wed, 28 Jun 2023 09:04:12 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 04:09:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:10:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c4c2a73576db8e1d5b385d67fe412db5e6cd146167f6c5fa6153b87f17abfc3d`  
		Last Modified: Tue, 04 Jul 2023 04:44:10 GMT  
		Size: 32.1 MB (32102426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:297facc34b9d65726d36999c1b9378836014f1dbb15725b2be4359b50bec9d21`  
		Last Modified: Tue, 04 Jul 2023 04:44:07 GMT  
		Size: 16.2 MB (16234063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9cb9fc38b5a1da1252223c33aa1381def6fb94284f39b6c1d6025d92bf99478`  
		Last Modified: Tue, 04 Jul 2023 04:44:34 GMT  
		Size: 44.2 MB (44231612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.10-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:d1bc086fc34aa7a36d0e1167a5767ca9f9e1817421f90a56fe4414d21a4f3286
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.1 MB (80057909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b9a8ff3339995ee87b2d7b6c3a9e615a3f0266ebfcd50b7f691d0097c79672e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:31:17 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:31:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:31:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:31:17 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 28 Jun 2023 08:31:19 GMT
ADD file:e6e44f70accdecf50c8942a8e70c4d2c1d419d1d61696730d8aeda653da7216b in / 
# Wed, 28 Jun 2023 08:31:20 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 12:58:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 12:59:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:db47f8f6e4cba14e75b8de75cdb67df7e0da147a37a6d957e95b908f84f113c9`  
		Last Modified: Tue, 04 Jul 2023 13:09:19 GMT  
		Size: 26.0 MB (26034734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9685e4e083ab19eb76163b6e53eae847ce6aae92708ff92c594d59a98c7b4838`  
		Last Modified: Tue, 04 Jul 2023 13:09:17 GMT  
		Size: 14.3 MB (14344539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5066de6f57445c9a11aa5d720bdf2ef58d4105ba79b5f66be22ddfeb03e89d5`  
		Last Modified: Tue, 04 Jul 2023 13:09:32 GMT  
		Size: 39.7 MB (39678636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:23.04`

```console
$ docker pull buildpack-deps@sha256:3af97726bdf17e4258a19ca66a6133fcba3a5e06827e9a4a850f0e8427a396f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:23.04` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:060c71d6a2053b21c4c5e8cd20ccd50f587f3dea37321b1af7f050c80e0ac040
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.8 MB (267815018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c17f80b562319d5fb916eb776f579020c47586fbfc79b3ae2ee8d0cbdfd3ce03`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:28:38 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:28:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:28:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:28:38 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:28:39 GMT
ADD file:708314051e878a0c6071fb2c8d4458a04ce058f47f2cfaa58c1b5a42e837ca0f in / 
# Thu, 15 Jun 2023 08:28:40 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:47:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:48:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:50:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ccc37bca66e7c29e0d65a4279511fe9a93932a4bb80e79e95144f3812632b61a`  
		Last Modified: Fri, 16 Jun 2023 01:56:54 GMT  
		Size: 27.6 MB (27612943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7beeb5a79f9bd13c90ee4c9f68636fc642df773adb1bd04e27e2115f6c12a6d`  
		Last Modified: Fri, 16 Jun 2023 01:56:52 GMT  
		Size: 13.7 MB (13744092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a98e278987c0da01adb1f6145dec78bd526ecc11c227e2e74c48de9cd72c40`  
		Last Modified: Fri, 16 Jun 2023 01:57:09 GMT  
		Size: 44.4 MB (44371533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ad6ec5ea91c193cf063d5afed2481b1bf6bd664ffc3a333154de164470c017`  
		Last Modified: Fri, 16 Jun 2023 01:57:40 GMT  
		Size: 182.1 MB (182086450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1775b10436d83e9c74fb94a701896a79959b60929ff867805f3af15e5887bdb7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.2 MB (232238791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d919701a0aadbffccea3bcfb66835adf40d30ec9815f9564db14e9f40b618ed`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:10:50 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:10:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:10:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:10:51 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:10:53 GMT
ADD file:8484efc06b5f22d170eef374f45df452d8e36f4cbef702f7ee4d1f130dd28093 in / 
# Thu, 15 Jun 2023 08:10:53 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 00:49:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 00:50:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 00:53:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ca5128fe76949cc104af7f40ce0f7213fe093079077d47dd525fa0189090c57e`  
		Last Modified: Fri, 16 Jun 2023 00:59:51 GMT  
		Size: 25.4 MB (25432780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d8ca764d56bdf14c46fabd5c4e2e988ce166d01c8c0631d7c345802ace7bf1`  
		Last Modified: Fri, 16 Jun 2023 00:59:50 GMT  
		Size: 12.7 MB (12662932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b3e8b607724476a55e2e23faa2859f1e37c17323d12df2f9b87de3745b98e3`  
		Last Modified: Fri, 16 Jun 2023 01:00:07 GMT  
		Size: 48.7 MB (48652729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b17d9a7a6b4123e5072aa4ab3b712d7b1a715d71ffb3014b99eee3394fe9fa02`  
		Last Modified: Fri, 16 Jun 2023 01:00:36 GMT  
		Size: 145.5 MB (145490350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:b6838fb7edbb355dd8edcd769f623d47cfef3c1ad6c0a3abbaaec22ce133921e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.9 MB (257937976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ba91a8a887dc40746a34ed310c28a682f2e87c3521de6e9c4324a2f41fb82b3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:33:24 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:33:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:33:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:33:25 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:33:58 GMT
ADD file:064ac1f238394a53372e0db107e28835aa3c39ed189a15fe85c532bbb50bfbaf in / 
# Thu, 15 Jun 2023 08:33:59 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:25:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:25:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:28:52 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fc6a8da5865fc488969148ca6c503307bba4023ecc0cdceaaae76a8b9852f031`  
		Last Modified: Fri, 16 Jun 2023 02:35:25 GMT  
		Size: 27.0 MB (27029986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8dde3bba356efbb171daed99ec516dc5c5c9a9b19d538fcb9fd0031bd92403a`  
		Last Modified: Fri, 16 Jun 2023 02:35:22 GMT  
		Size: 13.3 MB (13333143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a9f35a1267eac739bb82daa33daa3a21960fb88acbc2177a8156f23b857239`  
		Last Modified: Fri, 16 Jun 2023 02:35:38 GMT  
		Size: 44.2 MB (44217375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:458bfa897fdd09d151a3e8a28025d6adf7ed1844f5f0245ce523235d8c279bf5`  
		Last Modified: Fri, 16 Jun 2023 02:36:03 GMT  
		Size: 173.4 MB (173357472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:6d6ddf54830ccbd4828b9c92614b8428e223455821e4cf626b1a991e2f7c8aed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.7 MB (292741826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ca0901e8811adcec0e4685f99570016590fd216ba20798cea36a7bbfcb2d046`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:29:14 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:29:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:29:15 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:29:15 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:29:17 GMT
ADD file:5ebdf4bd4bc2b27019f20fb1964a395fa504d4f20e208c54237e363895b492d7 in / 
# Thu, 15 Jun 2023 08:29:18 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:11:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:12:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:17:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a58a0b662b0d4d5e271c7c17f35795b5782a33c69a079e473f7c2303bee50024`  
		Last Modified: Fri, 16 Jun 2023 01:28:52 GMT  
		Size: 32.0 MB (32010412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6f165de89ef5a3a93777200dd180f02a8fc30051f7eb6267300a3e6f27ae1e`  
		Last Modified: Fri, 16 Jun 2023 01:28:48 GMT  
		Size: 15.8 MB (15841962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06312954ebad2b0995222a924fae1923e9b3c87aa73ff14beea981d9235b706d`  
		Last Modified: Fri, 16 Jun 2023 01:29:15 GMT  
		Size: 49.1 MB (49073779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adcdba320d64983a5412706a631d98112285fa65575f90a37f1186e72671d860`  
		Last Modified: Fri, 16 Jun 2023 01:30:10 GMT  
		Size: 195.8 MB (195815673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:381572bf0ac103571328da2f7fe25e0972ddc48e59368440128ec280f685fac4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.9 MB (239916461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c3c5aaa14320304059fd5f516a647ad617ea98ce7d61ad3cd07d091c5376597`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:11:16 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:11:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:11:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:11:16 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:11:18 GMT
ADD file:3974fe053080180d99954042c25b3bd0c82e320fb4521b197cbc45f21885fc43 in / 
# Thu, 15 Jun 2023 08:11:18 GMT
CMD ["/bin/bash"]
# Sat, 17 Jun 2023 09:53:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 17 Jun 2023 09:54:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 17 Jun 2023 09:55:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:761ebd2058697796f2f98019cecedb81ef33759e6c1ec5a428e5bfcc3fe17d92`  
		Last Modified: Sat, 17 Jun 2023 10:02:12 GMT  
		Size: 26.2 MB (26245344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36084a86fb1b20f414b56d87cfcfa6dbc269df581ae9079da63a5c20f292984`  
		Last Modified: Sat, 17 Jun 2023 10:02:10 GMT  
		Size: 14.0 MB (14005266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a9be9d6364c4e6a0cc7388e754f4dea89849b8149102ccc37c8849f51879091`  
		Last Modified: Sat, 17 Jun 2023 10:02:24 GMT  
		Size: 44.2 MB (44249340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97e0d170e15949f28ed04940320f25faa3aaabf630a5deff17e662faf8174619`  
		Last Modified: Sat, 17 Jun 2023 10:02:50 GMT  
		Size: 155.4 MB (155416511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:23.04-curl`

```console
$ docker pull buildpack-deps@sha256:632adb935a5ed86a9a06b181c60d0112467852511409e4c2ff5725ebe3bec909
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:23.04-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:8b4a7037ab529927d19c652a98edece16c14a141220bb94b2ae137372a910662
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.4 MB (41357035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cb02a4320e2d201d51f16cac15f0e1a4bd615b6d5f6294bf6e3c45f3d864710`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:28:38 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:28:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:28:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:28:38 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:28:39 GMT
ADD file:708314051e878a0c6071fb2c8d4458a04ce058f47f2cfaa58c1b5a42e837ca0f in / 
# Thu, 15 Jun 2023 08:28:40 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:47:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ccc37bca66e7c29e0d65a4279511fe9a93932a4bb80e79e95144f3812632b61a`  
		Last Modified: Fri, 16 Jun 2023 01:56:54 GMT  
		Size: 27.6 MB (27612943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7beeb5a79f9bd13c90ee4c9f68636fc642df773adb1bd04e27e2115f6c12a6d`  
		Last Modified: Fri, 16 Jun 2023 01:56:52 GMT  
		Size: 13.7 MB (13744092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:61de8a1c369fb750af225159ced6e4c45df3ad711c10ad9598b6764df05f9f06
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.1 MB (38095712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:217162e2f73ec8805a9bcc072434a36250aaff6d65a445fba2cc1fc08f1ed000`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:10:50 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:10:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:10:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:10:51 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:10:53 GMT
ADD file:8484efc06b5f22d170eef374f45df452d8e36f4cbef702f7ee4d1f130dd28093 in / 
# Thu, 15 Jun 2023 08:10:53 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 00:49:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ca5128fe76949cc104af7f40ce0f7213fe093079077d47dd525fa0189090c57e`  
		Last Modified: Fri, 16 Jun 2023 00:59:51 GMT  
		Size: 25.4 MB (25432780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d8ca764d56bdf14c46fabd5c4e2e988ce166d01c8c0631d7c345802ace7bf1`  
		Last Modified: Fri, 16 Jun 2023 00:59:50 GMT  
		Size: 12.7 MB (12662932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:8204f0499f6b7fc2d2a56297ffc2dd01f35c30d598fd18c40ca2c24947ccf3be
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.4 MB (40363129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c55367957df75573ca685df1b793a902c55a42f9cd552150ccb1fa84d33226bb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:33:24 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:33:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:33:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:33:25 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:33:58 GMT
ADD file:064ac1f238394a53372e0db107e28835aa3c39ed189a15fe85c532bbb50bfbaf in / 
# Thu, 15 Jun 2023 08:33:59 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:25:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fc6a8da5865fc488969148ca6c503307bba4023ecc0cdceaaae76a8b9852f031`  
		Last Modified: Fri, 16 Jun 2023 02:35:25 GMT  
		Size: 27.0 MB (27029986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8dde3bba356efbb171daed99ec516dc5c5c9a9b19d538fcb9fd0031bd92403a`  
		Last Modified: Fri, 16 Jun 2023 02:35:22 GMT  
		Size: 13.3 MB (13333143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:dc5e0428f7f0c3135af8d7fee001e103cea834d13b0ec934142f1415dd644071
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47852374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c6d6cf91b670992b73799b26277cc6486e785cb084948d3c1fa3bb5d0d71f89`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:29:14 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:29:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:29:15 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:29:15 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:29:17 GMT
ADD file:5ebdf4bd4bc2b27019f20fb1964a395fa504d4f20e208c54237e363895b492d7 in / 
# Thu, 15 Jun 2023 08:29:18 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:11:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a58a0b662b0d4d5e271c7c17f35795b5782a33c69a079e473f7c2303bee50024`  
		Last Modified: Fri, 16 Jun 2023 01:28:52 GMT  
		Size: 32.0 MB (32010412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6f165de89ef5a3a93777200dd180f02a8fc30051f7eb6267300a3e6f27ae1e`  
		Last Modified: Fri, 16 Jun 2023 01:28:48 GMT  
		Size: 15.8 MB (15841962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:9ca9483cad5134ed4dc7b67acb9e8b817198119f4f1349d4158bdc50f6ba713b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40250610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3492b4e597fbe3726f466a64c487ccb85135bd0b3119510b80c42f8b19c7a16`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:11:16 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:11:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:11:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:11:16 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:11:18 GMT
ADD file:3974fe053080180d99954042c25b3bd0c82e320fb4521b197cbc45f21885fc43 in / 
# Thu, 15 Jun 2023 08:11:18 GMT
CMD ["/bin/bash"]
# Sat, 17 Jun 2023 09:53:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:761ebd2058697796f2f98019cecedb81ef33759e6c1ec5a428e5bfcc3fe17d92`  
		Last Modified: Sat, 17 Jun 2023 10:02:12 GMT  
		Size: 26.2 MB (26245344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36084a86fb1b20f414b56d87cfcfa6dbc269df581ae9079da63a5c20f292984`  
		Last Modified: Sat, 17 Jun 2023 10:02:10 GMT  
		Size: 14.0 MB (14005266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:23.04-scm`

```console
$ docker pull buildpack-deps@sha256:dbba68715899748e496e12c3807632c13e05ffd80b651787b7c5154d77340eb9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:23.04-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:41592dd1e67dbffba26634f00619f5da6af28bfaefed9cf9475afdaa03acbf6c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.7 MB (85728568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37fba109e84f956fa8db5ad6c4f1d621aa0184f493c6f92c176ecf3b10843533`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:28:38 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:28:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:28:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:28:38 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:28:39 GMT
ADD file:708314051e878a0c6071fb2c8d4458a04ce058f47f2cfaa58c1b5a42e837ca0f in / 
# Thu, 15 Jun 2023 08:28:40 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:47:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:48:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ccc37bca66e7c29e0d65a4279511fe9a93932a4bb80e79e95144f3812632b61a`  
		Last Modified: Fri, 16 Jun 2023 01:56:54 GMT  
		Size: 27.6 MB (27612943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7beeb5a79f9bd13c90ee4c9f68636fc642df773adb1bd04e27e2115f6c12a6d`  
		Last Modified: Fri, 16 Jun 2023 01:56:52 GMT  
		Size: 13.7 MB (13744092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a98e278987c0da01adb1f6145dec78bd526ecc11c227e2e74c48de9cd72c40`  
		Last Modified: Fri, 16 Jun 2023 01:57:09 GMT  
		Size: 44.4 MB (44371533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:5a6012c64abe5a1e4977712e462e6802d4c5e7a02f2030a15e71b72ff3dfe57a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.7 MB (86748441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23973e09ff69a4949c38d23ac559b76967b561c2e71a9c4d1998f800fc603a88`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:10:50 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:10:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:10:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:10:51 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:10:53 GMT
ADD file:8484efc06b5f22d170eef374f45df452d8e36f4cbef702f7ee4d1f130dd28093 in / 
# Thu, 15 Jun 2023 08:10:53 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 00:49:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 00:50:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ca5128fe76949cc104af7f40ce0f7213fe093079077d47dd525fa0189090c57e`  
		Last Modified: Fri, 16 Jun 2023 00:59:51 GMT  
		Size: 25.4 MB (25432780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d8ca764d56bdf14c46fabd5c4e2e988ce166d01c8c0631d7c345802ace7bf1`  
		Last Modified: Fri, 16 Jun 2023 00:59:50 GMT  
		Size: 12.7 MB (12662932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b3e8b607724476a55e2e23faa2859f1e37c17323d12df2f9b87de3745b98e3`  
		Last Modified: Fri, 16 Jun 2023 01:00:07 GMT  
		Size: 48.7 MB (48652729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f4b6f4db12ef63968941c8377fa0e0c0bcee84d18bdd0a12614b41b634f32314
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.6 MB (84580504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14bbc99976613f7010bfbffe01cff6a9c09074f1d54233d81f2928fa1eb6bfa6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:33:24 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:33:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:33:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:33:25 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:33:58 GMT
ADD file:064ac1f238394a53372e0db107e28835aa3c39ed189a15fe85c532bbb50bfbaf in / 
# Thu, 15 Jun 2023 08:33:59 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:25:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:25:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fc6a8da5865fc488969148ca6c503307bba4023ecc0cdceaaae76a8b9852f031`  
		Last Modified: Fri, 16 Jun 2023 02:35:25 GMT  
		Size: 27.0 MB (27029986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8dde3bba356efbb171daed99ec516dc5c5c9a9b19d538fcb9fd0031bd92403a`  
		Last Modified: Fri, 16 Jun 2023 02:35:22 GMT  
		Size: 13.3 MB (13333143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a9f35a1267eac739bb82daa33daa3a21960fb88acbc2177a8156f23b857239`  
		Last Modified: Fri, 16 Jun 2023 02:35:38 GMT  
		Size: 44.2 MB (44217375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:c5a83ab3770b99e11c2b4445afb7ee1d926562a534194746e3288c6e0f2fc9b6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.9 MB (96926153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c299a6b52971b8d036a8ccadd60c639e7831b2c4f677f2882df75e523a441b7f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:29:14 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:29:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:29:15 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:29:15 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:29:17 GMT
ADD file:5ebdf4bd4bc2b27019f20fb1964a395fa504d4f20e208c54237e363895b492d7 in / 
# Thu, 15 Jun 2023 08:29:18 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:11:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:12:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a58a0b662b0d4d5e271c7c17f35795b5782a33c69a079e473f7c2303bee50024`  
		Last Modified: Fri, 16 Jun 2023 01:28:52 GMT  
		Size: 32.0 MB (32010412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6f165de89ef5a3a93777200dd180f02a8fc30051f7eb6267300a3e6f27ae1e`  
		Last Modified: Fri, 16 Jun 2023 01:28:48 GMT  
		Size: 15.8 MB (15841962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06312954ebad2b0995222a924fae1923e9b3c87aa73ff14beea981d9235b706d`  
		Last Modified: Fri, 16 Jun 2023 01:29:15 GMT  
		Size: 49.1 MB (49073779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:1b75cd39b4b8028add596e3133c70e142effd651127b61c8b4819a154a3f6eb4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84499950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dbb05763b63f79a573454ce88736b2c772cce3080193c277b1e194c26f5597d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:11:16 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:11:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:11:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:11:16 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:11:18 GMT
ADD file:3974fe053080180d99954042c25b3bd0c82e320fb4521b197cbc45f21885fc43 in / 
# Thu, 15 Jun 2023 08:11:18 GMT
CMD ["/bin/bash"]
# Sat, 17 Jun 2023 09:53:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 17 Jun 2023 09:54:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:761ebd2058697796f2f98019cecedb81ef33759e6c1ec5a428e5bfcc3fe17d92`  
		Last Modified: Sat, 17 Jun 2023 10:02:12 GMT  
		Size: 26.2 MB (26245344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36084a86fb1b20f414b56d87cfcfa6dbc269df581ae9079da63a5c20f292984`  
		Last Modified: Sat, 17 Jun 2023 10:02:10 GMT  
		Size: 14.0 MB (14005266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a9be9d6364c4e6a0cc7388e754f4dea89849b8149102ccc37c8849f51879091`  
		Last Modified: Sat, 17 Jun 2023 10:02:24 GMT  
		Size: 44.2 MB (44249340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:23.10`

```console
$ docker pull buildpack-deps@sha256:0d94fcf7307ea7e5a21706c746b9eadb0372e5c4404d58c4066a76168bbc25c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:23.10` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:43bbe0dfe0048d31bb7cd9b7eb2b7881843a4f0a1ae20c10932f9f681d30c2ad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **264.0 MB (263967050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e86264f55ba5f4c343180d74c070d50549aea1e1f79057cd46e6a1d208a21be2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jul 2023 04:50:42 GMT
ARG RELEASE
# Wed, 12 Jul 2023 04:50:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 12 Jul 2023 04:50:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 12 Jul 2023 04:50:42 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 12 Jul 2023 04:50:44 GMT
ADD file:592c8f21973a80f096ca38aaf5ef478d80f666517a169bc638ebb325f5ae07f4 in / 
# Wed, 12 Jul 2023 04:50:44 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 01:45:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 18 Jul 2023 01:45:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 18 Jul 2023 01:48:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c57e6f7e53eccd34261640d6f245ad38a4ff7cc54ead279536b568d836363ae4`  
		Last Modified: Tue, 18 Jul 2023 01:49:46 GMT  
		Size: 27.8 MB (27758391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70262639a4fd505c867f716c40dd85135752950cc1aa365725b9e2967d66175a`  
		Last Modified: Tue, 18 Jul 2023 01:49:45 GMT  
		Size: 13.8 MB (13781000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade5aed8da7a4eb9b7d6f71f11a953d3491588e96cb6cd244876de5a69a96cea`  
		Last Modified: Tue, 18 Jul 2023 01:50:01 GMT  
		Size: 44.8 MB (44782483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bedca93e8e17ebc5f9ebd2b628460a33677641af0f83f30ebc916656b90372b7`  
		Last Modified: Tue, 18 Jul 2023 01:50:32 GMT  
		Size: 177.6 MB (177645176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.10` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:75f07b3d147e57addbeb6d779210d315e133163c662e7ad5c3f627da87d67f6a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.2 MB (229226030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e26b4bf7025f6e10a390f74b97289b98d233bbafe98ba0d78b0f9264885de7ef`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jul 2023 04:54:17 GMT
ARG RELEASE
# Wed, 12 Jul 2023 04:54:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 12 Jul 2023 04:54:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 12 Jul 2023 04:54:17 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 12 Jul 2023 04:54:20 GMT
ADD file:6f71de5b8467fdcd7bcf88fbae117a520f903a91b00a674bdf8d44b14141f0d6 in / 
# Wed, 12 Jul 2023 04:54:20 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 04:39:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 18 Jul 2023 04:40:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 18 Jul 2023 04:43:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2d27378af227ba4634a3837d7cb24660c6d297228e3b3a59b569c67e86c1b702`  
		Last Modified: Tue, 18 Jul 2023 04:44:33 GMT  
		Size: 25.3 MB (25310196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c20ac942533d1efa51f9b7223514a74aa29ec7a0272a22f2f548636534fd3f`  
		Last Modified: Tue, 18 Jul 2023 04:44:32 GMT  
		Size: 12.7 MB (12697617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5550cb2b09d3bf2b56d01eee2a5d36ef7263a4f3b0d35f84ebe938e6f64ab689`  
		Last Modified: Tue, 18 Jul 2023 04:44:49 GMT  
		Size: 48.9 MB (48925628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4833443a839e8ecc3c01096f5d85e9929c462a37f44010dcb41b46f6d73997`  
		Last Modified: Tue, 18 Jul 2023 04:45:17 GMT  
		Size: 142.3 MB (142292589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.10` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:2da519cc285d20321e77743bbe70ee727c2e6136b31cc3d2e07206ff2bcbbed2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.1 MB (255105368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05cec95d34923cff89a08436ace6f42700083d0033510ee441a90175265c3c4d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jul 2023 04:54:30 GMT
ARG RELEASE
# Wed, 12 Jul 2023 04:54:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 12 Jul 2023 04:54:31 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 12 Jul 2023 04:54:31 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 12 Jul 2023 04:54:38 GMT
ADD file:6eb08bb754e74bd297a54d5c56c7622fe3945c0e013d8a48b8d85b09f1818099 in / 
# Wed, 12 Jul 2023 04:54:39 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 01:46:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 18 Jul 2023 01:46:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 18 Jul 2023 01:50:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4f4369a81c2a2103bb37c89ff5ddb71caf0eefa6abc6ace3a6312b114b1b43f4`  
		Last Modified: Tue, 18 Jul 2023 01:51:33 GMT  
		Size: 27.1 MB (27116407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9605105b68496ddcb5871d9313b51b49ff984efaf7993f0d2e84539e1fd35b1d`  
		Last Modified: Tue, 18 Jul 2023 01:51:32 GMT  
		Size: 13.4 MB (13364288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7138fb2464b9037662e225fd640c60489c9bdfc93091ead842a55da631876df`  
		Last Modified: Tue, 18 Jul 2023 01:51:47 GMT  
		Size: 44.6 MB (44635979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccd9871927ef7cdded88c78380cff871c2321f9c0cade58af992c42da7a5b2c2`  
		Last Modified: Tue, 18 Jul 2023 01:52:13 GMT  
		Size: 170.0 MB (169988694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.10` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:1de851cd70a72ad80a5228ded09e8cd462ad2d158016d2ce9dbeab4d893aa1bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.0 MB (280978333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe3d22a2e38ab71f55edaa8bbafd38fd543dd9e87f837b4ee7be3a7d1b1ad1d1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jul 2023 04:53:28 GMT
ARG RELEASE
# Wed, 12 Jul 2023 04:53:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 12 Jul 2023 04:53:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 12 Jul 2023 04:53:28 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 12 Jul 2023 04:53:31 GMT
ADD file:7028e8b5bb04424a3fa537fa5b5a311cfcaf1c8b6f321b414b40ee0388d0f9e0 in / 
# Wed, 12 Jul 2023 04:53:31 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 01:52:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 18 Jul 2023 01:54:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 18 Jul 2023 01:59:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:eaefff58e8d715237ca48dbc24624ab97d73780134b6abfa9397a3fb107c7847`  
		Last Modified: Tue, 18 Jul 2023 02:02:03 GMT  
		Size: 32.0 MB (31995451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3142716ff35072c411419b141a83ce524bc1af91e86195277f4ca49673988b19`  
		Last Modified: Tue, 18 Jul 2023 02:01:59 GMT  
		Size: 15.9 MB (15880046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5986d60cc2d030634cd4d91824fd3926b4c50f5ff1bed4d038671c930e6dc5`  
		Last Modified: Tue, 18 Jul 2023 02:02:28 GMT  
		Size: 49.5 MB (49515259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565b0450a909c066455134dae59757cfb34c74497dcca3ded5fe9ca1a48c2718`  
		Last Modified: Tue, 18 Jul 2023 02:03:24 GMT  
		Size: 183.6 MB (183587577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.10` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:dde2f5b122c8c8e28653492c1d584028f22faca03ae20b746adf4f7def78e451
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.6 MB (237599006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bd06b65dfe50e847e71a12fc051aa3777176303bb94a4fac7c14a3ca594bca1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jul 2023 04:53:32 GMT
ARG RELEASE
# Wed, 12 Jul 2023 04:53:32 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 12 Jul 2023 04:53:32 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 12 Jul 2023 04:53:32 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 12 Jul 2023 04:53:34 GMT
ADD file:878995fa3a12c9df0a99fc88605932ffefec3e772a3c4ca89fe0c0aaa7dee67d in / 
# Wed, 12 Jul 2023 04:53:34 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 01:13:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 18 Jul 2023 01:14:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 18 Jul 2023 01:16:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f2b8f6b9cb3947ae25987d6e3685dc9709178b596bd7bf0d7a84ceeba23a2073`  
		Last Modified: Tue, 18 Jul 2023 01:18:14 GMT  
		Size: 26.3 MB (26322139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b736a5889ac0138557b62eaa679858540efdff47fa4079b2d261d5d981a0b7`  
		Last Modified: Tue, 18 Jul 2023 01:18:13 GMT  
		Size: 14.0 MB (14037874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15d33eaf6ee65a8ded43a590675151bb6e283880b75995e7651a1b22700ecbe`  
		Last Modified: Tue, 18 Jul 2023 01:18:27 GMT  
		Size: 44.6 MB (44645792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919012de24272d20e9cbb02ecdc2d11a6e2b3b30cd97c260c7b0ed02524b0b5d`  
		Last Modified: Tue, 18 Jul 2023 01:18:53 GMT  
		Size: 152.6 MB (152593201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:23.10-curl`

```console
$ docker pull buildpack-deps@sha256:0e4442494d1c195e5e6f434eb92c3ce0973a9b5703677da131bdac3854a1e256
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:23.10-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:67c5c72393daaa311813c147c29b11e206a74eaa529bedf9f39eb69ba579bf1e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41539391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:600cfbf723eb7c8bf4ce8d3f5a932754804867c8248e234b61709d417cfb2fa3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jul 2023 04:50:42 GMT
ARG RELEASE
# Wed, 12 Jul 2023 04:50:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 12 Jul 2023 04:50:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 12 Jul 2023 04:50:42 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 12 Jul 2023 04:50:44 GMT
ADD file:592c8f21973a80f096ca38aaf5ef478d80f666517a169bc638ebb325f5ae07f4 in / 
# Wed, 12 Jul 2023 04:50:44 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 01:45:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c57e6f7e53eccd34261640d6f245ad38a4ff7cc54ead279536b568d836363ae4`  
		Last Modified: Tue, 18 Jul 2023 01:49:46 GMT  
		Size: 27.8 MB (27758391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70262639a4fd505c867f716c40dd85135752950cc1aa365725b9e2967d66175a`  
		Last Modified: Tue, 18 Jul 2023 01:49:45 GMT  
		Size: 13.8 MB (13781000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.10-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:6f2765db9a30168dd4cd5bf233b36740ba02c8d21fcfbeab4455b971e0904e9f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (38007813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:407a9cce53487e562629cd48d377253d36b1f0c25d4a1e623d536ae203544f16`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jul 2023 04:54:17 GMT
ARG RELEASE
# Wed, 12 Jul 2023 04:54:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 12 Jul 2023 04:54:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 12 Jul 2023 04:54:17 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 12 Jul 2023 04:54:20 GMT
ADD file:6f71de5b8467fdcd7bcf88fbae117a520f903a91b00a674bdf8d44b14141f0d6 in / 
# Wed, 12 Jul 2023 04:54:20 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 04:39:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2d27378af227ba4634a3837d7cb24660c6d297228e3b3a59b569c67e86c1b702`  
		Last Modified: Tue, 18 Jul 2023 04:44:33 GMT  
		Size: 25.3 MB (25310196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c20ac942533d1efa51f9b7223514a74aa29ec7a0272a22f2f548636534fd3f`  
		Last Modified: Tue, 18 Jul 2023 04:44:32 GMT  
		Size: 12.7 MB (12697617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.10-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:10bb9957c553ac1c04cab432f23e71fd04ef05d3f508e6d3dbd79575f22c2155
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.5 MB (40480695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24c82d9a81946878d92e5085da84d06a6e9a112da2626ae0b6e6b6f5b163b5eb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jul 2023 04:54:30 GMT
ARG RELEASE
# Wed, 12 Jul 2023 04:54:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 12 Jul 2023 04:54:31 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 12 Jul 2023 04:54:31 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 12 Jul 2023 04:54:38 GMT
ADD file:6eb08bb754e74bd297a54d5c56c7622fe3945c0e013d8a48b8d85b09f1818099 in / 
# Wed, 12 Jul 2023 04:54:39 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 01:46:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4f4369a81c2a2103bb37c89ff5ddb71caf0eefa6abc6ace3a6312b114b1b43f4`  
		Last Modified: Tue, 18 Jul 2023 01:51:33 GMT  
		Size: 27.1 MB (27116407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9605105b68496ddcb5871d9313b51b49ff984efaf7993f0d2e84539e1fd35b1d`  
		Last Modified: Tue, 18 Jul 2023 01:51:32 GMT  
		Size: 13.4 MB (13364288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.10-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:421ccc57b89ad1944922fa394d2470b2be35a62b46beb5fa6f1f41f2c55d9fd8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47875497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ae0c1a5f5ac2b746df491ff907a5d5dac297aa1dd8f05331e7fad11dcddb89e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jul 2023 04:53:28 GMT
ARG RELEASE
# Wed, 12 Jul 2023 04:53:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 12 Jul 2023 04:53:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 12 Jul 2023 04:53:28 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 12 Jul 2023 04:53:31 GMT
ADD file:7028e8b5bb04424a3fa537fa5b5a311cfcaf1c8b6f321b414b40ee0388d0f9e0 in / 
# Wed, 12 Jul 2023 04:53:31 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 01:52:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:eaefff58e8d715237ca48dbc24624ab97d73780134b6abfa9397a3fb107c7847`  
		Last Modified: Tue, 18 Jul 2023 02:02:03 GMT  
		Size: 32.0 MB (31995451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3142716ff35072c411419b141a83ce524bc1af91e86195277f4ca49673988b19`  
		Last Modified: Tue, 18 Jul 2023 02:01:59 GMT  
		Size: 15.9 MB (15880046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.10-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:cc5d376a0d42b93c0b1aeb249929f492d1f04f9657bab633903b45c4d26539bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.4 MB (40360013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fb0b4528866fd72155a4910ab9744bcddf0bde069e7a9dba2084fe2d14eceb5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jul 2023 04:53:32 GMT
ARG RELEASE
# Wed, 12 Jul 2023 04:53:32 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 12 Jul 2023 04:53:32 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 12 Jul 2023 04:53:32 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 12 Jul 2023 04:53:34 GMT
ADD file:878995fa3a12c9df0a99fc88605932ffefec3e772a3c4ca89fe0c0aaa7dee67d in / 
# Wed, 12 Jul 2023 04:53:34 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 01:13:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f2b8f6b9cb3947ae25987d6e3685dc9709178b596bd7bf0d7a84ceeba23a2073`  
		Last Modified: Tue, 18 Jul 2023 01:18:14 GMT  
		Size: 26.3 MB (26322139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b736a5889ac0138557b62eaa679858540efdff47fa4079b2d261d5d981a0b7`  
		Last Modified: Tue, 18 Jul 2023 01:18:13 GMT  
		Size: 14.0 MB (14037874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:23.10-scm`

```console
$ docker pull buildpack-deps@sha256:6c84d5e0d47c58b2445b5df09de7e631d683929173e54ff24016b5de4f3a16e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:23.10-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:85d72857fea95aeb6d112513da095e1878f6e1efa45f440f9dcdee9d9a0b5370
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.3 MB (86321874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af7b8afe3427bf251dbae8dba5b9d858cdb087aeed3dc518427671aa5aea9ea4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jul 2023 04:50:42 GMT
ARG RELEASE
# Wed, 12 Jul 2023 04:50:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 12 Jul 2023 04:50:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 12 Jul 2023 04:50:42 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 12 Jul 2023 04:50:44 GMT
ADD file:592c8f21973a80f096ca38aaf5ef478d80f666517a169bc638ebb325f5ae07f4 in / 
# Wed, 12 Jul 2023 04:50:44 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 01:45:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 18 Jul 2023 01:45:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c57e6f7e53eccd34261640d6f245ad38a4ff7cc54ead279536b568d836363ae4`  
		Last Modified: Tue, 18 Jul 2023 01:49:46 GMT  
		Size: 27.8 MB (27758391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70262639a4fd505c867f716c40dd85135752950cc1aa365725b9e2967d66175a`  
		Last Modified: Tue, 18 Jul 2023 01:49:45 GMT  
		Size: 13.8 MB (13781000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade5aed8da7a4eb9b7d6f71f11a953d3491588e96cb6cd244876de5a69a96cea`  
		Last Modified: Tue, 18 Jul 2023 01:50:01 GMT  
		Size: 44.8 MB (44782483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.10-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:3b16df0cdce33f0ee6279409ac982bdb50248ac00be43888721544867e49c77c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.9 MB (86933441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21da3ba7664b82a047c70a8e69802637f613f60612974e0f52c505163dcdb1be`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jul 2023 04:54:17 GMT
ARG RELEASE
# Wed, 12 Jul 2023 04:54:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 12 Jul 2023 04:54:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 12 Jul 2023 04:54:17 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 12 Jul 2023 04:54:20 GMT
ADD file:6f71de5b8467fdcd7bcf88fbae117a520f903a91b00a674bdf8d44b14141f0d6 in / 
# Wed, 12 Jul 2023 04:54:20 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 04:39:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 18 Jul 2023 04:40:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2d27378af227ba4634a3837d7cb24660c6d297228e3b3a59b569c67e86c1b702`  
		Last Modified: Tue, 18 Jul 2023 04:44:33 GMT  
		Size: 25.3 MB (25310196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c20ac942533d1efa51f9b7223514a74aa29ec7a0272a22f2f548636534fd3f`  
		Last Modified: Tue, 18 Jul 2023 04:44:32 GMT  
		Size: 12.7 MB (12697617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5550cb2b09d3bf2b56d01eee2a5d36ef7263a4f3b0d35f84ebe938e6f64ab689`  
		Last Modified: Tue, 18 Jul 2023 04:44:49 GMT  
		Size: 48.9 MB (48925628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.10-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:29540c8fb7fe2cbff1c5b2ebbe79377102298bb93e3176b97416e36008ebef3d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.1 MB (85116674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f2d4533597e76b8d10fc71998896d25f47ab73decd47de07630f4cbb9c0e52e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jul 2023 04:54:30 GMT
ARG RELEASE
# Wed, 12 Jul 2023 04:54:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 12 Jul 2023 04:54:31 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 12 Jul 2023 04:54:31 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 12 Jul 2023 04:54:38 GMT
ADD file:6eb08bb754e74bd297a54d5c56c7622fe3945c0e013d8a48b8d85b09f1818099 in / 
# Wed, 12 Jul 2023 04:54:39 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 01:46:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 18 Jul 2023 01:46:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4f4369a81c2a2103bb37c89ff5ddb71caf0eefa6abc6ace3a6312b114b1b43f4`  
		Last Modified: Tue, 18 Jul 2023 01:51:33 GMT  
		Size: 27.1 MB (27116407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9605105b68496ddcb5871d9313b51b49ff984efaf7993f0d2e84539e1fd35b1d`  
		Last Modified: Tue, 18 Jul 2023 01:51:32 GMT  
		Size: 13.4 MB (13364288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7138fb2464b9037662e225fd640c60489c9bdfc93091ead842a55da631876df`  
		Last Modified: Tue, 18 Jul 2023 01:51:47 GMT  
		Size: 44.6 MB (44635979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.10-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:5427d53e2a0f36be11ddee624b8c2282efb28ea974220e842386fef4566bb3ce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.4 MB (97390756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1490ac353d73761f55f94aaa4b8e908f4e3c1ecdff0aeef98c7eb21967229e66`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jul 2023 04:53:28 GMT
ARG RELEASE
# Wed, 12 Jul 2023 04:53:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 12 Jul 2023 04:53:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 12 Jul 2023 04:53:28 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 12 Jul 2023 04:53:31 GMT
ADD file:7028e8b5bb04424a3fa537fa5b5a311cfcaf1c8b6f321b414b40ee0388d0f9e0 in / 
# Wed, 12 Jul 2023 04:53:31 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 01:52:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 18 Jul 2023 01:54:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:eaefff58e8d715237ca48dbc24624ab97d73780134b6abfa9397a3fb107c7847`  
		Last Modified: Tue, 18 Jul 2023 02:02:03 GMT  
		Size: 32.0 MB (31995451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3142716ff35072c411419b141a83ce524bc1af91e86195277f4ca49673988b19`  
		Last Modified: Tue, 18 Jul 2023 02:01:59 GMT  
		Size: 15.9 MB (15880046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5986d60cc2d030634cd4d91824fd3926b4c50f5ff1bed4d038671c930e6dc5`  
		Last Modified: Tue, 18 Jul 2023 02:02:28 GMT  
		Size: 49.5 MB (49515259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.10-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:0701a87a39ba7a5b13f5af26dd438551eae62de80cfb8e120b20da4016b92148
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.0 MB (85005805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c8e32e1c8a0607953bad4aa48adfe5b58e9641c89ddaa7c104660b0848cd95d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jul 2023 04:53:32 GMT
ARG RELEASE
# Wed, 12 Jul 2023 04:53:32 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 12 Jul 2023 04:53:32 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 12 Jul 2023 04:53:32 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 12 Jul 2023 04:53:34 GMT
ADD file:878995fa3a12c9df0a99fc88605932ffefec3e772a3c4ca89fe0c0aaa7dee67d in / 
# Wed, 12 Jul 2023 04:53:34 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 01:13:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 18 Jul 2023 01:14:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f2b8f6b9cb3947ae25987d6e3685dc9709178b596bd7bf0d7a84ceeba23a2073`  
		Last Modified: Tue, 18 Jul 2023 01:18:14 GMT  
		Size: 26.3 MB (26322139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b736a5889ac0138557b62eaa679858540efdff47fa4079b2d261d5d981a0b7`  
		Last Modified: Tue, 18 Jul 2023 01:18:13 GMT  
		Size: 14.0 MB (14037874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15d33eaf6ee65a8ded43a590675151bb6e283880b75995e7651a1b22700ecbe`  
		Last Modified: Tue, 18 Jul 2023 01:18:27 GMT  
		Size: 44.6 MB (44645792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bookworm`

```console
$ docker pull buildpack-deps@sha256:e8045f6c5b35d465af4400cf07baf28937774c70d0b67b75db9aa5a772245507
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
$ docker pull buildpack-deps@sha256:9fa042ef286f67914fb32a3dc539a9a9011d3030d11178a287fec058f4af2e0d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.7 MB (348696237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:870f7a6134d053997696565f36185aa08d0268c5d2ead2098c03ec2543d8c186`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:19:44 GMT
ADD file:5d17ca085473e890bd6eca4abf6d324c3181f80692523b83ef25d1c42576b99f in / 
# Tue, 04 Jul 2023 01:19:44 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:27:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:28:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:29:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d52e4f012db158bb7c0fe215b98af1facaddcbaee530efd69b1bae07d597b711`  
		Last Modified: Tue, 04 Jul 2023 01:24:39 GMT  
		Size: 49.6 MB (49551432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd206bea61ff3e3b54be1c20b58d8475ddd6f89df176146ddb7a2fd2c747ea2`  
		Last Modified: Tue, 04 Jul 2023 03:51:23 GMT  
		Size: 24.0 MB (24030593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2320f9be4a9c605d1ac847cf67cec42b91484a7cf7c94996417a0c7c316deadc`  
		Last Modified: Tue, 04 Jul 2023 03:51:42 GMT  
		Size: 64.1 MB (64111613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5565e0ba8dfce32b9049f21ceeb212946e0bb810d94cbd2db94ca61082f657`  
		Last Modified: Tue, 04 Jul 2023 03:52:18 GMT  
		Size: 211.0 MB (211002599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:7630e74069ab9afc052421fab33b53a63046a9f0a81ca78e752b60f0bf5e6f30
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.0 MB (315974639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efd6d55edc39161f4227507b095e44656ca35b9df7ba73a742e6d46ac8dcbac8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:48:22 GMT
ADD file:09001854dc5081f907ac2a66d301e4b3d6b4bf2c2483aad5395a535bf068698d in / 
# Tue, 04 Jul 2023 00:48:22 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:21:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:21:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:24:09 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7e0a1f476b42bcc214197ec9c5ef753ddf2ab36a314416a6ac96cd921ff0d41d`  
		Last Modified: Tue, 04 Jul 2023 00:51:29 GMT  
		Size: 47.4 MB (47402786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68311cc5ff511aa59283fdd7f1e25bc33dfc3ad9ae87e5c94447f36c3f7c4817`  
		Last Modified: Tue, 04 Jul 2023 04:28:32 GMT  
		Size: 22.7 MB (22708933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09518fc93ba137cac901dd7b0cc5fab1e20a21a7d6bbe3a35b7f921a069ddc5c`  
		Last Modified: Tue, 04 Jul 2023 04:28:53 GMT  
		Size: 61.6 MB (61553936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0a9d5bee850aae2d389dee19882ddf586d298ba8cc4d4100b77a7bc33204f0`  
		Last Modified: Tue, 04 Jul 2023 04:29:28 GMT  
		Size: 184.3 MB (184308984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:ccbb43b6d2ff2010f6972b17d2c35e80179b93721b3b4075a83d17fd211df4d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.4 MB (301419261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71ba632fe6ed398564cb984e2524c39cfe7c23c5d5ce9b754516330315011653`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:57:42 GMT
ADD file:279ef7213d41f1f7ae76bd76293a5107fd1f8caf557f837cab9c834d2841e031 in / 
# Tue, 04 Jul 2023 00:57:43 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:49:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:50:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:51:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b9bdcf1a9a6361f231594c76a75bfb4c2fef5f9745b9713bbd50efaf37ca11b8`  
		Last Modified: Tue, 04 Jul 2023 01:02:26 GMT  
		Size: 45.2 MB (45236201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8ee33ea63b2391e912423c14b2f1e789137ffb03659568cb361a2fa2b4efbd`  
		Last Modified: Tue, 04 Jul 2023 06:18:41 GMT  
		Size: 21.9 MB (21936446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2a5b4416a84ac4585c3e3879ca49a6fc3e8d46028a4f27098ae1bdb4ae710d`  
		Last Modified: Tue, 04 Jul 2023 06:19:01 GMT  
		Size: 59.3 MB (59261674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfb211eb5b07ec381fa590fdb20338a17e1ac7282488bfe67ebf61eb9d8ef36`  
		Last Modified: Tue, 04 Jul 2023 06:19:36 GMT  
		Size: 175.0 MB (174984940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a11d7b66e7e9ee6221856ac61d5a24ac2fa826652e2ad6decc9068462572a119
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.5 MB (339524386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41b72a638a02bcfb5b6fb54590f95199209e6bb9e8ba83b5675a76bdd3a62b4d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:26 GMT
ADD file:ab1761d899751c4d24e15179fc9e7e7ac3fb83798ee37ca13d6a6ac44fbeded3 in / 
# Tue, 04 Jul 2023 01:57:27 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:54:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:54:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:56:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:42cbebf8bc116ba1aed7897e2d0566bf49da9d5c70be71b6a7cb07805d2f5b7a`  
		Last Modified: Tue, 04 Jul 2023 02:00:57 GMT  
		Size: 49.6 MB (49572781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0518ec57568a70561f7c04650f9554c88dada973f54d88e36f65b0796d35de`  
		Last Modified: Tue, 04 Jul 2023 06:21:03 GMT  
		Size: 23.6 MB (23569546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356172c718acf9930d9465b170864319079e2d2ebac0ddef781d64e85789531e`  
		Last Modified: Tue, 04 Jul 2023 06:21:20 GMT  
		Size: 64.0 MB (63984075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dddcd3ceb9980caac379e8f8eeafe1e901f017e5768b867705a0834cc1274efa`  
		Last Modified: Tue, 04 Jul 2023 06:21:49 GMT  
		Size: 202.4 MB (202397984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:bd112b098fcf0109e2d3d75cb01da9035f9aa2b763863b2be966c3c1a892b655
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.3 MB (351325313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a527ba005f783dc8585ad58568efedd0ad8a89a20c2877cd3b9cd5bfc634702`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:38:25 GMT
ADD file:e0a25fe261e09183ec383698ab2c800f93c5b0805564d7104ad5119db52cccb7 in / 
# Tue, 04 Jul 2023 01:38:25 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:28:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:28:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:30:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:381263dab43af8bfb8e85c7a9a32f35492cbdcc3a046b35f947cf3bf3a55f4c1`  
		Last Modified: Tue, 04 Jul 2023 01:43:02 GMT  
		Size: 50.6 MB (50562388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af522778d6fcd5f4b85dafb1f21b89441dedee6ce875890b15ad8c454bbb9fe6`  
		Last Modified: Tue, 04 Jul 2023 05:38:10 GMT  
		Size: 24.9 MB (24869747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501f685d713d76bdc0731a917b074d79f3de7c84bfe09c53585642801175a72f`  
		Last Modified: Tue, 04 Jul 2023 05:38:34 GMT  
		Size: 66.0 MB (65972310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993e54703a4428a35a92b50b46a2b72088e5f98ec8687291e59ba960778653ce`  
		Last Modified: Tue, 04 Jul 2023 05:39:21 GMT  
		Size: 209.9 MB (209920868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:109dccdd704f2335380eafe52886c571b5ecc9fc6f8e8ff477f178f88a1bcd3a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.7 MB (325698556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63ff7002fa7f867935af5542ea11c588ff00e71b610322da6f1ee76d404f1372`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:08:42 GMT
ADD file:c567fc0f97f36ea531c05e159cd6ac2a8747f14ea5b6ccae39bab9d305da180d in / 
# Tue, 04 Jul 2023 01:08:47 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:34:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:36:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:42:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76240e493592cbc7ca56583a6e8e03ab12a967b65bbeb1df7828a5099fa271d9`  
		Last Modified: Tue, 04 Jul 2023 01:19:16 GMT  
		Size: 49.5 MB (49542143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85086244c52affe40f860feee6e34c03fd0f782e853b00950f1a9b8b6704d24f`  
		Last Modified: Tue, 04 Jul 2023 14:56:03 GMT  
		Size: 23.6 MB (23611680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2482ef924bba9e0b7ef4ad15506bbcf2a7db029acfc793f94b5d17435ed529`  
		Last Modified: Tue, 04 Jul 2023 14:56:55 GMT  
		Size: 63.0 MB (62950425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a976801f0e288a1695ce313557e999ec73ed5562492816ed2e559f8fadcba08`  
		Last Modified: Tue, 04 Jul 2023 14:58:59 GMT  
		Size: 189.6 MB (189594308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d118d12ab7bda84f249868aa497f83e1ee8489b9062b3d275991f7c9178fb44a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.8 MB (362817855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07b0cde07b2b8c19168a241b2b585bba6b27c80cdb9761dfd1dcba9a1d952f9f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:17:23 GMT
ADD file:5aaa642008df5a97014e76042a767f06bbfda91db1d5f336a1b3f98e9b11c7a1 in / 
# Tue, 04 Jul 2023 01:17:26 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:26:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:27:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:32:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e039cf6634cf83a31e97e2a56b4db40a8c38a62d6857c77e687d5edb3eb0dfde`  
		Last Modified: Tue, 04 Jul 2023 01:23:59 GMT  
		Size: 53.5 MB (53536740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54fff62f5ff539ace95f1581096d57b95ca024b9d5cc7c85bb4a2bf159ad845f`  
		Last Modified: Tue, 04 Jul 2023 04:36:20 GMT  
		Size: 25.7 MB (25681297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd5a2ec3d78fd420afc5e1c6739ad59505cf484be0ea1c2c2dfe00c7b2c00ec`  
		Last Modified: Tue, 04 Jul 2023 04:36:52 GMT  
		Size: 69.6 MB (69569498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c3418743f63acf6f2325abc19057fd064d786b061702494a8afd12dba2787ca`  
		Last Modified: Tue, 04 Jul 2023 04:37:57 GMT  
		Size: 214.0 MB (214030320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:8ae64baa0daee2c34ad05f273d64404d1daf9cbdcb9cf75baa84eaeee3aa34ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.1 MB (318132923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:208c88d3645147348e10f8100a5ad65a12fb037cebe1b20bfa7551fee026e98c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:31:54 GMT
ADD file:0ad7ffbe777e5367ad6dcbb4a182e1d578739aa7a4853f82f21bd71d824de7ae in / 
# Tue, 04 Jul 2023 01:31:56 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 12:47:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 12:47:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 12:48:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce9d001c0d31ec9b8072b1a9bd01771a10ea8ddfefa381cf9ce7e2d63538aaeb`  
		Last Modified: Tue, 04 Jul 2023 01:36:50 GMT  
		Size: 47.9 MB (47921709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024bda56b20d3018344098f67965337568b532ea03f09d87858a2bb5eae82bf7`  
		Last Modified: Tue, 04 Jul 2023 13:05:34 GMT  
		Size: 24.0 MB (24028793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da5b83dc971cc08c6baeb1ddd5fb5de06beefef83c0444c224b4e377d704705`  
		Last Modified: Tue, 04 Jul 2023 13:05:50 GMT  
		Size: 63.1 MB (63112809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3bc88ad73a4c8df0ca6b17f424b27e05a29533428b9a47f3576c9be9e81540c`  
		Last Modified: Tue, 04 Jul 2023 13:06:19 GMT  
		Size: 183.1 MB (183069612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bookworm-curl`

```console
$ docker pull buildpack-deps@sha256:5df62ac377f1dca70c63bb04aeacf175f11265542a35a451d592255cc0e38972
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

### `buildpack-deps:bookworm-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:4ce7e846f60727efea42b5abdfd8673e13a94e288c6a5d7c37da1973ce7c5d78
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73582025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c399a665f317215e5dd18dcf72a1723bc891edc5df1e57bf176d1c65f757cd0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:19:44 GMT
ADD file:5d17ca085473e890bd6eca4abf6d324c3181f80692523b83ef25d1c42576b99f in / 
# Tue, 04 Jul 2023 01:19:44 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:27:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d52e4f012db158bb7c0fe215b98af1facaddcbaee530efd69b1bae07d597b711`  
		Last Modified: Tue, 04 Jul 2023 01:24:39 GMT  
		Size: 49.6 MB (49551432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd206bea61ff3e3b54be1c20b58d8475ddd6f89df176146ddb7a2fd2c747ea2`  
		Last Modified: Tue, 04 Jul 2023 03:51:23 GMT  
		Size: 24.0 MB (24030593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:cd79b4dbc7daadcec5980ed2d535ce9340c36adea17ccf7dbb0c0d2712ca57e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.1 MB (70111719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dea85fcb87a6435ababbbc09b75d697c82c737049086f3d59690dca803e1758d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:48:22 GMT
ADD file:09001854dc5081f907ac2a66d301e4b3d6b4bf2c2483aad5395a535bf068698d in / 
# Tue, 04 Jul 2023 00:48:22 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:21:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7e0a1f476b42bcc214197ec9c5ef753ddf2ab36a314416a6ac96cd921ff0d41d`  
		Last Modified: Tue, 04 Jul 2023 00:51:29 GMT  
		Size: 47.4 MB (47402786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68311cc5ff511aa59283fdd7f1e25bc33dfc3ad9ae87e5c94447f36c3f7c4817`  
		Last Modified: Tue, 04 Jul 2023 04:28:32 GMT  
		Size: 22.7 MB (22708933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:ee52b93b57b097abb318a077905af9d187e98a1feb6c49f47ad7368f254dac9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67172647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7745cabe6a186fe38c73aa2d5384961dc430b541f6f0ccee40bb24c7865441c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:57:42 GMT
ADD file:279ef7213d41f1f7ae76bd76293a5107fd1f8caf557f837cab9c834d2841e031 in / 
# Tue, 04 Jul 2023 00:57:43 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:49:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b9bdcf1a9a6361f231594c76a75bfb4c2fef5f9745b9713bbd50efaf37ca11b8`  
		Last Modified: Tue, 04 Jul 2023 01:02:26 GMT  
		Size: 45.2 MB (45236201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8ee33ea63b2391e912423c14b2f1e789137ffb03659568cb361a2fa2b4efbd`  
		Last Modified: Tue, 04 Jul 2023 06:18:41 GMT  
		Size: 21.9 MB (21936446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c6b1b12d88f18474b52830b7189f2d54b534002ee9b00dbe7a5947684dbbef4d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.1 MB (73142327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ccf74d87c178f322cc3cc0e5b79bb62adfcb518a1c78943c8a7d7241427f748`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:26 GMT
ADD file:ab1761d899751c4d24e15179fc9e7e7ac3fb83798ee37ca13d6a6ac44fbeded3 in / 
# Tue, 04 Jul 2023 01:57:27 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:54:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:42cbebf8bc116ba1aed7897e2d0566bf49da9d5c70be71b6a7cb07805d2f5b7a`  
		Last Modified: Tue, 04 Jul 2023 02:00:57 GMT  
		Size: 49.6 MB (49572781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0518ec57568a70561f7c04650f9554c88dada973f54d88e36f65b0796d35de`  
		Last Modified: Tue, 04 Jul 2023 06:21:03 GMT  
		Size: 23.6 MB (23569546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:abb0cf0f3dc36c7e284598893d32388fe2b09b68e02ef75869a6ddce988d6624
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75432135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce569bff52f1ef304acf004cee953e9829211468502cb021457f297c7f8d098d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:38:25 GMT
ADD file:e0a25fe261e09183ec383698ab2c800f93c5b0805564d7104ad5119db52cccb7 in / 
# Tue, 04 Jul 2023 01:38:25 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:28:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:381263dab43af8bfb8e85c7a9a32f35492cbdcc3a046b35f947cf3bf3a55f4c1`  
		Last Modified: Tue, 04 Jul 2023 01:43:02 GMT  
		Size: 50.6 MB (50562388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af522778d6fcd5f4b85dafb1f21b89441dedee6ce875890b15ad8c454bbb9fe6`  
		Last Modified: Tue, 04 Jul 2023 05:38:10 GMT  
		Size: 24.9 MB (24869747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:daeb0fffa382ebd3757c35f7edef327defb7d926134b88529b5ac12bfe9bda74
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73153823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe85240ea372bde5df08e1b08faeb8632ed7dedae4aba518ab2d7bc1488ca70e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:08:42 GMT
ADD file:c567fc0f97f36ea531c05e159cd6ac2a8747f14ea5b6ccae39bab9d305da180d in / 
# Tue, 04 Jul 2023 01:08:47 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:34:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76240e493592cbc7ca56583a6e8e03ab12a967b65bbeb1df7828a5099fa271d9`  
		Last Modified: Tue, 04 Jul 2023 01:19:16 GMT  
		Size: 49.5 MB (49542143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85086244c52affe40f860feee6e34c03fd0f782e853b00950f1a9b8b6704d24f`  
		Last Modified: Tue, 04 Jul 2023 14:56:03 GMT  
		Size: 23.6 MB (23611680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:dd742426422d9d9c53b1f294d91895bd56b7748b0a559826babb53cec399ddef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.2 MB (79218037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4572b0656e7dfc6731b3f7dd64ee5baeb3421d7762079b77c60f1226bfa152f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:17:23 GMT
ADD file:5aaa642008df5a97014e76042a767f06bbfda91db1d5f336a1b3f98e9b11c7a1 in / 
# Tue, 04 Jul 2023 01:17:26 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:26:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e039cf6634cf83a31e97e2a56b4db40a8c38a62d6857c77e687d5edb3eb0dfde`  
		Last Modified: Tue, 04 Jul 2023 01:23:59 GMT  
		Size: 53.5 MB (53536740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54fff62f5ff539ace95f1581096d57b95ca024b9d5cc7c85bb4a2bf159ad845f`  
		Last Modified: Tue, 04 Jul 2023 04:36:20 GMT  
		Size: 25.7 MB (25681297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:d5f47922100fab7fa779f085640d993e6625e6f15956c228a3b1475b38baf460
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.0 MB (71950502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ebcb0cef8f138e8e985dd005eeee2dd6d64c40eef9668d4b648caec9ec37c6a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:31:54 GMT
ADD file:0ad7ffbe777e5367ad6dcbb4a182e1d578739aa7a4853f82f21bd71d824de7ae in / 
# Tue, 04 Jul 2023 01:31:56 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 12:47:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce9d001c0d31ec9b8072b1a9bd01771a10ea8ddfefa381cf9ce7e2d63538aaeb`  
		Last Modified: Tue, 04 Jul 2023 01:36:50 GMT  
		Size: 47.9 MB (47921709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024bda56b20d3018344098f67965337568b532ea03f09d87858a2bb5eae82bf7`  
		Last Modified: Tue, 04 Jul 2023 13:05:34 GMT  
		Size: 24.0 MB (24028793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bookworm-scm`

```console
$ docker pull buildpack-deps@sha256:12a2678b3eabf425fa2c142421e1db4dfe6ab854a537af91c289507745c71b36
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

### `buildpack-deps:bookworm-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:0f78de2b3312f09866ac4eaaba883d518e886b540ceeff548750914b935f8e50
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.7 MB (137693638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:064924f22ba6cc021e9ca9ae3e10d21b15e491c0d1387c5f62300c70241c04d1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:19:44 GMT
ADD file:5d17ca085473e890bd6eca4abf6d324c3181f80692523b83ef25d1c42576b99f in / 
# Tue, 04 Jul 2023 01:19:44 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:27:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:28:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d52e4f012db158bb7c0fe215b98af1facaddcbaee530efd69b1bae07d597b711`  
		Last Modified: Tue, 04 Jul 2023 01:24:39 GMT  
		Size: 49.6 MB (49551432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd206bea61ff3e3b54be1c20b58d8475ddd6f89df176146ddb7a2fd2c747ea2`  
		Last Modified: Tue, 04 Jul 2023 03:51:23 GMT  
		Size: 24.0 MB (24030593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2320f9be4a9c605d1ac847cf67cec42b91484a7cf7c94996417a0c7c316deadc`  
		Last Modified: Tue, 04 Jul 2023 03:51:42 GMT  
		Size: 64.1 MB (64111613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:27d15e25a27b8983778bfedc271e37fbf73269e16b907efc0f8c0a4af8c912b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.7 MB (131665655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dac77eebbb12f590d8e6de52e972d43c54544315b77364e7101d186dd5aad91c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:48:22 GMT
ADD file:09001854dc5081f907ac2a66d301e4b3d6b4bf2c2483aad5395a535bf068698d in / 
# Tue, 04 Jul 2023 00:48:22 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:21:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:21:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7e0a1f476b42bcc214197ec9c5ef753ddf2ab36a314416a6ac96cd921ff0d41d`  
		Last Modified: Tue, 04 Jul 2023 00:51:29 GMT  
		Size: 47.4 MB (47402786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68311cc5ff511aa59283fdd7f1e25bc33dfc3ad9ae87e5c94447f36c3f7c4817`  
		Last Modified: Tue, 04 Jul 2023 04:28:32 GMT  
		Size: 22.7 MB (22708933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09518fc93ba137cac901dd7b0cc5fab1e20a21a7d6bbe3a35b7f921a069ddc5c`  
		Last Modified: Tue, 04 Jul 2023 04:28:53 GMT  
		Size: 61.6 MB (61553936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:36fa95975190dc678d40a37a93185f66e9192b8c80dec22c959399e2f7ec2569
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.4 MB (126434321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3da8a85987ffb7432f4d6f66364a39ac772f3a9b6bff23ba597689223f28b4b3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:57:42 GMT
ADD file:279ef7213d41f1f7ae76bd76293a5107fd1f8caf557f837cab9c834d2841e031 in / 
# Tue, 04 Jul 2023 00:57:43 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:49:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:50:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b9bdcf1a9a6361f231594c76a75bfb4c2fef5f9745b9713bbd50efaf37ca11b8`  
		Last Modified: Tue, 04 Jul 2023 01:02:26 GMT  
		Size: 45.2 MB (45236201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8ee33ea63b2391e912423c14b2f1e789137ffb03659568cb361a2fa2b4efbd`  
		Last Modified: Tue, 04 Jul 2023 06:18:41 GMT  
		Size: 21.9 MB (21936446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2a5b4416a84ac4585c3e3879ca49a6fc3e8d46028a4f27098ae1bdb4ae710d`  
		Last Modified: Tue, 04 Jul 2023 06:19:01 GMT  
		Size: 59.3 MB (59261674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a5cb7353b2ce88aeffff9c11400ba2868c5da3edae5c9ee5c2c4c09312ced7e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.1 MB (137126402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb40501a95e932bb48d49f74d197ea8377d1ccba9e2dd9f66e63fdf9de21b409`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:26 GMT
ADD file:ab1761d899751c4d24e15179fc9e7e7ac3fb83798ee37ca13d6a6ac44fbeded3 in / 
# Tue, 04 Jul 2023 01:57:27 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:54:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:54:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:42cbebf8bc116ba1aed7897e2d0566bf49da9d5c70be71b6a7cb07805d2f5b7a`  
		Last Modified: Tue, 04 Jul 2023 02:00:57 GMT  
		Size: 49.6 MB (49572781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0518ec57568a70561f7c04650f9554c88dada973f54d88e36f65b0796d35de`  
		Last Modified: Tue, 04 Jul 2023 06:21:03 GMT  
		Size: 23.6 MB (23569546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356172c718acf9930d9465b170864319079e2d2ebac0ddef781d64e85789531e`  
		Last Modified: Tue, 04 Jul 2023 06:21:20 GMT  
		Size: 64.0 MB (63984075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:e93d1e1d0a091272e88d7d8bf0e0e21b3df095765d52c1007b9bbab8d01069f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.4 MB (141404445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d40934ac087de93ceffbf81437543947fc9c9c8b8184568346ac03da80f35bd7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:38:25 GMT
ADD file:e0a25fe261e09183ec383698ab2c800f93c5b0805564d7104ad5119db52cccb7 in / 
# Tue, 04 Jul 2023 01:38:25 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:28:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:28:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:381263dab43af8bfb8e85c7a9a32f35492cbdcc3a046b35f947cf3bf3a55f4c1`  
		Last Modified: Tue, 04 Jul 2023 01:43:02 GMT  
		Size: 50.6 MB (50562388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af522778d6fcd5f4b85dafb1f21b89441dedee6ce875890b15ad8c454bbb9fe6`  
		Last Modified: Tue, 04 Jul 2023 05:38:10 GMT  
		Size: 24.9 MB (24869747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501f685d713d76bdc0731a917b074d79f3de7c84bfe09c53585642801175a72f`  
		Last Modified: Tue, 04 Jul 2023 05:38:34 GMT  
		Size: 66.0 MB (65972310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:68087f9d2d7eb43f96f073504d68e5f68181fe9c905f47fb14815bec8db79572
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.1 MB (136104248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0d288a207994f6184d90c784bdde0152350cd4c6bf91f0777b8da30da1a0c3e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:08:42 GMT
ADD file:c567fc0f97f36ea531c05e159cd6ac2a8747f14ea5b6ccae39bab9d305da180d in / 
# Tue, 04 Jul 2023 01:08:47 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:34:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:36:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76240e493592cbc7ca56583a6e8e03ab12a967b65bbeb1df7828a5099fa271d9`  
		Last Modified: Tue, 04 Jul 2023 01:19:16 GMT  
		Size: 49.5 MB (49542143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85086244c52affe40f860feee6e34c03fd0f782e853b00950f1a9b8b6704d24f`  
		Last Modified: Tue, 04 Jul 2023 14:56:03 GMT  
		Size: 23.6 MB (23611680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2482ef924bba9e0b7ef4ad15506bbcf2a7db029acfc793f94b5d17435ed529`  
		Last Modified: Tue, 04 Jul 2023 14:56:55 GMT  
		Size: 63.0 MB (62950425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:a1876fdc603fdf011be6b83ff792c330a17e2743922fd5aabaf6a1ed5c037080
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.8 MB (148787535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62c051da923c5734b37ef3d706b3ecdfe384634edc45b782adb0b0e0f06f84db`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:17:23 GMT
ADD file:5aaa642008df5a97014e76042a767f06bbfda91db1d5f336a1b3f98e9b11c7a1 in / 
# Tue, 04 Jul 2023 01:17:26 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:26:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:27:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e039cf6634cf83a31e97e2a56b4db40a8c38a62d6857c77e687d5edb3eb0dfde`  
		Last Modified: Tue, 04 Jul 2023 01:23:59 GMT  
		Size: 53.5 MB (53536740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54fff62f5ff539ace95f1581096d57b95ca024b9d5cc7c85bb4a2bf159ad845f`  
		Last Modified: Tue, 04 Jul 2023 04:36:20 GMT  
		Size: 25.7 MB (25681297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd5a2ec3d78fd420afc5e1c6739ad59505cf484be0ea1c2c2dfe00c7b2c00ec`  
		Last Modified: Tue, 04 Jul 2023 04:36:52 GMT  
		Size: 69.6 MB (69569498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:26e61b2a6df1a810689cbf8a1b2b097496c6de014ff7013b8f3c0466dc100308
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.1 MB (135063311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:875d66c05f546cc0a92a5aed5599d58335c22c67b0706c82bc06056c3af12657`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:31:54 GMT
ADD file:0ad7ffbe777e5367ad6dcbb4a182e1d578739aa7a4853f82f21bd71d824de7ae in / 
# Tue, 04 Jul 2023 01:31:56 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 12:47:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 12:47:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce9d001c0d31ec9b8072b1a9bd01771a10ea8ddfefa381cf9ce7e2d63538aaeb`  
		Last Modified: Tue, 04 Jul 2023 01:36:50 GMT  
		Size: 47.9 MB (47921709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024bda56b20d3018344098f67965337568b532ea03f09d87858a2bb5eae82bf7`  
		Last Modified: Tue, 04 Jul 2023 13:05:34 GMT  
		Size: 24.0 MB (24028793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da5b83dc971cc08c6baeb1ddd5fb5de06beefef83c0444c224b4e377d704705`  
		Last Modified: Tue, 04 Jul 2023 13:05:50 GMT  
		Size: 63.1 MB (63112809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bullseye`

```console
$ docker pull buildpack-deps@sha256:7742ec0838b3c91afb08f8e2e3a5abc2a5379fe6f7e6c242ed4d3b472c7c5c73
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

### `buildpack-deps:bullseye` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:d4136e8b26283648c23085988ff9320469071a6d71af1d5f5652f0d0b0129090
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.3 MB (322251560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32c83682cffffc48f1d1da4b634def742c08aa1baeb486df6bfc1668b8cd44e9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:09 GMT
ADD file:b7c0be2bb90e88689b1c16da78dea0b85760b55b90ef2e5bc4a529c89e4fa25b in / 
# Tue, 04 Jul 2023 01:20:10 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:30:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:30:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:31:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:34df401c391c7595044379e04e8ad4856a5a3974cdbf5a160f0a204d761e88aa`  
		Last Modified: Tue, 04 Jul 2023 01:25:21 GMT  
		Size: 55.1 MB (55055300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fdd0e5b72ccae203ec30d533c0bcd34200af90265e0531c66356812e529af32`  
		Last Modified: Tue, 04 Jul 2023 03:52:30 GMT  
		Size: 15.8 MB (15760327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa786a946ae67fa18e07eaf82fefee1777449f7db1a8fea5abec1aadbe99e2ef`  
		Last Modified: Tue, 04 Jul 2023 03:52:45 GMT  
		Size: 54.6 MB (54585046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f8721393bc605f2b915d80eb2ad6d5219db374f36bbd1fee99b99174a0a4ca`  
		Last Modified: Tue, 04 Jul 2023 03:53:17 GMT  
		Size: 196.9 MB (196850887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:6454d0b087354a1aa979f21afba2a5cbb8bab6b79f7acf4f0803d163c31bef27
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.3 MB (295304664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efbe088d0d18e6bb5c2e2c2eb6d78bfa4d530fb7fb8b31688c675550427d1153`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:48:39 GMT
ADD file:fe1b9f9f6c7d67ad23a2ee839774be4bcee33c60c7b34c48df5a08eb33cafd1b in / 
# Tue, 04 Jul 2023 00:48:40 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:24:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:25:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:26:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:702dd8b607f626c689176debe921fe96009c1ce6dbd66f4f238c7def50080e3d`  
		Last Modified: Tue, 04 Jul 2023 00:52:15 GMT  
		Size: 52.6 MB (52556778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec773064e3ff5287bd9be0bdb7b99e708aed435b4920a0f64aeaf158d9631f5e`  
		Last Modified: Tue, 04 Jul 2023 04:29:40 GMT  
		Size: 15.4 MB (15369118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ae2fc9256b17aac11e221f2db3d50e0543fecf87896a99ff9be68ea2335989`  
		Last Modified: Tue, 04 Jul 2023 04:29:57 GMT  
		Size: 52.3 MB (52340564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8a9d92ba07e083e1f009e2a61ce148b9c2863820ac5942c814661045a26d3b`  
		Last Modified: Tue, 04 Jul 2023 04:30:31 GMT  
		Size: 175.0 MB (175038204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:04f584cada918fac3166adc6f013bb067993f06516c6d749c8483c02842523eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.8 MB (282774067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:205c60f2f252ed7b84d5173a49821829c6238b95be89b3b23444c8c69021f8e6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:06 GMT
ADD file:17e02296458241d9441f8da6a5dafb747d528a729106b17cec2f4c1c8cfe0ad8 in / 
# Tue, 04 Jul 2023 00:58:07 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:51:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:52:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:53:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:31edf2db9ca1650aa08e2d42e9b5bb7349413d7212110149a1a5d202ac20914b`  
		Last Modified: Tue, 04 Jul 2023 01:03:12 GMT  
		Size: 50.2 MB (50218247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e794b9a6d62ad67f31927f253d3a467d402da7b96769cef6b5503fde01f18eb9`  
		Last Modified: Tue, 04 Jul 2023 06:19:48 GMT  
		Size: 14.9 MB (14868644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fdbc75406b7868979ba89f96e015c45fbcf9efe34aa3863e52c0e926531784f`  
		Last Modified: Tue, 04 Jul 2023 06:20:06 GMT  
		Size: 50.4 MB (50355287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b5420e300d967980b7a87e93da33a82950c1fb7d2024379f913ad516ac3814`  
		Last Modified: Tue, 04 Jul 2023 06:20:40 GMT  
		Size: 167.3 MB (167331889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:efad222cb293be53dd7045e6faaa4051e909d2cf1d4f82116f8260bb7b1439fa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.9 MB (313904743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e4dd2ebe3088f8dc545dfc68984603c52f4c0a5ff021ffda0c146afe58c1307`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:43 GMT
ADD file:e626446584d8094b7b58d72a717380ca64d3e9ab924fc625406fe26a83fe1d8b in / 
# Tue, 04 Jul 2023 01:57:43 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:56:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:56:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:58:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:29279ac7c19f9c667f1c6b07bfba6fba20ca0d945b9fbc6edad6f75d13361fae`  
		Last Modified: Tue, 04 Jul 2023 02:01:38 GMT  
		Size: 53.7 MB (53703979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d0c3fcc5367be60f92df0774820f317a179565cd3ee9c222f5500a7be32151e`  
		Last Modified: Tue, 04 Jul 2023 06:22:01 GMT  
		Size: 15.7 MB (15746747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5fa66dbb545c6ff93c768ac595d874b2f22053e8d2f842f4b6ccc310ebfe0c`  
		Last Modified: Tue, 04 Jul 2023 06:22:15 GMT  
		Size: 54.7 MB (54676075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790673d5b08f786a9f9e0a1db5dd3941e80d10bde172f69852e2c405b2eb3ad3`  
		Last Modified: Tue, 04 Jul 2023 06:22:40 GMT  
		Size: 189.8 MB (189777942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; 386

```console
$ docker pull buildpack-deps@sha256:3614c9ca25a1730d80fefac448488f742bf8e12204b6a018b74e7886cc1d21d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.0 MB (327993696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fdb716512bdd67e2d576da09577000f35f580c4b3edec03b1d38dfa940db50b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:38:48 GMT
ADD file:c5739407c2c257fbb85ab4b9dcd2dc07e6fe172d7309aaaaab544c8df6c42b92 in / 
# Tue, 04 Jul 2023 01:38:49 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:30:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:31:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:32:48 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b700c8b35944e0d5f6ab9049dbe2262492e26327a8efad518b1011428393653f`  
		Last Modified: Tue, 04 Jul 2023 01:43:49 GMT  
		Size: 56.0 MB (56040756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414994a3b1789f89f704fcfc0e721c0036089a74368f21aa6fafa639fef2c93b`  
		Last Modified: Tue, 04 Jul 2023 05:39:34 GMT  
		Size: 16.3 MB (16263605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ee301eb66e57dfaf79983158c75b77a7775e1b6216c45ce247c6fac3786a46`  
		Last Modified: Tue, 04 Jul 2023 05:39:53 GMT  
		Size: 55.9 MB (55922990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28c7ac3e45d13ee62a7daff4eb413a3752789ab4b5620de47a04abff3a358cc`  
		Last Modified: Tue, 04 Jul 2023 05:40:36 GMT  
		Size: 199.8 MB (199766345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:3ae9f3837f9c3b468acf4a7e4d75ffa8718eba2055611425c88d9536f671a64f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.1 MB (301070599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75f1f194f73750062c6fdf2e936746353f2db097aa555efd67dd295da04000b2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:10:02 GMT
ADD file:f7ddd7406e3aa24165fc80933583fc2298f9792865511fe65def2f571fed2207 in / 
# Tue, 04 Jul 2023 01:10:07 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:43:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:45:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:51:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:af98e96208d7ce4cff5417a3e8a38f98d2ed3abbca318e1e6c323aa8b8c56690`  
		Last Modified: Tue, 04 Jul 2023 01:20:40 GMT  
		Size: 53.3 MB (53270472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b8f3d09abba473eec10e4fe5adebd33b18a790b9e57fdd8a5b484c925486df`  
		Last Modified: Tue, 04 Jul 2023 14:59:18 GMT  
		Size: 15.5 MB (15520537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427c4e665dab89a7a9a5cef3f1bab709cd38d4945e49ef760b95611e774a07e4`  
		Last Modified: Tue, 04 Jul 2023 15:00:02 GMT  
		Size: 53.3 MB (53306638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7915d90967431c4046270617a5aa6c09863c49d6e707dd149a919875c0326ad5`  
		Last Modified: Tue, 04 Jul 2023 15:01:58 GMT  
		Size: 179.0 MB (178972952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:24871bd43939bccce8bbff3de498e9bb620b00d2e7fe4ec7f90c016b206635ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.7 MB (330742890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a240664eeabe8f3b43cc9a1797fed091713e4cc8a20e28695d70e6059d7ef0d9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:18:11 GMT
ADD file:ff86c25854c28609c2852c1615270f0acd4c4efaa38ff8ed9c23afe5132f2135 in / 
# Tue, 04 Jul 2023 01:18:15 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:33:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:33:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:37:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a792749f62225048efdf85841bea6f3999f586371852f3dbce13a6c3d89b1fa7`  
		Last Modified: Tue, 04 Jul 2023 01:25:06 GMT  
		Size: 58.9 MB (58927745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf553284aac150acedeaf1c5f33c1820a34bff4f20ef96c32510ee19f2be0e83`  
		Last Modified: Tue, 04 Jul 2023 04:38:16 GMT  
		Size: 16.8 MB (16752898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b8f1977f7b061bf5ae7311bb1750877d9ba871f041ba604c8e1e9d1e1143e0`  
		Last Modified: Tue, 04 Jul 2023 04:38:44 GMT  
		Size: 58.9 MB (58864695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17f0a018912d7d71fedea77bea42cdadad1900e4a2885ca8b28fef63c5eba62`  
		Last Modified: Tue, 04 Jul 2023 04:39:40 GMT  
		Size: 196.2 MB (196197552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:cbd11f117fe42c23beeda51c054b1ccc7c594d40032aaa5c12f43b20793fcf59
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.8 MB (295837524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3bdd4f22e56b3046868680c31e879469345a5eeb73450696c18f7db32ad93dc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:32:26 GMT
ADD file:231ba6ce8d3ee30318948799a94cb007f1517ea0d14c2b84863012cac37d6c6b in / 
# Tue, 04 Jul 2023 01:32:29 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 12:48:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 12:49:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 12:50:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1e40ed2a44a8c2786b06584afad765d97e9b1c910f58ae426622ba17fbf3d4c3`  
		Last Modified: Tue, 04 Jul 2023 01:37:21 GMT  
		Size: 53.3 MB (53288197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf2b9bfea4ac32f9de9f19ff39e147a59dc0ed209ac66dbf1f57baa75c0eef4`  
		Last Modified: Tue, 04 Jul 2023 13:06:27 GMT  
		Size: 15.6 MB (15631899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b214fc39e8a77ee2b4618f8315eee93c861d035ba1cf9dc80e62081ee3aafe`  
		Last Modified: Tue, 04 Jul 2023 13:06:41 GMT  
		Size: 54.1 MB (54061732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6049a6d30b8104f609abf0afe200e7426f7a8c80bc63e5aa5ab08fd53fb7c8`  
		Last Modified: Tue, 04 Jul 2023 13:07:07 GMT  
		Size: 172.9 MB (172855696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bullseye-curl`

```console
$ docker pull buildpack-deps@sha256:8d6835a7cf657b7933e37bfbea95b89977689a0289402970e53f6159c2ef814f
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

### `buildpack-deps:bullseye-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:a04a4573f1877ebb1e4f77b2a67979fba929007fe8bd66db28c1bc21daf43f4e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.8 MB (70815627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e4f8f2737713528fa70fb13a9e1d83d4f175b195bb5f51cf6a3b71f785e9728`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:09 GMT
ADD file:b7c0be2bb90e88689b1c16da78dea0b85760b55b90ef2e5bc4a529c89e4fa25b in / 
# Tue, 04 Jul 2023 01:20:10 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:30:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:34df401c391c7595044379e04e8ad4856a5a3974cdbf5a160f0a204d761e88aa`  
		Last Modified: Tue, 04 Jul 2023 01:25:21 GMT  
		Size: 55.1 MB (55055300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fdd0e5b72ccae203ec30d533c0bcd34200af90265e0531c66356812e529af32`  
		Last Modified: Tue, 04 Jul 2023 03:52:30 GMT  
		Size: 15.8 MB (15760327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:dce5b0f9173c5aa9d4cdb22f8d553f5c7ad9b4a94d5d85c5dbef212f5bc86aae
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.9 MB (67925896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f61feaa3ac7bf64852d81afe2758a2f7c2d26b61da9e46d63e4a076b2e134095`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:48:39 GMT
ADD file:fe1b9f9f6c7d67ad23a2ee839774be4bcee33c60c7b34c48df5a08eb33cafd1b in / 
# Tue, 04 Jul 2023 00:48:40 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:24:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:702dd8b607f626c689176debe921fe96009c1ce6dbd66f4f238c7def50080e3d`  
		Last Modified: Tue, 04 Jul 2023 00:52:15 GMT  
		Size: 52.6 MB (52556778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec773064e3ff5287bd9be0bdb7b99e708aed435b4920a0f64aeaf158d9631f5e`  
		Last Modified: Tue, 04 Jul 2023 04:29:40 GMT  
		Size: 15.4 MB (15369118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:a961ee8bacf953c686c47a5ce87736a96620a4bb3e0d2d52a418e3b29114b731
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.1 MB (65086891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dffd5d1f662dbe3178c41c1f68eaa712177e4531caaefb808179447f39a3b337`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:06 GMT
ADD file:17e02296458241d9441f8da6a5dafb747d528a729106b17cec2f4c1c8cfe0ad8 in / 
# Tue, 04 Jul 2023 00:58:07 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:51:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:31edf2db9ca1650aa08e2d42e9b5bb7349413d7212110149a1a5d202ac20914b`  
		Last Modified: Tue, 04 Jul 2023 01:03:12 GMT  
		Size: 50.2 MB (50218247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e794b9a6d62ad67f31927f253d3a467d402da7b96769cef6b5503fde01f18eb9`  
		Last Modified: Tue, 04 Jul 2023 06:19:48 GMT  
		Size: 14.9 MB (14868644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:2ad82791ffc18d9af62246e621344922a9ca628ff9677f6ddc2995c3b5886118
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69450726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b6b69a80b96284b4cff1f89edcb4ea8a5430691981fe120af2033b18f8299d6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:43 GMT
ADD file:e626446584d8094b7b58d72a717380ca64d3e9ab924fc625406fe26a83fe1d8b in / 
# Tue, 04 Jul 2023 01:57:43 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:56:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:29279ac7c19f9c667f1c6b07bfba6fba20ca0d945b9fbc6edad6f75d13361fae`  
		Last Modified: Tue, 04 Jul 2023 02:01:38 GMT  
		Size: 53.7 MB (53703979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d0c3fcc5367be60f92df0774820f317a179565cd3ee9c222f5500a7be32151e`  
		Last Modified: Tue, 04 Jul 2023 06:22:01 GMT  
		Size: 15.7 MB (15746747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:e0fc072a9284c49c6bf1c3efd326932b88029bd7455798f0707b4137779bfd21
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.3 MB (72304361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7725e22264581a633b08cd831a6102bb24fd7d2b9f8e9b119c0fd4425de1705`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:38:48 GMT
ADD file:c5739407c2c257fbb85ab4b9dcd2dc07e6fe172d7309aaaaab544c8df6c42b92 in / 
# Tue, 04 Jul 2023 01:38:49 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:30:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b700c8b35944e0d5f6ab9049dbe2262492e26327a8efad518b1011428393653f`  
		Last Modified: Tue, 04 Jul 2023 01:43:49 GMT  
		Size: 56.0 MB (56040756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414994a3b1789f89f704fcfc0e721c0036089a74368f21aa6fafa639fef2c93b`  
		Last Modified: Tue, 04 Jul 2023 05:39:34 GMT  
		Size: 16.3 MB (16263605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:5284334ece9a4c74628f0ea0f15b42c69f8b7a690a808e8ad24aa684901a47ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68791009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3321735b4070a6315fe3ac262e5059feb2b4dc68eb837ed8cc3f5810373f7a3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:10:02 GMT
ADD file:f7ddd7406e3aa24165fc80933583fc2298f9792865511fe65def2f571fed2207 in / 
# Tue, 04 Jul 2023 01:10:07 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:43:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:af98e96208d7ce4cff5417a3e8a38f98d2ed3abbca318e1e6c323aa8b8c56690`  
		Last Modified: Tue, 04 Jul 2023 01:20:40 GMT  
		Size: 53.3 MB (53270472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b8f3d09abba473eec10e4fe5adebd33b18a790b9e57fdd8a5b484c925486df`  
		Last Modified: Tue, 04 Jul 2023 14:59:18 GMT  
		Size: 15.5 MB (15520537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:5b0e5a243d1ce71969d78d43a5e96c4f6827e71ce1f889b937069f96cfb19909
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75680643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:826ff0c5465ce834034c2c8aec49d5ae31c4b08991a486afbddc208db6ebb06c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:18:11 GMT
ADD file:ff86c25854c28609c2852c1615270f0acd4c4efaa38ff8ed9c23afe5132f2135 in / 
# Tue, 04 Jul 2023 01:18:15 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:33:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a792749f62225048efdf85841bea6f3999f586371852f3dbce13a6c3d89b1fa7`  
		Last Modified: Tue, 04 Jul 2023 01:25:06 GMT  
		Size: 58.9 MB (58927745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf553284aac150acedeaf1c5f33c1820a34bff4f20ef96c32510ee19f2be0e83`  
		Last Modified: Tue, 04 Jul 2023 04:38:16 GMT  
		Size: 16.8 MB (16752898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:769618a5b2bab0e90bd2133eb8ddf675f78ca808b6bb18cb99a82d773142c963
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68920096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b1d835d438212d2d9e3bc4d7ed1a6378d6b066e3545bedc9c90fcb1887fa155`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:32:26 GMT
ADD file:231ba6ce8d3ee30318948799a94cb007f1517ea0d14c2b84863012cac37d6c6b in / 
# Tue, 04 Jul 2023 01:32:29 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 12:48:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1e40ed2a44a8c2786b06584afad765d97e9b1c910f58ae426622ba17fbf3d4c3`  
		Last Modified: Tue, 04 Jul 2023 01:37:21 GMT  
		Size: 53.3 MB (53288197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf2b9bfea4ac32f9de9f19ff39e147a59dc0ed209ac66dbf1f57baa75c0eef4`  
		Last Modified: Tue, 04 Jul 2023 13:06:27 GMT  
		Size: 15.6 MB (15631899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bullseye-scm`

```console
$ docker pull buildpack-deps@sha256:01b47b8d5b8d592d95795e8d94f69b4dbfb9b99fb8f224daa19b1d665c87a9e2
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

### `buildpack-deps:bullseye-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:dd33e02b9d8fa4bc5631f3fee9dfa00166340d0172637f0a93ac2474b7198211
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.4 MB (125400673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b5c24127e49141c62bbc619c636c8a9fd47a079535d13ffc5a9048440857572`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:09 GMT
ADD file:b7c0be2bb90e88689b1c16da78dea0b85760b55b90ef2e5bc4a529c89e4fa25b in / 
# Tue, 04 Jul 2023 01:20:10 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:30:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:30:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:34df401c391c7595044379e04e8ad4856a5a3974cdbf5a160f0a204d761e88aa`  
		Last Modified: Tue, 04 Jul 2023 01:25:21 GMT  
		Size: 55.1 MB (55055300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fdd0e5b72ccae203ec30d533c0bcd34200af90265e0531c66356812e529af32`  
		Last Modified: Tue, 04 Jul 2023 03:52:30 GMT  
		Size: 15.8 MB (15760327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa786a946ae67fa18e07eaf82fefee1777449f7db1a8fea5abec1aadbe99e2ef`  
		Last Modified: Tue, 04 Jul 2023 03:52:45 GMT  
		Size: 54.6 MB (54585046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:6444b0291a1e57077fd144006676311385dc274ac4635349734805863890dc0a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.3 MB (120266460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2572b05d24e9060950a7b5ac48a29b0fb2d2cbf307f2215360bd0b0c66f68b9a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:48:39 GMT
ADD file:fe1b9f9f6c7d67ad23a2ee839774be4bcee33c60c7b34c48df5a08eb33cafd1b in / 
# Tue, 04 Jul 2023 00:48:40 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:24:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:25:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:702dd8b607f626c689176debe921fe96009c1ce6dbd66f4f238c7def50080e3d`  
		Last Modified: Tue, 04 Jul 2023 00:52:15 GMT  
		Size: 52.6 MB (52556778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec773064e3ff5287bd9be0bdb7b99e708aed435b4920a0f64aeaf158d9631f5e`  
		Last Modified: Tue, 04 Jul 2023 04:29:40 GMT  
		Size: 15.4 MB (15369118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ae2fc9256b17aac11e221f2db3d50e0543fecf87896a99ff9be68ea2335989`  
		Last Modified: Tue, 04 Jul 2023 04:29:57 GMT  
		Size: 52.3 MB (52340564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:9569373b56b793c8734d0731167d1e98d06a72c1bc73f2dbcd79eb702cc555bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115442178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e19dbbcdc9a0bbf8ee958a11f57adb53e7c4f9185065970af57187256c004e5d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:06 GMT
ADD file:17e02296458241d9441f8da6a5dafb747d528a729106b17cec2f4c1c8cfe0ad8 in / 
# Tue, 04 Jul 2023 00:58:07 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:51:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:52:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:31edf2db9ca1650aa08e2d42e9b5bb7349413d7212110149a1a5d202ac20914b`  
		Last Modified: Tue, 04 Jul 2023 01:03:12 GMT  
		Size: 50.2 MB (50218247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e794b9a6d62ad67f31927f253d3a467d402da7b96769cef6b5503fde01f18eb9`  
		Last Modified: Tue, 04 Jul 2023 06:19:48 GMT  
		Size: 14.9 MB (14868644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fdbc75406b7868979ba89f96e015c45fbcf9efe34aa3863e52c0e926531784f`  
		Last Modified: Tue, 04 Jul 2023 06:20:06 GMT  
		Size: 50.4 MB (50355287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:661446de2b43b6287b82e68aec7d4c3f2a6b2bd64e4a3e5765010400c4547a0e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.1 MB (124126801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9f39a9c3f22df829bd4eabc4d170b60fec575c4439a35d169828480baddecc7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:43 GMT
ADD file:e626446584d8094b7b58d72a717380ca64d3e9ab924fc625406fe26a83fe1d8b in / 
# Tue, 04 Jul 2023 01:57:43 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:56:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:56:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:29279ac7c19f9c667f1c6b07bfba6fba20ca0d945b9fbc6edad6f75d13361fae`  
		Last Modified: Tue, 04 Jul 2023 02:01:38 GMT  
		Size: 53.7 MB (53703979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d0c3fcc5367be60f92df0774820f317a179565cd3ee9c222f5500a7be32151e`  
		Last Modified: Tue, 04 Jul 2023 06:22:01 GMT  
		Size: 15.7 MB (15746747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5fa66dbb545c6ff93c768ac595d874b2f22053e8d2f842f4b6ccc310ebfe0c`  
		Last Modified: Tue, 04 Jul 2023 06:22:15 GMT  
		Size: 54.7 MB (54676075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:23e7ba60e97d2b78a0465a81a01d333d9a193b217b2b0f38bbea777ff2815faa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128227351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e144a202cd144d0e0b68a485990e7601e5c8114ac6ff9630063b8965660d0a69`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:38:48 GMT
ADD file:c5739407c2c257fbb85ab4b9dcd2dc07e6fe172d7309aaaaab544c8df6c42b92 in / 
# Tue, 04 Jul 2023 01:38:49 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:30:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:31:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b700c8b35944e0d5f6ab9049dbe2262492e26327a8efad518b1011428393653f`  
		Last Modified: Tue, 04 Jul 2023 01:43:49 GMT  
		Size: 56.0 MB (56040756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414994a3b1789f89f704fcfc0e721c0036089a74368f21aa6fafa639fef2c93b`  
		Last Modified: Tue, 04 Jul 2023 05:39:34 GMT  
		Size: 16.3 MB (16263605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ee301eb66e57dfaf79983158c75b77a7775e1b6216c45ce247c6fac3786a46`  
		Last Modified: Tue, 04 Jul 2023 05:39:53 GMT  
		Size: 55.9 MB (55922990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:700f08a72438adc954794c7d3a2fd5dbd704f8a9cc99287a3cfd5553fa328801
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122097647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32e876d3ef58fa796770e6bc26758ca966269bb2f0b41fd892cc7546c77b0b51`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:10:02 GMT
ADD file:f7ddd7406e3aa24165fc80933583fc2298f9792865511fe65def2f571fed2207 in / 
# Tue, 04 Jul 2023 01:10:07 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:43:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:45:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:af98e96208d7ce4cff5417a3e8a38f98d2ed3abbca318e1e6c323aa8b8c56690`  
		Last Modified: Tue, 04 Jul 2023 01:20:40 GMT  
		Size: 53.3 MB (53270472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b8f3d09abba473eec10e4fe5adebd33b18a790b9e57fdd8a5b484c925486df`  
		Last Modified: Tue, 04 Jul 2023 14:59:18 GMT  
		Size: 15.5 MB (15520537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427c4e665dab89a7a9a5cef3f1bab709cd38d4945e49ef760b95611e774a07e4`  
		Last Modified: Tue, 04 Jul 2023 15:00:02 GMT  
		Size: 53.3 MB (53306638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:92a3d9951e784acd6f21e0cdf396b60a964d1078dc1f61719d645f1e7eec914f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.5 MB (134545338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05f293bd1201dd82f48e60638e86ac0f42f4491c53208a613704b933e2417990`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:18:11 GMT
ADD file:ff86c25854c28609c2852c1615270f0acd4c4efaa38ff8ed9c23afe5132f2135 in / 
# Tue, 04 Jul 2023 01:18:15 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:33:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:33:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a792749f62225048efdf85841bea6f3999f586371852f3dbce13a6c3d89b1fa7`  
		Last Modified: Tue, 04 Jul 2023 01:25:06 GMT  
		Size: 58.9 MB (58927745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf553284aac150acedeaf1c5f33c1820a34bff4f20ef96c32510ee19f2be0e83`  
		Last Modified: Tue, 04 Jul 2023 04:38:16 GMT  
		Size: 16.8 MB (16752898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b8f1977f7b061bf5ae7311bb1750877d9ba871f041ba604c8e1e9d1e1143e0`  
		Last Modified: Tue, 04 Jul 2023 04:38:44 GMT  
		Size: 58.9 MB (58864695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:28964966888229ec79ac01c2034a5e759e7b04ea102ede17272baf6b71eeeb2d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (122981828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f6ffe961aa23647a1a72f2af8135528a958505fe0453d5bf132aebddb6636c1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:32:26 GMT
ADD file:231ba6ce8d3ee30318948799a94cb007f1517ea0d14c2b84863012cac37d6c6b in / 
# Tue, 04 Jul 2023 01:32:29 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 12:48:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 12:49:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1e40ed2a44a8c2786b06584afad765d97e9b1c910f58ae426622ba17fbf3d4c3`  
		Last Modified: Tue, 04 Jul 2023 01:37:21 GMT  
		Size: 53.3 MB (53288197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf2b9bfea4ac32f9de9f19ff39e147a59dc0ed209ac66dbf1f57baa75c0eef4`  
		Last Modified: Tue, 04 Jul 2023 13:06:27 GMT  
		Size: 15.6 MB (15631899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b214fc39e8a77ee2b4618f8315eee93c861d035ba1cf9dc80e62081ee3aafe`  
		Last Modified: Tue, 04 Jul 2023 13:06:41 GMT  
		Size: 54.1 MB (54061732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:buster`

```console
$ docker pull buildpack-deps@sha256:93d76989e9b0ebdfe9b96e96095ea6f87c710ecd01b66ce85418232c7af430c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:buster` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:fc6853c85c895526dc95b4774269365f5b600c184d2fd944b3181c58f4939e16
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.8 MB (311781265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7eb882719b28e6bbddb691ea7cbc3679551f1b68715fe48e477afa5d82c87afe`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:34 GMT
ADD file:2fa5242038736e48eaca794d061079c1cbd32fcc4336250001523c41b3177276 in / 
# Tue, 04 Jul 2023 01:20:35 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:32:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:32:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:33:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8eb6dba554cffc072c7a6c696c8a23fc311e543399d84ab3ebc55c07ab54414f`  
		Last Modified: Tue, 04 Jul 2023 01:26:01 GMT  
		Size: 50.4 MB (50448743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e4f798b8796023ecee944e089e79871ca261eedc4a2ee6a38b08418d9160f4`  
		Last Modified: Tue, 04 Jul 2023 03:53:27 GMT  
		Size: 17.6 MB (17579065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90cef27337073d2443e1c3dd4305cf98d70eadb31c10c267225d9639f1cd6de4`  
		Last Modified: Tue, 04 Jul 2023 03:53:43 GMT  
		Size: 51.9 MB (51870872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f89e257e0550870d02769e068a247cf3612acbb737425f707be9ea0d763772`  
		Last Modified: Tue, 04 Jul 2023 03:54:13 GMT  
		Size: 191.9 MB (191882585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:60f28694428765623be4e2f4c523c350281fa20a0eeabf003c9287ff63a16c27
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.6 MB (277592160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e810e54890f1fef5a1546e57ca582e7f104597aae4dd54a08edd435f2ed8c80`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:31 GMT
ADD file:e1c7c10335e2ac86eba02c2785d0ff530cba87131e91c42924072b4010418f93 in / 
# Tue, 04 Jul 2023 00:58:32 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:54:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:54:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:56:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b19cf971d5ed51e0bba0bd71ccd7b797ad4873a62fee0f49588f6ef19a58e659`  
		Last Modified: Tue, 04 Jul 2023 01:03:55 GMT  
		Size: 45.9 MB (45916488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de49cbcb6a4fd553472f2cf39947eef7d00374517274e95f1a822bfb3c8e2cb`  
		Last Modified: Tue, 04 Jul 2023 06:20:51 GMT  
		Size: 16.2 MB (16211416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:551952269cb797c2c924c3af99a03099c86099cd8186bdda487b965d4f08fff3`  
		Last Modified: Tue, 04 Jul 2023 06:21:10 GMT  
		Size: 47.4 MB (47369644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e84c841d1296aa856601262d7c4425787f09dfce1122d08b3b7ecf5b44a8a54e`  
		Last Modified: Tue, 04 Jul 2023 06:21:39 GMT  
		Size: 168.1 MB (168094612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:50b0cc42de9ec56d6d75b59f66665fbc6b800e29417804bdf18a1a60516a8362
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.4 MB (302372380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c378a277c6ab107528bb171956861a01656482088765346902a30334b4b322af`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:59 GMT
ADD file:a61276f534601d7b193af24e35c16b73a2913511d2b1ad997c9a8cb907685257 in / 
# Tue, 04 Jul 2023 01:58:00 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:58:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:58:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:00:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5e2555ae6edde2e7933c533234cb224b6d7ef3a3c90041851e31fe29ab7197c9`  
		Last Modified: Tue, 04 Jul 2023 02:02:18 GMT  
		Size: 49.2 MB (49238644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503bef164a5c225a74d09ad3b129d3bff71bea2ad1fb291b63c6d342493b62ba`  
		Last Modified: Tue, 04 Jul 2023 06:22:50 GMT  
		Size: 17.5 MB (17450024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3816d11f9d5d9a3bb643dd5c7291e610012ec9eef9c769ce5f6107abdf1eb6d`  
		Last Modified: Tue, 04 Jul 2023 06:23:05 GMT  
		Size: 52.2 MB (52217244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:456c8535b3af918c9b8d87c98c4d7bc631d833d1ebb4d816aefbf356372983c6`  
		Last Modified: Tue, 04 Jul 2023 06:23:29 GMT  
		Size: 183.5 MB (183466468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; 386

```console
$ docker pull buildpack-deps@sha256:0724af2107e33683fda67b85f730eb15e5087c5dcbfd73f7af46fa0c214deacc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.2 MB (321213990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9216ef434e3e7d93b84a05352e7de2c89cbadb8aa2ba1ff22f364785c53e5d1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:39:11 GMT
ADD file:6ecab94f7cb2bc0740a669cfef73f0837a2ecf6475dfb0fc072cbd1a7f60ec41 in / 
# Tue, 04 Jul 2023 01:39:11 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:33:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:34:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:36:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b3c3fd2dd1697ce9fed8a2be0142b2d1294d424c56d0ce6d44bb8055d77e35d`  
		Last Modified: Tue, 04 Jul 2023 01:44:33 GMT  
		Size: 51.2 MB (51206276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a0e83aa5cadecbd9663b4464fa33665e930f60918a3178f75983604fc64d38`  
		Last Modified: Tue, 04 Jul 2023 05:40:47 GMT  
		Size: 18.1 MB (18095483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88eede3a0f204f9d3d5eae24a7e5f5ddd9f533ad476bf4e77ee81a22bdb07f9a`  
		Last Modified: Tue, 04 Jul 2023 05:41:07 GMT  
		Size: 53.5 MB (53485728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d9ed1e05da0b79a86d6ca58ac78d81fd2bc66fa7ea1b33566e0aa62fc445f9`  
		Last Modified: Tue, 04 Jul 2023 05:41:49 GMT  
		Size: 198.4 MB (198426503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:buster-curl`

```console
$ docker pull buildpack-deps@sha256:9e90f92d4d4c4cc756adc20a63ed7cd3bcd4e2c58723c10a449484b8ff6aceea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:buster-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:b9a6fa925c3754fad97e1e096b2107d8809a8c2786947ea28ebca51ee9791bc7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.0 MB (68027808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fba93f010c9f896ebc93161f6655c1b59d288182d9e9e6d2e1bbecc0f8c94e4f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:34 GMT
ADD file:2fa5242038736e48eaca794d061079c1cbd32fcc4336250001523c41b3177276 in / 
# Tue, 04 Jul 2023 01:20:35 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:32:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8eb6dba554cffc072c7a6c696c8a23fc311e543399d84ab3ebc55c07ab54414f`  
		Last Modified: Tue, 04 Jul 2023 01:26:01 GMT  
		Size: 50.4 MB (50448743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e4f798b8796023ecee944e089e79871ca261eedc4a2ee6a38b08418d9160f4`  
		Last Modified: Tue, 04 Jul 2023 03:53:27 GMT  
		Size: 17.6 MB (17579065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:afa7a1bada87fb5441651d43e1b4349bd9cc466f0622739367455cd376a740b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.1 MB (62127904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68f107e1a900a7b124105c82ffff25b2a060dee6cff73cdec89337f4a23449b9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:31 GMT
ADD file:e1c7c10335e2ac86eba02c2785d0ff530cba87131e91c42924072b4010418f93 in / 
# Tue, 04 Jul 2023 00:58:32 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:54:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b19cf971d5ed51e0bba0bd71ccd7b797ad4873a62fee0f49588f6ef19a58e659`  
		Last Modified: Tue, 04 Jul 2023 01:03:55 GMT  
		Size: 45.9 MB (45916488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de49cbcb6a4fd553472f2cf39947eef7d00374517274e95f1a822bfb3c8e2cb`  
		Last Modified: Tue, 04 Jul 2023 06:20:51 GMT  
		Size: 16.2 MB (16211416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:80e630bea99e712a913b713c63ff3adf1eacb86af6629feb11b0e0227ca80219
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66688668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdad1a1cc278d9d35c38b92f4d110b39952f68f5271c652b7ad103623ae9c8de`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:59 GMT
ADD file:a61276f534601d7b193af24e35c16b73a2913511d2b1ad997c9a8cb907685257 in / 
# Tue, 04 Jul 2023 01:58:00 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:58:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5e2555ae6edde2e7933c533234cb224b6d7ef3a3c90041851e31fe29ab7197c9`  
		Last Modified: Tue, 04 Jul 2023 02:02:18 GMT  
		Size: 49.2 MB (49238644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503bef164a5c225a74d09ad3b129d3bff71bea2ad1fb291b63c6d342493b62ba`  
		Last Modified: Tue, 04 Jul 2023 06:22:50 GMT  
		Size: 17.5 MB (17450024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:31a0d9c686cbc2328cd57c3363515049f391593d8dc552dea36b5acd6aadd135
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.3 MB (69301759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:553a8774245bf544e4a5813eb3fc8b73b523c6ce15b6d5278ded782d365eab85`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:39:11 GMT
ADD file:6ecab94f7cb2bc0740a669cfef73f0837a2ecf6475dfb0fc072cbd1a7f60ec41 in / 
# Tue, 04 Jul 2023 01:39:11 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:33:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b3c3fd2dd1697ce9fed8a2be0142b2d1294d424c56d0ce6d44bb8055d77e35d`  
		Last Modified: Tue, 04 Jul 2023 01:44:33 GMT  
		Size: 51.2 MB (51206276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a0e83aa5cadecbd9663b4464fa33665e930f60918a3178f75983604fc64d38`  
		Last Modified: Tue, 04 Jul 2023 05:40:47 GMT  
		Size: 18.1 MB (18095483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:buster-scm`

```console
$ docker pull buildpack-deps@sha256:190191e3a02c364d2538051d10cf6b972bf5f388de64ee88a0cd912f98d7b294
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:buster-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:d3872f4bbda84746d3e023839278b5380cc83b5f2e57e27812e359cdcfec8cec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.9 MB (119898680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e42250bcc32f41abbf71048b5d3f02f09de55ed4c1502afbaef04096b190463`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:34 GMT
ADD file:2fa5242038736e48eaca794d061079c1cbd32fcc4336250001523c41b3177276 in / 
# Tue, 04 Jul 2023 01:20:35 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:32:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:32:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8eb6dba554cffc072c7a6c696c8a23fc311e543399d84ab3ebc55c07ab54414f`  
		Last Modified: Tue, 04 Jul 2023 01:26:01 GMT  
		Size: 50.4 MB (50448743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e4f798b8796023ecee944e089e79871ca261eedc4a2ee6a38b08418d9160f4`  
		Last Modified: Tue, 04 Jul 2023 03:53:27 GMT  
		Size: 17.6 MB (17579065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90cef27337073d2443e1c3dd4305cf98d70eadb31c10c267225d9639f1cd6de4`  
		Last Modified: Tue, 04 Jul 2023 03:53:43 GMT  
		Size: 51.9 MB (51870872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1b4d9a7f073580e03ec7c8b3e0243dd260f0d9a360b5d6428cf51566261433df
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.5 MB (109497548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce83dc96a23dafaf7a58ec0f31d70b644e4715d465e1128b15d0bd604e283def`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:31 GMT
ADD file:e1c7c10335e2ac86eba02c2785d0ff530cba87131e91c42924072b4010418f93 in / 
# Tue, 04 Jul 2023 00:58:32 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:54:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:54:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b19cf971d5ed51e0bba0bd71ccd7b797ad4873a62fee0f49588f6ef19a58e659`  
		Last Modified: Tue, 04 Jul 2023 01:03:55 GMT  
		Size: 45.9 MB (45916488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de49cbcb6a4fd553472f2cf39947eef7d00374517274e95f1a822bfb3c8e2cb`  
		Last Modified: Tue, 04 Jul 2023 06:20:51 GMT  
		Size: 16.2 MB (16211416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:551952269cb797c2c924c3af99a03099c86099cd8186bdda487b965d4f08fff3`  
		Last Modified: Tue, 04 Jul 2023 06:21:10 GMT  
		Size: 47.4 MB (47369644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:042c8cbba1e5ec8945d2a178da4a4ab2a7aa52c981f75e0ff0949d2fc8422b11
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.9 MB (118905912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6568bf4370a5bad76d3890ece5e6279395b2d0ae33a68af33183174c29a61ed9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:59 GMT
ADD file:a61276f534601d7b193af24e35c16b73a2913511d2b1ad997c9a8cb907685257 in / 
# Tue, 04 Jul 2023 01:58:00 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:58:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:58:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5e2555ae6edde2e7933c533234cb224b6d7ef3a3c90041851e31fe29ab7197c9`  
		Last Modified: Tue, 04 Jul 2023 02:02:18 GMT  
		Size: 49.2 MB (49238644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503bef164a5c225a74d09ad3b129d3bff71bea2ad1fb291b63c6d342493b62ba`  
		Last Modified: Tue, 04 Jul 2023 06:22:50 GMT  
		Size: 17.5 MB (17450024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3816d11f9d5d9a3bb643dd5c7291e610012ec9eef9c769ce5f6107abdf1eb6d`  
		Last Modified: Tue, 04 Jul 2023 06:23:05 GMT  
		Size: 52.2 MB (52217244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:c8e540d022779ddb0a2e6fdb3d322469c3d320d485cf84cefb7f9dff9c5024f5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.8 MB (122787487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a44252762afe1bc6205da39e4217bfd4fda4800ee9de78325ef92703f7312a27`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:39:11 GMT
ADD file:6ecab94f7cb2bc0740a669cfef73f0837a2ecf6475dfb0fc072cbd1a7f60ec41 in / 
# Tue, 04 Jul 2023 01:39:11 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:33:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:34:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b3c3fd2dd1697ce9fed8a2be0142b2d1294d424c56d0ce6d44bb8055d77e35d`  
		Last Modified: Tue, 04 Jul 2023 01:44:33 GMT  
		Size: 51.2 MB (51206276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a0e83aa5cadecbd9663b4464fa33665e930f60918a3178f75983604fc64d38`  
		Last Modified: Tue, 04 Jul 2023 05:40:47 GMT  
		Size: 18.1 MB (18095483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88eede3a0f204f9d3d5eae24a7e5f5ddd9f533ad476bf4e77ee81a22bdb07f9a`  
		Last Modified: Tue, 04 Jul 2023 05:41:07 GMT  
		Size: 53.5 MB (53485728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:curl`

```console
$ docker pull buildpack-deps@sha256:5df62ac377f1dca70c63bb04aeacf175f11265542a35a451d592255cc0e38972
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

### `buildpack-deps:curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:4ce7e846f60727efea42b5abdfd8673e13a94e288c6a5d7c37da1973ce7c5d78
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73582025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c399a665f317215e5dd18dcf72a1723bc891edc5df1e57bf176d1c65f757cd0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:19:44 GMT
ADD file:5d17ca085473e890bd6eca4abf6d324c3181f80692523b83ef25d1c42576b99f in / 
# Tue, 04 Jul 2023 01:19:44 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:27:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d52e4f012db158bb7c0fe215b98af1facaddcbaee530efd69b1bae07d597b711`  
		Last Modified: Tue, 04 Jul 2023 01:24:39 GMT  
		Size: 49.6 MB (49551432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd206bea61ff3e3b54be1c20b58d8475ddd6f89df176146ddb7a2fd2c747ea2`  
		Last Modified: Tue, 04 Jul 2023 03:51:23 GMT  
		Size: 24.0 MB (24030593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:cd79b4dbc7daadcec5980ed2d535ce9340c36adea17ccf7dbb0c0d2712ca57e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.1 MB (70111719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dea85fcb87a6435ababbbc09b75d697c82c737049086f3d59690dca803e1758d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:48:22 GMT
ADD file:09001854dc5081f907ac2a66d301e4b3d6b4bf2c2483aad5395a535bf068698d in / 
# Tue, 04 Jul 2023 00:48:22 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:21:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7e0a1f476b42bcc214197ec9c5ef753ddf2ab36a314416a6ac96cd921ff0d41d`  
		Last Modified: Tue, 04 Jul 2023 00:51:29 GMT  
		Size: 47.4 MB (47402786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68311cc5ff511aa59283fdd7f1e25bc33dfc3ad9ae87e5c94447f36c3f7c4817`  
		Last Modified: Tue, 04 Jul 2023 04:28:32 GMT  
		Size: 22.7 MB (22708933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:ee52b93b57b097abb318a077905af9d187e98a1feb6c49f47ad7368f254dac9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67172647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7745cabe6a186fe38c73aa2d5384961dc430b541f6f0ccee40bb24c7865441c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:57:42 GMT
ADD file:279ef7213d41f1f7ae76bd76293a5107fd1f8caf557f837cab9c834d2841e031 in / 
# Tue, 04 Jul 2023 00:57:43 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:49:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b9bdcf1a9a6361f231594c76a75bfb4c2fef5f9745b9713bbd50efaf37ca11b8`  
		Last Modified: Tue, 04 Jul 2023 01:02:26 GMT  
		Size: 45.2 MB (45236201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8ee33ea63b2391e912423c14b2f1e789137ffb03659568cb361a2fa2b4efbd`  
		Last Modified: Tue, 04 Jul 2023 06:18:41 GMT  
		Size: 21.9 MB (21936446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c6b1b12d88f18474b52830b7189f2d54b534002ee9b00dbe7a5947684dbbef4d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.1 MB (73142327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ccf74d87c178f322cc3cc0e5b79bb62adfcb518a1c78943c8a7d7241427f748`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:26 GMT
ADD file:ab1761d899751c4d24e15179fc9e7e7ac3fb83798ee37ca13d6a6ac44fbeded3 in / 
# Tue, 04 Jul 2023 01:57:27 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:54:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:42cbebf8bc116ba1aed7897e2d0566bf49da9d5c70be71b6a7cb07805d2f5b7a`  
		Last Modified: Tue, 04 Jul 2023 02:00:57 GMT  
		Size: 49.6 MB (49572781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0518ec57568a70561f7c04650f9554c88dada973f54d88e36f65b0796d35de`  
		Last Modified: Tue, 04 Jul 2023 06:21:03 GMT  
		Size: 23.6 MB (23569546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:abb0cf0f3dc36c7e284598893d32388fe2b09b68e02ef75869a6ddce988d6624
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75432135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce569bff52f1ef304acf004cee953e9829211468502cb021457f297c7f8d098d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:38:25 GMT
ADD file:e0a25fe261e09183ec383698ab2c800f93c5b0805564d7104ad5119db52cccb7 in / 
# Tue, 04 Jul 2023 01:38:25 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:28:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:381263dab43af8bfb8e85c7a9a32f35492cbdcc3a046b35f947cf3bf3a55f4c1`  
		Last Modified: Tue, 04 Jul 2023 01:43:02 GMT  
		Size: 50.6 MB (50562388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af522778d6fcd5f4b85dafb1f21b89441dedee6ce875890b15ad8c454bbb9fe6`  
		Last Modified: Tue, 04 Jul 2023 05:38:10 GMT  
		Size: 24.9 MB (24869747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:daeb0fffa382ebd3757c35f7edef327defb7d926134b88529b5ac12bfe9bda74
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73153823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe85240ea372bde5df08e1b08faeb8632ed7dedae4aba518ab2d7bc1488ca70e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:08:42 GMT
ADD file:c567fc0f97f36ea531c05e159cd6ac2a8747f14ea5b6ccae39bab9d305da180d in / 
# Tue, 04 Jul 2023 01:08:47 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:34:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76240e493592cbc7ca56583a6e8e03ab12a967b65bbeb1df7828a5099fa271d9`  
		Last Modified: Tue, 04 Jul 2023 01:19:16 GMT  
		Size: 49.5 MB (49542143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85086244c52affe40f860feee6e34c03fd0f782e853b00950f1a9b8b6704d24f`  
		Last Modified: Tue, 04 Jul 2023 14:56:03 GMT  
		Size: 23.6 MB (23611680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:dd742426422d9d9c53b1f294d91895bd56b7748b0a559826babb53cec399ddef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.2 MB (79218037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4572b0656e7dfc6731b3f7dd64ee5baeb3421d7762079b77c60f1226bfa152f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:17:23 GMT
ADD file:5aaa642008df5a97014e76042a767f06bbfda91db1d5f336a1b3f98e9b11c7a1 in / 
# Tue, 04 Jul 2023 01:17:26 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:26:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e039cf6634cf83a31e97e2a56b4db40a8c38a62d6857c77e687d5edb3eb0dfde`  
		Last Modified: Tue, 04 Jul 2023 01:23:59 GMT  
		Size: 53.5 MB (53536740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54fff62f5ff539ace95f1581096d57b95ca024b9d5cc7c85bb4a2bf159ad845f`  
		Last Modified: Tue, 04 Jul 2023 04:36:20 GMT  
		Size: 25.7 MB (25681297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:d5f47922100fab7fa779f085640d993e6625e6f15956c228a3b1475b38baf460
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.0 MB (71950502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ebcb0cef8f138e8e985dd005eeee2dd6d64c40eef9668d4b648caec9ec37c6a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:31:54 GMT
ADD file:0ad7ffbe777e5367ad6dcbb4a182e1d578739aa7a4853f82f21bd71d824de7ae in / 
# Tue, 04 Jul 2023 01:31:56 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 12:47:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce9d001c0d31ec9b8072b1a9bd01771a10ea8ddfefa381cf9ce7e2d63538aaeb`  
		Last Modified: Tue, 04 Jul 2023 01:36:50 GMT  
		Size: 47.9 MB (47921709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024bda56b20d3018344098f67965337568b532ea03f09d87858a2bb5eae82bf7`  
		Last Modified: Tue, 04 Jul 2023 13:05:34 GMT  
		Size: 24.0 MB (24028793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:focal`

```console
$ docker pull buildpack-deps@sha256:a185db68283db441b7051eb46a43aeb48529a876fa53a19aea0fc2eaf8adb22c
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
$ docker pull buildpack-deps@sha256:c7c9e01f525b7b71c896947f93c1886f61cf600947fe9c6f52bb89306e9d837c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.7 MB (245713038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4fdc424c21a7faa2bb99b875d2ce47d52685d1f0692f07b0f4ae504cdab83c3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:59:08 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:59:08 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:59:10 GMT
ADD file:12f97b7b044d0d1166dd59408c67f5610a764127aa8a01bc57db23bee48911af in / 
# Wed, 28 Jun 2023 09:59:10 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 03:35:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:36:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:39:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0fb668748fc8bb961f4580895692ae741be788857ac2e8220adc2265ffb38e10`  
		Last Modified: Wed, 28 Jun 2023 18:43:28 GMT  
		Size: 28.6 MB (28580012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de25fa69197a0fe88312b7c08a3a8c96d4062222b035243751e6b307e1087e46`  
		Last Modified: Tue, 04 Jul 2023 03:54:52 GMT  
		Size: 11.1 MB (11129679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02e98539424ab3fee447b177cb642cceab5a0f5bcc7ac4658a3199d8a2efe22`  
		Last Modified: Tue, 04 Jul 2023 03:55:11 GMT  
		Size: 60.9 MB (60915116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10814cb888f2d0dc3b2fd0b1086cf83dffd5b89704534a791348878994befe3a`  
		Last Modified: Tue, 04 Jul 2023 03:55:39 GMT  
		Size: 145.1 MB (145088231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:93218030091d490ac3709f8ca1b26d36a56614c26e83306fce917bc01b3d5b9d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.9 MB (211948612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6217c3d30436343fdbea1735e914455a8eef4374a3879019fc7a6153849ebce`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:58:19 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:58:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:58:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:58:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:58:22 GMT
ADD file:8bedca16bf416520f5df29175a99b07585281465c459544b9f9679016f59762a in / 
# Wed, 28 Jun 2023 09:58:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 05:58:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:59:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:02:59 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:06e53fabee8df31622850c604f9242a52a466ec4eb75320019bdfdc8ec311692`  
		Last Modified: Tue, 04 Jul 2023 06:22:20 GMT  
		Size: 24.6 MB (24588135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7655bda15200da93eaa77218c915efbf215e822d3a7ef693f5fbc78a94b8e906`  
		Last Modified: Tue, 04 Jul 2023 06:22:17 GMT  
		Size: 9.6 MB (9599087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bf5309ca27fafde797ae93665faceb2bf2d10325336e4a2004fad3ea3a3928`  
		Last Modified: Tue, 04 Jul 2023 06:22:38 GMT  
		Size: 55.8 MB (55826315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60345e5479f7c8f72ad47b6401099a23948d09f83264bf4fbd7a1c5b8a8b120b`  
		Last Modified: Tue, 04 Jul 2023 06:23:07 GMT  
		Size: 121.9 MB (121935075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d643b544b4d5c4c222904b1995d0d52f516df830f01583a13eecaf761e02aadd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.0 MB (235966654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cf414eb726738eb2bed47de53bc51399a1a8044efc47ea93ff22a1feac978bf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:54:46 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:54:46 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:54:48 GMT
ADD file:a6db9f7789e57b7119f68e4e4ec9ec5aab8c3c8bd53fd932f3c59c54b1c20a26 in / 
# Wed, 28 Jun 2023 09:54:49 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 06:01:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:02:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:05:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1e77eb131c5c9032ce8e6e512f601714ce7ba48e296f5b7a5191703bdcbc904d`  
		Last Modified: Tue, 04 Jul 2023 04:05:23 GMT  
		Size: 27.2 MB (27198330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ae43f445a875bd258928e514043770667dbc9ab823c2a244e3c8d2fb4520ad`  
		Last Modified: Tue, 04 Jul 2023 06:24:04 GMT  
		Size: 11.0 MB (10982532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf4e8446ca8d143e3e482c4d70cf26e4702ff9b4e40c36c27fc3dd2a3c27c556`  
		Last Modified: Tue, 04 Jul 2023 06:24:19 GMT  
		Size: 61.0 MB (61006780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1bc3cd52da7ce05900d047fd4cda3ce90636414f72af90486f6e969e2d2f6b0`  
		Last Modified: Tue, 04 Jul 2023 06:24:41 GMT  
		Size: 136.8 MB (136779012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:cc828381ce76a725b9d89f134a8d0cfa74d055174d4575477f34a423c98ea367
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.5 MB (269491158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbd8a25659464d102bb1ecbe6cc4007a51d569800d490f7ee98b20f4430850ac`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 10:04:43 GMT
ARG RELEASE
# Wed, 28 Jun 2023 10:04:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 10:04:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 10:04:43 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 10:04:46 GMT
ADD file:df651ead0b69eb261098e765354dbdf5ffca51275c037d8881fedcaa1c91c36d in / 
# Wed, 28 Jun 2023 10:04:46 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 03:40:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:42:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:52:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4e95615eadb7a0d90a47ca15a5c0693371494902f54d8d78a50d53e89e7a20de`  
		Last Modified: Tue, 04 Jul 2023 04:40:49 GMT  
		Size: 33.3 MB (33308759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276026532e2897addfb94053c99fabaff128631b0106992fca31995a4e07ee2f`  
		Last Modified: Tue, 04 Jul 2023 04:40:45 GMT  
		Size: 12.9 MB (12937997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f779e3d18cc00d1bfffc494a86c621971575cc7b49852f3e69213662057902`  
		Last Modified: Tue, 04 Jul 2023 04:41:19 GMT  
		Size: 69.6 MB (69626921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e13418b66e9f4c1f9d947e9d444eb0fb640256ac2ee6d0a41723d673cf1b16`  
		Last Modified: Tue, 04 Jul 2023 04:42:10 GMT  
		Size: 153.6 MB (153617481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:580cefb616a99fcf46bb964c69f12ed5649224e80a0008d94866de16639a35ea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.4 MB (226422472 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cf7de8cb660b68cf94254f5b979338baf341742f41e919e60ccae14144fdd64`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 10:01:13 GMT
ARG RELEASE
# Wed, 28 Jun 2023 10:01:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 10:01:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 10:01:14 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 10:01:15 GMT
ADD file:777fd71e798b91bf768b21e1ca4403f388db9936ef55ef68b4b019cb167fa707 in / 
# Wed, 28 Jun 2023 10:01:15 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 12:51:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 12:52:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 12:54:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f5ebe8481b30a6d3b710b0efdec29843cca805811e3be1a4e375761725c40e5a`  
		Last Modified: Tue, 04 Jul 2023 13:07:41 GMT  
		Size: 27.0 MB (27013645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e76df5c29baf17b24cc9ec09debb6341e7d2b72276cb8ded9c6f9b91e2c3c457`  
		Last Modified: Tue, 04 Jul 2023 13:07:39 GMT  
		Size: 10.7 MB (10688202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d32cf23175b375841e6e543d986dd4143c7fffdb28041799bded0d024fec5d7`  
		Last Modified: Tue, 04 Jul 2023 13:07:56 GMT  
		Size: 60.3 MB (60306044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56679d2cc4435a4de5a03dc496c0e2a79d465112d7a7c30997f027f96e1154a`  
		Last Modified: Tue, 04 Jul 2023 13:08:19 GMT  
		Size: 128.4 MB (128414581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:focal-curl`

```console
$ docker pull buildpack-deps@sha256:7ac75c83428eead00cdc790f512da48b07fc284c70f6dc20c1e8de6c094c5076
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:focal-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:29349b0eaca1f8811a3d7d38a9846ab3314f69a804183b6e90a44aa3770e6fb2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.7 MB (39709691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb7221a59874eaac8926a513c75cfa4b39d8bf1d7d8e7c901e1896ef56bf7fbb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:59:08 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:59:08 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:59:10 GMT
ADD file:12f97b7b044d0d1166dd59408c67f5610a764127aa8a01bc57db23bee48911af in / 
# Wed, 28 Jun 2023 09:59:10 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 03:35:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0fb668748fc8bb961f4580895692ae741be788857ac2e8220adc2265ffb38e10`  
		Last Modified: Wed, 28 Jun 2023 18:43:28 GMT  
		Size: 28.6 MB (28580012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de25fa69197a0fe88312b7c08a3a8c96d4062222b035243751e6b307e1087e46`  
		Last Modified: Tue, 04 Jul 2023 03:54:52 GMT  
		Size: 11.1 MB (11129679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:0303a169ab81f1dd2dcd58af96b0874f72e751171dcd991e2d77d1e7e92b34bb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.2 MB (34187222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f37c50d81dcfa785320e75ef3b32c0ee9dae56393ee924c9005dd45710e8ddba`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:58:19 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:58:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:58:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:58:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:58:22 GMT
ADD file:8bedca16bf416520f5df29175a99b07585281465c459544b9f9679016f59762a in / 
# Wed, 28 Jun 2023 09:58:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 05:58:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:06e53fabee8df31622850c604f9242a52a466ec4eb75320019bdfdc8ec311692`  
		Last Modified: Tue, 04 Jul 2023 06:22:20 GMT  
		Size: 24.6 MB (24588135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7655bda15200da93eaa77218c915efbf215e822d3a7ef693f5fbc78a94b8e906`  
		Last Modified: Tue, 04 Jul 2023 06:22:17 GMT  
		Size: 9.6 MB (9599087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:2c0578c721a498af48cd9ef0884245d87b60ef60dd0a1f08d13b8ad59dfc24c2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38180862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05adb6402d4b50ffe9531fcbf9bc27b370c6736ee6bff914e4c2831eea2588c9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:54:46 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:54:46 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:54:48 GMT
ADD file:a6db9f7789e57b7119f68e4e4ec9ec5aab8c3c8bd53fd932f3c59c54b1c20a26 in / 
# Wed, 28 Jun 2023 09:54:49 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 06:01:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1e77eb131c5c9032ce8e6e512f601714ce7ba48e296f5b7a5191703bdcbc904d`  
		Last Modified: Tue, 04 Jul 2023 04:05:23 GMT  
		Size: 27.2 MB (27198330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ae43f445a875bd258928e514043770667dbc9ab823c2a244e3c8d2fb4520ad`  
		Last Modified: Tue, 04 Jul 2023 06:24:04 GMT  
		Size: 11.0 MB (10982532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:ebda49b806b5084f69baf79430dc3b5d2b8bb4631404e64e4c0f786e269e465c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.2 MB (46246756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fdf46f3154cdfb9e896f4ee40532dbbe0b2abd9fb58f55aff17d4b11dd6aebf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 10:04:43 GMT
ARG RELEASE
# Wed, 28 Jun 2023 10:04:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 10:04:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 10:04:43 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 10:04:46 GMT
ADD file:df651ead0b69eb261098e765354dbdf5ffca51275c037d8881fedcaa1c91c36d in / 
# Wed, 28 Jun 2023 10:04:46 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 03:40:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4e95615eadb7a0d90a47ca15a5c0693371494902f54d8d78a50d53e89e7a20de`  
		Last Modified: Tue, 04 Jul 2023 04:40:49 GMT  
		Size: 33.3 MB (33308759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276026532e2897addfb94053c99fabaff128631b0106992fca31995a4e07ee2f`  
		Last Modified: Tue, 04 Jul 2023 04:40:45 GMT  
		Size: 12.9 MB (12937997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:a1a74cd349bbde56ebcc8338244ffbe81f589de4017b9e4804563da5551adc4f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37701847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8de47ab95f94694c1633d536a99595b02886af13b8c51cc75b5f5afcc9b17e98`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 10:01:13 GMT
ARG RELEASE
# Wed, 28 Jun 2023 10:01:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 10:01:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 10:01:14 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 10:01:15 GMT
ADD file:777fd71e798b91bf768b21e1ca4403f388db9936ef55ef68b4b019cb167fa707 in / 
# Wed, 28 Jun 2023 10:01:15 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 12:51:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f5ebe8481b30a6d3b710b0efdec29843cca805811e3be1a4e375761725c40e5a`  
		Last Modified: Tue, 04 Jul 2023 13:07:41 GMT  
		Size: 27.0 MB (27013645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e76df5c29baf17b24cc9ec09debb6341e7d2b72276cb8ded9c6f9b91e2c3c457`  
		Last Modified: Tue, 04 Jul 2023 13:07:39 GMT  
		Size: 10.7 MB (10688202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:focal-scm`

```console
$ docker pull buildpack-deps@sha256:cf75c25ab50018af643899159854d52e05aeeb25dc53c2728a16b5ea7ea40a4d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:focal-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:273eb870a63a22e195a285cb24188c8ed3a97fb62309d8a4f27b6027c040928f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.6 MB (100624807 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87826ce481cf6aeaf241e717c398c87ff39180797900c7007e6808e03fab8921`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:59:08 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:59:08 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:59:08 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:59:10 GMT
ADD file:12f97b7b044d0d1166dd59408c67f5610a764127aa8a01bc57db23bee48911af in / 
# Wed, 28 Jun 2023 09:59:10 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 03:35:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:36:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0fb668748fc8bb961f4580895692ae741be788857ac2e8220adc2265ffb38e10`  
		Last Modified: Wed, 28 Jun 2023 18:43:28 GMT  
		Size: 28.6 MB (28580012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de25fa69197a0fe88312b7c08a3a8c96d4062222b035243751e6b307e1087e46`  
		Last Modified: Tue, 04 Jul 2023 03:54:52 GMT  
		Size: 11.1 MB (11129679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02e98539424ab3fee447b177cb642cceab5a0f5bcc7ac4658a3199d8a2efe22`  
		Last Modified: Tue, 04 Jul 2023 03:55:11 GMT  
		Size: 60.9 MB (60915116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:6375f2580b96022d4e2a789ebdb9260867c8f5ed0ecb27617d0f77093c37460d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.0 MB (90013537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d00851b856224282b6ead89b40dcd53b77538aec6d069855dea50a5297ceda2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:58:19 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:58:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:58:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:58:20 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:58:22 GMT
ADD file:8bedca16bf416520f5df29175a99b07585281465c459544b9f9679016f59762a in / 
# Wed, 28 Jun 2023 09:58:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 05:58:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:59:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:06e53fabee8df31622850c604f9242a52a466ec4eb75320019bdfdc8ec311692`  
		Last Modified: Tue, 04 Jul 2023 06:22:20 GMT  
		Size: 24.6 MB (24588135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7655bda15200da93eaa77218c915efbf215e822d3a7ef693f5fbc78a94b8e906`  
		Last Modified: Tue, 04 Jul 2023 06:22:17 GMT  
		Size: 9.6 MB (9599087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bf5309ca27fafde797ae93665faceb2bf2d10325336e4a2004fad3ea3a3928`  
		Last Modified: Tue, 04 Jul 2023 06:22:38 GMT  
		Size: 55.8 MB (55826315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:9e3ca944812a58a43d49c9389e13da1888d89316938b46ade73769204e83877c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99187642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf051e6d28b3c08f77351d519508701a4cc2b452556275a4ec5249d1dff91fb8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:54:46 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:54:46 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:54:46 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 09:54:48 GMT
ADD file:a6db9f7789e57b7119f68e4e4ec9ec5aab8c3c8bd53fd932f3c59c54b1c20a26 in / 
# Wed, 28 Jun 2023 09:54:49 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 06:01:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:02:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1e77eb131c5c9032ce8e6e512f601714ce7ba48e296f5b7a5191703bdcbc904d`  
		Last Modified: Tue, 04 Jul 2023 04:05:23 GMT  
		Size: 27.2 MB (27198330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ae43f445a875bd258928e514043770667dbc9ab823c2a244e3c8d2fb4520ad`  
		Last Modified: Tue, 04 Jul 2023 06:24:04 GMT  
		Size: 11.0 MB (10982532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf4e8446ca8d143e3e482c4d70cf26e4702ff9b4e40c36c27fc3dd2a3c27c556`  
		Last Modified: Tue, 04 Jul 2023 06:24:19 GMT  
		Size: 61.0 MB (61006780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:83bc9f99ef1a1d5eae5dc903bba37c760a0360920680682a5fafb3add76595c8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.9 MB (115873677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9a6dfad5115f5ece291290e14905952c3f87983f65565590978f5b4f04d59cb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 10:04:43 GMT
ARG RELEASE
# Wed, 28 Jun 2023 10:04:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 10:04:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 10:04:43 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 10:04:46 GMT
ADD file:df651ead0b69eb261098e765354dbdf5ffca51275c037d8881fedcaa1c91c36d in / 
# Wed, 28 Jun 2023 10:04:46 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 03:40:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:42:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4e95615eadb7a0d90a47ca15a5c0693371494902f54d8d78a50d53e89e7a20de`  
		Last Modified: Tue, 04 Jul 2023 04:40:49 GMT  
		Size: 33.3 MB (33308759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:276026532e2897addfb94053c99fabaff128631b0106992fca31995a4e07ee2f`  
		Last Modified: Tue, 04 Jul 2023 04:40:45 GMT  
		Size: 12.9 MB (12937997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f779e3d18cc00d1bfffc494a86c621971575cc7b49852f3e69213662057902`  
		Last Modified: Tue, 04 Jul 2023 04:41:19 GMT  
		Size: 69.6 MB (69626921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:de8f76734b0c65cfa398d2ff4bbe8b0ffa917e8c1dff84edff6cf976da2bf84d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.0 MB (98007891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:771aca25ec8f105d9609f3e0abdbb6606b7b5f6217243c0ebf33378d8123b6a4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 10:01:13 GMT
ARG RELEASE
# Wed, 28 Jun 2023 10:01:13 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 10:01:13 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 10:01:14 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 28 Jun 2023 10:01:15 GMT
ADD file:777fd71e798b91bf768b21e1ca4403f388db9936ef55ef68b4b019cb167fa707 in / 
# Wed, 28 Jun 2023 10:01:15 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 12:51:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 12:52:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f5ebe8481b30a6d3b710b0efdec29843cca805811e3be1a4e375761725c40e5a`  
		Last Modified: Tue, 04 Jul 2023 13:07:41 GMT  
		Size: 27.0 MB (27013645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e76df5c29baf17b24cc9ec09debb6341e7d2b72276cb8ded9c6f9b91e2c3c457`  
		Last Modified: Tue, 04 Jul 2023 13:07:39 GMT  
		Size: 10.7 MB (10688202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d32cf23175b375841e6e543d986dd4143c7fffdb28041799bded0d024fec5d7`  
		Last Modified: Tue, 04 Jul 2023 13:07:56 GMT  
		Size: 60.3 MB (60306044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:jammy`

```console
$ docker pull buildpack-deps@sha256:9b7ec77e64b6837e10968f9e2b0760af52fe7da4f66c1d008532f2bb80c0f1e2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:jammy` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:8f28bd087741849791b564aea220968c88f2cace4063336681cd238858e05a79
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.8 MB (249847907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:442a35809fbea57170756e05e1a3bbb375ae8094fe1dbba784e092fd2935b0d5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 03:39:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:40:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:42:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97966f3f03442a3d645f8354f49cc622b4416879f6c59142fab244ca2663677b`  
		Last Modified: Tue, 04 Jul 2023 03:55:49 GMT  
		Size: 7.1 MB (7119871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e29c969f29843010dfda55528bfc810b4e577e4ba39fb2c788a8ea55bb92763`  
		Last Modified: Tue, 04 Jul 2023 03:56:05 GMT  
		Size: 39.4 MB (39428797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13d40b1da6010e8c9c1adb56fc6fb577c2db289f338cac71cc1c97fd28e6bdb`  
		Last Modified: Tue, 04 Jul 2023 03:56:35 GMT  
		Size: 172.9 MB (172868010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f84a66f57eb9a7526b7f1bb0427dd87c3672e42f677bb33bac7970d1c9ee6232
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.7 MB (216723569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2283fac8c756eddab693df3e3369926d3a93560b25cb7c61053ba83125fea69`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:41:15 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:41:15 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:41:15 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:41:15 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:41:18 GMT
ADD file:c13f43a31510c7a4eaa7e4ca90e4f973b19895658b1f9993cab5f93979d4e2dc in / 
# Wed, 28 Jun 2023 08:41:18 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 06:04:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:04:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:08:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:63b96265cfe95b9cec847027033d4226b783ecd042036f5c809a7386027f56b0`  
		Last Modified: Fri, 30 Jun 2023 02:08:02 GMT  
		Size: 27.0 MB (27026961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7ab0e6b76129c24867f4152f7c8da7289c6b5f4a0922ae184713f26945af72`  
		Last Modified: Tue, 04 Jul 2023 06:23:16 GMT  
		Size: 7.0 MB (7019201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78a55edb4070b31d77ce5a81d68e5d76539c587fdaf49d4e2a8b380e36371187`  
		Last Modified: Tue, 04 Jul 2023 06:23:36 GMT  
		Size: 42.2 MB (42222602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6038ce0ab4df67f1a1fb7fd041b97c4c222339ed93b979813ce2703dc8acbd9`  
		Last Modified: Tue, 04 Jul 2023 06:24:04 GMT  
		Size: 140.5 MB (140454805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:20528a086d9dc7bf09bc195454c032fa8d0576fd17267e5120c400ad0ab680e0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.2 MB (241179903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:761bc5ffd9cec06e5f9c4b6b62aac9f90e5db77fbf359088e2c3339804508de6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 06:06:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:07:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:10:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00483067c1437c60cceadf9b4d31783bc9e1adb93770b38287f24ef2943b3c0`  
		Last Modified: Tue, 04 Jul 2023 06:24:51 GMT  
		Size: 7.1 MB (7067072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c1fabd67ce9ecbf104292a6591b53f2a57503bf444faef66c672ca9017fc31`  
		Last Modified: Tue, 04 Jul 2023 06:25:03 GMT  
		Size: 39.3 MB (39345851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b86e59c87a49dd6808d4971ca94a4faea222b3461d58e99bbfb47b5505fd88`  
		Last Modified: Tue, 04 Jul 2023 06:25:28 GMT  
		Size: 166.4 MB (166375969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:36c2809c31013b604a1f6e752eb699bb2ed20f1ecad9ecba0ad16454e70315b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.7 MB (271695715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ed585ef780750325abbece0e460523e6e025223c2ca714512a7db9bd671b94f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:45:53 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:45:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:45:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:45:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:45:56 GMT
ADD file:8c2fc380378944326d602742fde0e30458cd3e82012847b0f7e09c7184bfd135 in / 
# Wed, 28 Jun 2023 08:45:57 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 03:54:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:57:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:07:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7faa46ce6b6f5c34485980029504c3995e38149d0bca67d8b976c5dbb3673644`  
		Last Modified: Tue, 04 Jul 2023 04:42:31 GMT  
		Size: 35.7 MB (35711469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5028dc76c028f10e8828b80e411d373e4db95e0d5232b4f5a0dde9146f46cf`  
		Last Modified: Tue, 04 Jul 2023 04:42:24 GMT  
		Size: 8.3 MB (8260592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e056faa463b64fc04b6eb21623bad5611901f025c629a92bcaf9337b98644f`  
		Last Modified: Tue, 04 Jul 2023 04:42:54 GMT  
		Size: 43.9 MB (43874959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:496391575eedb44a7a5322b38c22ae05c7096680d5c21faa2f1793cd55852ac1`  
		Last Modified: Tue, 04 Jul 2023 04:43:51 GMT  
		Size: 183.8 MB (183848695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:df4cc2c63e69e5b07ee3466abb67396de15ed40b36e9e85e9cd80a17e7bf7bf6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.6 MB (223589120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0893b5590f1c90958e2f8a2b9b84d4a59ded9649b871d31c2014a5057e09d07f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:53:20 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:53:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:53:22 GMT
ADD file:fa0aef35be7808c8fd6751a52bdec4dd81057e2fcaa075c547a1db53640dae9a in / 
# Wed, 28 Jun 2023 08:53:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 12:55:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 12:55:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 12:57:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce02ee0330980398d6a84a50abfa1a8c4d1cba27cbd7442b79f4aa1b1a14020d`  
		Last Modified: Tue, 04 Jul 2023 13:08:30 GMT  
		Size: 28.6 MB (28645696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7aba4ce682de5293312667253fd0a7af53c579484786de09b36208aab9d22c`  
		Last Modified: Tue, 04 Jul 2023 13:08:26 GMT  
		Size: 7.0 MB (7033603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1c12ddc9521fd58bc71f4494c40a5c8889571901807762f83f2db5e8d7d6dc`  
		Last Modified: Tue, 04 Jul 2023 13:08:43 GMT  
		Size: 39.4 MB (39392616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6037f928a3a3f348ad27e66c8ef12e21545b65e48b071cbeeb2990c42fdcad97`  
		Last Modified: Tue, 04 Jul 2023 13:09:09 GMT  
		Size: 148.5 MB (148517205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:jammy-curl`

```console
$ docker pull buildpack-deps@sha256:1ec10719ed03e1ebeb0689d9af0543c4346cf37e8ba423bf4004b7dd3a350ba7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:jammy-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:483b82bc040102243b07bcbb2bb61e88294953b57782d2ee84dc0b81db449cc0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37551100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57a6f6f87887de69ba89a8eba29dd185ff073609b204037b4931d8322101cad3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 03:39:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97966f3f03442a3d645f8354f49cc622b4416879f6c59142fab244ca2663677b`  
		Last Modified: Tue, 04 Jul 2023 03:55:49 GMT  
		Size: 7.1 MB (7119871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:07e89f118c913b2585d650a226dc9954fc9951947e7926291adee70259dfd3f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34046162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c7a7f90ea62180724401b9d98d6cf69cdc58225b859ab44d433bc271d7e9560`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:41:15 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:41:15 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:41:15 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:41:15 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:41:18 GMT
ADD file:c13f43a31510c7a4eaa7e4ca90e4f973b19895658b1f9993cab5f93979d4e2dc in / 
# Wed, 28 Jun 2023 08:41:18 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 06:04:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:63b96265cfe95b9cec847027033d4226b783ecd042036f5c809a7386027f56b0`  
		Last Modified: Fri, 30 Jun 2023 02:08:02 GMT  
		Size: 27.0 MB (27026961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7ab0e6b76129c24867f4152f7c8da7289c6b5f4a0922ae184713f26945af72`  
		Last Modified: Tue, 04 Jul 2023 06:23:16 GMT  
		Size: 7.0 MB (7019201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:9a3b66500d95e556a3251f402d1a2cd06cf9a8d29812d76b179e6627d98c5a2f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 MB (35458083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:296393feca5c587e3328a58596b57de868f32b92cfbe7d8d3dd30578b8aa4e51`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 06:06:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00483067c1437c60cceadf9b4d31783bc9e1adb93770b38287f24ef2943b3c0`  
		Last Modified: Tue, 04 Jul 2023 06:24:51 GMT  
		Size: 7.1 MB (7067072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:a30f0fc4dd7363c101b3c0a6ddf8d05701c93d716bcfb3987a6440a256e02ef2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (43972061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66bb953f4cadc10c7aa36623450ee63de56159a9445d0ff555a886fd1cfa49ff`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:45:53 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:45:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:45:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:45:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:45:56 GMT
ADD file:8c2fc380378944326d602742fde0e30458cd3e82012847b0f7e09c7184bfd135 in / 
# Wed, 28 Jun 2023 08:45:57 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 03:54:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7faa46ce6b6f5c34485980029504c3995e38149d0bca67d8b976c5dbb3673644`  
		Last Modified: Tue, 04 Jul 2023 04:42:31 GMT  
		Size: 35.7 MB (35711469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5028dc76c028f10e8828b80e411d373e4db95e0d5232b4f5a0dde9146f46cf`  
		Last Modified: Tue, 04 Jul 2023 04:42:24 GMT  
		Size: 8.3 MB (8260592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:15dd98493e4ec64bad67c254e1518893e14856b6cc690172a22783584f2f914e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35679299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47ba8f5e175da4bc3069b45bf99ec082ea72d15c9e9924284125f1f00e92d24f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:53:20 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:53:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:53:22 GMT
ADD file:fa0aef35be7808c8fd6751a52bdec4dd81057e2fcaa075c547a1db53640dae9a in / 
# Wed, 28 Jun 2023 08:53:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 12:55:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce02ee0330980398d6a84a50abfa1a8c4d1cba27cbd7442b79f4aa1b1a14020d`  
		Last Modified: Tue, 04 Jul 2023 13:08:30 GMT  
		Size: 28.6 MB (28645696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7aba4ce682de5293312667253fd0a7af53c579484786de09b36208aab9d22c`  
		Last Modified: Tue, 04 Jul 2023 13:08:26 GMT  
		Size: 7.0 MB (7033603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:jammy-scm`

```console
$ docker pull buildpack-deps@sha256:f8d47bd7614fb9021e6e796abc17af03eabd4eb05bd18824ba436ff80c1acdfd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:jammy-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:c79e22f6262ffcc9eb5eee479f1728247ee7c37e1419034d7ef047a9cd8b649f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76979897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4da96a2a7c92bf335b49390e599ef90eeedbad15d69f1c2f3bac70574468ac75`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 03:39:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:40:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97966f3f03442a3d645f8354f49cc622b4416879f6c59142fab244ca2663677b`  
		Last Modified: Tue, 04 Jul 2023 03:55:49 GMT  
		Size: 7.1 MB (7119871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e29c969f29843010dfda55528bfc810b4e577e4ba39fb2c788a8ea55bb92763`  
		Last Modified: Tue, 04 Jul 2023 03:56:05 GMT  
		Size: 39.4 MB (39428797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:57bbae5325f47855ffd8c210e1d028f7d0b6100f91d555c8e12439d8b5eb447a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.3 MB (76268764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:733e20783ce4aabcb2e52abd12bf08f9433f8727787cdaccf590511d8a51f0b8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:41:15 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:41:15 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:41:15 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:41:15 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:41:18 GMT
ADD file:c13f43a31510c7a4eaa7e4ca90e4f973b19895658b1f9993cab5f93979d4e2dc in / 
# Wed, 28 Jun 2023 08:41:18 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 06:04:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:04:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:63b96265cfe95b9cec847027033d4226b783ecd042036f5c809a7386027f56b0`  
		Last Modified: Fri, 30 Jun 2023 02:08:02 GMT  
		Size: 27.0 MB (27026961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7ab0e6b76129c24867f4152f7c8da7289c6b5f4a0922ae184713f26945af72`  
		Last Modified: Tue, 04 Jul 2023 06:23:16 GMT  
		Size: 7.0 MB (7019201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78a55edb4070b31d77ce5a81d68e5d76539c587fdaf49d4e2a8b380e36371187`  
		Last Modified: Tue, 04 Jul 2023 06:23:36 GMT  
		Size: 42.2 MB (42222602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:e6eb6a297d3d042a39568d9807858287b9e33904800427dbc6cd381ca2fb5a18
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74803934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57426953690b8699e351256723056c42ba681320fd297019188c4e0e691a2c4a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:42:48 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:42:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:42:48 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:42:50 GMT
ADD file:262490f82459c14632f5c9a6d6a5cf6c07b4f307e8fd380fa764662cda46e88f in / 
# Wed, 28 Jun 2023 08:42:50 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 06:06:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:07:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ac34a2e0269ced3acc355be706239ee0f3f1e73a035c40dd2fac74827164ee53`  
		Last Modified: Wed, 28 Jun 2023 23:23:40 GMT  
		Size: 28.4 MB (28391011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a00483067c1437c60cceadf9b4d31783bc9e1adb93770b38287f24ef2943b3c0`  
		Last Modified: Tue, 04 Jul 2023 06:24:51 GMT  
		Size: 7.1 MB (7067072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c1fabd67ce9ecbf104292a6591b53f2a57503bf444faef66c672ca9017fc31`  
		Last Modified: Tue, 04 Jul 2023 06:25:03 GMT  
		Size: 39.3 MB (39345851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d55364691bb1f9651472826186b92d4833f75b622cdbe27162c05407de6bf49f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.8 MB (87847020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b10e613256e8e7d422110f0c7e9c8b8862359fce3750e27a2181eda7e3baf12`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:45:53 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:45:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:45:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:45:54 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:45:56 GMT
ADD file:8c2fc380378944326d602742fde0e30458cd3e82012847b0f7e09c7184bfd135 in / 
# Wed, 28 Jun 2023 08:45:57 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 03:54:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:57:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7faa46ce6b6f5c34485980029504c3995e38149d0bca67d8b976c5dbb3673644`  
		Last Modified: Tue, 04 Jul 2023 04:42:31 GMT  
		Size: 35.7 MB (35711469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad5028dc76c028f10e8828b80e411d373e4db95e0d5232b4f5a0dde9146f46cf`  
		Last Modified: Tue, 04 Jul 2023 04:42:24 GMT  
		Size: 8.3 MB (8260592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e056faa463b64fc04b6eb21623bad5611901f025c629a92bcaf9337b98644f`  
		Last Modified: Tue, 04 Jul 2023 04:42:54 GMT  
		Size: 43.9 MB (43874959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:3668467811030c710e7b4d32a58fa54ea53a8eb5e4d1150de312f66aff3c804b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75071915 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48d3bea1f433841c762ab73ba3e96579b91de4f23225f8ec515a383ab6cef371`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:53:20 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:53:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:53:20 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:53:22 GMT
ADD file:fa0aef35be7808c8fd6751a52bdec4dd81057e2fcaa075c547a1db53640dae9a in / 
# Wed, 28 Jun 2023 08:53:22 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 12:55:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 12:55:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce02ee0330980398d6a84a50abfa1a8c4d1cba27cbd7442b79f4aa1b1a14020d`  
		Last Modified: Tue, 04 Jul 2023 13:08:30 GMT  
		Size: 28.6 MB (28645696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7aba4ce682de5293312667253fd0a7af53c579484786de09b36208aab9d22c`  
		Last Modified: Tue, 04 Jul 2023 13:08:26 GMT  
		Size: 7.0 MB (7033603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1c12ddc9521fd58bc71f4494c40a5c8889571901807762f83f2db5e8d7d6dc`  
		Last Modified: Tue, 04 Jul 2023 13:08:43 GMT  
		Size: 39.4 MB (39392616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:kinetic`

```console
$ docker pull buildpack-deps@sha256:c8182962268601e999685babfa78b460a948d4e6f8bebeaf9ac94dd7766a410c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:kinetic` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:0b34490510c29fa74353ade9e5d90182d82346a3246992c1ae54ee125ccb8ed4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.7 MB (262660283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1957599663a9fb73a6c45227894308eee2990917cb02b30a6fa23a66f56f5b74`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:23:07 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:23:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:23:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:23:07 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 28 Jun 2023 08:23:09 GMT
ADD file:50094673f74cf3945ac21e23bb84d41d3516bc1ac90ebf7f17379288c33c17b2 in / 
# Wed, 28 Jun 2023 08:23:09 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 03:43:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:44:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:46:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e4ae0f456d5b5ed53c0d0f67cd1948207060810837f2b15dcdf5bd97bbceb300`  
		Last Modified: Tue, 04 Jul 2023 03:56:47 GMT  
		Size: 27.5 MB (27488903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f7fd2e9f809d0b31bf96fde0b09fb68493e5499b9a4dae5f3dfc0a0ed0b7ce`  
		Last Modified: Tue, 04 Jul 2023 03:56:46 GMT  
		Size: 14.2 MB (14189206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e60069d839c80c438523487b52eb9073ef4a8fd32af5b8a6dfe8480792c8a57`  
		Last Modified: Tue, 04 Jul 2023 03:57:02 GMT  
		Size: 39.8 MB (39825912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbc9753f2da447aadff4044bd763bb11c8f004fa9ab7cccc88048ddacb264aa`  
		Last Modified: Tue, 04 Jul 2023 03:57:35 GMT  
		Size: 181.2 MB (181156262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f78e0e5d6707a04956b352cf8fb6883cb9ce87a31fa7befcfb88144d5a452357
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.6 MB (225624695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3685089673bda68c20b3c886018604ff1e74c04bdd8989f7fca96ba999fab182`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:50:23 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:50:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:50:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:50:23 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 28 Jun 2023 08:50:29 GMT
ADD file:1c3ce20a4b19d1c7779aa47e9799d2887ac4d142bb495eb0bdca08ff1c8fd106 in / 
# Wed, 28 Jun 2023 08:50:30 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 06:09:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:09:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:12:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b2a8550df843bc39f9334e8b8d8524b0e0abe390674577c839e53aa1c6afb06`  
		Last Modified: Tue, 04 Jul 2023 06:24:17 GMT  
		Size: 25.9 MB (25912764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eef66710f99af0d044d772f07b2eaf0c9da9559b1b10f9da05b104e86fb12a7`  
		Last Modified: Tue, 04 Jul 2023 06:24:15 GMT  
		Size: 13.1 MB (13141364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f28d29b0c8e6083c797c1ed79183346245421c696c0b8365d1b4027561dc13e`  
		Last Modified: Tue, 04 Jul 2023 06:24:34 GMT  
		Size: 42.9 MB (42939065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f417099045b65e1689b25195d9a5ca52532043778ba15ae89200da7da00efea`  
		Last Modified: Tue, 04 Jul 2023 06:25:06 GMT  
		Size: 143.6 MB (143631502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:fe77e6e21c64105552429c5273332cc2e769d79bfbf74c26a92cb9cbec3d2d7a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.4 MB (250423813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b20fadd9a6936babea6d9dafc67064e118c913a7342ca0cfd0a522d03de2fd4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:16:50 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:16:51 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:16:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:16:51 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 28 Jun 2023 09:16:58 GMT
ADD file:a41ad4058e77a6f1ee9800af03cf13403d5d844e876246ba55c4ceb2106b6d5f in / 
# Wed, 28 Jun 2023 09:16:59 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 06:11:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:12:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:15:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c5528eed9908e3645e0eff6666ba300d135b6ff9801f5ae1cc49bb06a3f29fcf`  
		Last Modified: Tue, 04 Jul 2023 06:25:40 GMT  
		Size: 26.7 MB (26730941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8785a3c2b399ffc53927bd8e5eea56d2819ea053d0d78910ae32f88d2f9ec680`  
		Last Modified: Tue, 04 Jul 2023 06:25:37 GMT  
		Size: 13.7 MB (13727615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af381f44d3219c7eab50c1af5c7bf36233fa1a694569f8a29e1be2e7d55cd37`  
		Last Modified: Tue, 04 Jul 2023 06:25:53 GMT  
		Size: 39.6 MB (39636653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1160a4dcea08cb2cc3585710f41a7615c6d7bc8668f20d79b85391142f1910b`  
		Last Modified: Tue, 04 Jul 2023 06:26:18 GMT  
		Size: 170.3 MB (170328604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:015d6829eda0af44d4186f2cf2c0b6726a23f5b9574881a0b21e75e419f6f601
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.5 MB (285537534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41cee9ff03f244bfd65fcb2ce00a37aa729796de6aee6a06366fecbcef36eb6c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:04:09 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:04:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:04:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:04:09 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 28 Jun 2023 09:04:12 GMT
ADD file:8c5e727842a7ff4d34b93a1ee45f14532c9b03594ad53400240e6f0f4b99b390 in / 
# Wed, 28 Jun 2023 09:04:12 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 04:09:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:10:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:19:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c4c2a73576db8e1d5b385d67fe412db5e6cd146167f6c5fa6153b87f17abfc3d`  
		Last Modified: Tue, 04 Jul 2023 04:44:10 GMT  
		Size: 32.1 MB (32102426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:297facc34b9d65726d36999c1b9378836014f1dbb15725b2be4359b50bec9d21`  
		Last Modified: Tue, 04 Jul 2023 04:44:07 GMT  
		Size: 16.2 MB (16234063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9cb9fc38b5a1da1252223c33aa1381def6fb94284f39b6c1d6025d92bf99478`  
		Last Modified: Tue, 04 Jul 2023 04:44:34 GMT  
		Size: 44.2 MB (44231612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd62a63c22d9416c3b46dccf9da4cb3234f7549206282332be98c282450d9c7d`  
		Last Modified: Tue, 04 Jul 2023 04:45:31 GMT  
		Size: 193.0 MB (192969433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:5f93f187202e8c33d59f11df9460958e7bb82006e7f5c352aa3396e2f84c24ea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.1 MB (233054315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49759ff9442c254584b8c51244f18d3f1e16237357cf7762aae94572b5536be5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:31:17 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:31:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:31:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:31:17 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 28 Jun 2023 08:31:19 GMT
ADD file:e6e44f70accdecf50c8942a8e70c4d2c1d419d1d61696730d8aeda653da7216b in / 
# Wed, 28 Jun 2023 08:31:20 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 12:58:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 12:59:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 13:00:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:db47f8f6e4cba14e75b8de75cdb67df7e0da147a37a6d957e95b908f84f113c9`  
		Last Modified: Tue, 04 Jul 2023 13:09:19 GMT  
		Size: 26.0 MB (26034734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9685e4e083ab19eb76163b6e53eae847ce6aae92708ff92c594d59a98c7b4838`  
		Last Modified: Tue, 04 Jul 2023 13:09:17 GMT  
		Size: 14.3 MB (14344539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5066de6f57445c9a11aa5d720bdf2ef58d4105ba79b5f66be22ddfeb03e89d5`  
		Last Modified: Tue, 04 Jul 2023 13:09:32 GMT  
		Size: 39.7 MB (39678636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd20890008cbd35e672a467d9b7fe96a6dc49fcc4e9f24865edb1d639b3c2d82`  
		Last Modified: Tue, 04 Jul 2023 13:09:57 GMT  
		Size: 153.0 MB (152996406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:kinetic-curl`

```console
$ docker pull buildpack-deps@sha256:10dc553ad4a9ec6df694b1bf115cd6fcb55239d60d0b42de46a26b1082fd45a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:kinetic-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:9864a6a8920e10635a22be668dff1a9169c7e666efc7a51cf9cbd0fdacbd6a6d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41678109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6c7af30dd7e2311fbf3138dfcad631878055c64260ae8f409b8c95880e15e2c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:23:07 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:23:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:23:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:23:07 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 28 Jun 2023 08:23:09 GMT
ADD file:50094673f74cf3945ac21e23bb84d41d3516bc1ac90ebf7f17379288c33c17b2 in / 
# Wed, 28 Jun 2023 08:23:09 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 03:43:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e4ae0f456d5b5ed53c0d0f67cd1948207060810837f2b15dcdf5bd97bbceb300`  
		Last Modified: Tue, 04 Jul 2023 03:56:47 GMT  
		Size: 27.5 MB (27488903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f7fd2e9f809d0b31bf96fde0b09fb68493e5499b9a4dae5f3dfc0a0ed0b7ce`  
		Last Modified: Tue, 04 Jul 2023 03:56:46 GMT  
		Size: 14.2 MB (14189206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1f30c94b4bb67a6deaf734529e1d2c320e9c3f922b7b943f713c89b4f3ca87ac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39054128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75cd405b115352482c61020e337a99b4f2384b9fd08dced23ea846b4a6c434f2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:50:23 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:50:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:50:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:50:23 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 28 Jun 2023 08:50:29 GMT
ADD file:1c3ce20a4b19d1c7779aa47e9799d2887ac4d142bb495eb0bdca08ff1c8fd106 in / 
# Wed, 28 Jun 2023 08:50:30 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 06:09:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b2a8550df843bc39f9334e8b8d8524b0e0abe390674577c839e53aa1c6afb06`  
		Last Modified: Tue, 04 Jul 2023 06:24:17 GMT  
		Size: 25.9 MB (25912764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eef66710f99af0d044d772f07b2eaf0c9da9559b1b10f9da05b104e86fb12a7`  
		Last Modified: Tue, 04 Jul 2023 06:24:15 GMT  
		Size: 13.1 MB (13141364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:bb8b48791f089f579a9f0afb2d153d2446b2043976784a576a2f273109ffb37a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.5 MB (40458556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5284d33edbce56f17809d71b6dbbe0d5a70d631472e3c6d187c5e08e7f4ca3a4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:16:50 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:16:51 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:16:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:16:51 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 28 Jun 2023 09:16:58 GMT
ADD file:a41ad4058e77a6f1ee9800af03cf13403d5d844e876246ba55c4ceb2106b6d5f in / 
# Wed, 28 Jun 2023 09:16:59 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 06:11:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c5528eed9908e3645e0eff6666ba300d135b6ff9801f5ae1cc49bb06a3f29fcf`  
		Last Modified: Tue, 04 Jul 2023 06:25:40 GMT  
		Size: 26.7 MB (26730941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8785a3c2b399ffc53927bd8e5eea56d2819ea053d0d78910ae32f88d2f9ec680`  
		Last Modified: Tue, 04 Jul 2023 06:25:37 GMT  
		Size: 13.7 MB (13727615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:1a07aad2e6e2c52838bd9242961c6789330426428afb48c14562883694a9b122
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.3 MB (48336489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:679e8eb78bb21e03123228167c1acc8b09581ee954f76ba102155947e6cb639a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:04:09 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:04:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:04:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:04:09 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 28 Jun 2023 09:04:12 GMT
ADD file:8c5e727842a7ff4d34b93a1ee45f14532c9b03594ad53400240e6f0f4b99b390 in / 
# Wed, 28 Jun 2023 09:04:12 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 04:09:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c4c2a73576db8e1d5b385d67fe412db5e6cd146167f6c5fa6153b87f17abfc3d`  
		Last Modified: Tue, 04 Jul 2023 04:44:10 GMT  
		Size: 32.1 MB (32102426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:297facc34b9d65726d36999c1b9378836014f1dbb15725b2be4359b50bec9d21`  
		Last Modified: Tue, 04 Jul 2023 04:44:07 GMT  
		Size: 16.2 MB (16234063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:e908ca3d7bfcf4e6d6f2dc17aeca9c4457ff23e236f684e242b64d000694465c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.4 MB (40379273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2ccbd6c1f7c17aaac71be9909dcf08a4573fd11727adc6d75fadb51f36b2095`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:31:17 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:31:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:31:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:31:17 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 28 Jun 2023 08:31:19 GMT
ADD file:e6e44f70accdecf50c8942a8e70c4d2c1d419d1d61696730d8aeda653da7216b in / 
# Wed, 28 Jun 2023 08:31:20 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 12:58:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:db47f8f6e4cba14e75b8de75cdb67df7e0da147a37a6d957e95b908f84f113c9`  
		Last Modified: Tue, 04 Jul 2023 13:09:19 GMT  
		Size: 26.0 MB (26034734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9685e4e083ab19eb76163b6e53eae847ce6aae92708ff92c594d59a98c7b4838`  
		Last Modified: Tue, 04 Jul 2023 13:09:17 GMT  
		Size: 14.3 MB (14344539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:kinetic-scm`

```console
$ docker pull buildpack-deps@sha256:1ca7f8e293e400892c469b069eae7e97b60cd0a1d2a6f58ffa6aafaf45bedda0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:kinetic-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:d52ddd72ddd4f630e64370ad14d0ec6b99705784fc76f396c2d3d67230db3403
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.5 MB (81504021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ec8c6e4d643fed5a6197bd272d12574893b6727b71d0bddc0526d40019fb457`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:23:07 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:23:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:23:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:23:07 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 28 Jun 2023 08:23:09 GMT
ADD file:50094673f74cf3945ac21e23bb84d41d3516bc1ac90ebf7f17379288c33c17b2 in / 
# Wed, 28 Jun 2023 08:23:09 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 03:43:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:44:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e4ae0f456d5b5ed53c0d0f67cd1948207060810837f2b15dcdf5bd97bbceb300`  
		Last Modified: Tue, 04 Jul 2023 03:56:47 GMT  
		Size: 27.5 MB (27488903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f7fd2e9f809d0b31bf96fde0b09fb68493e5499b9a4dae5f3dfc0a0ed0b7ce`  
		Last Modified: Tue, 04 Jul 2023 03:56:46 GMT  
		Size: 14.2 MB (14189206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e60069d839c80c438523487b52eb9073ef4a8fd32af5b8a6dfe8480792c8a57`  
		Last Modified: Tue, 04 Jul 2023 03:57:02 GMT  
		Size: 39.8 MB (39825912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:44b7926bef25e86fda0ce933db0a51672dd4b6569f40fbde5413b85c40259d7b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.0 MB (81993193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1888d5faa20899d778ded8b8bc5a0d939c3c81a8d6ffeffa5669bf0f8dc8a9d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:50:23 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:50:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:50:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:50:23 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 28 Jun 2023 08:50:29 GMT
ADD file:1c3ce20a4b19d1c7779aa47e9799d2887ac4d142bb495eb0bdca08ff1c8fd106 in / 
# Wed, 28 Jun 2023 08:50:30 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 06:09:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:09:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b2a8550df843bc39f9334e8b8d8524b0e0abe390674577c839e53aa1c6afb06`  
		Last Modified: Tue, 04 Jul 2023 06:24:17 GMT  
		Size: 25.9 MB (25912764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eef66710f99af0d044d772f07b2eaf0c9da9559b1b10f9da05b104e86fb12a7`  
		Last Modified: Tue, 04 Jul 2023 06:24:15 GMT  
		Size: 13.1 MB (13141364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f28d29b0c8e6083c797c1ed79183346245421c696c0b8365d1b4027561dc13e`  
		Last Modified: Tue, 04 Jul 2023 06:24:34 GMT  
		Size: 42.9 MB (42939065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d82da2a7c889be494f08719c2be0bae60e0130d8f57987e9dbbefe8771bc942f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.1 MB (80095209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04eaa9e6f7cd4097cd50bf0de7c32b8d39d1c5d8ac59cf278e3defea8e03a703`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:16:50 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:16:51 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:16:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:16:51 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 28 Jun 2023 09:16:58 GMT
ADD file:a41ad4058e77a6f1ee9800af03cf13403d5d844e876246ba55c4ceb2106b6d5f in / 
# Wed, 28 Jun 2023 09:16:59 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 06:11:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:12:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c5528eed9908e3645e0eff6666ba300d135b6ff9801f5ae1cc49bb06a3f29fcf`  
		Last Modified: Tue, 04 Jul 2023 06:25:40 GMT  
		Size: 26.7 MB (26730941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8785a3c2b399ffc53927bd8e5eea56d2819ea053d0d78910ae32f88d2f9ec680`  
		Last Modified: Tue, 04 Jul 2023 06:25:37 GMT  
		Size: 13.7 MB (13727615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af381f44d3219c7eab50c1af5c7bf36233fa1a694569f8a29e1be2e7d55cd37`  
		Last Modified: Tue, 04 Jul 2023 06:25:53 GMT  
		Size: 39.6 MB (39636653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:264fc69c8de3193a7191aae5bb3f4c3db4fbf1a9f0e72d801c70971713aadbda
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.6 MB (92568101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6367bde1dbdeeadc100e3b50d95455d079ffc7c8f892d24e31742464e7e00931`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 09:04:09 GMT
ARG RELEASE
# Wed, 28 Jun 2023 09:04:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 09:04:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 09:04:09 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 28 Jun 2023 09:04:12 GMT
ADD file:8c5e727842a7ff4d34b93a1ee45f14532c9b03594ad53400240e6f0f4b99b390 in / 
# Wed, 28 Jun 2023 09:04:12 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 04:09:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:10:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c4c2a73576db8e1d5b385d67fe412db5e6cd146167f6c5fa6153b87f17abfc3d`  
		Last Modified: Tue, 04 Jul 2023 04:44:10 GMT  
		Size: 32.1 MB (32102426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:297facc34b9d65726d36999c1b9378836014f1dbb15725b2be4359b50bec9d21`  
		Last Modified: Tue, 04 Jul 2023 04:44:07 GMT  
		Size: 16.2 MB (16234063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9cb9fc38b5a1da1252223c33aa1381def6fb94284f39b6c1d6025d92bf99478`  
		Last Modified: Tue, 04 Jul 2023 04:44:34 GMT  
		Size: 44.2 MB (44231612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:d1bc086fc34aa7a36d0e1167a5767ca9f9e1817421f90a56fe4414d21a4f3286
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.1 MB (80057909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b9a8ff3339995ee87b2d7b6c3a9e615a3f0266ebfcd50b7f691d0097c79672e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:31:17 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:31:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:31:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:31:17 GMT
LABEL org.opencontainers.image.version=22.10
# Wed, 28 Jun 2023 08:31:19 GMT
ADD file:e6e44f70accdecf50c8942a8e70c4d2c1d419d1d61696730d8aeda653da7216b in / 
# Wed, 28 Jun 2023 08:31:20 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 12:58:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 12:59:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:db47f8f6e4cba14e75b8de75cdb67df7e0da147a37a6d957e95b908f84f113c9`  
		Last Modified: Tue, 04 Jul 2023 13:09:19 GMT  
		Size: 26.0 MB (26034734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9685e4e083ab19eb76163b6e53eae847ce6aae92708ff92c594d59a98c7b4838`  
		Last Modified: Tue, 04 Jul 2023 13:09:17 GMT  
		Size: 14.3 MB (14344539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5066de6f57445c9a11aa5d720bdf2ef58d4105ba79b5f66be22ddfeb03e89d5`  
		Last Modified: Tue, 04 Jul 2023 13:09:32 GMT  
		Size: 39.7 MB (39678636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:latest`

```console
$ docker pull buildpack-deps@sha256:e8045f6c5b35d465af4400cf07baf28937774c70d0b67b75db9aa5a772245507
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

### `buildpack-deps:latest` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:9fa042ef286f67914fb32a3dc539a9a9011d3030d11178a287fec058f4af2e0d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.7 MB (348696237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:870f7a6134d053997696565f36185aa08d0268c5d2ead2098c03ec2543d8c186`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:19:44 GMT
ADD file:5d17ca085473e890bd6eca4abf6d324c3181f80692523b83ef25d1c42576b99f in / 
# Tue, 04 Jul 2023 01:19:44 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:27:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:28:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:29:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d52e4f012db158bb7c0fe215b98af1facaddcbaee530efd69b1bae07d597b711`  
		Last Modified: Tue, 04 Jul 2023 01:24:39 GMT  
		Size: 49.6 MB (49551432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd206bea61ff3e3b54be1c20b58d8475ddd6f89df176146ddb7a2fd2c747ea2`  
		Last Modified: Tue, 04 Jul 2023 03:51:23 GMT  
		Size: 24.0 MB (24030593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2320f9be4a9c605d1ac847cf67cec42b91484a7cf7c94996417a0c7c316deadc`  
		Last Modified: Tue, 04 Jul 2023 03:51:42 GMT  
		Size: 64.1 MB (64111613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5565e0ba8dfce32b9049f21ceeb212946e0bb810d94cbd2db94ca61082f657`  
		Last Modified: Tue, 04 Jul 2023 03:52:18 GMT  
		Size: 211.0 MB (211002599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:7630e74069ab9afc052421fab33b53a63046a9f0a81ca78e752b60f0bf5e6f30
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.0 MB (315974639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efd6d55edc39161f4227507b095e44656ca35b9df7ba73a742e6d46ac8dcbac8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:48:22 GMT
ADD file:09001854dc5081f907ac2a66d301e4b3d6b4bf2c2483aad5395a535bf068698d in / 
# Tue, 04 Jul 2023 00:48:22 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:21:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:21:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:24:09 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7e0a1f476b42bcc214197ec9c5ef753ddf2ab36a314416a6ac96cd921ff0d41d`  
		Last Modified: Tue, 04 Jul 2023 00:51:29 GMT  
		Size: 47.4 MB (47402786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68311cc5ff511aa59283fdd7f1e25bc33dfc3ad9ae87e5c94447f36c3f7c4817`  
		Last Modified: Tue, 04 Jul 2023 04:28:32 GMT  
		Size: 22.7 MB (22708933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09518fc93ba137cac901dd7b0cc5fab1e20a21a7d6bbe3a35b7f921a069ddc5c`  
		Last Modified: Tue, 04 Jul 2023 04:28:53 GMT  
		Size: 61.6 MB (61553936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0a9d5bee850aae2d389dee19882ddf586d298ba8cc4d4100b77a7bc33204f0`  
		Last Modified: Tue, 04 Jul 2023 04:29:28 GMT  
		Size: 184.3 MB (184308984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:ccbb43b6d2ff2010f6972b17d2c35e80179b93721b3b4075a83d17fd211df4d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.4 MB (301419261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71ba632fe6ed398564cb984e2524c39cfe7c23c5d5ce9b754516330315011653`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:57:42 GMT
ADD file:279ef7213d41f1f7ae76bd76293a5107fd1f8caf557f837cab9c834d2841e031 in / 
# Tue, 04 Jul 2023 00:57:43 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:49:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:50:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:51:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b9bdcf1a9a6361f231594c76a75bfb4c2fef5f9745b9713bbd50efaf37ca11b8`  
		Last Modified: Tue, 04 Jul 2023 01:02:26 GMT  
		Size: 45.2 MB (45236201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8ee33ea63b2391e912423c14b2f1e789137ffb03659568cb361a2fa2b4efbd`  
		Last Modified: Tue, 04 Jul 2023 06:18:41 GMT  
		Size: 21.9 MB (21936446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2a5b4416a84ac4585c3e3879ca49a6fc3e8d46028a4f27098ae1bdb4ae710d`  
		Last Modified: Tue, 04 Jul 2023 06:19:01 GMT  
		Size: 59.3 MB (59261674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfb211eb5b07ec381fa590fdb20338a17e1ac7282488bfe67ebf61eb9d8ef36`  
		Last Modified: Tue, 04 Jul 2023 06:19:36 GMT  
		Size: 175.0 MB (174984940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a11d7b66e7e9ee6221856ac61d5a24ac2fa826652e2ad6decc9068462572a119
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.5 MB (339524386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41b72a638a02bcfb5b6fb54590f95199209e6bb9e8ba83b5675a76bdd3a62b4d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:26 GMT
ADD file:ab1761d899751c4d24e15179fc9e7e7ac3fb83798ee37ca13d6a6ac44fbeded3 in / 
# Tue, 04 Jul 2023 01:57:27 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:54:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:54:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:56:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:42cbebf8bc116ba1aed7897e2d0566bf49da9d5c70be71b6a7cb07805d2f5b7a`  
		Last Modified: Tue, 04 Jul 2023 02:00:57 GMT  
		Size: 49.6 MB (49572781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0518ec57568a70561f7c04650f9554c88dada973f54d88e36f65b0796d35de`  
		Last Modified: Tue, 04 Jul 2023 06:21:03 GMT  
		Size: 23.6 MB (23569546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356172c718acf9930d9465b170864319079e2d2ebac0ddef781d64e85789531e`  
		Last Modified: Tue, 04 Jul 2023 06:21:20 GMT  
		Size: 64.0 MB (63984075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dddcd3ceb9980caac379e8f8eeafe1e901f017e5768b867705a0834cc1274efa`  
		Last Modified: Tue, 04 Jul 2023 06:21:49 GMT  
		Size: 202.4 MB (202397984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; 386

```console
$ docker pull buildpack-deps@sha256:bd112b098fcf0109e2d3d75cb01da9035f9aa2b763863b2be966c3c1a892b655
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.3 MB (351325313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a527ba005f783dc8585ad58568efedd0ad8a89a20c2877cd3b9cd5bfc634702`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:38:25 GMT
ADD file:e0a25fe261e09183ec383698ab2c800f93c5b0805564d7104ad5119db52cccb7 in / 
# Tue, 04 Jul 2023 01:38:25 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:28:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:28:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:30:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:381263dab43af8bfb8e85c7a9a32f35492cbdcc3a046b35f947cf3bf3a55f4c1`  
		Last Modified: Tue, 04 Jul 2023 01:43:02 GMT  
		Size: 50.6 MB (50562388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af522778d6fcd5f4b85dafb1f21b89441dedee6ce875890b15ad8c454bbb9fe6`  
		Last Modified: Tue, 04 Jul 2023 05:38:10 GMT  
		Size: 24.9 MB (24869747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501f685d713d76bdc0731a917b074d79f3de7c84bfe09c53585642801175a72f`  
		Last Modified: Tue, 04 Jul 2023 05:38:34 GMT  
		Size: 66.0 MB (65972310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993e54703a4428a35a92b50b46a2b72088e5f98ec8687291e59ba960778653ce`  
		Last Modified: Tue, 04 Jul 2023 05:39:21 GMT  
		Size: 209.9 MB (209920868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:109dccdd704f2335380eafe52886c571b5ecc9fc6f8e8ff477f178f88a1bcd3a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.7 MB (325698556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63ff7002fa7f867935af5542ea11c588ff00e71b610322da6f1ee76d404f1372`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:08:42 GMT
ADD file:c567fc0f97f36ea531c05e159cd6ac2a8747f14ea5b6ccae39bab9d305da180d in / 
# Tue, 04 Jul 2023 01:08:47 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:34:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:36:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:42:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76240e493592cbc7ca56583a6e8e03ab12a967b65bbeb1df7828a5099fa271d9`  
		Last Modified: Tue, 04 Jul 2023 01:19:16 GMT  
		Size: 49.5 MB (49542143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85086244c52affe40f860feee6e34c03fd0f782e853b00950f1a9b8b6704d24f`  
		Last Modified: Tue, 04 Jul 2023 14:56:03 GMT  
		Size: 23.6 MB (23611680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2482ef924bba9e0b7ef4ad15506bbcf2a7db029acfc793f94b5d17435ed529`  
		Last Modified: Tue, 04 Jul 2023 14:56:55 GMT  
		Size: 63.0 MB (62950425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a976801f0e288a1695ce313557e999ec73ed5562492816ed2e559f8fadcba08`  
		Last Modified: Tue, 04 Jul 2023 14:58:59 GMT  
		Size: 189.6 MB (189594308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d118d12ab7bda84f249868aa497f83e1ee8489b9062b3d275991f7c9178fb44a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.8 MB (362817855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07b0cde07b2b8c19168a241b2b585bba6b27c80cdb9761dfd1dcba9a1d952f9f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:17:23 GMT
ADD file:5aaa642008df5a97014e76042a767f06bbfda91db1d5f336a1b3f98e9b11c7a1 in / 
# Tue, 04 Jul 2023 01:17:26 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:26:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:27:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:32:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e039cf6634cf83a31e97e2a56b4db40a8c38a62d6857c77e687d5edb3eb0dfde`  
		Last Modified: Tue, 04 Jul 2023 01:23:59 GMT  
		Size: 53.5 MB (53536740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54fff62f5ff539ace95f1581096d57b95ca024b9d5cc7c85bb4a2bf159ad845f`  
		Last Modified: Tue, 04 Jul 2023 04:36:20 GMT  
		Size: 25.7 MB (25681297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd5a2ec3d78fd420afc5e1c6739ad59505cf484be0ea1c2c2dfe00c7b2c00ec`  
		Last Modified: Tue, 04 Jul 2023 04:36:52 GMT  
		Size: 69.6 MB (69569498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c3418743f63acf6f2325abc19057fd064d786b061702494a8afd12dba2787ca`  
		Last Modified: Tue, 04 Jul 2023 04:37:57 GMT  
		Size: 214.0 MB (214030320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:8ae64baa0daee2c34ad05f273d64404d1daf9cbdcb9cf75baa84eaeee3aa34ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.1 MB (318132923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:208c88d3645147348e10f8100a5ad65a12fb037cebe1b20bfa7551fee026e98c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:31:54 GMT
ADD file:0ad7ffbe777e5367ad6dcbb4a182e1d578739aa7a4853f82f21bd71d824de7ae in / 
# Tue, 04 Jul 2023 01:31:56 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 12:47:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 12:47:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 12:48:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce9d001c0d31ec9b8072b1a9bd01771a10ea8ddfefa381cf9ce7e2d63538aaeb`  
		Last Modified: Tue, 04 Jul 2023 01:36:50 GMT  
		Size: 47.9 MB (47921709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024bda56b20d3018344098f67965337568b532ea03f09d87858a2bb5eae82bf7`  
		Last Modified: Tue, 04 Jul 2023 13:05:34 GMT  
		Size: 24.0 MB (24028793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da5b83dc971cc08c6baeb1ddd5fb5de06beefef83c0444c224b4e377d704705`  
		Last Modified: Tue, 04 Jul 2023 13:05:50 GMT  
		Size: 63.1 MB (63112809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3bc88ad73a4c8df0ca6b17f424b27e05a29533428b9a47f3576c9be9e81540c`  
		Last Modified: Tue, 04 Jul 2023 13:06:19 GMT  
		Size: 183.1 MB (183069612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:lunar`

```console
$ docker pull buildpack-deps@sha256:3af97726bdf17e4258a19ca66a6133fcba3a5e06827e9a4a850f0e8427a396f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:lunar` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:060c71d6a2053b21c4c5e8cd20ccd50f587f3dea37321b1af7f050c80e0ac040
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.8 MB (267815018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c17f80b562319d5fb916eb776f579020c47586fbfc79b3ae2ee8d0cbdfd3ce03`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:28:38 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:28:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:28:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:28:38 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:28:39 GMT
ADD file:708314051e878a0c6071fb2c8d4458a04ce058f47f2cfaa58c1b5a42e837ca0f in / 
# Thu, 15 Jun 2023 08:28:40 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:47:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:48:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:50:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ccc37bca66e7c29e0d65a4279511fe9a93932a4bb80e79e95144f3812632b61a`  
		Last Modified: Fri, 16 Jun 2023 01:56:54 GMT  
		Size: 27.6 MB (27612943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7beeb5a79f9bd13c90ee4c9f68636fc642df773adb1bd04e27e2115f6c12a6d`  
		Last Modified: Fri, 16 Jun 2023 01:56:52 GMT  
		Size: 13.7 MB (13744092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a98e278987c0da01adb1f6145dec78bd526ecc11c227e2e74c48de9cd72c40`  
		Last Modified: Fri, 16 Jun 2023 01:57:09 GMT  
		Size: 44.4 MB (44371533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ad6ec5ea91c193cf063d5afed2481b1bf6bd664ffc3a333154de164470c017`  
		Last Modified: Fri, 16 Jun 2023 01:57:40 GMT  
		Size: 182.1 MB (182086450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1775b10436d83e9c74fb94a701896a79959b60929ff867805f3af15e5887bdb7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.2 MB (232238791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d919701a0aadbffccea3bcfb66835adf40d30ec9815f9564db14e9f40b618ed`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:10:50 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:10:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:10:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:10:51 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:10:53 GMT
ADD file:8484efc06b5f22d170eef374f45df452d8e36f4cbef702f7ee4d1f130dd28093 in / 
# Thu, 15 Jun 2023 08:10:53 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 00:49:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 00:50:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 00:53:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ca5128fe76949cc104af7f40ce0f7213fe093079077d47dd525fa0189090c57e`  
		Last Modified: Fri, 16 Jun 2023 00:59:51 GMT  
		Size: 25.4 MB (25432780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d8ca764d56bdf14c46fabd5c4e2e988ce166d01c8c0631d7c345802ace7bf1`  
		Last Modified: Fri, 16 Jun 2023 00:59:50 GMT  
		Size: 12.7 MB (12662932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b3e8b607724476a55e2e23faa2859f1e37c17323d12df2f9b87de3745b98e3`  
		Last Modified: Fri, 16 Jun 2023 01:00:07 GMT  
		Size: 48.7 MB (48652729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b17d9a7a6b4123e5072aa4ab3b712d7b1a715d71ffb3014b99eee3394fe9fa02`  
		Last Modified: Fri, 16 Jun 2023 01:00:36 GMT  
		Size: 145.5 MB (145490350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:b6838fb7edbb355dd8edcd769f623d47cfef3c1ad6c0a3abbaaec22ce133921e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.9 MB (257937976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ba91a8a887dc40746a34ed310c28a682f2e87c3521de6e9c4324a2f41fb82b3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:33:24 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:33:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:33:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:33:25 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:33:58 GMT
ADD file:064ac1f238394a53372e0db107e28835aa3c39ed189a15fe85c532bbb50bfbaf in / 
# Thu, 15 Jun 2023 08:33:59 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:25:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:25:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:28:52 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fc6a8da5865fc488969148ca6c503307bba4023ecc0cdceaaae76a8b9852f031`  
		Last Modified: Fri, 16 Jun 2023 02:35:25 GMT  
		Size: 27.0 MB (27029986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8dde3bba356efbb171daed99ec516dc5c5c9a9b19d538fcb9fd0031bd92403a`  
		Last Modified: Fri, 16 Jun 2023 02:35:22 GMT  
		Size: 13.3 MB (13333143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a9f35a1267eac739bb82daa33daa3a21960fb88acbc2177a8156f23b857239`  
		Last Modified: Fri, 16 Jun 2023 02:35:38 GMT  
		Size: 44.2 MB (44217375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:458bfa897fdd09d151a3e8a28025d6adf7ed1844f5f0245ce523235d8c279bf5`  
		Last Modified: Fri, 16 Jun 2023 02:36:03 GMT  
		Size: 173.4 MB (173357472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:6d6ddf54830ccbd4828b9c92614b8428e223455821e4cf626b1a991e2f7c8aed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.7 MB (292741826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ca0901e8811adcec0e4685f99570016590fd216ba20798cea36a7bbfcb2d046`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:29:14 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:29:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:29:15 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:29:15 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:29:17 GMT
ADD file:5ebdf4bd4bc2b27019f20fb1964a395fa504d4f20e208c54237e363895b492d7 in / 
# Thu, 15 Jun 2023 08:29:18 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:11:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:12:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:17:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a58a0b662b0d4d5e271c7c17f35795b5782a33c69a079e473f7c2303bee50024`  
		Last Modified: Fri, 16 Jun 2023 01:28:52 GMT  
		Size: 32.0 MB (32010412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6f165de89ef5a3a93777200dd180f02a8fc30051f7eb6267300a3e6f27ae1e`  
		Last Modified: Fri, 16 Jun 2023 01:28:48 GMT  
		Size: 15.8 MB (15841962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06312954ebad2b0995222a924fae1923e9b3c87aa73ff14beea981d9235b706d`  
		Last Modified: Fri, 16 Jun 2023 01:29:15 GMT  
		Size: 49.1 MB (49073779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adcdba320d64983a5412706a631d98112285fa65575f90a37f1186e72671d860`  
		Last Modified: Fri, 16 Jun 2023 01:30:10 GMT  
		Size: 195.8 MB (195815673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:381572bf0ac103571328da2f7fe25e0972ddc48e59368440128ec280f685fac4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.9 MB (239916461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c3c5aaa14320304059fd5f516a647ad617ea98ce7d61ad3cd07d091c5376597`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:11:16 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:11:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:11:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:11:16 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:11:18 GMT
ADD file:3974fe053080180d99954042c25b3bd0c82e320fb4521b197cbc45f21885fc43 in / 
# Thu, 15 Jun 2023 08:11:18 GMT
CMD ["/bin/bash"]
# Sat, 17 Jun 2023 09:53:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 17 Jun 2023 09:54:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 17 Jun 2023 09:55:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:761ebd2058697796f2f98019cecedb81ef33759e6c1ec5a428e5bfcc3fe17d92`  
		Last Modified: Sat, 17 Jun 2023 10:02:12 GMT  
		Size: 26.2 MB (26245344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36084a86fb1b20f414b56d87cfcfa6dbc269df581ae9079da63a5c20f292984`  
		Last Modified: Sat, 17 Jun 2023 10:02:10 GMT  
		Size: 14.0 MB (14005266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a9be9d6364c4e6a0cc7388e754f4dea89849b8149102ccc37c8849f51879091`  
		Last Modified: Sat, 17 Jun 2023 10:02:24 GMT  
		Size: 44.2 MB (44249340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97e0d170e15949f28ed04940320f25faa3aaabf630a5deff17e662faf8174619`  
		Last Modified: Sat, 17 Jun 2023 10:02:50 GMT  
		Size: 155.4 MB (155416511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:lunar-curl`

```console
$ docker pull buildpack-deps@sha256:632adb935a5ed86a9a06b181c60d0112467852511409e4c2ff5725ebe3bec909
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:lunar-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:8b4a7037ab529927d19c652a98edece16c14a141220bb94b2ae137372a910662
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.4 MB (41357035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cb02a4320e2d201d51f16cac15f0e1a4bd615b6d5f6294bf6e3c45f3d864710`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:28:38 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:28:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:28:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:28:38 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:28:39 GMT
ADD file:708314051e878a0c6071fb2c8d4458a04ce058f47f2cfaa58c1b5a42e837ca0f in / 
# Thu, 15 Jun 2023 08:28:40 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:47:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ccc37bca66e7c29e0d65a4279511fe9a93932a4bb80e79e95144f3812632b61a`  
		Last Modified: Fri, 16 Jun 2023 01:56:54 GMT  
		Size: 27.6 MB (27612943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7beeb5a79f9bd13c90ee4c9f68636fc642df773adb1bd04e27e2115f6c12a6d`  
		Last Modified: Fri, 16 Jun 2023 01:56:52 GMT  
		Size: 13.7 MB (13744092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:61de8a1c369fb750af225159ced6e4c45df3ad711c10ad9598b6764df05f9f06
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.1 MB (38095712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:217162e2f73ec8805a9bcc072434a36250aaff6d65a445fba2cc1fc08f1ed000`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:10:50 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:10:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:10:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:10:51 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:10:53 GMT
ADD file:8484efc06b5f22d170eef374f45df452d8e36f4cbef702f7ee4d1f130dd28093 in / 
# Thu, 15 Jun 2023 08:10:53 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 00:49:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ca5128fe76949cc104af7f40ce0f7213fe093079077d47dd525fa0189090c57e`  
		Last Modified: Fri, 16 Jun 2023 00:59:51 GMT  
		Size: 25.4 MB (25432780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d8ca764d56bdf14c46fabd5c4e2e988ce166d01c8c0631d7c345802ace7bf1`  
		Last Modified: Fri, 16 Jun 2023 00:59:50 GMT  
		Size: 12.7 MB (12662932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:8204f0499f6b7fc2d2a56297ffc2dd01f35c30d598fd18c40ca2c24947ccf3be
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.4 MB (40363129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c55367957df75573ca685df1b793a902c55a42f9cd552150ccb1fa84d33226bb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:33:24 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:33:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:33:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:33:25 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:33:58 GMT
ADD file:064ac1f238394a53372e0db107e28835aa3c39ed189a15fe85c532bbb50bfbaf in / 
# Thu, 15 Jun 2023 08:33:59 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:25:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fc6a8da5865fc488969148ca6c503307bba4023ecc0cdceaaae76a8b9852f031`  
		Last Modified: Fri, 16 Jun 2023 02:35:25 GMT  
		Size: 27.0 MB (27029986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8dde3bba356efbb171daed99ec516dc5c5c9a9b19d538fcb9fd0031bd92403a`  
		Last Modified: Fri, 16 Jun 2023 02:35:22 GMT  
		Size: 13.3 MB (13333143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:dc5e0428f7f0c3135af8d7fee001e103cea834d13b0ec934142f1415dd644071
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47852374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c6d6cf91b670992b73799b26277cc6486e785cb084948d3c1fa3bb5d0d71f89`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:29:14 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:29:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:29:15 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:29:15 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:29:17 GMT
ADD file:5ebdf4bd4bc2b27019f20fb1964a395fa504d4f20e208c54237e363895b492d7 in / 
# Thu, 15 Jun 2023 08:29:18 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:11:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a58a0b662b0d4d5e271c7c17f35795b5782a33c69a079e473f7c2303bee50024`  
		Last Modified: Fri, 16 Jun 2023 01:28:52 GMT  
		Size: 32.0 MB (32010412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6f165de89ef5a3a93777200dd180f02a8fc30051f7eb6267300a3e6f27ae1e`  
		Last Modified: Fri, 16 Jun 2023 01:28:48 GMT  
		Size: 15.8 MB (15841962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:9ca9483cad5134ed4dc7b67acb9e8b817198119f4f1349d4158bdc50f6ba713b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40250610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3492b4e597fbe3726f466a64c487ccb85135bd0b3119510b80c42f8b19c7a16`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:11:16 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:11:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:11:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:11:16 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:11:18 GMT
ADD file:3974fe053080180d99954042c25b3bd0c82e320fb4521b197cbc45f21885fc43 in / 
# Thu, 15 Jun 2023 08:11:18 GMT
CMD ["/bin/bash"]
# Sat, 17 Jun 2023 09:53:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:761ebd2058697796f2f98019cecedb81ef33759e6c1ec5a428e5bfcc3fe17d92`  
		Last Modified: Sat, 17 Jun 2023 10:02:12 GMT  
		Size: 26.2 MB (26245344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36084a86fb1b20f414b56d87cfcfa6dbc269df581ae9079da63a5c20f292984`  
		Last Modified: Sat, 17 Jun 2023 10:02:10 GMT  
		Size: 14.0 MB (14005266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:lunar-scm`

```console
$ docker pull buildpack-deps@sha256:dbba68715899748e496e12c3807632c13e05ffd80b651787b7c5154d77340eb9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:lunar-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:41592dd1e67dbffba26634f00619f5da6af28bfaefed9cf9475afdaa03acbf6c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.7 MB (85728568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37fba109e84f956fa8db5ad6c4f1d621aa0184f493c6f92c176ecf3b10843533`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:28:38 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:28:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:28:38 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:28:38 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:28:39 GMT
ADD file:708314051e878a0c6071fb2c8d4458a04ce058f47f2cfaa58c1b5a42e837ca0f in / 
# Thu, 15 Jun 2023 08:28:40 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:47:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:48:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ccc37bca66e7c29e0d65a4279511fe9a93932a4bb80e79e95144f3812632b61a`  
		Last Modified: Fri, 16 Jun 2023 01:56:54 GMT  
		Size: 27.6 MB (27612943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7beeb5a79f9bd13c90ee4c9f68636fc642df773adb1bd04e27e2115f6c12a6d`  
		Last Modified: Fri, 16 Jun 2023 01:56:52 GMT  
		Size: 13.7 MB (13744092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a98e278987c0da01adb1f6145dec78bd526ecc11c227e2e74c48de9cd72c40`  
		Last Modified: Fri, 16 Jun 2023 01:57:09 GMT  
		Size: 44.4 MB (44371533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:5a6012c64abe5a1e4977712e462e6802d4c5e7a02f2030a15e71b72ff3dfe57a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.7 MB (86748441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23973e09ff69a4949c38d23ac559b76967b561c2e71a9c4d1998f800fc603a88`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:10:50 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:10:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:10:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:10:51 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:10:53 GMT
ADD file:8484efc06b5f22d170eef374f45df452d8e36f4cbef702f7ee4d1f130dd28093 in / 
# Thu, 15 Jun 2023 08:10:53 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 00:49:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 00:50:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ca5128fe76949cc104af7f40ce0f7213fe093079077d47dd525fa0189090c57e`  
		Last Modified: Fri, 16 Jun 2023 00:59:51 GMT  
		Size: 25.4 MB (25432780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d8ca764d56bdf14c46fabd5c4e2e988ce166d01c8c0631d7c345802ace7bf1`  
		Last Modified: Fri, 16 Jun 2023 00:59:50 GMT  
		Size: 12.7 MB (12662932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b3e8b607724476a55e2e23faa2859f1e37c17323d12df2f9b87de3745b98e3`  
		Last Modified: Fri, 16 Jun 2023 01:00:07 GMT  
		Size: 48.7 MB (48652729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f4b6f4db12ef63968941c8377fa0e0c0bcee84d18bdd0a12614b41b634f32314
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.6 MB (84580504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14bbc99976613f7010bfbffe01cff6a9c09074f1d54233d81f2928fa1eb6bfa6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:33:24 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:33:25 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:33:25 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:33:25 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:33:58 GMT
ADD file:064ac1f238394a53372e0db107e28835aa3c39ed189a15fe85c532bbb50bfbaf in / 
# Thu, 15 Jun 2023 08:33:59 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:25:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:25:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fc6a8da5865fc488969148ca6c503307bba4023ecc0cdceaaae76a8b9852f031`  
		Last Modified: Fri, 16 Jun 2023 02:35:25 GMT  
		Size: 27.0 MB (27029986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8dde3bba356efbb171daed99ec516dc5c5c9a9b19d538fcb9fd0031bd92403a`  
		Last Modified: Fri, 16 Jun 2023 02:35:22 GMT  
		Size: 13.3 MB (13333143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a9f35a1267eac739bb82daa33daa3a21960fb88acbc2177a8156f23b857239`  
		Last Modified: Fri, 16 Jun 2023 02:35:38 GMT  
		Size: 44.2 MB (44217375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:c5a83ab3770b99e11c2b4445afb7ee1d926562a534194746e3288c6e0f2fc9b6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.9 MB (96926153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c299a6b52971b8d036a8ccadd60c639e7831b2c4f677f2882df75e523a441b7f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:29:14 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:29:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:29:15 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:29:15 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:29:17 GMT
ADD file:5ebdf4bd4bc2b27019f20fb1964a395fa504d4f20e208c54237e363895b492d7 in / 
# Thu, 15 Jun 2023 08:29:18 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:11:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:12:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a58a0b662b0d4d5e271c7c17f35795b5782a33c69a079e473f7c2303bee50024`  
		Last Modified: Fri, 16 Jun 2023 01:28:52 GMT  
		Size: 32.0 MB (32010412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6f165de89ef5a3a93777200dd180f02a8fc30051f7eb6267300a3e6f27ae1e`  
		Last Modified: Fri, 16 Jun 2023 01:28:48 GMT  
		Size: 15.8 MB (15841962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06312954ebad2b0995222a924fae1923e9b3c87aa73ff14beea981d9235b706d`  
		Last Modified: Fri, 16 Jun 2023 01:29:15 GMT  
		Size: 49.1 MB (49073779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:1b75cd39b4b8028add596e3133c70e142effd651127b61c8b4819a154a3f6eb4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84499950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dbb05763b63f79a573454ce88736b2c772cce3080193c277b1e194c26f5597d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 15 Jun 2023 08:11:16 GMT
ARG RELEASE
# Thu, 15 Jun 2023 08:11:16 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 15 Jun 2023 08:11:16 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 15 Jun 2023 08:11:16 GMT
LABEL org.opencontainers.image.version=23.04
# Thu, 15 Jun 2023 08:11:18 GMT
ADD file:3974fe053080180d99954042c25b3bd0c82e320fb4521b197cbc45f21885fc43 in / 
# Thu, 15 Jun 2023 08:11:18 GMT
CMD ["/bin/bash"]
# Sat, 17 Jun 2023 09:53:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 17 Jun 2023 09:54:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:761ebd2058697796f2f98019cecedb81ef33759e6c1ec5a428e5bfcc3fe17d92`  
		Last Modified: Sat, 17 Jun 2023 10:02:12 GMT  
		Size: 26.2 MB (26245344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a36084a86fb1b20f414b56d87cfcfa6dbc269df581ae9079da63a5c20f292984`  
		Last Modified: Sat, 17 Jun 2023 10:02:10 GMT  
		Size: 14.0 MB (14005266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a9be9d6364c4e6a0cc7388e754f4dea89849b8149102ccc37c8849f51879091`  
		Last Modified: Sat, 17 Jun 2023 10:02:24 GMT  
		Size: 44.2 MB (44249340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:mantic`

```console
$ docker pull buildpack-deps@sha256:0d94fcf7307ea7e5a21706c746b9eadb0372e5c4404d58c4066a76168bbc25c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:mantic` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:43bbe0dfe0048d31bb7cd9b7eb2b7881843a4f0a1ae20c10932f9f681d30c2ad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **264.0 MB (263967050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e86264f55ba5f4c343180d74c070d50549aea1e1f79057cd46e6a1d208a21be2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jul 2023 04:50:42 GMT
ARG RELEASE
# Wed, 12 Jul 2023 04:50:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 12 Jul 2023 04:50:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 12 Jul 2023 04:50:42 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 12 Jul 2023 04:50:44 GMT
ADD file:592c8f21973a80f096ca38aaf5ef478d80f666517a169bc638ebb325f5ae07f4 in / 
# Wed, 12 Jul 2023 04:50:44 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 01:45:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 18 Jul 2023 01:45:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 18 Jul 2023 01:48:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c57e6f7e53eccd34261640d6f245ad38a4ff7cc54ead279536b568d836363ae4`  
		Last Modified: Tue, 18 Jul 2023 01:49:46 GMT  
		Size: 27.8 MB (27758391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70262639a4fd505c867f716c40dd85135752950cc1aa365725b9e2967d66175a`  
		Last Modified: Tue, 18 Jul 2023 01:49:45 GMT  
		Size: 13.8 MB (13781000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade5aed8da7a4eb9b7d6f71f11a953d3491588e96cb6cd244876de5a69a96cea`  
		Last Modified: Tue, 18 Jul 2023 01:50:01 GMT  
		Size: 44.8 MB (44782483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bedca93e8e17ebc5f9ebd2b628460a33677641af0f83f30ebc916656b90372b7`  
		Last Modified: Tue, 18 Jul 2023 01:50:32 GMT  
		Size: 177.6 MB (177645176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:75f07b3d147e57addbeb6d779210d315e133163c662e7ad5c3f627da87d67f6a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.2 MB (229226030 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e26b4bf7025f6e10a390f74b97289b98d233bbafe98ba0d78b0f9264885de7ef`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jul 2023 04:54:17 GMT
ARG RELEASE
# Wed, 12 Jul 2023 04:54:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 12 Jul 2023 04:54:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 12 Jul 2023 04:54:17 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 12 Jul 2023 04:54:20 GMT
ADD file:6f71de5b8467fdcd7bcf88fbae117a520f903a91b00a674bdf8d44b14141f0d6 in / 
# Wed, 12 Jul 2023 04:54:20 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 04:39:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 18 Jul 2023 04:40:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 18 Jul 2023 04:43:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2d27378af227ba4634a3837d7cb24660c6d297228e3b3a59b569c67e86c1b702`  
		Last Modified: Tue, 18 Jul 2023 04:44:33 GMT  
		Size: 25.3 MB (25310196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c20ac942533d1efa51f9b7223514a74aa29ec7a0272a22f2f548636534fd3f`  
		Last Modified: Tue, 18 Jul 2023 04:44:32 GMT  
		Size: 12.7 MB (12697617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5550cb2b09d3bf2b56d01eee2a5d36ef7263a4f3b0d35f84ebe938e6f64ab689`  
		Last Modified: Tue, 18 Jul 2023 04:44:49 GMT  
		Size: 48.9 MB (48925628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e4833443a839e8ecc3c01096f5d85e9929c462a37f44010dcb41b46f6d73997`  
		Last Modified: Tue, 18 Jul 2023 04:45:17 GMT  
		Size: 142.3 MB (142292589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:2da519cc285d20321e77743bbe70ee727c2e6136b31cc3d2e07206ff2bcbbed2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.1 MB (255105368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05cec95d34923cff89a08436ace6f42700083d0033510ee441a90175265c3c4d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jul 2023 04:54:30 GMT
ARG RELEASE
# Wed, 12 Jul 2023 04:54:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 12 Jul 2023 04:54:31 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 12 Jul 2023 04:54:31 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 12 Jul 2023 04:54:38 GMT
ADD file:6eb08bb754e74bd297a54d5c56c7622fe3945c0e013d8a48b8d85b09f1818099 in / 
# Wed, 12 Jul 2023 04:54:39 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 01:46:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 18 Jul 2023 01:46:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 18 Jul 2023 01:50:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4f4369a81c2a2103bb37c89ff5ddb71caf0eefa6abc6ace3a6312b114b1b43f4`  
		Last Modified: Tue, 18 Jul 2023 01:51:33 GMT  
		Size: 27.1 MB (27116407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9605105b68496ddcb5871d9313b51b49ff984efaf7993f0d2e84539e1fd35b1d`  
		Last Modified: Tue, 18 Jul 2023 01:51:32 GMT  
		Size: 13.4 MB (13364288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7138fb2464b9037662e225fd640c60489c9bdfc93091ead842a55da631876df`  
		Last Modified: Tue, 18 Jul 2023 01:51:47 GMT  
		Size: 44.6 MB (44635979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccd9871927ef7cdded88c78380cff871c2321f9c0cade58af992c42da7a5b2c2`  
		Last Modified: Tue, 18 Jul 2023 01:52:13 GMT  
		Size: 170.0 MB (169988694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:1de851cd70a72ad80a5228ded09e8cd462ad2d158016d2ce9dbeab4d893aa1bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.0 MB (280978333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe3d22a2e38ab71f55edaa8bbafd38fd543dd9e87f837b4ee7be3a7d1b1ad1d1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jul 2023 04:53:28 GMT
ARG RELEASE
# Wed, 12 Jul 2023 04:53:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 12 Jul 2023 04:53:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 12 Jul 2023 04:53:28 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 12 Jul 2023 04:53:31 GMT
ADD file:7028e8b5bb04424a3fa537fa5b5a311cfcaf1c8b6f321b414b40ee0388d0f9e0 in / 
# Wed, 12 Jul 2023 04:53:31 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 01:52:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 18 Jul 2023 01:54:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 18 Jul 2023 01:59:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:eaefff58e8d715237ca48dbc24624ab97d73780134b6abfa9397a3fb107c7847`  
		Last Modified: Tue, 18 Jul 2023 02:02:03 GMT  
		Size: 32.0 MB (31995451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3142716ff35072c411419b141a83ce524bc1af91e86195277f4ca49673988b19`  
		Last Modified: Tue, 18 Jul 2023 02:01:59 GMT  
		Size: 15.9 MB (15880046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5986d60cc2d030634cd4d91824fd3926b4c50f5ff1bed4d038671c930e6dc5`  
		Last Modified: Tue, 18 Jul 2023 02:02:28 GMT  
		Size: 49.5 MB (49515259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565b0450a909c066455134dae59757cfb34c74497dcca3ded5fe9ca1a48c2718`  
		Last Modified: Tue, 18 Jul 2023 02:03:24 GMT  
		Size: 183.6 MB (183587577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:dde2f5b122c8c8e28653492c1d584028f22faca03ae20b746adf4f7def78e451
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.6 MB (237599006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bd06b65dfe50e847e71a12fc051aa3777176303bb94a4fac7c14a3ca594bca1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jul 2023 04:53:32 GMT
ARG RELEASE
# Wed, 12 Jul 2023 04:53:32 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 12 Jul 2023 04:53:32 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 12 Jul 2023 04:53:32 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 12 Jul 2023 04:53:34 GMT
ADD file:878995fa3a12c9df0a99fc88605932ffefec3e772a3c4ca89fe0c0aaa7dee67d in / 
# Wed, 12 Jul 2023 04:53:34 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 01:13:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 18 Jul 2023 01:14:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 18 Jul 2023 01:16:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f2b8f6b9cb3947ae25987d6e3685dc9709178b596bd7bf0d7a84ceeba23a2073`  
		Last Modified: Tue, 18 Jul 2023 01:18:14 GMT  
		Size: 26.3 MB (26322139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b736a5889ac0138557b62eaa679858540efdff47fa4079b2d261d5d981a0b7`  
		Last Modified: Tue, 18 Jul 2023 01:18:13 GMT  
		Size: 14.0 MB (14037874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15d33eaf6ee65a8ded43a590675151bb6e283880b75995e7651a1b22700ecbe`  
		Last Modified: Tue, 18 Jul 2023 01:18:27 GMT  
		Size: 44.6 MB (44645792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:919012de24272d20e9cbb02ecdc2d11a6e2b3b30cd97c260c7b0ed02524b0b5d`  
		Last Modified: Tue, 18 Jul 2023 01:18:53 GMT  
		Size: 152.6 MB (152593201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:mantic-curl`

```console
$ docker pull buildpack-deps@sha256:0e4442494d1c195e5e6f434eb92c3ce0973a9b5703677da131bdac3854a1e256
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:mantic-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:67c5c72393daaa311813c147c29b11e206a74eaa529bedf9f39eb69ba579bf1e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.5 MB (41539391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:600cfbf723eb7c8bf4ce8d3f5a932754804867c8248e234b61709d417cfb2fa3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jul 2023 04:50:42 GMT
ARG RELEASE
# Wed, 12 Jul 2023 04:50:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 12 Jul 2023 04:50:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 12 Jul 2023 04:50:42 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 12 Jul 2023 04:50:44 GMT
ADD file:592c8f21973a80f096ca38aaf5ef478d80f666517a169bc638ebb325f5ae07f4 in / 
# Wed, 12 Jul 2023 04:50:44 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 01:45:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c57e6f7e53eccd34261640d6f245ad38a4ff7cc54ead279536b568d836363ae4`  
		Last Modified: Tue, 18 Jul 2023 01:49:46 GMT  
		Size: 27.8 MB (27758391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70262639a4fd505c867f716c40dd85135752950cc1aa365725b9e2967d66175a`  
		Last Modified: Tue, 18 Jul 2023 01:49:45 GMT  
		Size: 13.8 MB (13781000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:6f2765db9a30168dd4cd5bf233b36740ba02c8d21fcfbeab4455b971e0904e9f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (38007813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:407a9cce53487e562629cd48d377253d36b1f0c25d4a1e623d536ae203544f16`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jul 2023 04:54:17 GMT
ARG RELEASE
# Wed, 12 Jul 2023 04:54:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 12 Jul 2023 04:54:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 12 Jul 2023 04:54:17 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 12 Jul 2023 04:54:20 GMT
ADD file:6f71de5b8467fdcd7bcf88fbae117a520f903a91b00a674bdf8d44b14141f0d6 in / 
# Wed, 12 Jul 2023 04:54:20 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 04:39:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2d27378af227ba4634a3837d7cb24660c6d297228e3b3a59b569c67e86c1b702`  
		Last Modified: Tue, 18 Jul 2023 04:44:33 GMT  
		Size: 25.3 MB (25310196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c20ac942533d1efa51f9b7223514a74aa29ec7a0272a22f2f548636534fd3f`  
		Last Modified: Tue, 18 Jul 2023 04:44:32 GMT  
		Size: 12.7 MB (12697617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:10bb9957c553ac1c04cab432f23e71fd04ef05d3f508e6d3dbd79575f22c2155
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.5 MB (40480695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24c82d9a81946878d92e5085da84d06a6e9a112da2626ae0b6e6b6f5b163b5eb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jul 2023 04:54:30 GMT
ARG RELEASE
# Wed, 12 Jul 2023 04:54:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 12 Jul 2023 04:54:31 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 12 Jul 2023 04:54:31 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 12 Jul 2023 04:54:38 GMT
ADD file:6eb08bb754e74bd297a54d5c56c7622fe3945c0e013d8a48b8d85b09f1818099 in / 
# Wed, 12 Jul 2023 04:54:39 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 01:46:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4f4369a81c2a2103bb37c89ff5ddb71caf0eefa6abc6ace3a6312b114b1b43f4`  
		Last Modified: Tue, 18 Jul 2023 01:51:33 GMT  
		Size: 27.1 MB (27116407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9605105b68496ddcb5871d9313b51b49ff984efaf7993f0d2e84539e1fd35b1d`  
		Last Modified: Tue, 18 Jul 2023 01:51:32 GMT  
		Size: 13.4 MB (13364288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:421ccc57b89ad1944922fa394d2470b2be35a62b46beb5fa6f1f41f2c55d9fd8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47875497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ae0c1a5f5ac2b746df491ff907a5d5dac297aa1dd8f05331e7fad11dcddb89e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jul 2023 04:53:28 GMT
ARG RELEASE
# Wed, 12 Jul 2023 04:53:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 12 Jul 2023 04:53:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 12 Jul 2023 04:53:28 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 12 Jul 2023 04:53:31 GMT
ADD file:7028e8b5bb04424a3fa537fa5b5a311cfcaf1c8b6f321b414b40ee0388d0f9e0 in / 
# Wed, 12 Jul 2023 04:53:31 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 01:52:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:eaefff58e8d715237ca48dbc24624ab97d73780134b6abfa9397a3fb107c7847`  
		Last Modified: Tue, 18 Jul 2023 02:02:03 GMT  
		Size: 32.0 MB (31995451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3142716ff35072c411419b141a83ce524bc1af91e86195277f4ca49673988b19`  
		Last Modified: Tue, 18 Jul 2023 02:01:59 GMT  
		Size: 15.9 MB (15880046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:cc5d376a0d42b93c0b1aeb249929f492d1f04f9657bab633903b45c4d26539bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.4 MB (40360013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fb0b4528866fd72155a4910ab9744bcddf0bde069e7a9dba2084fe2d14eceb5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jul 2023 04:53:32 GMT
ARG RELEASE
# Wed, 12 Jul 2023 04:53:32 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 12 Jul 2023 04:53:32 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 12 Jul 2023 04:53:32 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 12 Jul 2023 04:53:34 GMT
ADD file:878995fa3a12c9df0a99fc88605932ffefec3e772a3c4ca89fe0c0aaa7dee67d in / 
# Wed, 12 Jul 2023 04:53:34 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 01:13:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f2b8f6b9cb3947ae25987d6e3685dc9709178b596bd7bf0d7a84ceeba23a2073`  
		Last Modified: Tue, 18 Jul 2023 01:18:14 GMT  
		Size: 26.3 MB (26322139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b736a5889ac0138557b62eaa679858540efdff47fa4079b2d261d5d981a0b7`  
		Last Modified: Tue, 18 Jul 2023 01:18:13 GMT  
		Size: 14.0 MB (14037874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:mantic-scm`

```console
$ docker pull buildpack-deps@sha256:6c84d5e0d47c58b2445b5df09de7e631d683929173e54ff24016b5de4f3a16e0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:mantic-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:85d72857fea95aeb6d112513da095e1878f6e1efa45f440f9dcdee9d9a0b5370
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.3 MB (86321874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af7b8afe3427bf251dbae8dba5b9d858cdb087aeed3dc518427671aa5aea9ea4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jul 2023 04:50:42 GMT
ARG RELEASE
# Wed, 12 Jul 2023 04:50:42 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 12 Jul 2023 04:50:42 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 12 Jul 2023 04:50:42 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 12 Jul 2023 04:50:44 GMT
ADD file:592c8f21973a80f096ca38aaf5ef478d80f666517a169bc638ebb325f5ae07f4 in / 
# Wed, 12 Jul 2023 04:50:44 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 01:45:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 18 Jul 2023 01:45:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c57e6f7e53eccd34261640d6f245ad38a4ff7cc54ead279536b568d836363ae4`  
		Last Modified: Tue, 18 Jul 2023 01:49:46 GMT  
		Size: 27.8 MB (27758391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70262639a4fd505c867f716c40dd85135752950cc1aa365725b9e2967d66175a`  
		Last Modified: Tue, 18 Jul 2023 01:49:45 GMT  
		Size: 13.8 MB (13781000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade5aed8da7a4eb9b7d6f71f11a953d3491588e96cb6cd244876de5a69a96cea`  
		Last Modified: Tue, 18 Jul 2023 01:50:01 GMT  
		Size: 44.8 MB (44782483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:3b16df0cdce33f0ee6279409ac982bdb50248ac00be43888721544867e49c77c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.9 MB (86933441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21da3ba7664b82a047c70a8e69802637f613f60612974e0f52c505163dcdb1be`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jul 2023 04:54:17 GMT
ARG RELEASE
# Wed, 12 Jul 2023 04:54:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 12 Jul 2023 04:54:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 12 Jul 2023 04:54:17 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 12 Jul 2023 04:54:20 GMT
ADD file:6f71de5b8467fdcd7bcf88fbae117a520f903a91b00a674bdf8d44b14141f0d6 in / 
# Wed, 12 Jul 2023 04:54:20 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 04:39:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 18 Jul 2023 04:40:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2d27378af227ba4634a3837d7cb24660c6d297228e3b3a59b569c67e86c1b702`  
		Last Modified: Tue, 18 Jul 2023 04:44:33 GMT  
		Size: 25.3 MB (25310196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c20ac942533d1efa51f9b7223514a74aa29ec7a0272a22f2f548636534fd3f`  
		Last Modified: Tue, 18 Jul 2023 04:44:32 GMT  
		Size: 12.7 MB (12697617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5550cb2b09d3bf2b56d01eee2a5d36ef7263a4f3b0d35f84ebe938e6f64ab689`  
		Last Modified: Tue, 18 Jul 2023 04:44:49 GMT  
		Size: 48.9 MB (48925628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:29540c8fb7fe2cbff1c5b2ebbe79377102298bb93e3176b97416e36008ebef3d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.1 MB (85116674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f2d4533597e76b8d10fc71998896d25f47ab73decd47de07630f4cbb9c0e52e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jul 2023 04:54:30 GMT
ARG RELEASE
# Wed, 12 Jul 2023 04:54:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 12 Jul 2023 04:54:31 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 12 Jul 2023 04:54:31 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 12 Jul 2023 04:54:38 GMT
ADD file:6eb08bb754e74bd297a54d5c56c7622fe3945c0e013d8a48b8d85b09f1818099 in / 
# Wed, 12 Jul 2023 04:54:39 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 01:46:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 18 Jul 2023 01:46:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4f4369a81c2a2103bb37c89ff5ddb71caf0eefa6abc6ace3a6312b114b1b43f4`  
		Last Modified: Tue, 18 Jul 2023 01:51:33 GMT  
		Size: 27.1 MB (27116407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9605105b68496ddcb5871d9313b51b49ff984efaf7993f0d2e84539e1fd35b1d`  
		Last Modified: Tue, 18 Jul 2023 01:51:32 GMT  
		Size: 13.4 MB (13364288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7138fb2464b9037662e225fd640c60489c9bdfc93091ead842a55da631876df`  
		Last Modified: Tue, 18 Jul 2023 01:51:47 GMT  
		Size: 44.6 MB (44635979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:5427d53e2a0f36be11ddee624b8c2282efb28ea974220e842386fef4566bb3ce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.4 MB (97390756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1490ac353d73761f55f94aaa4b8e908f4e3c1ecdff0aeef98c7eb21967229e66`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jul 2023 04:53:28 GMT
ARG RELEASE
# Wed, 12 Jul 2023 04:53:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 12 Jul 2023 04:53:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 12 Jul 2023 04:53:28 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 12 Jul 2023 04:53:31 GMT
ADD file:7028e8b5bb04424a3fa537fa5b5a311cfcaf1c8b6f321b414b40ee0388d0f9e0 in / 
# Wed, 12 Jul 2023 04:53:31 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 01:52:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 18 Jul 2023 01:54:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:eaefff58e8d715237ca48dbc24624ab97d73780134b6abfa9397a3fb107c7847`  
		Last Modified: Tue, 18 Jul 2023 02:02:03 GMT  
		Size: 32.0 MB (31995451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3142716ff35072c411419b141a83ce524bc1af91e86195277f4ca49673988b19`  
		Last Modified: Tue, 18 Jul 2023 02:01:59 GMT  
		Size: 15.9 MB (15880046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5986d60cc2d030634cd4d91824fd3926b4c50f5ff1bed4d038671c930e6dc5`  
		Last Modified: Tue, 18 Jul 2023 02:02:28 GMT  
		Size: 49.5 MB (49515259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:0701a87a39ba7a5b13f5af26dd438551eae62de80cfb8e120b20da4016b92148
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.0 MB (85005805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c8e32e1c8a0607953bad4aa48adfe5b58e9641c89ddaa7c104660b0848cd95d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 12 Jul 2023 04:53:32 GMT
ARG RELEASE
# Wed, 12 Jul 2023 04:53:32 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 12 Jul 2023 04:53:32 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 12 Jul 2023 04:53:32 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 12 Jul 2023 04:53:34 GMT
ADD file:878995fa3a12c9df0a99fc88605932ffefec3e772a3c4ca89fe0c0aaa7dee67d in / 
# Wed, 12 Jul 2023 04:53:34 GMT
CMD ["/bin/bash"]
# Tue, 18 Jul 2023 01:13:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 18 Jul 2023 01:14:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f2b8f6b9cb3947ae25987d6e3685dc9709178b596bd7bf0d7a84ceeba23a2073`  
		Last Modified: Tue, 18 Jul 2023 01:18:14 GMT  
		Size: 26.3 MB (26322139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b736a5889ac0138557b62eaa679858540efdff47fa4079b2d261d5d981a0b7`  
		Last Modified: Tue, 18 Jul 2023 01:18:13 GMT  
		Size: 14.0 MB (14037874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d15d33eaf6ee65a8ded43a590675151bb6e283880b75995e7651a1b22700ecbe`  
		Last Modified: Tue, 18 Jul 2023 01:18:27 GMT  
		Size: 44.6 MB (44645792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldoldstable`

```console
$ docker pull buildpack-deps@sha256:93d76989e9b0ebdfe9b96e96095ea6f87c710ecd01b66ce85418232c7af430c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:oldoldstable` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:fc6853c85c895526dc95b4774269365f5b600c184d2fd944b3181c58f4939e16
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.8 MB (311781265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7eb882719b28e6bbddb691ea7cbc3679551f1b68715fe48e477afa5d82c87afe`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:34 GMT
ADD file:2fa5242038736e48eaca794d061079c1cbd32fcc4336250001523c41b3177276 in / 
# Tue, 04 Jul 2023 01:20:35 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:32:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:32:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:33:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8eb6dba554cffc072c7a6c696c8a23fc311e543399d84ab3ebc55c07ab54414f`  
		Last Modified: Tue, 04 Jul 2023 01:26:01 GMT  
		Size: 50.4 MB (50448743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e4f798b8796023ecee944e089e79871ca261eedc4a2ee6a38b08418d9160f4`  
		Last Modified: Tue, 04 Jul 2023 03:53:27 GMT  
		Size: 17.6 MB (17579065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90cef27337073d2443e1c3dd4305cf98d70eadb31c10c267225d9639f1cd6de4`  
		Last Modified: Tue, 04 Jul 2023 03:53:43 GMT  
		Size: 51.9 MB (51870872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f89e257e0550870d02769e068a247cf3612acbb737425f707be9ea0d763772`  
		Last Modified: Tue, 04 Jul 2023 03:54:13 GMT  
		Size: 191.9 MB (191882585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:60f28694428765623be4e2f4c523c350281fa20a0eeabf003c9287ff63a16c27
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.6 MB (277592160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e810e54890f1fef5a1546e57ca582e7f104597aae4dd54a08edd435f2ed8c80`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:31 GMT
ADD file:e1c7c10335e2ac86eba02c2785d0ff530cba87131e91c42924072b4010418f93 in / 
# Tue, 04 Jul 2023 00:58:32 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:54:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:54:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:56:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b19cf971d5ed51e0bba0bd71ccd7b797ad4873a62fee0f49588f6ef19a58e659`  
		Last Modified: Tue, 04 Jul 2023 01:03:55 GMT  
		Size: 45.9 MB (45916488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de49cbcb6a4fd553472f2cf39947eef7d00374517274e95f1a822bfb3c8e2cb`  
		Last Modified: Tue, 04 Jul 2023 06:20:51 GMT  
		Size: 16.2 MB (16211416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:551952269cb797c2c924c3af99a03099c86099cd8186bdda487b965d4f08fff3`  
		Last Modified: Tue, 04 Jul 2023 06:21:10 GMT  
		Size: 47.4 MB (47369644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e84c841d1296aa856601262d7c4425787f09dfce1122d08b3b7ecf5b44a8a54e`  
		Last Modified: Tue, 04 Jul 2023 06:21:39 GMT  
		Size: 168.1 MB (168094612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:50b0cc42de9ec56d6d75b59f66665fbc6b800e29417804bdf18a1a60516a8362
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.4 MB (302372380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c378a277c6ab107528bb171956861a01656482088765346902a30334b4b322af`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:59 GMT
ADD file:a61276f534601d7b193af24e35c16b73a2913511d2b1ad997c9a8cb907685257 in / 
# Tue, 04 Jul 2023 01:58:00 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:58:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:58:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:00:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5e2555ae6edde2e7933c533234cb224b6d7ef3a3c90041851e31fe29ab7197c9`  
		Last Modified: Tue, 04 Jul 2023 02:02:18 GMT  
		Size: 49.2 MB (49238644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503bef164a5c225a74d09ad3b129d3bff71bea2ad1fb291b63c6d342493b62ba`  
		Last Modified: Tue, 04 Jul 2023 06:22:50 GMT  
		Size: 17.5 MB (17450024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3816d11f9d5d9a3bb643dd5c7291e610012ec9eef9c769ce5f6107abdf1eb6d`  
		Last Modified: Tue, 04 Jul 2023 06:23:05 GMT  
		Size: 52.2 MB (52217244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:456c8535b3af918c9b8d87c98c4d7bc631d833d1ebb4d816aefbf356372983c6`  
		Last Modified: Tue, 04 Jul 2023 06:23:29 GMT  
		Size: 183.5 MB (183466468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:0724af2107e33683fda67b85f730eb15e5087c5dcbfd73f7af46fa0c214deacc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.2 MB (321213990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9216ef434e3e7d93b84a05352e7de2c89cbadb8aa2ba1ff22f364785c53e5d1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:39:11 GMT
ADD file:6ecab94f7cb2bc0740a669cfef73f0837a2ecf6475dfb0fc072cbd1a7f60ec41 in / 
# Tue, 04 Jul 2023 01:39:11 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:33:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:34:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:36:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b3c3fd2dd1697ce9fed8a2be0142b2d1294d424c56d0ce6d44bb8055d77e35d`  
		Last Modified: Tue, 04 Jul 2023 01:44:33 GMT  
		Size: 51.2 MB (51206276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a0e83aa5cadecbd9663b4464fa33665e930f60918a3178f75983604fc64d38`  
		Last Modified: Tue, 04 Jul 2023 05:40:47 GMT  
		Size: 18.1 MB (18095483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88eede3a0f204f9d3d5eae24a7e5f5ddd9f533ad476bf4e77ee81a22bdb07f9a`  
		Last Modified: Tue, 04 Jul 2023 05:41:07 GMT  
		Size: 53.5 MB (53485728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d9ed1e05da0b79a86d6ca58ac78d81fd2bc66fa7ea1b33566e0aa62fc445f9`  
		Last Modified: Tue, 04 Jul 2023 05:41:49 GMT  
		Size: 198.4 MB (198426503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldoldstable-curl`

```console
$ docker pull buildpack-deps@sha256:9e90f92d4d4c4cc756adc20a63ed7cd3bcd4e2c58723c10a449484b8ff6aceea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:oldoldstable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:b9a6fa925c3754fad97e1e096b2107d8809a8c2786947ea28ebca51ee9791bc7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.0 MB (68027808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fba93f010c9f896ebc93161f6655c1b59d288182d9e9e6d2e1bbecc0f8c94e4f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:34 GMT
ADD file:2fa5242038736e48eaca794d061079c1cbd32fcc4336250001523c41b3177276 in / 
# Tue, 04 Jul 2023 01:20:35 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:32:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8eb6dba554cffc072c7a6c696c8a23fc311e543399d84ab3ebc55c07ab54414f`  
		Last Modified: Tue, 04 Jul 2023 01:26:01 GMT  
		Size: 50.4 MB (50448743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e4f798b8796023ecee944e089e79871ca261eedc4a2ee6a38b08418d9160f4`  
		Last Modified: Tue, 04 Jul 2023 03:53:27 GMT  
		Size: 17.6 MB (17579065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:afa7a1bada87fb5441651d43e1b4349bd9cc466f0622739367455cd376a740b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.1 MB (62127904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68f107e1a900a7b124105c82ffff25b2a060dee6cff73cdec89337f4a23449b9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:31 GMT
ADD file:e1c7c10335e2ac86eba02c2785d0ff530cba87131e91c42924072b4010418f93 in / 
# Tue, 04 Jul 2023 00:58:32 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:54:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b19cf971d5ed51e0bba0bd71ccd7b797ad4873a62fee0f49588f6ef19a58e659`  
		Last Modified: Tue, 04 Jul 2023 01:03:55 GMT  
		Size: 45.9 MB (45916488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de49cbcb6a4fd553472f2cf39947eef7d00374517274e95f1a822bfb3c8e2cb`  
		Last Modified: Tue, 04 Jul 2023 06:20:51 GMT  
		Size: 16.2 MB (16211416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:80e630bea99e712a913b713c63ff3adf1eacb86af6629feb11b0e0227ca80219
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66688668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdad1a1cc278d9d35c38b92f4d110b39952f68f5271c652b7ad103623ae9c8de`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:59 GMT
ADD file:a61276f534601d7b193af24e35c16b73a2913511d2b1ad997c9a8cb907685257 in / 
# Tue, 04 Jul 2023 01:58:00 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:58:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5e2555ae6edde2e7933c533234cb224b6d7ef3a3c90041851e31fe29ab7197c9`  
		Last Modified: Tue, 04 Jul 2023 02:02:18 GMT  
		Size: 49.2 MB (49238644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503bef164a5c225a74d09ad3b129d3bff71bea2ad1fb291b63c6d342493b62ba`  
		Last Modified: Tue, 04 Jul 2023 06:22:50 GMT  
		Size: 17.5 MB (17450024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:31a0d9c686cbc2328cd57c3363515049f391593d8dc552dea36b5acd6aadd135
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.3 MB (69301759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:553a8774245bf544e4a5813eb3fc8b73b523c6ce15b6d5278ded782d365eab85`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:39:11 GMT
ADD file:6ecab94f7cb2bc0740a669cfef73f0837a2ecf6475dfb0fc072cbd1a7f60ec41 in / 
# Tue, 04 Jul 2023 01:39:11 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:33:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b3c3fd2dd1697ce9fed8a2be0142b2d1294d424c56d0ce6d44bb8055d77e35d`  
		Last Modified: Tue, 04 Jul 2023 01:44:33 GMT  
		Size: 51.2 MB (51206276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a0e83aa5cadecbd9663b4464fa33665e930f60918a3178f75983604fc64d38`  
		Last Modified: Tue, 04 Jul 2023 05:40:47 GMT  
		Size: 18.1 MB (18095483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldoldstable-scm`

```console
$ docker pull buildpack-deps@sha256:190191e3a02c364d2538051d10cf6b972bf5f388de64ee88a0cd912f98d7b294
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:oldoldstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:d3872f4bbda84746d3e023839278b5380cc83b5f2e57e27812e359cdcfec8cec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.9 MB (119898680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e42250bcc32f41abbf71048b5d3f02f09de55ed4c1502afbaef04096b190463`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:34 GMT
ADD file:2fa5242038736e48eaca794d061079c1cbd32fcc4336250001523c41b3177276 in / 
# Tue, 04 Jul 2023 01:20:35 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:32:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:32:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8eb6dba554cffc072c7a6c696c8a23fc311e543399d84ab3ebc55c07ab54414f`  
		Last Modified: Tue, 04 Jul 2023 01:26:01 GMT  
		Size: 50.4 MB (50448743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79e4f798b8796023ecee944e089e79871ca261eedc4a2ee6a38b08418d9160f4`  
		Last Modified: Tue, 04 Jul 2023 03:53:27 GMT  
		Size: 17.6 MB (17579065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90cef27337073d2443e1c3dd4305cf98d70eadb31c10c267225d9639f1cd6de4`  
		Last Modified: Tue, 04 Jul 2023 03:53:43 GMT  
		Size: 51.9 MB (51870872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1b4d9a7f073580e03ec7c8b3e0243dd260f0d9a360b5d6428cf51566261433df
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.5 MB (109497548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce83dc96a23dafaf7a58ec0f31d70b644e4715d465e1128b15d0bd604e283def`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:31 GMT
ADD file:e1c7c10335e2ac86eba02c2785d0ff530cba87131e91c42924072b4010418f93 in / 
# Tue, 04 Jul 2023 00:58:32 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:54:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:54:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b19cf971d5ed51e0bba0bd71ccd7b797ad4873a62fee0f49588f6ef19a58e659`  
		Last Modified: Tue, 04 Jul 2023 01:03:55 GMT  
		Size: 45.9 MB (45916488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de49cbcb6a4fd553472f2cf39947eef7d00374517274e95f1a822bfb3c8e2cb`  
		Last Modified: Tue, 04 Jul 2023 06:20:51 GMT  
		Size: 16.2 MB (16211416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:551952269cb797c2c924c3af99a03099c86099cd8186bdda487b965d4f08fff3`  
		Last Modified: Tue, 04 Jul 2023 06:21:10 GMT  
		Size: 47.4 MB (47369644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:042c8cbba1e5ec8945d2a178da4a4ab2a7aa52c981f75e0ff0949d2fc8422b11
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.9 MB (118905912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6568bf4370a5bad76d3890ece5e6279395b2d0ae33a68af33183174c29a61ed9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:59 GMT
ADD file:a61276f534601d7b193af24e35c16b73a2913511d2b1ad997c9a8cb907685257 in / 
# Tue, 04 Jul 2023 01:58:00 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:58:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:58:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5e2555ae6edde2e7933c533234cb224b6d7ef3a3c90041851e31fe29ab7197c9`  
		Last Modified: Tue, 04 Jul 2023 02:02:18 GMT  
		Size: 49.2 MB (49238644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503bef164a5c225a74d09ad3b129d3bff71bea2ad1fb291b63c6d342493b62ba`  
		Last Modified: Tue, 04 Jul 2023 06:22:50 GMT  
		Size: 17.5 MB (17450024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3816d11f9d5d9a3bb643dd5c7291e610012ec9eef9c769ce5f6107abdf1eb6d`  
		Last Modified: Tue, 04 Jul 2023 06:23:05 GMT  
		Size: 52.2 MB (52217244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:c8e540d022779ddb0a2e6fdb3d322469c3d320d485cf84cefb7f9dff9c5024f5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.8 MB (122787487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a44252762afe1bc6205da39e4217bfd4fda4800ee9de78325ef92703f7312a27`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:39:11 GMT
ADD file:6ecab94f7cb2bc0740a669cfef73f0837a2ecf6475dfb0fc072cbd1a7f60ec41 in / 
# Tue, 04 Jul 2023 01:39:11 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:33:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:34:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b3c3fd2dd1697ce9fed8a2be0142b2d1294d424c56d0ce6d44bb8055d77e35d`  
		Last Modified: Tue, 04 Jul 2023 01:44:33 GMT  
		Size: 51.2 MB (51206276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a0e83aa5cadecbd9663b4464fa33665e930f60918a3178f75983604fc64d38`  
		Last Modified: Tue, 04 Jul 2023 05:40:47 GMT  
		Size: 18.1 MB (18095483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88eede3a0f204f9d3d5eae24a7e5f5ddd9f533ad476bf4e77ee81a22bdb07f9a`  
		Last Modified: Tue, 04 Jul 2023 05:41:07 GMT  
		Size: 53.5 MB (53485728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldstable`

```console
$ docker pull buildpack-deps@sha256:7742ec0838b3c91afb08f8e2e3a5abc2a5379fe6f7e6c242ed4d3b472c7c5c73
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
$ docker pull buildpack-deps@sha256:d4136e8b26283648c23085988ff9320469071a6d71af1d5f5652f0d0b0129090
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.3 MB (322251560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32c83682cffffc48f1d1da4b634def742c08aa1baeb486df6bfc1668b8cd44e9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:09 GMT
ADD file:b7c0be2bb90e88689b1c16da78dea0b85760b55b90ef2e5bc4a529c89e4fa25b in / 
# Tue, 04 Jul 2023 01:20:10 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:30:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:30:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:31:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:34df401c391c7595044379e04e8ad4856a5a3974cdbf5a160f0a204d761e88aa`  
		Last Modified: Tue, 04 Jul 2023 01:25:21 GMT  
		Size: 55.1 MB (55055300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fdd0e5b72ccae203ec30d533c0bcd34200af90265e0531c66356812e529af32`  
		Last Modified: Tue, 04 Jul 2023 03:52:30 GMT  
		Size: 15.8 MB (15760327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa786a946ae67fa18e07eaf82fefee1777449f7db1a8fea5abec1aadbe99e2ef`  
		Last Modified: Tue, 04 Jul 2023 03:52:45 GMT  
		Size: 54.6 MB (54585046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f8721393bc605f2b915d80eb2ad6d5219db374f36bbd1fee99b99174a0a4ca`  
		Last Modified: Tue, 04 Jul 2023 03:53:17 GMT  
		Size: 196.9 MB (196850887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:6454d0b087354a1aa979f21afba2a5cbb8bab6b79f7acf4f0803d163c31bef27
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.3 MB (295304664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efbe088d0d18e6bb5c2e2c2eb6d78bfa4d530fb7fb8b31688c675550427d1153`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:48:39 GMT
ADD file:fe1b9f9f6c7d67ad23a2ee839774be4bcee33c60c7b34c48df5a08eb33cafd1b in / 
# Tue, 04 Jul 2023 00:48:40 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:24:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:25:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:26:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:702dd8b607f626c689176debe921fe96009c1ce6dbd66f4f238c7def50080e3d`  
		Last Modified: Tue, 04 Jul 2023 00:52:15 GMT  
		Size: 52.6 MB (52556778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec773064e3ff5287bd9be0bdb7b99e708aed435b4920a0f64aeaf158d9631f5e`  
		Last Modified: Tue, 04 Jul 2023 04:29:40 GMT  
		Size: 15.4 MB (15369118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ae2fc9256b17aac11e221f2db3d50e0543fecf87896a99ff9be68ea2335989`  
		Last Modified: Tue, 04 Jul 2023 04:29:57 GMT  
		Size: 52.3 MB (52340564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8a9d92ba07e083e1f009e2a61ce148b9c2863820ac5942c814661045a26d3b`  
		Last Modified: Tue, 04 Jul 2023 04:30:31 GMT  
		Size: 175.0 MB (175038204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:04f584cada918fac3166adc6f013bb067993f06516c6d749c8483c02842523eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.8 MB (282774067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:205c60f2f252ed7b84d5173a49821829c6238b95be89b3b23444c8c69021f8e6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:06 GMT
ADD file:17e02296458241d9441f8da6a5dafb747d528a729106b17cec2f4c1c8cfe0ad8 in / 
# Tue, 04 Jul 2023 00:58:07 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:51:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:52:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:53:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:31edf2db9ca1650aa08e2d42e9b5bb7349413d7212110149a1a5d202ac20914b`  
		Last Modified: Tue, 04 Jul 2023 01:03:12 GMT  
		Size: 50.2 MB (50218247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e794b9a6d62ad67f31927f253d3a467d402da7b96769cef6b5503fde01f18eb9`  
		Last Modified: Tue, 04 Jul 2023 06:19:48 GMT  
		Size: 14.9 MB (14868644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fdbc75406b7868979ba89f96e015c45fbcf9efe34aa3863e52c0e926531784f`  
		Last Modified: Tue, 04 Jul 2023 06:20:06 GMT  
		Size: 50.4 MB (50355287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b5420e300d967980b7a87e93da33a82950c1fb7d2024379f913ad516ac3814`  
		Last Modified: Tue, 04 Jul 2023 06:20:40 GMT  
		Size: 167.3 MB (167331889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:efad222cb293be53dd7045e6faaa4051e909d2cf1d4f82116f8260bb7b1439fa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.9 MB (313904743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e4dd2ebe3088f8dc545dfc68984603c52f4c0a5ff021ffda0c146afe58c1307`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:43 GMT
ADD file:e626446584d8094b7b58d72a717380ca64d3e9ab924fc625406fe26a83fe1d8b in / 
# Tue, 04 Jul 2023 01:57:43 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:56:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:56:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:58:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:29279ac7c19f9c667f1c6b07bfba6fba20ca0d945b9fbc6edad6f75d13361fae`  
		Last Modified: Tue, 04 Jul 2023 02:01:38 GMT  
		Size: 53.7 MB (53703979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d0c3fcc5367be60f92df0774820f317a179565cd3ee9c222f5500a7be32151e`  
		Last Modified: Tue, 04 Jul 2023 06:22:01 GMT  
		Size: 15.7 MB (15746747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5fa66dbb545c6ff93c768ac595d874b2f22053e8d2f842f4b6ccc310ebfe0c`  
		Last Modified: Tue, 04 Jul 2023 06:22:15 GMT  
		Size: 54.7 MB (54676075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790673d5b08f786a9f9e0a1db5dd3941e80d10bde172f69852e2c405b2eb3ad3`  
		Last Modified: Tue, 04 Jul 2023 06:22:40 GMT  
		Size: 189.8 MB (189777942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:3614c9ca25a1730d80fefac448488f742bf8e12204b6a018b74e7886cc1d21d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.0 MB (327993696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fdb716512bdd67e2d576da09577000f35f580c4b3edec03b1d38dfa940db50b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:38:48 GMT
ADD file:c5739407c2c257fbb85ab4b9dcd2dc07e6fe172d7309aaaaab544c8df6c42b92 in / 
# Tue, 04 Jul 2023 01:38:49 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:30:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:31:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:32:48 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b700c8b35944e0d5f6ab9049dbe2262492e26327a8efad518b1011428393653f`  
		Last Modified: Tue, 04 Jul 2023 01:43:49 GMT  
		Size: 56.0 MB (56040756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414994a3b1789f89f704fcfc0e721c0036089a74368f21aa6fafa639fef2c93b`  
		Last Modified: Tue, 04 Jul 2023 05:39:34 GMT  
		Size: 16.3 MB (16263605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ee301eb66e57dfaf79983158c75b77a7775e1b6216c45ce247c6fac3786a46`  
		Last Modified: Tue, 04 Jul 2023 05:39:53 GMT  
		Size: 55.9 MB (55922990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28c7ac3e45d13ee62a7daff4eb413a3752789ab4b5620de47a04abff3a358cc`  
		Last Modified: Tue, 04 Jul 2023 05:40:36 GMT  
		Size: 199.8 MB (199766345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:3ae9f3837f9c3b468acf4a7e4d75ffa8718eba2055611425c88d9536f671a64f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.1 MB (301070599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75f1f194f73750062c6fdf2e936746353f2db097aa555efd67dd295da04000b2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:10:02 GMT
ADD file:f7ddd7406e3aa24165fc80933583fc2298f9792865511fe65def2f571fed2207 in / 
# Tue, 04 Jul 2023 01:10:07 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:43:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:45:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:51:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:af98e96208d7ce4cff5417a3e8a38f98d2ed3abbca318e1e6c323aa8b8c56690`  
		Last Modified: Tue, 04 Jul 2023 01:20:40 GMT  
		Size: 53.3 MB (53270472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b8f3d09abba473eec10e4fe5adebd33b18a790b9e57fdd8a5b484c925486df`  
		Last Modified: Tue, 04 Jul 2023 14:59:18 GMT  
		Size: 15.5 MB (15520537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427c4e665dab89a7a9a5cef3f1bab709cd38d4945e49ef760b95611e774a07e4`  
		Last Modified: Tue, 04 Jul 2023 15:00:02 GMT  
		Size: 53.3 MB (53306638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7915d90967431c4046270617a5aa6c09863c49d6e707dd149a919875c0326ad5`  
		Last Modified: Tue, 04 Jul 2023 15:01:58 GMT  
		Size: 179.0 MB (178972952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:24871bd43939bccce8bbff3de498e9bb620b00d2e7fe4ec7f90c016b206635ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.7 MB (330742890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a240664eeabe8f3b43cc9a1797fed091713e4cc8a20e28695d70e6059d7ef0d9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:18:11 GMT
ADD file:ff86c25854c28609c2852c1615270f0acd4c4efaa38ff8ed9c23afe5132f2135 in / 
# Tue, 04 Jul 2023 01:18:15 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:33:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:33:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:37:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a792749f62225048efdf85841bea6f3999f586371852f3dbce13a6c3d89b1fa7`  
		Last Modified: Tue, 04 Jul 2023 01:25:06 GMT  
		Size: 58.9 MB (58927745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf553284aac150acedeaf1c5f33c1820a34bff4f20ef96c32510ee19f2be0e83`  
		Last Modified: Tue, 04 Jul 2023 04:38:16 GMT  
		Size: 16.8 MB (16752898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b8f1977f7b061bf5ae7311bb1750877d9ba871f041ba604c8e1e9d1e1143e0`  
		Last Modified: Tue, 04 Jul 2023 04:38:44 GMT  
		Size: 58.9 MB (58864695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17f0a018912d7d71fedea77bea42cdadad1900e4a2885ca8b28fef63c5eba62`  
		Last Modified: Tue, 04 Jul 2023 04:39:40 GMT  
		Size: 196.2 MB (196197552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:cbd11f117fe42c23beeda51c054b1ccc7c594d40032aaa5c12f43b20793fcf59
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.8 MB (295837524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3bdd4f22e56b3046868680c31e879469345a5eeb73450696c18f7db32ad93dc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:32:26 GMT
ADD file:231ba6ce8d3ee30318948799a94cb007f1517ea0d14c2b84863012cac37d6c6b in / 
# Tue, 04 Jul 2023 01:32:29 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 12:48:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 12:49:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 12:50:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1e40ed2a44a8c2786b06584afad765d97e9b1c910f58ae426622ba17fbf3d4c3`  
		Last Modified: Tue, 04 Jul 2023 01:37:21 GMT  
		Size: 53.3 MB (53288197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf2b9bfea4ac32f9de9f19ff39e147a59dc0ed209ac66dbf1f57baa75c0eef4`  
		Last Modified: Tue, 04 Jul 2023 13:06:27 GMT  
		Size: 15.6 MB (15631899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b214fc39e8a77ee2b4618f8315eee93c861d035ba1cf9dc80e62081ee3aafe`  
		Last Modified: Tue, 04 Jul 2023 13:06:41 GMT  
		Size: 54.1 MB (54061732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6049a6d30b8104f609abf0afe200e7426f7a8c80bc63e5aa5ab08fd53fb7c8`  
		Last Modified: Tue, 04 Jul 2023 13:07:07 GMT  
		Size: 172.9 MB (172855696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldstable-curl`

```console
$ docker pull buildpack-deps@sha256:8d6835a7cf657b7933e37bfbea95b89977689a0289402970e53f6159c2ef814f
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

### `buildpack-deps:oldstable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:a04a4573f1877ebb1e4f77b2a67979fba929007fe8bd66db28c1bc21daf43f4e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.8 MB (70815627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e4f8f2737713528fa70fb13a9e1d83d4f175b195bb5f51cf6a3b71f785e9728`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:09 GMT
ADD file:b7c0be2bb90e88689b1c16da78dea0b85760b55b90ef2e5bc4a529c89e4fa25b in / 
# Tue, 04 Jul 2023 01:20:10 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:30:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:34df401c391c7595044379e04e8ad4856a5a3974cdbf5a160f0a204d761e88aa`  
		Last Modified: Tue, 04 Jul 2023 01:25:21 GMT  
		Size: 55.1 MB (55055300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fdd0e5b72ccae203ec30d533c0bcd34200af90265e0531c66356812e529af32`  
		Last Modified: Tue, 04 Jul 2023 03:52:30 GMT  
		Size: 15.8 MB (15760327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:dce5b0f9173c5aa9d4cdb22f8d553f5c7ad9b4a94d5d85c5dbef212f5bc86aae
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.9 MB (67925896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f61feaa3ac7bf64852d81afe2758a2f7c2d26b61da9e46d63e4a076b2e134095`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:48:39 GMT
ADD file:fe1b9f9f6c7d67ad23a2ee839774be4bcee33c60c7b34c48df5a08eb33cafd1b in / 
# Tue, 04 Jul 2023 00:48:40 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:24:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:702dd8b607f626c689176debe921fe96009c1ce6dbd66f4f238c7def50080e3d`  
		Last Modified: Tue, 04 Jul 2023 00:52:15 GMT  
		Size: 52.6 MB (52556778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec773064e3ff5287bd9be0bdb7b99e708aed435b4920a0f64aeaf158d9631f5e`  
		Last Modified: Tue, 04 Jul 2023 04:29:40 GMT  
		Size: 15.4 MB (15369118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:a961ee8bacf953c686c47a5ce87736a96620a4bb3e0d2d52a418e3b29114b731
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.1 MB (65086891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dffd5d1f662dbe3178c41c1f68eaa712177e4531caaefb808179447f39a3b337`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:06 GMT
ADD file:17e02296458241d9441f8da6a5dafb747d528a729106b17cec2f4c1c8cfe0ad8 in / 
# Tue, 04 Jul 2023 00:58:07 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:51:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:31edf2db9ca1650aa08e2d42e9b5bb7349413d7212110149a1a5d202ac20914b`  
		Last Modified: Tue, 04 Jul 2023 01:03:12 GMT  
		Size: 50.2 MB (50218247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e794b9a6d62ad67f31927f253d3a467d402da7b96769cef6b5503fde01f18eb9`  
		Last Modified: Tue, 04 Jul 2023 06:19:48 GMT  
		Size: 14.9 MB (14868644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:2ad82791ffc18d9af62246e621344922a9ca628ff9677f6ddc2995c3b5886118
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69450726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b6b69a80b96284b4cff1f89edcb4ea8a5430691981fe120af2033b18f8299d6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:43 GMT
ADD file:e626446584d8094b7b58d72a717380ca64d3e9ab924fc625406fe26a83fe1d8b in / 
# Tue, 04 Jul 2023 01:57:43 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:56:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:29279ac7c19f9c667f1c6b07bfba6fba20ca0d945b9fbc6edad6f75d13361fae`  
		Last Modified: Tue, 04 Jul 2023 02:01:38 GMT  
		Size: 53.7 MB (53703979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d0c3fcc5367be60f92df0774820f317a179565cd3ee9c222f5500a7be32151e`  
		Last Modified: Tue, 04 Jul 2023 06:22:01 GMT  
		Size: 15.7 MB (15746747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:e0fc072a9284c49c6bf1c3efd326932b88029bd7455798f0707b4137779bfd21
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.3 MB (72304361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7725e22264581a633b08cd831a6102bb24fd7d2b9f8e9b119c0fd4425de1705`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:38:48 GMT
ADD file:c5739407c2c257fbb85ab4b9dcd2dc07e6fe172d7309aaaaab544c8df6c42b92 in / 
# Tue, 04 Jul 2023 01:38:49 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:30:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b700c8b35944e0d5f6ab9049dbe2262492e26327a8efad518b1011428393653f`  
		Last Modified: Tue, 04 Jul 2023 01:43:49 GMT  
		Size: 56.0 MB (56040756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414994a3b1789f89f704fcfc0e721c0036089a74368f21aa6fafa639fef2c93b`  
		Last Modified: Tue, 04 Jul 2023 05:39:34 GMT  
		Size: 16.3 MB (16263605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:5284334ece9a4c74628f0ea0f15b42c69f8b7a690a808e8ad24aa684901a47ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68791009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3321735b4070a6315fe3ac262e5059feb2b4dc68eb837ed8cc3f5810373f7a3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:10:02 GMT
ADD file:f7ddd7406e3aa24165fc80933583fc2298f9792865511fe65def2f571fed2207 in / 
# Tue, 04 Jul 2023 01:10:07 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:43:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:af98e96208d7ce4cff5417a3e8a38f98d2ed3abbca318e1e6c323aa8b8c56690`  
		Last Modified: Tue, 04 Jul 2023 01:20:40 GMT  
		Size: 53.3 MB (53270472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b8f3d09abba473eec10e4fe5adebd33b18a790b9e57fdd8a5b484c925486df`  
		Last Modified: Tue, 04 Jul 2023 14:59:18 GMT  
		Size: 15.5 MB (15520537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:5b0e5a243d1ce71969d78d43a5e96c4f6827e71ce1f889b937069f96cfb19909
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75680643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:826ff0c5465ce834034c2c8aec49d5ae31c4b08991a486afbddc208db6ebb06c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:18:11 GMT
ADD file:ff86c25854c28609c2852c1615270f0acd4c4efaa38ff8ed9c23afe5132f2135 in / 
# Tue, 04 Jul 2023 01:18:15 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:33:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a792749f62225048efdf85841bea6f3999f586371852f3dbce13a6c3d89b1fa7`  
		Last Modified: Tue, 04 Jul 2023 01:25:06 GMT  
		Size: 58.9 MB (58927745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf553284aac150acedeaf1c5f33c1820a34bff4f20ef96c32510ee19f2be0e83`  
		Last Modified: Tue, 04 Jul 2023 04:38:16 GMT  
		Size: 16.8 MB (16752898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:769618a5b2bab0e90bd2133eb8ddf675f78ca808b6bb18cb99a82d773142c963
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68920096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b1d835d438212d2d9e3bc4d7ed1a6378d6b066e3545bedc9c90fcb1887fa155`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:32:26 GMT
ADD file:231ba6ce8d3ee30318948799a94cb007f1517ea0d14c2b84863012cac37d6c6b in / 
# Tue, 04 Jul 2023 01:32:29 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 12:48:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1e40ed2a44a8c2786b06584afad765d97e9b1c910f58ae426622ba17fbf3d4c3`  
		Last Modified: Tue, 04 Jul 2023 01:37:21 GMT  
		Size: 53.3 MB (53288197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf2b9bfea4ac32f9de9f19ff39e147a59dc0ed209ac66dbf1f57baa75c0eef4`  
		Last Modified: Tue, 04 Jul 2023 13:06:27 GMT  
		Size: 15.6 MB (15631899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldstable-scm`

```console
$ docker pull buildpack-deps@sha256:01b47b8d5b8d592d95795e8d94f69b4dbfb9b99fb8f224daa19b1d665c87a9e2
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

### `buildpack-deps:oldstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:dd33e02b9d8fa4bc5631f3fee9dfa00166340d0172637f0a93ac2474b7198211
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.4 MB (125400673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b5c24127e49141c62bbc619c636c8a9fd47a079535d13ffc5a9048440857572`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:09 GMT
ADD file:b7c0be2bb90e88689b1c16da78dea0b85760b55b90ef2e5bc4a529c89e4fa25b in / 
# Tue, 04 Jul 2023 01:20:10 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:30:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:30:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:34df401c391c7595044379e04e8ad4856a5a3974cdbf5a160f0a204d761e88aa`  
		Last Modified: Tue, 04 Jul 2023 01:25:21 GMT  
		Size: 55.1 MB (55055300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fdd0e5b72ccae203ec30d533c0bcd34200af90265e0531c66356812e529af32`  
		Last Modified: Tue, 04 Jul 2023 03:52:30 GMT  
		Size: 15.8 MB (15760327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa786a946ae67fa18e07eaf82fefee1777449f7db1a8fea5abec1aadbe99e2ef`  
		Last Modified: Tue, 04 Jul 2023 03:52:45 GMT  
		Size: 54.6 MB (54585046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:6444b0291a1e57077fd144006676311385dc274ac4635349734805863890dc0a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.3 MB (120266460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2572b05d24e9060950a7b5ac48a29b0fb2d2cbf307f2215360bd0b0c66f68b9a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:48:39 GMT
ADD file:fe1b9f9f6c7d67ad23a2ee839774be4bcee33c60c7b34c48df5a08eb33cafd1b in / 
# Tue, 04 Jul 2023 00:48:40 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:24:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:25:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:702dd8b607f626c689176debe921fe96009c1ce6dbd66f4f238c7def50080e3d`  
		Last Modified: Tue, 04 Jul 2023 00:52:15 GMT  
		Size: 52.6 MB (52556778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec773064e3ff5287bd9be0bdb7b99e708aed435b4920a0f64aeaf158d9631f5e`  
		Last Modified: Tue, 04 Jul 2023 04:29:40 GMT  
		Size: 15.4 MB (15369118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ae2fc9256b17aac11e221f2db3d50e0543fecf87896a99ff9be68ea2335989`  
		Last Modified: Tue, 04 Jul 2023 04:29:57 GMT  
		Size: 52.3 MB (52340564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:9569373b56b793c8734d0731167d1e98d06a72c1bc73f2dbcd79eb702cc555bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115442178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e19dbbcdc9a0bbf8ee958a11f57adb53e7c4f9185065970af57187256c004e5d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:58:06 GMT
ADD file:17e02296458241d9441f8da6a5dafb747d528a729106b17cec2f4c1c8cfe0ad8 in / 
# Tue, 04 Jul 2023 00:58:07 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:51:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:52:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:31edf2db9ca1650aa08e2d42e9b5bb7349413d7212110149a1a5d202ac20914b`  
		Last Modified: Tue, 04 Jul 2023 01:03:12 GMT  
		Size: 50.2 MB (50218247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e794b9a6d62ad67f31927f253d3a467d402da7b96769cef6b5503fde01f18eb9`  
		Last Modified: Tue, 04 Jul 2023 06:19:48 GMT  
		Size: 14.9 MB (14868644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fdbc75406b7868979ba89f96e015c45fbcf9efe34aa3863e52c0e926531784f`  
		Last Modified: Tue, 04 Jul 2023 06:20:06 GMT  
		Size: 50.4 MB (50355287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:661446de2b43b6287b82e68aec7d4c3f2a6b2bd64e4a3e5765010400c4547a0e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.1 MB (124126801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9f39a9c3f22df829bd4eabc4d170b60fec575c4439a35d169828480baddecc7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:43 GMT
ADD file:e626446584d8094b7b58d72a717380ca64d3e9ab924fc625406fe26a83fe1d8b in / 
# Tue, 04 Jul 2023 01:57:43 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:56:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:56:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:29279ac7c19f9c667f1c6b07bfba6fba20ca0d945b9fbc6edad6f75d13361fae`  
		Last Modified: Tue, 04 Jul 2023 02:01:38 GMT  
		Size: 53.7 MB (53703979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d0c3fcc5367be60f92df0774820f317a179565cd3ee9c222f5500a7be32151e`  
		Last Modified: Tue, 04 Jul 2023 06:22:01 GMT  
		Size: 15.7 MB (15746747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5fa66dbb545c6ff93c768ac595d874b2f22053e8d2f842f4b6ccc310ebfe0c`  
		Last Modified: Tue, 04 Jul 2023 06:22:15 GMT  
		Size: 54.7 MB (54676075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:23e7ba60e97d2b78a0465a81a01d333d9a193b217b2b0f38bbea777ff2815faa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128227351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e144a202cd144d0e0b68a485990e7601e5c8114ac6ff9630063b8965660d0a69`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:38:48 GMT
ADD file:c5739407c2c257fbb85ab4b9dcd2dc07e6fe172d7309aaaaab544c8df6c42b92 in / 
# Tue, 04 Jul 2023 01:38:49 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:30:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:31:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b700c8b35944e0d5f6ab9049dbe2262492e26327a8efad518b1011428393653f`  
		Last Modified: Tue, 04 Jul 2023 01:43:49 GMT  
		Size: 56.0 MB (56040756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414994a3b1789f89f704fcfc0e721c0036089a74368f21aa6fafa639fef2c93b`  
		Last Modified: Tue, 04 Jul 2023 05:39:34 GMT  
		Size: 16.3 MB (16263605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ee301eb66e57dfaf79983158c75b77a7775e1b6216c45ce247c6fac3786a46`  
		Last Modified: Tue, 04 Jul 2023 05:39:53 GMT  
		Size: 55.9 MB (55922990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:700f08a72438adc954794c7d3a2fd5dbd704f8a9cc99287a3cfd5553fa328801
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122097647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32e876d3ef58fa796770e6bc26758ca966269bb2f0b41fd892cc7546c77b0b51`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:10:02 GMT
ADD file:f7ddd7406e3aa24165fc80933583fc2298f9792865511fe65def2f571fed2207 in / 
# Tue, 04 Jul 2023 01:10:07 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:43:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:45:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:af98e96208d7ce4cff5417a3e8a38f98d2ed3abbca318e1e6c323aa8b8c56690`  
		Last Modified: Tue, 04 Jul 2023 01:20:40 GMT  
		Size: 53.3 MB (53270472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b8f3d09abba473eec10e4fe5adebd33b18a790b9e57fdd8a5b484c925486df`  
		Last Modified: Tue, 04 Jul 2023 14:59:18 GMT  
		Size: 15.5 MB (15520537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427c4e665dab89a7a9a5cef3f1bab709cd38d4945e49ef760b95611e774a07e4`  
		Last Modified: Tue, 04 Jul 2023 15:00:02 GMT  
		Size: 53.3 MB (53306638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:92a3d9951e784acd6f21e0cdf396b60a964d1078dc1f61719d645f1e7eec914f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.5 MB (134545338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05f293bd1201dd82f48e60638e86ac0f42f4491c53208a613704b933e2417990`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:18:11 GMT
ADD file:ff86c25854c28609c2852c1615270f0acd4c4efaa38ff8ed9c23afe5132f2135 in / 
# Tue, 04 Jul 2023 01:18:15 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:33:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:33:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a792749f62225048efdf85841bea6f3999f586371852f3dbce13a6c3d89b1fa7`  
		Last Modified: Tue, 04 Jul 2023 01:25:06 GMT  
		Size: 58.9 MB (58927745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf553284aac150acedeaf1c5f33c1820a34bff4f20ef96c32510ee19f2be0e83`  
		Last Modified: Tue, 04 Jul 2023 04:38:16 GMT  
		Size: 16.8 MB (16752898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b8f1977f7b061bf5ae7311bb1750877d9ba871f041ba604c8e1e9d1e1143e0`  
		Last Modified: Tue, 04 Jul 2023 04:38:44 GMT  
		Size: 58.9 MB (58864695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:28964966888229ec79ac01c2034a5e759e7b04ea102ede17272baf6b71eeeb2d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (122981828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f6ffe961aa23647a1a72f2af8135528a958505fe0453d5bf132aebddb6636c1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:32:26 GMT
ADD file:231ba6ce8d3ee30318948799a94cb007f1517ea0d14c2b84863012cac37d6c6b in / 
# Tue, 04 Jul 2023 01:32:29 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 12:48:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 12:49:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1e40ed2a44a8c2786b06584afad765d97e9b1c910f58ae426622ba17fbf3d4c3`  
		Last Modified: Tue, 04 Jul 2023 01:37:21 GMT  
		Size: 53.3 MB (53288197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf2b9bfea4ac32f9de9f19ff39e147a59dc0ed209ac66dbf1f57baa75c0eef4`  
		Last Modified: Tue, 04 Jul 2023 13:06:27 GMT  
		Size: 15.6 MB (15631899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b214fc39e8a77ee2b4618f8315eee93c861d035ba1cf9dc80e62081ee3aafe`  
		Last Modified: Tue, 04 Jul 2023 13:06:41 GMT  
		Size: 54.1 MB (54061732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:scm`

```console
$ docker pull buildpack-deps@sha256:12a2678b3eabf425fa2c142421e1db4dfe6ab854a537af91c289507745c71b36
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

### `buildpack-deps:scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:0f78de2b3312f09866ac4eaaba883d518e886b540ceeff548750914b935f8e50
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.7 MB (137693638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:064924f22ba6cc021e9ca9ae3e10d21b15e491c0d1387c5f62300c70241c04d1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:19:44 GMT
ADD file:5d17ca085473e890bd6eca4abf6d324c3181f80692523b83ef25d1c42576b99f in / 
# Tue, 04 Jul 2023 01:19:44 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:27:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:28:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d52e4f012db158bb7c0fe215b98af1facaddcbaee530efd69b1bae07d597b711`  
		Last Modified: Tue, 04 Jul 2023 01:24:39 GMT  
		Size: 49.6 MB (49551432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd206bea61ff3e3b54be1c20b58d8475ddd6f89df176146ddb7a2fd2c747ea2`  
		Last Modified: Tue, 04 Jul 2023 03:51:23 GMT  
		Size: 24.0 MB (24030593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2320f9be4a9c605d1ac847cf67cec42b91484a7cf7c94996417a0c7c316deadc`  
		Last Modified: Tue, 04 Jul 2023 03:51:42 GMT  
		Size: 64.1 MB (64111613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:27d15e25a27b8983778bfedc271e37fbf73269e16b907efc0f8c0a4af8c912b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.7 MB (131665655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dac77eebbb12f590d8e6de52e972d43c54544315b77364e7101d186dd5aad91c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:48:22 GMT
ADD file:09001854dc5081f907ac2a66d301e4b3d6b4bf2c2483aad5395a535bf068698d in / 
# Tue, 04 Jul 2023 00:48:22 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:21:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:21:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7e0a1f476b42bcc214197ec9c5ef753ddf2ab36a314416a6ac96cd921ff0d41d`  
		Last Modified: Tue, 04 Jul 2023 00:51:29 GMT  
		Size: 47.4 MB (47402786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68311cc5ff511aa59283fdd7f1e25bc33dfc3ad9ae87e5c94447f36c3f7c4817`  
		Last Modified: Tue, 04 Jul 2023 04:28:32 GMT  
		Size: 22.7 MB (22708933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09518fc93ba137cac901dd7b0cc5fab1e20a21a7d6bbe3a35b7f921a069ddc5c`  
		Last Modified: Tue, 04 Jul 2023 04:28:53 GMT  
		Size: 61.6 MB (61553936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:36fa95975190dc678d40a37a93185f66e9192b8c80dec22c959399e2f7ec2569
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.4 MB (126434321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3da8a85987ffb7432f4d6f66364a39ac772f3a9b6bff23ba597689223f28b4b3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:57:42 GMT
ADD file:279ef7213d41f1f7ae76bd76293a5107fd1f8caf557f837cab9c834d2841e031 in / 
# Tue, 04 Jul 2023 00:57:43 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:49:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:50:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b9bdcf1a9a6361f231594c76a75bfb4c2fef5f9745b9713bbd50efaf37ca11b8`  
		Last Modified: Tue, 04 Jul 2023 01:02:26 GMT  
		Size: 45.2 MB (45236201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8ee33ea63b2391e912423c14b2f1e789137ffb03659568cb361a2fa2b4efbd`  
		Last Modified: Tue, 04 Jul 2023 06:18:41 GMT  
		Size: 21.9 MB (21936446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2a5b4416a84ac4585c3e3879ca49a6fc3e8d46028a4f27098ae1bdb4ae710d`  
		Last Modified: Tue, 04 Jul 2023 06:19:01 GMT  
		Size: 59.3 MB (59261674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a5cb7353b2ce88aeffff9c11400ba2868c5da3edae5c9ee5c2c4c09312ced7e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.1 MB (137126402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb40501a95e932bb48d49f74d197ea8377d1ccba9e2dd9f66e63fdf9de21b409`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:26 GMT
ADD file:ab1761d899751c4d24e15179fc9e7e7ac3fb83798ee37ca13d6a6ac44fbeded3 in / 
# Tue, 04 Jul 2023 01:57:27 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:54:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:54:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:42cbebf8bc116ba1aed7897e2d0566bf49da9d5c70be71b6a7cb07805d2f5b7a`  
		Last Modified: Tue, 04 Jul 2023 02:00:57 GMT  
		Size: 49.6 MB (49572781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0518ec57568a70561f7c04650f9554c88dada973f54d88e36f65b0796d35de`  
		Last Modified: Tue, 04 Jul 2023 06:21:03 GMT  
		Size: 23.6 MB (23569546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356172c718acf9930d9465b170864319079e2d2ebac0ddef781d64e85789531e`  
		Last Modified: Tue, 04 Jul 2023 06:21:20 GMT  
		Size: 64.0 MB (63984075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:e93d1e1d0a091272e88d7d8bf0e0e21b3df095765d52c1007b9bbab8d01069f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.4 MB (141404445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d40934ac087de93ceffbf81437543947fc9c9c8b8184568346ac03da80f35bd7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:38:25 GMT
ADD file:e0a25fe261e09183ec383698ab2c800f93c5b0805564d7104ad5119db52cccb7 in / 
# Tue, 04 Jul 2023 01:38:25 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:28:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:28:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:381263dab43af8bfb8e85c7a9a32f35492cbdcc3a046b35f947cf3bf3a55f4c1`  
		Last Modified: Tue, 04 Jul 2023 01:43:02 GMT  
		Size: 50.6 MB (50562388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af522778d6fcd5f4b85dafb1f21b89441dedee6ce875890b15ad8c454bbb9fe6`  
		Last Modified: Tue, 04 Jul 2023 05:38:10 GMT  
		Size: 24.9 MB (24869747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501f685d713d76bdc0731a917b074d79f3de7c84bfe09c53585642801175a72f`  
		Last Modified: Tue, 04 Jul 2023 05:38:34 GMT  
		Size: 66.0 MB (65972310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:68087f9d2d7eb43f96f073504d68e5f68181fe9c905f47fb14815bec8db79572
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.1 MB (136104248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0d288a207994f6184d90c784bdde0152350cd4c6bf91f0777b8da30da1a0c3e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:08:42 GMT
ADD file:c567fc0f97f36ea531c05e159cd6ac2a8747f14ea5b6ccae39bab9d305da180d in / 
# Tue, 04 Jul 2023 01:08:47 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:34:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:36:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76240e493592cbc7ca56583a6e8e03ab12a967b65bbeb1df7828a5099fa271d9`  
		Last Modified: Tue, 04 Jul 2023 01:19:16 GMT  
		Size: 49.5 MB (49542143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85086244c52affe40f860feee6e34c03fd0f782e853b00950f1a9b8b6704d24f`  
		Last Modified: Tue, 04 Jul 2023 14:56:03 GMT  
		Size: 23.6 MB (23611680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2482ef924bba9e0b7ef4ad15506bbcf2a7db029acfc793f94b5d17435ed529`  
		Last Modified: Tue, 04 Jul 2023 14:56:55 GMT  
		Size: 63.0 MB (62950425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:a1876fdc603fdf011be6b83ff792c330a17e2743922fd5aabaf6a1ed5c037080
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.8 MB (148787535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62c051da923c5734b37ef3d706b3ecdfe384634edc45b782adb0b0e0f06f84db`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:17:23 GMT
ADD file:5aaa642008df5a97014e76042a767f06bbfda91db1d5f336a1b3f98e9b11c7a1 in / 
# Tue, 04 Jul 2023 01:17:26 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:26:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:27:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e039cf6634cf83a31e97e2a56b4db40a8c38a62d6857c77e687d5edb3eb0dfde`  
		Last Modified: Tue, 04 Jul 2023 01:23:59 GMT  
		Size: 53.5 MB (53536740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54fff62f5ff539ace95f1581096d57b95ca024b9d5cc7c85bb4a2bf159ad845f`  
		Last Modified: Tue, 04 Jul 2023 04:36:20 GMT  
		Size: 25.7 MB (25681297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd5a2ec3d78fd420afc5e1c6739ad59505cf484be0ea1c2c2dfe00c7b2c00ec`  
		Last Modified: Tue, 04 Jul 2023 04:36:52 GMT  
		Size: 69.6 MB (69569498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:26e61b2a6df1a810689cbf8a1b2b097496c6de014ff7013b8f3c0466dc100308
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.1 MB (135063311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:875d66c05f546cc0a92a5aed5599d58335c22c67b0706c82bc06056c3af12657`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:31:54 GMT
ADD file:0ad7ffbe777e5367ad6dcbb4a182e1d578739aa7a4853f82f21bd71d824de7ae in / 
# Tue, 04 Jul 2023 01:31:56 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 12:47:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 12:47:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce9d001c0d31ec9b8072b1a9bd01771a10ea8ddfefa381cf9ce7e2d63538aaeb`  
		Last Modified: Tue, 04 Jul 2023 01:36:50 GMT  
		Size: 47.9 MB (47921709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024bda56b20d3018344098f67965337568b532ea03f09d87858a2bb5eae82bf7`  
		Last Modified: Tue, 04 Jul 2023 13:05:34 GMT  
		Size: 24.0 MB (24028793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da5b83dc971cc08c6baeb1ddd5fb5de06beefef83c0444c224b4e377d704705`  
		Last Modified: Tue, 04 Jul 2023 13:05:50 GMT  
		Size: 63.1 MB (63112809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:sid`

```console
$ docker pull buildpack-deps@sha256:bdb6490a62623952a85a6e205d00be1168a5573d1654942fb8145cec9f795f42
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
$ docker pull buildpack-deps@sha256:528b5311a9ae6696bcd00391123c4bc54f3b31b58c58e64d74bc86267eb03278
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.5 MB (351457721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b9832bf13f8edec5c1794ddc2768c54640f872d1d3ba82cf610164cf5a2e673`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:22:34 GMT
ADD file:8ed2c72091b90575b320038c2ad715760d6382aeea5c416dd16f7ed04e955217 in / 
# Mon, 12 Jun 2023 23:22:35 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:34:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:34:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:35:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2e79cba44192968ca6ea42058e67723ae58bebd2ea54b31f432b1ffed9fea9d9`  
		Last Modified: Mon, 12 Jun 2023 23:28:29 GMT  
		Size: 49.6 MB (49551965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cda7b25305de24c8cc4e88d990c3c3c70e109b190f7411b9d3237528081a161`  
		Last Modified: Tue, 13 Jun 2023 03:39:26 GMT  
		Size: 24.0 MB (24019326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c71d2bfd3c86199eb06493b2f6d0258d7576aca3f851198b940bb3b1505989`  
		Last Modified: Tue, 13 Jun 2023 03:39:43 GMT  
		Size: 64.5 MB (64535333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75a9b221ba575bef197107054a01083b3dc2b0d4bedc07f7e6c3fcbde4df462`  
		Last Modified: Tue, 13 Jun 2023 03:40:16 GMT  
		Size: 213.4 MB (213351097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:425577d4371532d7a1016ddbb8661097ceb1b3d84c34fd7797ae4b12cd690ad2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.2 MB (318155740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b0af6d02dd2c68e48fc43dcbeca22913a6160330fab418584d083f8d500e97b`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:49:10 GMT
ADD file:b79d69fc6594f6ca5e9e76165017858724482b88aa3aa49e3db7b07a3dcabc0a in / 
# Mon, 12 Jun 2023 23:49:11 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 07:40:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:40:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:41:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:13ee4e7971510c95d7e625030699b854921da16f6d5ef29884b269a308a37afc`  
		Last Modified: Mon, 12 Jun 2023 23:52:56 GMT  
		Size: 47.4 MB (47417325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8374a5ed08b072c6f518c88ddf07dd3d9e04e3ccc51d0810b12cd2ae53c998`  
		Last Modified: Tue, 13 Jun 2023 07:44:30 GMT  
		Size: 23.6 MB (23622159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c640f3b5ffb5f4fc9722d6fca3f771a8db79e177cf1b0cfd035587f4d4dcf4ae`  
		Last Modified: Tue, 13 Jun 2023 07:44:48 GMT  
		Size: 62.2 MB (62150140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638239f1655f4299ec88f74ea4b5a44b44817cf56b426104a7b6e23df2031def`  
		Last Modified: Tue, 13 Jun 2023 07:45:23 GMT  
		Size: 185.0 MB (184966116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:bc482d01bcfba9d59704601f01b9f3890277671f0f5ae65064ffc8bfd8a092bc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.0 MB (301978210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:993c7c66f179e1f8a499111f4da05a053490bbe72ab3e5d29a35162ec157f3cf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jun 2023 00:00:33 GMT
ADD file:82567bde3caa9ad83c0c12c0525e6fd51cc833f0b29e733c2da572ed00150220 in / 
# Tue, 13 Jun 2023 00:00:39 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 05:00:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:00:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:01:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1d80e7ebc54969ad575378cf66dc58999cbf341e0d2a92c9ff0bfd5b3b9fb1c3`  
		Last Modified: Tue, 13 Jun 2023 00:06:30 GMT  
		Size: 45.2 MB (45234838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a26e461ec0e64583c2acfbef48942f57c9de9da65ff1a078a62e910baf3ce05`  
		Last Modified: Tue, 13 Jun 2023 05:05:32 GMT  
		Size: 21.9 MB (21922951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4da543e1cb7517b023e6ef07f0f0385da6f0c3f832cfd7ade1c7381c2ffe580b`  
		Last Modified: Tue, 13 Jun 2023 05:05:49 GMT  
		Size: 59.8 MB (59799388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a6dd7ea367162c4002f5bdde6db8bbbef4671fde6486cf888d7a0bb5c07e29`  
		Last Modified: Tue, 13 Jun 2023 05:06:19 GMT  
		Size: 175.0 MB (175021033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:9b1e52d6511e5cfbcb6ad379788c4aba30e2dd9ab3e9909a0843477506f3d785
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **340.1 MB (340130427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4578dc30c4d05d7a1fed527a3d742d540a2f37c1cbac255db25eb945baf702b1`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:41:38 GMT
ADD file:94f1432513f9a03b38028af02b1d1720fb0558559faf3e7f9d7097cf6b962056 in / 
# Mon, 12 Jun 2023 23:41:39 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:05:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:05:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:06:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8ba9ab3e6f12b9702649c2e0c7d78e22ffb9183f68c288b9edef2387bd8d4efd`  
		Last Modified: Mon, 12 Jun 2023 23:46:36 GMT  
		Size: 49.6 MB (49592096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:393fb89bae1d5f0307a283cb7c3b5f54cc63fde2e90b7b65ceae29bcd27126f5`  
		Last Modified: Tue, 13 Jun 2023 03:10:09 GMT  
		Size: 23.6 MB (23558237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4483fcef438011d245d9be3906ab5e6a92c139027fe4286dc7e46b975299183`  
		Last Modified: Tue, 13 Jun 2023 03:10:24 GMT  
		Size: 64.5 MB (64490917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cddf934afceb08172df763ffcde92b9665c3c8ae9c4810b008715669ad3d58e`  
		Last Modified: Tue, 13 Jun 2023 03:10:52 GMT  
		Size: 202.5 MB (202489177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; 386

```console
$ docker pull buildpack-deps@sha256:b4764a5e07b05e2bdd8d6d90fa4ff2e34c122e475fc4aa317242bebe454cba77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **353.6 MB (353591470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27e185958c518f02129b840a8ea93d9703f29c31e0bb0ee3ca1e71acfb27d11b`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:42:10 GMT
ADD file:209e3bb955801ad81eb18a280f9fbd5500a0e1f04565e6c94c9cd24dcba4c0af in / 
# Mon, 12 Jun 2023 23:42:10 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 01:09:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 01:09:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 01:10:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8bce10b6f772acc79b03d87add4bd359f98c767e3599f82d8e351cced14c1a11`  
		Last Modified: Mon, 12 Jun 2023 23:49:26 GMT  
		Size: 50.6 MB (50562699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d6b7d433b6a8b07b01e4b262b82f2b882380e41bcd3a6e8b88ca32ea66321e`  
		Last Modified: Tue, 13 Jun 2023 01:15:14 GMT  
		Size: 24.9 MB (24858532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1c9493cccdfcd2c44a013f62ecc08283137f3fd2d7a483cf56387dc987b536`  
		Last Modified: Tue, 13 Jun 2023 01:15:36 GMT  
		Size: 66.4 MB (66355536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e30574996c34012fa193dace0f01bb334e773810647079cb6d2a76b7945342d`  
		Last Modified: Tue, 13 Jun 2023 01:16:23 GMT  
		Size: 211.8 MB (211814703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:0d42590a778653226abaaaeba3e4d95d9f165e2cb3520044566e699afa0f811f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.3 MB (326264556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:732624570cf9a1dec3651b64baba5195328bdb63e629cb11fed831a9a8341e59`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jun 2023 00:12:52 GMT
ADD file:b2a9cefcdd223b4cbf9b1abac81e8c0c158a24f9c272910a8822619ea9d55ae9 in / 
# Tue, 13 Jun 2023 00:12:57 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 02:12:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 02:13:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 02:19:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:65733d4f161a7d2fd9cef6d80eb7fe00897e936eb78d018361809f7384b08c28`  
		Last Modified: Tue, 13 Jun 2023 00:25:52 GMT  
		Size: 49.6 MB (49561285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8cac982d96cd0724a1a282faecd42ae997cf2e6c468441bdcf2ce718f092f4d`  
		Last Modified: Tue, 13 Jun 2023 02:26:09 GMT  
		Size: 23.6 MB (23606470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec621985ebc463298904a643b89d8805cdefe9a156edc65db797295bf5ce37d`  
		Last Modified: Tue, 13 Jun 2023 02:26:58 GMT  
		Size: 63.4 MB (63449697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43067e7ef8f78b7740cb05aa82b22965d78ae240348e6c33c24dca2d27e8f056`  
		Last Modified: Tue, 13 Jun 2023 02:29:12 GMT  
		Size: 189.6 MB (189647104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:eacd16ff9356ba0c57dfa909efcc62d6405fa44679146f06c15e26d48ec5c4a1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **365.8 MB (365821306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e00dce918605ba965c51b6e622e0516b98b712cdb92b58dee885ac0e9d72b0b0`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:19:31 GMT
ADD file:aded196ce7e0c005fe55d5a92492be8cc5d7934fac082b7ab95b8c946e71e0a2 in / 
# Mon, 12 Jun 2023 23:19:34 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 07:34:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:35:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:38:16 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e3f8e732e00762188b5ba00db7db3f36c97d0fccdf3d6121db4ca1febc7d190`  
		Last Modified: Mon, 12 Jun 2023 23:26:13 GMT  
		Size: 53.6 MB (53558517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3615faaadea50ed31520dc05aeaebf1283ee0aae09227fb97c1a9de87beec2f8`  
		Last Modified: Tue, 13 Jun 2023 07:43:30 GMT  
		Size: 25.7 MB (25673673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cdc90af7293b0d3b333a9a6a8a60e61400bc5577336008e14e772e6041c6bce`  
		Last Modified: Tue, 13 Jun 2023 07:43:56 GMT  
		Size: 70.0 MB (69985119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ffd035648c807001473ccb0f1a04d6d76990ef3e357d8f0b665979b64afe78b`  
		Last Modified: Tue, 13 Jun 2023 07:44:54 GMT  
		Size: 216.6 MB (216603997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:686f023ac15591767c0b4e0500c685efdb6b599766b972305a425e11dcd9a937
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **358.0 MB (357978583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:273cc13afc1bb50107f431972b90d2c10c44f10a0b401ed1207a8378f3fe8675`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:09:05 GMT
ADD file:dc2a1586d12e833e5dc300033838059f3946ddddccde6c62d17cba40536ead15 in / 
# Tue, 04 Jul 2023 01:09:07 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 01:31:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 01:34:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 01:42:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d273b82777a979179469448ba9e255d7f7e1671f28d5610f47e8530093aaa04e`  
		Last Modified: Tue, 04 Jul 2023 01:12:27 GMT  
		Size: 45.7 MB (45695454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f7ece03f0359914c61a65ea80744e3ec92ac1afbb1ddab79b6c7276dae0614`  
		Last Modified: Tue, 04 Jul 2023 01:43:00 GMT  
		Size: 22.3 MB (22287386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e6bfc3fa16d519518bec2169bd35f0eeede077436e581f9c80725f413e6788e`  
		Last Modified: Tue, 04 Jul 2023 01:44:21 GMT  
		Size: 60.1 MB (60140546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91c63bc964adf497f1164977ba456068b24b0b242c5b16276b6bfc9b1723b41`  
		Last Modified: Tue, 04 Jul 2023 01:49:51 GMT  
		Size: 229.9 MB (229855197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b0b9dab7c2e1f21c627113aa1c6b9c21050761ca06e8b97d1d0e19434da79de6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **320.6 MB (320614417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f275f768edd7209671adc00107c2353b50953ca84973ce178959ce461e831127`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jun 2023 04:30:54 GMT
ADD file:7ea0e5c460c626891cd3fc90639d6bfb9a27beeb7f5c79fd9c348c5b6244bd0d in / 
# Tue, 13 Jun 2023 04:30:58 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 18:33:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 18:34:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 18:34:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a129144c9fdcf79f6394b7f7bfa3d7e6a0c8ebfd424dca918695356a1b3bf970`  
		Last Modified: Tue, 13 Jun 2023 04:35:27 GMT  
		Size: 47.9 MB (47920583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d42182bfe271810fa332f879c12433ca046660729997bdce646aa7157138984`  
		Last Modified: Tue, 13 Jun 2023 18:39:25 GMT  
		Size: 24.0 MB (24020404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b53f300fd0adc6e321c844bd2e2fb478de90848743069202361df4928dd446b`  
		Last Modified: Tue, 13 Jun 2023 18:39:39 GMT  
		Size: 63.6 MB (63617737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eeb3234b4fe971e1c4b0c7127991671379ecc9df17d1b611ddf4553cd898f10`  
		Last Modified: Tue, 13 Jun 2023 18:40:07 GMT  
		Size: 185.1 MB (185055693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:ac7eb2111638a4f5590c0464e43a1b8f3541fd80e0446f40c46d30f640c882b6
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

### `buildpack-deps:sid-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:1444ecae199d3a84f514fffd3e96a07d956d068d696e22a6668f3a8b7b69bea0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73558597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3b07e6edfec497631a8a3716b0e973fce8f54eb68ded798958b4befa07050d2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:21:50 GMT
ADD file:4bfda8f11e59383c37bfa6038bb5d22f58b9724d249a62568a2e7d2908821cd3 in / 
# Tue, 04 Jul 2023 01:21:50 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:34:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6efa412d16b908043ec01c4ac9ff7323c0f488dd5d7ea4b9b086f1e80350b9b3`  
		Last Modified: Tue, 04 Jul 2023 01:27:46 GMT  
		Size: 49.5 MB (49475944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad8fa89586d6eb7c1bf3add3cde8c80b2da78794ef30be11a97f2dad784809a`  
		Last Modified: Tue, 04 Jul 2023 03:54:24 GMT  
		Size: 24.1 MB (24082653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:d1a9056c98835bada87f4138da4b902136cb795eca133e00ff0b1c407fb52bc1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.1 MB (70080759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a9b5fce7ee5621e0e2234d3e15d91216d47839ce7270d9e7ac54cf651eecc62`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:49:11 GMT
ADD file:e6181e27889c016519d8d701345aafff7138df96a76fb6a29403c8a33a3365fe in / 
# Tue, 04 Jul 2023 00:49:11 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:27:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:667272d8fe1bc81ce33874dbc84976c86d6b95f50198465a6ab672c71d87f666`  
		Last Modified: Tue, 04 Jul 2023 00:53:33 GMT  
		Size: 47.3 MB (47322473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b5934a15453e5e63936a0201a34b820f06d7c27f091dc017bac7d92e1e58d7`  
		Last Modified: Tue, 04 Jul 2023 04:30:42 GMT  
		Size: 22.8 MB (22758286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:b786440d5fa9313cfe4c6e947e1e06bff0b361070ae00db02f93c8a902770278
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67108518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57f38aa572847a45b4cc64179b342a4010030a0cfacec4a3e125ba276bc94ea4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:59:44 GMT
ADD file:5be8eee7722dc860882f26018d8a0de49a4db6fcaa0f35d1dfbb74eff22929cb in / 
# Tue, 04 Jul 2023 00:59:45 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:57:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:42cc2becb0b735f0260d9f678fb1201bbe47c438212c5faf04879fab6a2dd73f`  
		Last Modified: Tue, 04 Jul 2023 01:05:43 GMT  
		Size: 45.1 MB (45123975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5cb3f60ee8390c8cae75e83a5b95ebc4f3589ca1af647965d02fe99b974827b`  
		Last Modified: Tue, 04 Jul 2023 06:21:50 GMT  
		Size: 22.0 MB (21984543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:168cc096593e0cdf7b4e13f9739eb5733adc9069d240de7ed0fe35aeb2a2d2cc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.1 MB (73103142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:344af7b87e9677178d16f959dfdde57f165ec1af4db8ab0e3a034476ef16a070`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:58:49 GMT
ADD file:2c2c0588b93f9af7d93f19033795edf9e61a692ff56e65d9e9500915276782c9 in / 
# Tue, 04 Jul 2023 01:58:50 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:00:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d1b52151d5bb774f3680f8697c343bae1b64b7308354db57dc6bbeb7d65d0964`  
		Last Modified: Tue, 04 Jul 2023 02:03:59 GMT  
		Size: 49.5 MB (49482570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03e94cfcd9a2ac0ccda7b085606ef5174003eb543c68b5bf077a91230b8a7f7`  
		Last Modified: Tue, 04 Jul 2023 06:23:39 GMT  
		Size: 23.6 MB (23620572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:555e0c926152f63f4be81642923a7d416a6db8de6cdeffaf232ce9a51950f704
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75427637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43878012a9d69af31988db85d06eed454cfed8f9f71f7baeaf892725ce675e3e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:40:19 GMT
ADD file:565f8487c71b5de967f1bf16d4bd86291107b68f4152a61e35a8ab86e9f83b7b in / 
# Tue, 04 Jul 2023 01:40:20 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:37:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:46685592106ba6554716942e180f6b4cd8a73f1ec934554b40aee89b47118f5e`  
		Last Modified: Tue, 04 Jul 2023 01:46:32 GMT  
		Size: 50.5 MB (50505825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf3084ac7ee091f26af470878c8197f67d44c09670c27921a26209c909a5c0b`  
		Last Modified: Tue, 04 Jul 2023 05:42:02 GMT  
		Size: 24.9 MB (24921812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:9c445cebfd89383262612bba3ffcd90741aead0f8078a8c553fa99aa51180e70
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.1 MB (73116035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:563c80671a9f694e8c110c810f67d406dc3c68ae2109676af03b778087a4bdc1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:12:32 GMT
ADD file:ab2873cb088258c79fab5dde2d754d1967ca11e58adcf6a08811206759a323d5 in / 
# Tue, 04 Jul 2023 01:12:35 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:52:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:796c2f1009ce9a433d10a1f4708cbb79ef733dcb0ca992041a6aa621e85d8410`  
		Last Modified: Tue, 04 Jul 2023 01:23:15 GMT  
		Size: 49.5 MB (49455398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44357c89fac3bdc147daa7fe48fcf65b83dae0a924631c0b3e9ddb3f7ad71da2`  
		Last Modified: Tue, 04 Jul 2023 15:02:20 GMT  
		Size: 23.7 MB (23660637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:a5807b1f6748c228dc4b2b9be5b8dd6d43925344484a7ac9794dd5a809331ce1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.2 MB (79206895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:985fda4e25a501fb5c76ae42a7c2ebc1fccc03a9dad9be7395da923cac261da5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:19:33 GMT
ADD file:4c1d6f76704d32b9b503bd61c4b485555ec28037fb500403ffb5cbb102cf4509 in / 
# Tue, 04 Jul 2023 01:19:36 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:37:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3e4e6efa69b637e0e8ca00ddcae1aed23aef874a92a2904bdc6c9fa5b3212b8a`  
		Last Modified: Tue, 04 Jul 2023 01:27:02 GMT  
		Size: 53.5 MB (53474414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b5bee4b9196ae6959902bca430113379429a2f075e1553977c6d0442f46233`  
		Last Modified: Tue, 04 Jul 2023 04:39:59 GMT  
		Size: 25.7 MB (25732481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:44d3a4e55beac77f423ed6b86a5ec1b7f0f8420391a51ef5818256b5db0eeda5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.0 MB (67982840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb302f8c83e3c25737152a29d46030f5f78fa08610c71bf94fd362290d41d72d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:09:05 GMT
ADD file:dc2a1586d12e833e5dc300033838059f3946ddddccde6c62d17cba40536ead15 in / 
# Tue, 04 Jul 2023 01:09:07 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 01:31:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d273b82777a979179469448ba9e255d7f7e1671f28d5610f47e8530093aaa04e`  
		Last Modified: Tue, 04 Jul 2023 01:12:27 GMT  
		Size: 45.7 MB (45695454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f7ece03f0359914c61a65ea80744e3ec92ac1afbb1ddab79b6c7276dae0614`  
		Last Modified: Tue, 04 Jul 2023 01:43:00 GMT  
		Size: 22.3 MB (22287386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:f1ec0279f9d18d011062cad1be25abd66e64da40536c135db02b31f9b273289a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.1 MB (73060723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af73a45fd027437fc482806008569b16e9a19209902b6ef1ead753d323426a3c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:33:27 GMT
ADD file:9c12086273bf86ac1b3f72beebd17cc357bb749a95ac64d0f5ecdbbe7631cec4 in / 
# Tue, 04 Jul 2023 01:33:29 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 12:50:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3dcb3b9eb8abea3e1994db2e9f2073832965384334d3e204d1df1e3dcd09cffa`  
		Last Modified: Tue, 04 Jul 2023 01:38:16 GMT  
		Size: 47.9 MB (47890767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d5c8c8644c840146ba18a3d20250a3f49997785afe106720a31e6e3bc0bdcf`  
		Last Modified: Tue, 04 Jul 2023 13:07:16 GMT  
		Size: 25.2 MB (25169956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:sid-scm`

```console
$ docker pull buildpack-deps@sha256:e770a17b3b5af783abd7b0178ea83e788b97a9107a5e1e074ac2f2cee327a204
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

### `buildpack-deps:sid-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:db8046e6728be4a319bf8c9c7fc53191969676c1aff3dc192ecb5e1acfc6dd44
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.2 MB (138245050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84c9f688e3f355ba0028691806d887b635ae646386d3bf3d5b1b6cda070e4e10`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:21:50 GMT
ADD file:4bfda8f11e59383c37bfa6038bb5d22f58b9724d249a62568a2e7d2908821cd3 in / 
# Tue, 04 Jul 2023 01:21:50 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:34:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:34:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6efa412d16b908043ec01c4ac9ff7323c0f488dd5d7ea4b9b086f1e80350b9b3`  
		Last Modified: Tue, 04 Jul 2023 01:27:46 GMT  
		Size: 49.5 MB (49475944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad8fa89586d6eb7c1bf3add3cde8c80b2da78794ef30be11a97f2dad784809a`  
		Last Modified: Tue, 04 Jul 2023 03:54:24 GMT  
		Size: 24.1 MB (24082653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80dbf573225a65ee45360f0a43a08f5e1809ec65e4c5fd3634aa3c651ce0aa3`  
		Last Modified: Tue, 04 Jul 2023 03:54:42 GMT  
		Size: 64.7 MB (64686453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:0841006a6e7ae7124fb49383c6e729393fe97fdd7d5a764ba2cf3524717ac5d3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.4 MB (132387410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3a1dbd93f213db0dc50fa2e522af5b935f1ec468cdef913e9ba7a9874021b31`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:49:11 GMT
ADD file:e6181e27889c016519d8d701345aafff7138df96a76fb6a29403c8a33a3365fe in / 
# Tue, 04 Jul 2023 00:49:11 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:27:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:27:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:667272d8fe1bc81ce33874dbc84976c86d6b95f50198465a6ab672c71d87f666`  
		Last Modified: Tue, 04 Jul 2023 00:53:33 GMT  
		Size: 47.3 MB (47322473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b5934a15453e5e63936a0201a34b820f06d7c27f091dc017bac7d92e1e58d7`  
		Last Modified: Tue, 04 Jul 2023 04:30:42 GMT  
		Size: 22.8 MB (22758286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4231c799b91b6f2c6d3090483baafb52160bc63bb7459deb8ea264e4018f2d3b`  
		Last Modified: Tue, 04 Jul 2023 04:31:01 GMT  
		Size: 62.3 MB (62306651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:ef3af5ff6fe6345574d568b9ba626175b69ded771ab30deacab706cc412c49b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.1 MB (127062025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45c39f924f6ca9f00579aa7a0e37403b02cd47ce2ba59130218cfd6f5fd31a0a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:59:44 GMT
ADD file:5be8eee7722dc860882f26018d8a0de49a4db6fcaa0f35d1dfbb74eff22929cb in / 
# Tue, 04 Jul 2023 00:59:45 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:57:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:57:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:42cc2becb0b735f0260d9f678fb1201bbe47c438212c5faf04879fab6a2dd73f`  
		Last Modified: Tue, 04 Jul 2023 01:05:43 GMT  
		Size: 45.1 MB (45123975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5cb3f60ee8390c8cae75e83a5b95ebc4f3589ca1af647965d02fe99b974827b`  
		Last Modified: Tue, 04 Jul 2023 06:21:50 GMT  
		Size: 22.0 MB (21984543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c1e5d5a935736b670eec63e61b0bdcc50ea4bc384b4ef00a257b7d98cbe0f6`  
		Last Modified: Tue, 04 Jul 2023 06:22:08 GMT  
		Size: 60.0 MB (59953507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:6547b0fb05aa47c02279476c9c339b27a73ba686a8d964767bf51542e495f10d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.8 MB (137764860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b44f02907bd19b65d492b7fc136b89c412638c71ddb02410f4c3172aa8847bc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:58:49 GMT
ADD file:2c2c0588b93f9af7d93f19033795edf9e61a692ff56e65d9e9500915276782c9 in / 
# Tue, 04 Jul 2023 01:58:50 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:00:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:01:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d1b52151d5bb774f3680f8697c343bae1b64b7308354db57dc6bbeb7d65d0964`  
		Last Modified: Tue, 04 Jul 2023 02:03:59 GMT  
		Size: 49.5 MB (49482570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03e94cfcd9a2ac0ccda7b085606ef5174003eb543c68b5bf077a91230b8a7f7`  
		Last Modified: Tue, 04 Jul 2023 06:23:39 GMT  
		Size: 23.6 MB (23620572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12422f578439e0f8042c87a47638ea9651cb9d674e8c89b05c5e4d333833ca02`  
		Last Modified: Tue, 04 Jul 2023 06:23:55 GMT  
		Size: 64.7 MB (64661718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:08ac98188b4d99022ddf9f16dc0a488ec35f19e9d09d3930aef1e2f733ae81d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.9 MB (141945829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6989e556ea04ee7a099cc0e1e2fa0719d9fbf6a8ce54cc152f9844ccdc9f46e4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:40:19 GMT
ADD file:565f8487c71b5de967f1bf16d4bd86291107b68f4152a61e35a8ab86e9f83b7b in / 
# Tue, 04 Jul 2023 01:40:20 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:37:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:37:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:46685592106ba6554716942e180f6b4cd8a73f1ec934554b40aee89b47118f5e`  
		Last Modified: Tue, 04 Jul 2023 01:46:32 GMT  
		Size: 50.5 MB (50505825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf3084ac7ee091f26af470878c8197f67d44c09670c27921a26209c909a5c0b`  
		Last Modified: Tue, 04 Jul 2023 05:42:02 GMT  
		Size: 24.9 MB (24921812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef6611c0dbf9970353c5c08585b89e28e50531495ee733b7f098fa9c3501067d`  
		Last Modified: Tue, 04 Jul 2023 05:42:24 GMT  
		Size: 66.5 MB (66518192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:776e2afd9426f5f202780c44cb0d6c0ed2e77466bbee1fe230f4f8b68bb0bbe3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.7 MB (136723315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57625595c83aae207b1a1028993f73dcc398eeefcdafe5589ab032b376a5fd51`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:12:32 GMT
ADD file:ab2873cb088258c79fab5dde2d754d1967ca11e58adcf6a08811206759a323d5 in / 
# Tue, 04 Jul 2023 01:12:35 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:52:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:54:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:796c2f1009ce9a433d10a1f4708cbb79ef733dcb0ca992041a6aa621e85d8410`  
		Last Modified: Tue, 04 Jul 2023 01:23:15 GMT  
		Size: 49.5 MB (49455398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44357c89fac3bdc147daa7fe48fcf65b83dae0a924631c0b3e9ddb3f7ad71da2`  
		Last Modified: Tue, 04 Jul 2023 15:02:20 GMT  
		Size: 23.7 MB (23660637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360a64085c52bd3ade25ff3dffcad4ccd2db7944aad983d6da8f5a3e148e1a44`  
		Last Modified: Tue, 04 Jul 2023 15:03:11 GMT  
		Size: 63.6 MB (63607280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:c6db7b3d9b8b7b9461c958da7d9061423f995b3e3d3d4d9e2dfd8ab01cefab08
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.4 MB (149354347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1705ece1fdfc0d296b55a24fb47d71cd633a54e73ff649b62e797ad1429ca2c7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:19:33 GMT
ADD file:4c1d6f76704d32b9b503bd61c4b485555ec28037fb500403ffb5cbb102cf4509 in / 
# Tue, 04 Jul 2023 01:19:36 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:37:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:38:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3e4e6efa69b637e0e8ca00ddcae1aed23aef874a92a2904bdc6c9fa5b3212b8a`  
		Last Modified: Tue, 04 Jul 2023 01:27:02 GMT  
		Size: 53.5 MB (53474414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b5bee4b9196ae6959902bca430113379429a2f075e1553977c6d0442f46233`  
		Last Modified: Tue, 04 Jul 2023 04:39:59 GMT  
		Size: 25.7 MB (25732481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b347de1638edf48069dc551f9b7887a170d69f36e44b3d711a5f35da08e29100`  
		Last Modified: Tue, 04 Jul 2023 04:40:30 GMT  
		Size: 70.1 MB (70147452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:2fdda162727e88b07827fd912da5214d4e6184a7a61eff30378d465a4e8af39d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.1 MB (128123386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37b066cf94438556c4df6f89a1bade9a9e6151382e24685619bb268b0a2ca495`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:09:05 GMT
ADD file:dc2a1586d12e833e5dc300033838059f3946ddddccde6c62d17cba40536ead15 in / 
# Tue, 04 Jul 2023 01:09:07 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 01:31:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 01:34:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d273b82777a979179469448ba9e255d7f7e1671f28d5610f47e8530093aaa04e`  
		Last Modified: Tue, 04 Jul 2023 01:12:27 GMT  
		Size: 45.7 MB (45695454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f7ece03f0359914c61a65ea80744e3ec92ac1afbb1ddab79b6c7276dae0614`  
		Last Modified: Tue, 04 Jul 2023 01:43:00 GMT  
		Size: 22.3 MB (22287386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e6bfc3fa16d519518bec2169bd35f0eeede077436e581f9c80725f413e6788e`  
		Last Modified: Tue, 04 Jul 2023 01:44:21 GMT  
		Size: 60.1 MB (60140546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:96941110e49ead9aca1f19c783cee74c1ba60437aa646cb579afcefb7ad4b433
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.8 MB (136838024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d21031b741572c9c946128adaf02584158a5ab375ff2bcf317eb2d6bf3597828`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:33:27 GMT
ADD file:9c12086273bf86ac1b3f72beebd17cc357bb749a95ac64d0f5ecdbbe7631cec4 in / 
# Tue, 04 Jul 2023 01:33:29 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 12:50:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 12:50:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3dcb3b9eb8abea3e1994db2e9f2073832965384334d3e204d1df1e3dcd09cffa`  
		Last Modified: Tue, 04 Jul 2023 01:38:16 GMT  
		Size: 47.9 MB (47890767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d5c8c8644c840146ba18a3d20250a3f49997785afe106720a31e6e3bc0bdcf`  
		Last Modified: Tue, 04 Jul 2023 13:07:16 GMT  
		Size: 25.2 MB (25169956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac95edda4f2261a710fe6cece76ae1adadaa655ad92be633a48ffbfffceaba9`  
		Last Modified: Tue, 04 Jul 2023 13:07:30 GMT  
		Size: 63.8 MB (63777301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stable`

```console
$ docker pull buildpack-deps@sha256:e8045f6c5b35d465af4400cf07baf28937774c70d0b67b75db9aa5a772245507
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

### `buildpack-deps:stable` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:9fa042ef286f67914fb32a3dc539a9a9011d3030d11178a287fec058f4af2e0d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.7 MB (348696237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:870f7a6134d053997696565f36185aa08d0268c5d2ead2098c03ec2543d8c186`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:19:44 GMT
ADD file:5d17ca085473e890bd6eca4abf6d324c3181f80692523b83ef25d1c42576b99f in / 
# Tue, 04 Jul 2023 01:19:44 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:27:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:28:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:29:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d52e4f012db158bb7c0fe215b98af1facaddcbaee530efd69b1bae07d597b711`  
		Last Modified: Tue, 04 Jul 2023 01:24:39 GMT  
		Size: 49.6 MB (49551432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd206bea61ff3e3b54be1c20b58d8475ddd6f89df176146ddb7a2fd2c747ea2`  
		Last Modified: Tue, 04 Jul 2023 03:51:23 GMT  
		Size: 24.0 MB (24030593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2320f9be4a9c605d1ac847cf67cec42b91484a7cf7c94996417a0c7c316deadc`  
		Last Modified: Tue, 04 Jul 2023 03:51:42 GMT  
		Size: 64.1 MB (64111613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5565e0ba8dfce32b9049f21ceeb212946e0bb810d94cbd2db94ca61082f657`  
		Last Modified: Tue, 04 Jul 2023 03:52:18 GMT  
		Size: 211.0 MB (211002599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:7630e74069ab9afc052421fab33b53a63046a9f0a81ca78e752b60f0bf5e6f30
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.0 MB (315974639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efd6d55edc39161f4227507b095e44656ca35b9df7ba73a742e6d46ac8dcbac8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:48:22 GMT
ADD file:09001854dc5081f907ac2a66d301e4b3d6b4bf2c2483aad5395a535bf068698d in / 
# Tue, 04 Jul 2023 00:48:22 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:21:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:21:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:24:09 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7e0a1f476b42bcc214197ec9c5ef753ddf2ab36a314416a6ac96cd921ff0d41d`  
		Last Modified: Tue, 04 Jul 2023 00:51:29 GMT  
		Size: 47.4 MB (47402786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68311cc5ff511aa59283fdd7f1e25bc33dfc3ad9ae87e5c94447f36c3f7c4817`  
		Last Modified: Tue, 04 Jul 2023 04:28:32 GMT  
		Size: 22.7 MB (22708933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09518fc93ba137cac901dd7b0cc5fab1e20a21a7d6bbe3a35b7f921a069ddc5c`  
		Last Modified: Tue, 04 Jul 2023 04:28:53 GMT  
		Size: 61.6 MB (61553936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0a9d5bee850aae2d389dee19882ddf586d298ba8cc4d4100b77a7bc33204f0`  
		Last Modified: Tue, 04 Jul 2023 04:29:28 GMT  
		Size: 184.3 MB (184308984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:ccbb43b6d2ff2010f6972b17d2c35e80179b93721b3b4075a83d17fd211df4d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.4 MB (301419261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71ba632fe6ed398564cb984e2524c39cfe7c23c5d5ce9b754516330315011653`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:57:42 GMT
ADD file:279ef7213d41f1f7ae76bd76293a5107fd1f8caf557f837cab9c834d2841e031 in / 
# Tue, 04 Jul 2023 00:57:43 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:49:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:50:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:51:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b9bdcf1a9a6361f231594c76a75bfb4c2fef5f9745b9713bbd50efaf37ca11b8`  
		Last Modified: Tue, 04 Jul 2023 01:02:26 GMT  
		Size: 45.2 MB (45236201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8ee33ea63b2391e912423c14b2f1e789137ffb03659568cb361a2fa2b4efbd`  
		Last Modified: Tue, 04 Jul 2023 06:18:41 GMT  
		Size: 21.9 MB (21936446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2a5b4416a84ac4585c3e3879ca49a6fc3e8d46028a4f27098ae1bdb4ae710d`  
		Last Modified: Tue, 04 Jul 2023 06:19:01 GMT  
		Size: 59.3 MB (59261674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfb211eb5b07ec381fa590fdb20338a17e1ac7282488bfe67ebf61eb9d8ef36`  
		Last Modified: Tue, 04 Jul 2023 06:19:36 GMT  
		Size: 175.0 MB (174984940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a11d7b66e7e9ee6221856ac61d5a24ac2fa826652e2ad6decc9068462572a119
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.5 MB (339524386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41b72a638a02bcfb5b6fb54590f95199209e6bb9e8ba83b5675a76bdd3a62b4d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:26 GMT
ADD file:ab1761d899751c4d24e15179fc9e7e7ac3fb83798ee37ca13d6a6ac44fbeded3 in / 
# Tue, 04 Jul 2023 01:57:27 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:54:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:54:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:56:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:42cbebf8bc116ba1aed7897e2d0566bf49da9d5c70be71b6a7cb07805d2f5b7a`  
		Last Modified: Tue, 04 Jul 2023 02:00:57 GMT  
		Size: 49.6 MB (49572781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0518ec57568a70561f7c04650f9554c88dada973f54d88e36f65b0796d35de`  
		Last Modified: Tue, 04 Jul 2023 06:21:03 GMT  
		Size: 23.6 MB (23569546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356172c718acf9930d9465b170864319079e2d2ebac0ddef781d64e85789531e`  
		Last Modified: Tue, 04 Jul 2023 06:21:20 GMT  
		Size: 64.0 MB (63984075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dddcd3ceb9980caac379e8f8eeafe1e901f017e5768b867705a0834cc1274efa`  
		Last Modified: Tue, 04 Jul 2023 06:21:49 GMT  
		Size: 202.4 MB (202397984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:bd112b098fcf0109e2d3d75cb01da9035f9aa2b763863b2be966c3c1a892b655
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.3 MB (351325313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a527ba005f783dc8585ad58568efedd0ad8a89a20c2877cd3b9cd5bfc634702`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:38:25 GMT
ADD file:e0a25fe261e09183ec383698ab2c800f93c5b0805564d7104ad5119db52cccb7 in / 
# Tue, 04 Jul 2023 01:38:25 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:28:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:28:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:30:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:381263dab43af8bfb8e85c7a9a32f35492cbdcc3a046b35f947cf3bf3a55f4c1`  
		Last Modified: Tue, 04 Jul 2023 01:43:02 GMT  
		Size: 50.6 MB (50562388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af522778d6fcd5f4b85dafb1f21b89441dedee6ce875890b15ad8c454bbb9fe6`  
		Last Modified: Tue, 04 Jul 2023 05:38:10 GMT  
		Size: 24.9 MB (24869747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501f685d713d76bdc0731a917b074d79f3de7c84bfe09c53585642801175a72f`  
		Last Modified: Tue, 04 Jul 2023 05:38:34 GMT  
		Size: 66.0 MB (65972310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993e54703a4428a35a92b50b46a2b72088e5f98ec8687291e59ba960778653ce`  
		Last Modified: Tue, 04 Jul 2023 05:39:21 GMT  
		Size: 209.9 MB (209920868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:109dccdd704f2335380eafe52886c571b5ecc9fc6f8e8ff477f178f88a1bcd3a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.7 MB (325698556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63ff7002fa7f867935af5542ea11c588ff00e71b610322da6f1ee76d404f1372`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:08:42 GMT
ADD file:c567fc0f97f36ea531c05e159cd6ac2a8747f14ea5b6ccae39bab9d305da180d in / 
# Tue, 04 Jul 2023 01:08:47 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:34:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:36:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:42:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76240e493592cbc7ca56583a6e8e03ab12a967b65bbeb1df7828a5099fa271d9`  
		Last Modified: Tue, 04 Jul 2023 01:19:16 GMT  
		Size: 49.5 MB (49542143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85086244c52affe40f860feee6e34c03fd0f782e853b00950f1a9b8b6704d24f`  
		Last Modified: Tue, 04 Jul 2023 14:56:03 GMT  
		Size: 23.6 MB (23611680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2482ef924bba9e0b7ef4ad15506bbcf2a7db029acfc793f94b5d17435ed529`  
		Last Modified: Tue, 04 Jul 2023 14:56:55 GMT  
		Size: 63.0 MB (62950425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a976801f0e288a1695ce313557e999ec73ed5562492816ed2e559f8fadcba08`  
		Last Modified: Tue, 04 Jul 2023 14:58:59 GMT  
		Size: 189.6 MB (189594308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d118d12ab7bda84f249868aa497f83e1ee8489b9062b3d275991f7c9178fb44a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.8 MB (362817855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07b0cde07b2b8c19168a241b2b585bba6b27c80cdb9761dfd1dcba9a1d952f9f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:17:23 GMT
ADD file:5aaa642008df5a97014e76042a767f06bbfda91db1d5f336a1b3f98e9b11c7a1 in / 
# Tue, 04 Jul 2023 01:17:26 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:26:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:27:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:32:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e039cf6634cf83a31e97e2a56b4db40a8c38a62d6857c77e687d5edb3eb0dfde`  
		Last Modified: Tue, 04 Jul 2023 01:23:59 GMT  
		Size: 53.5 MB (53536740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54fff62f5ff539ace95f1581096d57b95ca024b9d5cc7c85bb4a2bf159ad845f`  
		Last Modified: Tue, 04 Jul 2023 04:36:20 GMT  
		Size: 25.7 MB (25681297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd5a2ec3d78fd420afc5e1c6739ad59505cf484be0ea1c2c2dfe00c7b2c00ec`  
		Last Modified: Tue, 04 Jul 2023 04:36:52 GMT  
		Size: 69.6 MB (69569498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c3418743f63acf6f2325abc19057fd064d786b061702494a8afd12dba2787ca`  
		Last Modified: Tue, 04 Jul 2023 04:37:57 GMT  
		Size: 214.0 MB (214030320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:8ae64baa0daee2c34ad05f273d64404d1daf9cbdcb9cf75baa84eaeee3aa34ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.1 MB (318132923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:208c88d3645147348e10f8100a5ad65a12fb037cebe1b20bfa7551fee026e98c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:31:54 GMT
ADD file:0ad7ffbe777e5367ad6dcbb4a182e1d578739aa7a4853f82f21bd71d824de7ae in / 
# Tue, 04 Jul 2023 01:31:56 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 12:47:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 12:47:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 12:48:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce9d001c0d31ec9b8072b1a9bd01771a10ea8ddfefa381cf9ce7e2d63538aaeb`  
		Last Modified: Tue, 04 Jul 2023 01:36:50 GMT  
		Size: 47.9 MB (47921709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024bda56b20d3018344098f67965337568b532ea03f09d87858a2bb5eae82bf7`  
		Last Modified: Tue, 04 Jul 2023 13:05:34 GMT  
		Size: 24.0 MB (24028793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da5b83dc971cc08c6baeb1ddd5fb5de06beefef83c0444c224b4e377d704705`  
		Last Modified: Tue, 04 Jul 2023 13:05:50 GMT  
		Size: 63.1 MB (63112809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3bc88ad73a4c8df0ca6b17f424b27e05a29533428b9a47f3576c9be9e81540c`  
		Last Modified: Tue, 04 Jul 2023 13:06:19 GMT  
		Size: 183.1 MB (183069612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stable-curl`

```console
$ docker pull buildpack-deps@sha256:5df62ac377f1dca70c63bb04aeacf175f11265542a35a451d592255cc0e38972
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

### `buildpack-deps:stable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:4ce7e846f60727efea42b5abdfd8673e13a94e288c6a5d7c37da1973ce7c5d78
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73582025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c399a665f317215e5dd18dcf72a1723bc891edc5df1e57bf176d1c65f757cd0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:19:44 GMT
ADD file:5d17ca085473e890bd6eca4abf6d324c3181f80692523b83ef25d1c42576b99f in / 
# Tue, 04 Jul 2023 01:19:44 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:27:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d52e4f012db158bb7c0fe215b98af1facaddcbaee530efd69b1bae07d597b711`  
		Last Modified: Tue, 04 Jul 2023 01:24:39 GMT  
		Size: 49.6 MB (49551432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd206bea61ff3e3b54be1c20b58d8475ddd6f89df176146ddb7a2fd2c747ea2`  
		Last Modified: Tue, 04 Jul 2023 03:51:23 GMT  
		Size: 24.0 MB (24030593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:cd79b4dbc7daadcec5980ed2d535ce9340c36adea17ccf7dbb0c0d2712ca57e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.1 MB (70111719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dea85fcb87a6435ababbbc09b75d697c82c737049086f3d59690dca803e1758d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:48:22 GMT
ADD file:09001854dc5081f907ac2a66d301e4b3d6b4bf2c2483aad5395a535bf068698d in / 
# Tue, 04 Jul 2023 00:48:22 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:21:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7e0a1f476b42bcc214197ec9c5ef753ddf2ab36a314416a6ac96cd921ff0d41d`  
		Last Modified: Tue, 04 Jul 2023 00:51:29 GMT  
		Size: 47.4 MB (47402786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68311cc5ff511aa59283fdd7f1e25bc33dfc3ad9ae87e5c94447f36c3f7c4817`  
		Last Modified: Tue, 04 Jul 2023 04:28:32 GMT  
		Size: 22.7 MB (22708933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:ee52b93b57b097abb318a077905af9d187e98a1feb6c49f47ad7368f254dac9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67172647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7745cabe6a186fe38c73aa2d5384961dc430b541f6f0ccee40bb24c7865441c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:57:42 GMT
ADD file:279ef7213d41f1f7ae76bd76293a5107fd1f8caf557f837cab9c834d2841e031 in / 
# Tue, 04 Jul 2023 00:57:43 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:49:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b9bdcf1a9a6361f231594c76a75bfb4c2fef5f9745b9713bbd50efaf37ca11b8`  
		Last Modified: Tue, 04 Jul 2023 01:02:26 GMT  
		Size: 45.2 MB (45236201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8ee33ea63b2391e912423c14b2f1e789137ffb03659568cb361a2fa2b4efbd`  
		Last Modified: Tue, 04 Jul 2023 06:18:41 GMT  
		Size: 21.9 MB (21936446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c6b1b12d88f18474b52830b7189f2d54b534002ee9b00dbe7a5947684dbbef4d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.1 MB (73142327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ccf74d87c178f322cc3cc0e5b79bb62adfcb518a1c78943c8a7d7241427f748`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:26 GMT
ADD file:ab1761d899751c4d24e15179fc9e7e7ac3fb83798ee37ca13d6a6ac44fbeded3 in / 
# Tue, 04 Jul 2023 01:57:27 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:54:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:42cbebf8bc116ba1aed7897e2d0566bf49da9d5c70be71b6a7cb07805d2f5b7a`  
		Last Modified: Tue, 04 Jul 2023 02:00:57 GMT  
		Size: 49.6 MB (49572781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0518ec57568a70561f7c04650f9554c88dada973f54d88e36f65b0796d35de`  
		Last Modified: Tue, 04 Jul 2023 06:21:03 GMT  
		Size: 23.6 MB (23569546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:abb0cf0f3dc36c7e284598893d32388fe2b09b68e02ef75869a6ddce988d6624
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75432135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce569bff52f1ef304acf004cee953e9829211468502cb021457f297c7f8d098d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:38:25 GMT
ADD file:e0a25fe261e09183ec383698ab2c800f93c5b0805564d7104ad5119db52cccb7 in / 
# Tue, 04 Jul 2023 01:38:25 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:28:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:381263dab43af8bfb8e85c7a9a32f35492cbdcc3a046b35f947cf3bf3a55f4c1`  
		Last Modified: Tue, 04 Jul 2023 01:43:02 GMT  
		Size: 50.6 MB (50562388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af522778d6fcd5f4b85dafb1f21b89441dedee6ce875890b15ad8c454bbb9fe6`  
		Last Modified: Tue, 04 Jul 2023 05:38:10 GMT  
		Size: 24.9 MB (24869747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:daeb0fffa382ebd3757c35f7edef327defb7d926134b88529b5ac12bfe9bda74
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73153823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe85240ea372bde5df08e1b08faeb8632ed7dedae4aba518ab2d7bc1488ca70e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:08:42 GMT
ADD file:c567fc0f97f36ea531c05e159cd6ac2a8747f14ea5b6ccae39bab9d305da180d in / 
# Tue, 04 Jul 2023 01:08:47 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:34:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76240e493592cbc7ca56583a6e8e03ab12a967b65bbeb1df7828a5099fa271d9`  
		Last Modified: Tue, 04 Jul 2023 01:19:16 GMT  
		Size: 49.5 MB (49542143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85086244c52affe40f860feee6e34c03fd0f782e853b00950f1a9b8b6704d24f`  
		Last Modified: Tue, 04 Jul 2023 14:56:03 GMT  
		Size: 23.6 MB (23611680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:dd742426422d9d9c53b1f294d91895bd56b7748b0a559826babb53cec399ddef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.2 MB (79218037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4572b0656e7dfc6731b3f7dd64ee5baeb3421d7762079b77c60f1226bfa152f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:17:23 GMT
ADD file:5aaa642008df5a97014e76042a767f06bbfda91db1d5f336a1b3f98e9b11c7a1 in / 
# Tue, 04 Jul 2023 01:17:26 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:26:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e039cf6634cf83a31e97e2a56b4db40a8c38a62d6857c77e687d5edb3eb0dfde`  
		Last Modified: Tue, 04 Jul 2023 01:23:59 GMT  
		Size: 53.5 MB (53536740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54fff62f5ff539ace95f1581096d57b95ca024b9d5cc7c85bb4a2bf159ad845f`  
		Last Modified: Tue, 04 Jul 2023 04:36:20 GMT  
		Size: 25.7 MB (25681297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:d5f47922100fab7fa779f085640d993e6625e6f15956c228a3b1475b38baf460
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.0 MB (71950502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ebcb0cef8f138e8e985dd005eeee2dd6d64c40eef9668d4b648caec9ec37c6a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:31:54 GMT
ADD file:0ad7ffbe777e5367ad6dcbb4a182e1d578739aa7a4853f82f21bd71d824de7ae in / 
# Tue, 04 Jul 2023 01:31:56 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 12:47:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce9d001c0d31ec9b8072b1a9bd01771a10ea8ddfefa381cf9ce7e2d63538aaeb`  
		Last Modified: Tue, 04 Jul 2023 01:36:50 GMT  
		Size: 47.9 MB (47921709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024bda56b20d3018344098f67965337568b532ea03f09d87858a2bb5eae82bf7`  
		Last Modified: Tue, 04 Jul 2023 13:05:34 GMT  
		Size: 24.0 MB (24028793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stable-scm`

```console
$ docker pull buildpack-deps@sha256:12a2678b3eabf425fa2c142421e1db4dfe6ab854a537af91c289507745c71b36
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

### `buildpack-deps:stable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:0f78de2b3312f09866ac4eaaba883d518e886b540ceeff548750914b935f8e50
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.7 MB (137693638 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:064924f22ba6cc021e9ca9ae3e10d21b15e491c0d1387c5f62300c70241c04d1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:19:44 GMT
ADD file:5d17ca085473e890bd6eca4abf6d324c3181f80692523b83ef25d1c42576b99f in / 
# Tue, 04 Jul 2023 01:19:44 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:27:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:28:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d52e4f012db158bb7c0fe215b98af1facaddcbaee530efd69b1bae07d597b711`  
		Last Modified: Tue, 04 Jul 2023 01:24:39 GMT  
		Size: 49.6 MB (49551432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd206bea61ff3e3b54be1c20b58d8475ddd6f89df176146ddb7a2fd2c747ea2`  
		Last Modified: Tue, 04 Jul 2023 03:51:23 GMT  
		Size: 24.0 MB (24030593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2320f9be4a9c605d1ac847cf67cec42b91484a7cf7c94996417a0c7c316deadc`  
		Last Modified: Tue, 04 Jul 2023 03:51:42 GMT  
		Size: 64.1 MB (64111613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:27d15e25a27b8983778bfedc271e37fbf73269e16b907efc0f8c0a4af8c912b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.7 MB (131665655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dac77eebbb12f590d8e6de52e972d43c54544315b77364e7101d186dd5aad91c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:48:22 GMT
ADD file:09001854dc5081f907ac2a66d301e4b3d6b4bf2c2483aad5395a535bf068698d in / 
# Tue, 04 Jul 2023 00:48:22 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:21:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:21:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7e0a1f476b42bcc214197ec9c5ef753ddf2ab36a314416a6ac96cd921ff0d41d`  
		Last Modified: Tue, 04 Jul 2023 00:51:29 GMT  
		Size: 47.4 MB (47402786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68311cc5ff511aa59283fdd7f1e25bc33dfc3ad9ae87e5c94447f36c3f7c4817`  
		Last Modified: Tue, 04 Jul 2023 04:28:32 GMT  
		Size: 22.7 MB (22708933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09518fc93ba137cac901dd7b0cc5fab1e20a21a7d6bbe3a35b7f921a069ddc5c`  
		Last Modified: Tue, 04 Jul 2023 04:28:53 GMT  
		Size: 61.6 MB (61553936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:36fa95975190dc678d40a37a93185f66e9192b8c80dec22c959399e2f7ec2569
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.4 MB (126434321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3da8a85987ffb7432f4d6f66364a39ac772f3a9b6bff23ba597689223f28b4b3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:57:42 GMT
ADD file:279ef7213d41f1f7ae76bd76293a5107fd1f8caf557f837cab9c834d2841e031 in / 
# Tue, 04 Jul 2023 00:57:43 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:49:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:50:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b9bdcf1a9a6361f231594c76a75bfb4c2fef5f9745b9713bbd50efaf37ca11b8`  
		Last Modified: Tue, 04 Jul 2023 01:02:26 GMT  
		Size: 45.2 MB (45236201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a8ee33ea63b2391e912423c14b2f1e789137ffb03659568cb361a2fa2b4efbd`  
		Last Modified: Tue, 04 Jul 2023 06:18:41 GMT  
		Size: 21.9 MB (21936446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2a5b4416a84ac4585c3e3879ca49a6fc3e8d46028a4f27098ae1bdb4ae710d`  
		Last Modified: Tue, 04 Jul 2023 06:19:01 GMT  
		Size: 59.3 MB (59261674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a5cb7353b2ce88aeffff9c11400ba2868c5da3edae5c9ee5c2c4c09312ced7e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.1 MB (137126402 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb40501a95e932bb48d49f74d197ea8377d1ccba9e2dd9f66e63fdf9de21b409`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:26 GMT
ADD file:ab1761d899751c4d24e15179fc9e7e7ac3fb83798ee37ca13d6a6ac44fbeded3 in / 
# Tue, 04 Jul 2023 01:57:27 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:54:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:54:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:42cbebf8bc116ba1aed7897e2d0566bf49da9d5c70be71b6a7cb07805d2f5b7a`  
		Last Modified: Tue, 04 Jul 2023 02:00:57 GMT  
		Size: 49.6 MB (49572781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0518ec57568a70561f7c04650f9554c88dada973f54d88e36f65b0796d35de`  
		Last Modified: Tue, 04 Jul 2023 06:21:03 GMT  
		Size: 23.6 MB (23569546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356172c718acf9930d9465b170864319079e2d2ebac0ddef781d64e85789531e`  
		Last Modified: Tue, 04 Jul 2023 06:21:20 GMT  
		Size: 64.0 MB (63984075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:e93d1e1d0a091272e88d7d8bf0e0e21b3df095765d52c1007b9bbab8d01069f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.4 MB (141404445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d40934ac087de93ceffbf81437543947fc9c9c8b8184568346ac03da80f35bd7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:38:25 GMT
ADD file:e0a25fe261e09183ec383698ab2c800f93c5b0805564d7104ad5119db52cccb7 in / 
# Tue, 04 Jul 2023 01:38:25 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:28:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:28:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:381263dab43af8bfb8e85c7a9a32f35492cbdcc3a046b35f947cf3bf3a55f4c1`  
		Last Modified: Tue, 04 Jul 2023 01:43:02 GMT  
		Size: 50.6 MB (50562388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af522778d6fcd5f4b85dafb1f21b89441dedee6ce875890b15ad8c454bbb9fe6`  
		Last Modified: Tue, 04 Jul 2023 05:38:10 GMT  
		Size: 24.9 MB (24869747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501f685d713d76bdc0731a917b074d79f3de7c84bfe09c53585642801175a72f`  
		Last Modified: Tue, 04 Jul 2023 05:38:34 GMT  
		Size: 66.0 MB (65972310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:68087f9d2d7eb43f96f073504d68e5f68181fe9c905f47fb14815bec8db79572
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.1 MB (136104248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0d288a207994f6184d90c784bdde0152350cd4c6bf91f0777b8da30da1a0c3e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:08:42 GMT
ADD file:c567fc0f97f36ea531c05e159cd6ac2a8747f14ea5b6ccae39bab9d305da180d in / 
# Tue, 04 Jul 2023 01:08:47 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:34:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:36:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76240e493592cbc7ca56583a6e8e03ab12a967b65bbeb1df7828a5099fa271d9`  
		Last Modified: Tue, 04 Jul 2023 01:19:16 GMT  
		Size: 49.5 MB (49542143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85086244c52affe40f860feee6e34c03fd0f782e853b00950f1a9b8b6704d24f`  
		Last Modified: Tue, 04 Jul 2023 14:56:03 GMT  
		Size: 23.6 MB (23611680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2482ef924bba9e0b7ef4ad15506bbcf2a7db029acfc793f94b5d17435ed529`  
		Last Modified: Tue, 04 Jul 2023 14:56:55 GMT  
		Size: 63.0 MB (62950425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:a1876fdc603fdf011be6b83ff792c330a17e2743922fd5aabaf6a1ed5c037080
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.8 MB (148787535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62c051da923c5734b37ef3d706b3ecdfe384634edc45b782adb0b0e0f06f84db`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:17:23 GMT
ADD file:5aaa642008df5a97014e76042a767f06bbfda91db1d5f336a1b3f98e9b11c7a1 in / 
# Tue, 04 Jul 2023 01:17:26 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:26:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:27:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e039cf6634cf83a31e97e2a56b4db40a8c38a62d6857c77e687d5edb3eb0dfde`  
		Last Modified: Tue, 04 Jul 2023 01:23:59 GMT  
		Size: 53.5 MB (53536740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54fff62f5ff539ace95f1581096d57b95ca024b9d5cc7c85bb4a2bf159ad845f`  
		Last Modified: Tue, 04 Jul 2023 04:36:20 GMT  
		Size: 25.7 MB (25681297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd5a2ec3d78fd420afc5e1c6739ad59505cf484be0ea1c2c2dfe00c7b2c00ec`  
		Last Modified: Tue, 04 Jul 2023 04:36:52 GMT  
		Size: 69.6 MB (69569498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:26e61b2a6df1a810689cbf8a1b2b097496c6de014ff7013b8f3c0466dc100308
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.1 MB (135063311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:875d66c05f546cc0a92a5aed5599d58335c22c67b0706c82bc06056c3af12657`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:31:54 GMT
ADD file:0ad7ffbe777e5367ad6dcbb4a182e1d578739aa7a4853f82f21bd71d824de7ae in / 
# Tue, 04 Jul 2023 01:31:56 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 12:47:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 12:47:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce9d001c0d31ec9b8072b1a9bd01771a10ea8ddfefa381cf9ce7e2d63538aaeb`  
		Last Modified: Tue, 04 Jul 2023 01:36:50 GMT  
		Size: 47.9 MB (47921709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024bda56b20d3018344098f67965337568b532ea03f09d87858a2bb5eae82bf7`  
		Last Modified: Tue, 04 Jul 2023 13:05:34 GMT  
		Size: 24.0 MB (24028793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da5b83dc971cc08c6baeb1ddd5fb5de06beefef83c0444c224b4e377d704705`  
		Last Modified: Tue, 04 Jul 2023 13:05:50 GMT  
		Size: 63.1 MB (63112809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:unstable`

```console
$ docker pull buildpack-deps@sha256:bdb6490a62623952a85a6e205d00be1168a5573d1654942fb8145cec9f795f42
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

### `buildpack-deps:unstable` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:528b5311a9ae6696bcd00391123c4bc54f3b31b58c58e64d74bc86267eb03278
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.5 MB (351457721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b9832bf13f8edec5c1794ddc2768c54640f872d1d3ba82cf610164cf5a2e673`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:22:34 GMT
ADD file:8ed2c72091b90575b320038c2ad715760d6382aeea5c416dd16f7ed04e955217 in / 
# Mon, 12 Jun 2023 23:22:35 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:34:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:34:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:35:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2e79cba44192968ca6ea42058e67723ae58bebd2ea54b31f432b1ffed9fea9d9`  
		Last Modified: Mon, 12 Jun 2023 23:28:29 GMT  
		Size: 49.6 MB (49551965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cda7b25305de24c8cc4e88d990c3c3c70e109b190f7411b9d3237528081a161`  
		Last Modified: Tue, 13 Jun 2023 03:39:26 GMT  
		Size: 24.0 MB (24019326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c71d2bfd3c86199eb06493b2f6d0258d7576aca3f851198b940bb3b1505989`  
		Last Modified: Tue, 13 Jun 2023 03:39:43 GMT  
		Size: 64.5 MB (64535333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75a9b221ba575bef197107054a01083b3dc2b0d4bedc07f7e6c3fcbde4df462`  
		Last Modified: Tue, 13 Jun 2023 03:40:16 GMT  
		Size: 213.4 MB (213351097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:425577d4371532d7a1016ddbb8661097ceb1b3d84c34fd7797ae4b12cd690ad2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.2 MB (318155740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b0af6d02dd2c68e48fc43dcbeca22913a6160330fab418584d083f8d500e97b`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:49:10 GMT
ADD file:b79d69fc6594f6ca5e9e76165017858724482b88aa3aa49e3db7b07a3dcabc0a in / 
# Mon, 12 Jun 2023 23:49:11 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 07:40:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:40:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:41:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:13ee4e7971510c95d7e625030699b854921da16f6d5ef29884b269a308a37afc`  
		Last Modified: Mon, 12 Jun 2023 23:52:56 GMT  
		Size: 47.4 MB (47417325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8374a5ed08b072c6f518c88ddf07dd3d9e04e3ccc51d0810b12cd2ae53c998`  
		Last Modified: Tue, 13 Jun 2023 07:44:30 GMT  
		Size: 23.6 MB (23622159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c640f3b5ffb5f4fc9722d6fca3f771a8db79e177cf1b0cfd035587f4d4dcf4ae`  
		Last Modified: Tue, 13 Jun 2023 07:44:48 GMT  
		Size: 62.2 MB (62150140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638239f1655f4299ec88f74ea4b5a44b44817cf56b426104a7b6e23df2031def`  
		Last Modified: Tue, 13 Jun 2023 07:45:23 GMT  
		Size: 185.0 MB (184966116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:bc482d01bcfba9d59704601f01b9f3890277671f0f5ae65064ffc8bfd8a092bc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.0 MB (301978210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:993c7c66f179e1f8a499111f4da05a053490bbe72ab3e5d29a35162ec157f3cf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jun 2023 00:00:33 GMT
ADD file:82567bde3caa9ad83c0c12c0525e6fd51cc833f0b29e733c2da572ed00150220 in / 
# Tue, 13 Jun 2023 00:00:39 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 05:00:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:00:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:01:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1d80e7ebc54969ad575378cf66dc58999cbf341e0d2a92c9ff0bfd5b3b9fb1c3`  
		Last Modified: Tue, 13 Jun 2023 00:06:30 GMT  
		Size: 45.2 MB (45234838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a26e461ec0e64583c2acfbef48942f57c9de9da65ff1a078a62e910baf3ce05`  
		Last Modified: Tue, 13 Jun 2023 05:05:32 GMT  
		Size: 21.9 MB (21922951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4da543e1cb7517b023e6ef07f0f0385da6f0c3f832cfd7ade1c7381c2ffe580b`  
		Last Modified: Tue, 13 Jun 2023 05:05:49 GMT  
		Size: 59.8 MB (59799388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a6dd7ea367162c4002f5bdde6db8bbbef4671fde6486cf888d7a0bb5c07e29`  
		Last Modified: Tue, 13 Jun 2023 05:06:19 GMT  
		Size: 175.0 MB (175021033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:9b1e52d6511e5cfbcb6ad379788c4aba30e2dd9ab3e9909a0843477506f3d785
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **340.1 MB (340130427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4578dc30c4d05d7a1fed527a3d742d540a2f37c1cbac255db25eb945baf702b1`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:41:38 GMT
ADD file:94f1432513f9a03b38028af02b1d1720fb0558559faf3e7f9d7097cf6b962056 in / 
# Mon, 12 Jun 2023 23:41:39 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:05:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:05:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:06:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8ba9ab3e6f12b9702649c2e0c7d78e22ffb9183f68c288b9edef2387bd8d4efd`  
		Last Modified: Mon, 12 Jun 2023 23:46:36 GMT  
		Size: 49.6 MB (49592096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:393fb89bae1d5f0307a283cb7c3b5f54cc63fde2e90b7b65ceae29bcd27126f5`  
		Last Modified: Tue, 13 Jun 2023 03:10:09 GMT  
		Size: 23.6 MB (23558237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4483fcef438011d245d9be3906ab5e6a92c139027fe4286dc7e46b975299183`  
		Last Modified: Tue, 13 Jun 2023 03:10:24 GMT  
		Size: 64.5 MB (64490917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cddf934afceb08172df763ffcde92b9665c3c8ae9c4810b008715669ad3d58e`  
		Last Modified: Tue, 13 Jun 2023 03:10:52 GMT  
		Size: 202.5 MB (202489177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:b4764a5e07b05e2bdd8d6d90fa4ff2e34c122e475fc4aa317242bebe454cba77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **353.6 MB (353591470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27e185958c518f02129b840a8ea93d9703f29c31e0bb0ee3ca1e71acfb27d11b`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:42:10 GMT
ADD file:209e3bb955801ad81eb18a280f9fbd5500a0e1f04565e6c94c9cd24dcba4c0af in / 
# Mon, 12 Jun 2023 23:42:10 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 01:09:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 01:09:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 01:10:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8bce10b6f772acc79b03d87add4bd359f98c767e3599f82d8e351cced14c1a11`  
		Last Modified: Mon, 12 Jun 2023 23:49:26 GMT  
		Size: 50.6 MB (50562699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d6b7d433b6a8b07b01e4b262b82f2b882380e41bcd3a6e8b88ca32ea66321e`  
		Last Modified: Tue, 13 Jun 2023 01:15:14 GMT  
		Size: 24.9 MB (24858532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1c9493cccdfcd2c44a013f62ecc08283137f3fd2d7a483cf56387dc987b536`  
		Last Modified: Tue, 13 Jun 2023 01:15:36 GMT  
		Size: 66.4 MB (66355536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e30574996c34012fa193dace0f01bb334e773810647079cb6d2a76b7945342d`  
		Last Modified: Tue, 13 Jun 2023 01:16:23 GMT  
		Size: 211.8 MB (211814703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:0d42590a778653226abaaaeba3e4d95d9f165e2cb3520044566e699afa0f811f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.3 MB (326264556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:732624570cf9a1dec3651b64baba5195328bdb63e629cb11fed831a9a8341e59`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jun 2023 00:12:52 GMT
ADD file:b2a9cefcdd223b4cbf9b1abac81e8c0c158a24f9c272910a8822619ea9d55ae9 in / 
# Tue, 13 Jun 2023 00:12:57 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 02:12:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 02:13:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 02:19:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:65733d4f161a7d2fd9cef6d80eb7fe00897e936eb78d018361809f7384b08c28`  
		Last Modified: Tue, 13 Jun 2023 00:25:52 GMT  
		Size: 49.6 MB (49561285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8cac982d96cd0724a1a282faecd42ae997cf2e6c468441bdcf2ce718f092f4d`  
		Last Modified: Tue, 13 Jun 2023 02:26:09 GMT  
		Size: 23.6 MB (23606470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec621985ebc463298904a643b89d8805cdefe9a156edc65db797295bf5ce37d`  
		Last Modified: Tue, 13 Jun 2023 02:26:58 GMT  
		Size: 63.4 MB (63449697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43067e7ef8f78b7740cb05aa82b22965d78ae240348e6c33c24dca2d27e8f056`  
		Last Modified: Tue, 13 Jun 2023 02:29:12 GMT  
		Size: 189.6 MB (189647104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:eacd16ff9356ba0c57dfa909efcc62d6405fa44679146f06c15e26d48ec5c4a1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **365.8 MB (365821306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e00dce918605ba965c51b6e622e0516b98b712cdb92b58dee885ac0e9d72b0b0`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:19:31 GMT
ADD file:aded196ce7e0c005fe55d5a92492be8cc5d7934fac082b7ab95b8c946e71e0a2 in / 
# Mon, 12 Jun 2023 23:19:34 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 07:34:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:35:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:38:16 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e3f8e732e00762188b5ba00db7db3f36c97d0fccdf3d6121db4ca1febc7d190`  
		Last Modified: Mon, 12 Jun 2023 23:26:13 GMT  
		Size: 53.6 MB (53558517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3615faaadea50ed31520dc05aeaebf1283ee0aae09227fb97c1a9de87beec2f8`  
		Last Modified: Tue, 13 Jun 2023 07:43:30 GMT  
		Size: 25.7 MB (25673673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cdc90af7293b0d3b333a9a6a8a60e61400bc5577336008e14e772e6041c6bce`  
		Last Modified: Tue, 13 Jun 2023 07:43:56 GMT  
		Size: 70.0 MB (69985119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ffd035648c807001473ccb0f1a04d6d76990ef3e357d8f0b665979b64afe78b`  
		Last Modified: Tue, 13 Jun 2023 07:44:54 GMT  
		Size: 216.6 MB (216603997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:686f023ac15591767c0b4e0500c685efdb6b599766b972305a425e11dcd9a937
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **358.0 MB (357978583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:273cc13afc1bb50107f431972b90d2c10c44f10a0b401ed1207a8378f3fe8675`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:09:05 GMT
ADD file:dc2a1586d12e833e5dc300033838059f3946ddddccde6c62d17cba40536ead15 in / 
# Tue, 04 Jul 2023 01:09:07 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 01:31:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 01:34:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 01:42:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d273b82777a979179469448ba9e255d7f7e1671f28d5610f47e8530093aaa04e`  
		Last Modified: Tue, 04 Jul 2023 01:12:27 GMT  
		Size: 45.7 MB (45695454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f7ece03f0359914c61a65ea80744e3ec92ac1afbb1ddab79b6c7276dae0614`  
		Last Modified: Tue, 04 Jul 2023 01:43:00 GMT  
		Size: 22.3 MB (22287386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e6bfc3fa16d519518bec2169bd35f0eeede077436e581f9c80725f413e6788e`  
		Last Modified: Tue, 04 Jul 2023 01:44:21 GMT  
		Size: 60.1 MB (60140546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91c63bc964adf497f1164977ba456068b24b0b242c5b16276b6bfc9b1723b41`  
		Last Modified: Tue, 04 Jul 2023 01:49:51 GMT  
		Size: 229.9 MB (229855197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b0b9dab7c2e1f21c627113aa1c6b9c21050761ca06e8b97d1d0e19434da79de6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **320.6 MB (320614417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f275f768edd7209671adc00107c2353b50953ca84973ce178959ce461e831127`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jun 2023 04:30:54 GMT
ADD file:7ea0e5c460c626891cd3fc90639d6bfb9a27beeb7f5c79fd9c348c5b6244bd0d in / 
# Tue, 13 Jun 2023 04:30:58 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 18:33:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 18:34:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 18:34:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a129144c9fdcf79f6394b7f7bfa3d7e6a0c8ebfd424dca918695356a1b3bf970`  
		Last Modified: Tue, 13 Jun 2023 04:35:27 GMT  
		Size: 47.9 MB (47920583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d42182bfe271810fa332f879c12433ca046660729997bdce646aa7157138984`  
		Last Modified: Tue, 13 Jun 2023 18:39:25 GMT  
		Size: 24.0 MB (24020404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b53f300fd0adc6e321c844bd2e2fb478de90848743069202361df4928dd446b`  
		Last Modified: Tue, 13 Jun 2023 18:39:39 GMT  
		Size: 63.6 MB (63617737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eeb3234b4fe971e1c4b0c7127991671379ecc9df17d1b611ddf4553cd898f10`  
		Last Modified: Tue, 13 Jun 2023 18:40:07 GMT  
		Size: 185.1 MB (185055693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:unstable-curl`

```console
$ docker pull buildpack-deps@sha256:ac7eb2111638a4f5590c0464e43a1b8f3541fd80e0446f40c46d30f640c882b6
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

### `buildpack-deps:unstable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:1444ecae199d3a84f514fffd3e96a07d956d068d696e22a6668f3a8b7b69bea0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73558597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3b07e6edfec497631a8a3716b0e973fce8f54eb68ded798958b4befa07050d2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:21:50 GMT
ADD file:4bfda8f11e59383c37bfa6038bb5d22f58b9724d249a62568a2e7d2908821cd3 in / 
# Tue, 04 Jul 2023 01:21:50 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:34:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6efa412d16b908043ec01c4ac9ff7323c0f488dd5d7ea4b9b086f1e80350b9b3`  
		Last Modified: Tue, 04 Jul 2023 01:27:46 GMT  
		Size: 49.5 MB (49475944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad8fa89586d6eb7c1bf3add3cde8c80b2da78794ef30be11a97f2dad784809a`  
		Last Modified: Tue, 04 Jul 2023 03:54:24 GMT  
		Size: 24.1 MB (24082653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:d1a9056c98835bada87f4138da4b902136cb795eca133e00ff0b1c407fb52bc1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.1 MB (70080759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a9b5fce7ee5621e0e2234d3e15d91216d47839ce7270d9e7ac54cf651eecc62`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:49:11 GMT
ADD file:e6181e27889c016519d8d701345aafff7138df96a76fb6a29403c8a33a3365fe in / 
# Tue, 04 Jul 2023 00:49:11 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:27:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:667272d8fe1bc81ce33874dbc84976c86d6b95f50198465a6ab672c71d87f666`  
		Last Modified: Tue, 04 Jul 2023 00:53:33 GMT  
		Size: 47.3 MB (47322473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b5934a15453e5e63936a0201a34b820f06d7c27f091dc017bac7d92e1e58d7`  
		Last Modified: Tue, 04 Jul 2023 04:30:42 GMT  
		Size: 22.8 MB (22758286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:b786440d5fa9313cfe4c6e947e1e06bff0b361070ae00db02f93c8a902770278
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67108518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57f38aa572847a45b4cc64179b342a4010030a0cfacec4a3e125ba276bc94ea4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:59:44 GMT
ADD file:5be8eee7722dc860882f26018d8a0de49a4db6fcaa0f35d1dfbb74eff22929cb in / 
# Tue, 04 Jul 2023 00:59:45 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:57:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:42cc2becb0b735f0260d9f678fb1201bbe47c438212c5faf04879fab6a2dd73f`  
		Last Modified: Tue, 04 Jul 2023 01:05:43 GMT  
		Size: 45.1 MB (45123975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5cb3f60ee8390c8cae75e83a5b95ebc4f3589ca1af647965d02fe99b974827b`  
		Last Modified: Tue, 04 Jul 2023 06:21:50 GMT  
		Size: 22.0 MB (21984543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:168cc096593e0cdf7b4e13f9739eb5733adc9069d240de7ed0fe35aeb2a2d2cc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.1 MB (73103142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:344af7b87e9677178d16f959dfdde57f165ec1af4db8ab0e3a034476ef16a070`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:58:49 GMT
ADD file:2c2c0588b93f9af7d93f19033795edf9e61a692ff56e65d9e9500915276782c9 in / 
# Tue, 04 Jul 2023 01:58:50 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:00:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d1b52151d5bb774f3680f8697c343bae1b64b7308354db57dc6bbeb7d65d0964`  
		Last Modified: Tue, 04 Jul 2023 02:03:59 GMT  
		Size: 49.5 MB (49482570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03e94cfcd9a2ac0ccda7b085606ef5174003eb543c68b5bf077a91230b8a7f7`  
		Last Modified: Tue, 04 Jul 2023 06:23:39 GMT  
		Size: 23.6 MB (23620572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:555e0c926152f63f4be81642923a7d416a6db8de6cdeffaf232ce9a51950f704
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75427637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43878012a9d69af31988db85d06eed454cfed8f9f71f7baeaf892725ce675e3e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:40:19 GMT
ADD file:565f8487c71b5de967f1bf16d4bd86291107b68f4152a61e35a8ab86e9f83b7b in / 
# Tue, 04 Jul 2023 01:40:20 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:37:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:46685592106ba6554716942e180f6b4cd8a73f1ec934554b40aee89b47118f5e`  
		Last Modified: Tue, 04 Jul 2023 01:46:32 GMT  
		Size: 50.5 MB (50505825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf3084ac7ee091f26af470878c8197f67d44c09670c27921a26209c909a5c0b`  
		Last Modified: Tue, 04 Jul 2023 05:42:02 GMT  
		Size: 24.9 MB (24921812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:9c445cebfd89383262612bba3ffcd90741aead0f8078a8c553fa99aa51180e70
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.1 MB (73116035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:563c80671a9f694e8c110c810f67d406dc3c68ae2109676af03b778087a4bdc1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:12:32 GMT
ADD file:ab2873cb088258c79fab5dde2d754d1967ca11e58adcf6a08811206759a323d5 in / 
# Tue, 04 Jul 2023 01:12:35 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:52:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:796c2f1009ce9a433d10a1f4708cbb79ef733dcb0ca992041a6aa621e85d8410`  
		Last Modified: Tue, 04 Jul 2023 01:23:15 GMT  
		Size: 49.5 MB (49455398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44357c89fac3bdc147daa7fe48fcf65b83dae0a924631c0b3e9ddb3f7ad71da2`  
		Last Modified: Tue, 04 Jul 2023 15:02:20 GMT  
		Size: 23.7 MB (23660637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:a5807b1f6748c228dc4b2b9be5b8dd6d43925344484a7ac9794dd5a809331ce1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.2 MB (79206895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:985fda4e25a501fb5c76ae42a7c2ebc1fccc03a9dad9be7395da923cac261da5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:19:33 GMT
ADD file:4c1d6f76704d32b9b503bd61c4b485555ec28037fb500403ffb5cbb102cf4509 in / 
# Tue, 04 Jul 2023 01:19:36 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:37:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3e4e6efa69b637e0e8ca00ddcae1aed23aef874a92a2904bdc6c9fa5b3212b8a`  
		Last Modified: Tue, 04 Jul 2023 01:27:02 GMT  
		Size: 53.5 MB (53474414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b5bee4b9196ae6959902bca430113379429a2f075e1553977c6d0442f46233`  
		Last Modified: Tue, 04 Jul 2023 04:39:59 GMT  
		Size: 25.7 MB (25732481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:44d3a4e55beac77f423ed6b86a5ec1b7f0f8420391a51ef5818256b5db0eeda5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.0 MB (67982840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb302f8c83e3c25737152a29d46030f5f78fa08610c71bf94fd362290d41d72d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:09:05 GMT
ADD file:dc2a1586d12e833e5dc300033838059f3946ddddccde6c62d17cba40536ead15 in / 
# Tue, 04 Jul 2023 01:09:07 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 01:31:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d273b82777a979179469448ba9e255d7f7e1671f28d5610f47e8530093aaa04e`  
		Last Modified: Tue, 04 Jul 2023 01:12:27 GMT  
		Size: 45.7 MB (45695454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f7ece03f0359914c61a65ea80744e3ec92ac1afbb1ddab79b6c7276dae0614`  
		Last Modified: Tue, 04 Jul 2023 01:43:00 GMT  
		Size: 22.3 MB (22287386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:f1ec0279f9d18d011062cad1be25abd66e64da40536c135db02b31f9b273289a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.1 MB (73060723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af73a45fd027437fc482806008569b16e9a19209902b6ef1ead753d323426a3c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:33:27 GMT
ADD file:9c12086273bf86ac1b3f72beebd17cc357bb749a95ac64d0f5ecdbbe7631cec4 in / 
# Tue, 04 Jul 2023 01:33:29 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 12:50:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3dcb3b9eb8abea3e1994db2e9f2073832965384334d3e204d1df1e3dcd09cffa`  
		Last Modified: Tue, 04 Jul 2023 01:38:16 GMT  
		Size: 47.9 MB (47890767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d5c8c8644c840146ba18a3d20250a3f49997785afe106720a31e6e3bc0bdcf`  
		Last Modified: Tue, 04 Jul 2023 13:07:16 GMT  
		Size: 25.2 MB (25169956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:unstable-scm`

```console
$ docker pull buildpack-deps@sha256:e770a17b3b5af783abd7b0178ea83e788b97a9107a5e1e074ac2f2cee327a204
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

### `buildpack-deps:unstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:db8046e6728be4a319bf8c9c7fc53191969676c1aff3dc192ecb5e1acfc6dd44
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.2 MB (138245050 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84c9f688e3f355ba0028691806d887b635ae646386d3bf3d5b1b6cda070e4e10`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:21:50 GMT
ADD file:4bfda8f11e59383c37bfa6038bb5d22f58b9724d249a62568a2e7d2908821cd3 in / 
# Tue, 04 Jul 2023 01:21:50 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:34:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:34:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6efa412d16b908043ec01c4ac9ff7323c0f488dd5d7ea4b9b086f1e80350b9b3`  
		Last Modified: Tue, 04 Jul 2023 01:27:46 GMT  
		Size: 49.5 MB (49475944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad8fa89586d6eb7c1bf3add3cde8c80b2da78794ef30be11a97f2dad784809a`  
		Last Modified: Tue, 04 Jul 2023 03:54:24 GMT  
		Size: 24.1 MB (24082653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80dbf573225a65ee45360f0a43a08f5e1809ec65e4c5fd3634aa3c651ce0aa3`  
		Last Modified: Tue, 04 Jul 2023 03:54:42 GMT  
		Size: 64.7 MB (64686453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:0841006a6e7ae7124fb49383c6e729393fe97fdd7d5a764ba2cf3524717ac5d3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.4 MB (132387410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3a1dbd93f213db0dc50fa2e522af5b935f1ec468cdef913e9ba7a9874021b31`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:49:11 GMT
ADD file:e6181e27889c016519d8d701345aafff7138df96a76fb6a29403c8a33a3365fe in / 
# Tue, 04 Jul 2023 00:49:11 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 04:27:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 04:27:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:667272d8fe1bc81ce33874dbc84976c86d6b95f50198465a6ab672c71d87f666`  
		Last Modified: Tue, 04 Jul 2023 00:53:33 GMT  
		Size: 47.3 MB (47322473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b5934a15453e5e63936a0201a34b820f06d7c27f091dc017bac7d92e1e58d7`  
		Last Modified: Tue, 04 Jul 2023 04:30:42 GMT  
		Size: 22.8 MB (22758286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4231c799b91b6f2c6d3090483baafb52160bc63bb7459deb8ea264e4018f2d3b`  
		Last Modified: Tue, 04 Jul 2023 04:31:01 GMT  
		Size: 62.3 MB (62306651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:ef3af5ff6fe6345574d568b9ba626175b69ded771ab30deacab706cc412c49b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.1 MB (127062025 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45c39f924f6ca9f00579aa7a0e37403b02cd47ce2ba59130218cfd6f5fd31a0a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 00:59:44 GMT
ADD file:5be8eee7722dc860882f26018d8a0de49a4db6fcaa0f35d1dfbb74eff22929cb in / 
# Tue, 04 Jul 2023 00:59:45 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:57:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:57:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:42cc2becb0b735f0260d9f678fb1201bbe47c438212c5faf04879fab6a2dd73f`  
		Last Modified: Tue, 04 Jul 2023 01:05:43 GMT  
		Size: 45.1 MB (45123975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5cb3f60ee8390c8cae75e83a5b95ebc4f3589ca1af647965d02fe99b974827b`  
		Last Modified: Tue, 04 Jul 2023 06:21:50 GMT  
		Size: 22.0 MB (21984543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c1e5d5a935736b670eec63e61b0bdcc50ea4bc384b4ef00a257b7d98cbe0f6`  
		Last Modified: Tue, 04 Jul 2023 06:22:08 GMT  
		Size: 60.0 MB (59953507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:6547b0fb05aa47c02279476c9c339b27a73ba686a8d964767bf51542e495f10d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.8 MB (137764860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b44f02907bd19b65d492b7fc136b89c412638c71ddb02410f4c3172aa8847bc`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:58:49 GMT
ADD file:2c2c0588b93f9af7d93f19033795edf9e61a692ff56e65d9e9500915276782c9 in / 
# Tue, 04 Jul 2023 01:58:50 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 06:00:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 06:01:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d1b52151d5bb774f3680f8697c343bae1b64b7308354db57dc6bbeb7d65d0964`  
		Last Modified: Tue, 04 Jul 2023 02:03:59 GMT  
		Size: 49.5 MB (49482570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03e94cfcd9a2ac0ccda7b085606ef5174003eb543c68b5bf077a91230b8a7f7`  
		Last Modified: Tue, 04 Jul 2023 06:23:39 GMT  
		Size: 23.6 MB (23620572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12422f578439e0f8042c87a47638ea9651cb9d674e8c89b05c5e4d333833ca02`  
		Last Modified: Tue, 04 Jul 2023 06:23:55 GMT  
		Size: 64.7 MB (64661718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:08ac98188b4d99022ddf9f16dc0a488ec35f19e9d09d3930aef1e2f733ae81d9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.9 MB (141945829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6989e556ea04ee7a099cc0e1e2fa0719d9fbf6a8ce54cc152f9844ccdc9f46e4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:40:19 GMT
ADD file:565f8487c71b5de967f1bf16d4bd86291107b68f4152a61e35a8ab86e9f83b7b in / 
# Tue, 04 Jul 2023 01:40:20 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:37:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 05:37:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:46685592106ba6554716942e180f6b4cd8a73f1ec934554b40aee89b47118f5e`  
		Last Modified: Tue, 04 Jul 2023 01:46:32 GMT  
		Size: 50.5 MB (50505825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bf3084ac7ee091f26af470878c8197f67d44c09670c27921a26209c909a5c0b`  
		Last Modified: Tue, 04 Jul 2023 05:42:02 GMT  
		Size: 24.9 MB (24921812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef6611c0dbf9970353c5c08585b89e28e50531495ee733b7f098fa9c3501067d`  
		Last Modified: Tue, 04 Jul 2023 05:42:24 GMT  
		Size: 66.5 MB (66518192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:776e2afd9426f5f202780c44cb0d6c0ed2e77466bbee1fe230f4f8b68bb0bbe3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.7 MB (136723315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57625595c83aae207b1a1028993f73dcc398eeefcdafe5589ab032b376a5fd51`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:12:32 GMT
ADD file:ab2873cb088258c79fab5dde2d754d1967ca11e58adcf6a08811206759a323d5 in / 
# Tue, 04 Jul 2023 01:12:35 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 14:52:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 14:54:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:796c2f1009ce9a433d10a1f4708cbb79ef733dcb0ca992041a6aa621e85d8410`  
		Last Modified: Tue, 04 Jul 2023 01:23:15 GMT  
		Size: 49.5 MB (49455398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44357c89fac3bdc147daa7fe48fcf65b83dae0a924631c0b3e9ddb3f7ad71da2`  
		Last Modified: Tue, 04 Jul 2023 15:02:20 GMT  
		Size: 23.7 MB (23660637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:360a64085c52bd3ade25ff3dffcad4ccd2db7944aad983d6da8f5a3e148e1a44`  
		Last Modified: Tue, 04 Jul 2023 15:03:11 GMT  
		Size: 63.6 MB (63607280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:c6db7b3d9b8b7b9461c958da7d9061423f995b3e3d3d4d9e2dfd8ab01cefab08
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.4 MB (149354347 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1705ece1fdfc0d296b55a24fb47d71cd633a54e73ff649b62e797ad1429ca2c7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:19:33 GMT
ADD file:4c1d6f76704d32b9b503bd61c4b485555ec28037fb500403ffb5cbb102cf4509 in / 
# Tue, 04 Jul 2023 01:19:36 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:37:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:38:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3e4e6efa69b637e0e8ca00ddcae1aed23aef874a92a2904bdc6c9fa5b3212b8a`  
		Last Modified: Tue, 04 Jul 2023 01:27:02 GMT  
		Size: 53.5 MB (53474414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b5bee4b9196ae6959902bca430113379429a2f075e1553977c6d0442f46233`  
		Last Modified: Tue, 04 Jul 2023 04:39:59 GMT  
		Size: 25.7 MB (25732481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b347de1638edf48069dc551f9b7887a170d69f36e44b3d711a5f35da08e29100`  
		Last Modified: Tue, 04 Jul 2023 04:40:30 GMT  
		Size: 70.1 MB (70147452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:2fdda162727e88b07827fd912da5214d4e6184a7a61eff30378d465a4e8af39d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.1 MB (128123386 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37b066cf94438556c4df6f89a1bade9a9e6151382e24685619bb268b0a2ca495`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:09:05 GMT
ADD file:dc2a1586d12e833e5dc300033838059f3946ddddccde6c62d17cba40536ead15 in / 
# Tue, 04 Jul 2023 01:09:07 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 01:31:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 01:34:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d273b82777a979179469448ba9e255d7f7e1671f28d5610f47e8530093aaa04e`  
		Last Modified: Tue, 04 Jul 2023 01:12:27 GMT  
		Size: 45.7 MB (45695454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f7ece03f0359914c61a65ea80744e3ec92ac1afbb1ddab79b6c7276dae0614`  
		Last Modified: Tue, 04 Jul 2023 01:43:00 GMT  
		Size: 22.3 MB (22287386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e6bfc3fa16d519518bec2169bd35f0eeede077436e581f9c80725f413e6788e`  
		Last Modified: Tue, 04 Jul 2023 01:44:21 GMT  
		Size: 60.1 MB (60140546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:96941110e49ead9aca1f19c783cee74c1ba60437aa646cb579afcefb7ad4b433
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.8 MB (136838024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d21031b741572c9c946128adaf02584158a5ab375ff2bcf317eb2d6bf3597828`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Jul 2023 01:33:27 GMT
ADD file:9c12086273bf86ac1b3f72beebd17cc357bb749a95ac64d0f5ecdbbe7631cec4 in / 
# Tue, 04 Jul 2023 01:33:29 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 12:50:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 12:50:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3dcb3b9eb8abea3e1994db2e9f2073832965384334d3e204d1df1e3dcd09cffa`  
		Last Modified: Tue, 04 Jul 2023 01:38:16 GMT  
		Size: 47.9 MB (47890767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d5c8c8644c840146ba18a3d20250a3f49997785afe106720a31e6e3bc0bdcf`  
		Last Modified: Tue, 04 Jul 2023 13:07:16 GMT  
		Size: 25.2 MB (25169956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac95edda4f2261a710fe6cece76ae1adadaa655ad92be633a48ffbfffceaba9`  
		Last Modified: Tue, 04 Jul 2023 13:07:30 GMT  
		Size: 63.8 MB (63777301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
