<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `buildpack-deps`

-	[`buildpack-deps:20.04`](#buildpack-deps2004)
-	[`buildpack-deps:20.04-curl`](#buildpack-deps2004-curl)
-	[`buildpack-deps:20.04-scm`](#buildpack-deps2004-scm)
-	[`buildpack-deps:22.04`](#buildpack-deps2204)
-	[`buildpack-deps:22.04-curl`](#buildpack-deps2204-curl)
-	[`buildpack-deps:22.04-scm`](#buildpack-deps2204-scm)
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
-	[`buildpack-deps:testing`](#buildpack-depstesting)
-	[`buildpack-deps:testing-curl`](#buildpack-depstesting-curl)
-	[`buildpack-deps:testing-scm`](#buildpack-depstesting-scm)
-	[`buildpack-deps:trixie`](#buildpack-depstrixie)
-	[`buildpack-deps:trixie-curl`](#buildpack-depstrixie-curl)
-	[`buildpack-deps:trixie-scm`](#buildpack-depstrixie-scm)
-	[`buildpack-deps:unstable`](#buildpack-depsunstable)
-	[`buildpack-deps:unstable-curl`](#buildpack-depsunstable-curl)
-	[`buildpack-deps:unstable-scm`](#buildpack-depsunstable-scm)

## `buildpack-deps:20.04`

```console
$ docker pull buildpack-deps@sha256:bfdf1ac658ab3c2da2a75ca6e60428056f2478e3eba675f2b5639eb96957a711
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
$ docker pull buildpack-deps@sha256:b5fde3cb8a892f44fcc5cd00f64984c2dfbc1f716ae0f3102cd4e87be3075da8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.8 MB (245752605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d936a0f2edffab8e89ae578c7ac39d7c7d57edd069dc932d27927c98628a571f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 Oct 2023 10:45:50 GMT
ARG RELEASE
# Tue, 03 Oct 2023 10:45:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 10:45:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 10:45:50 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 10:45:51 GMT
ADD file:4809da414c2d478b4d991cbdaa2df457f2b3d07d0ff6cf673f09a66f90833e81 in / 
# Tue, 03 Oct 2023 10:45:52 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:11:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 07:12:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 07:15:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a2c559011895d255fce249c00396abff5ae7e0c0a92931d0ed493e71de78e3a`  
		Last Modified: Tue, 03 Oct 2023 17:02:08 GMT  
		Size: 28.6 MB (28580681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c93f97937844870a0d591bb295de8f5d1a3c6b7ea71083ccc820afd4282b3a2`  
		Last Modified: Fri, 13 Oct 2023 07:25:30 GMT  
		Size: 11.1 MB (11129460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd72b323778a4e704264ff859c0e8ef49d0d285cd057d0781881ee1ca649a67`  
		Last Modified: Fri, 13 Oct 2023 07:25:48 GMT  
		Size: 60.9 MB (60923941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f14c4b8174ea549d7ff9050fe9d305f59153eddecfae52c56d0f0c7821e6d4`  
		Last Modified: Fri, 13 Oct 2023 07:26:16 GMT  
		Size: 145.1 MB (145118523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:72e23dbcf10bc3d9f43d4e5f6481fc5724226a4bb3e74ad540729cad2db4e985
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.0 MB (211950429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b3706a3084dfe4471fcf5717dd0c407744133880c98f0a940274260275eb2ae`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 Oct 2023 10:47:59 GMT
ARG RELEASE
# Tue, 03 Oct 2023 10:47:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 10:47:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 10:47:59 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 10:48:06 GMT
ADD file:8dffbfada6e0bebb2858525182aef87ac2cbd88c624f32696ec2cb947e71a4f3 in / 
# Tue, 03 Oct 2023 10:48:07 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 00:57:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 00:57:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 01:00:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3b5f1ba1b648ae0824ed6a95ab17335537f8e689df99917fd374af5dd34078eb`  
		Last Modified: Fri, 13 Oct 2023 01:11:42 GMT  
		Size: 24.6 MB (24592174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccfc7436cda39ac35ae7ab16bdcc8269d47169c65ddf58da5fecf28ab6816624`  
		Last Modified: Fri, 13 Oct 2023 01:11:39 GMT  
		Size: 9.6 MB (9600386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2f3dfd8fbd9e1ce1164f9cf7d74790a3955b9019e8988f682380b086407df7`  
		Last Modified: Fri, 13 Oct 2023 01:12:04 GMT  
		Size: 55.8 MB (55823641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3aa5772d8f961cf51ee5a3fda8e29375c98387fc11a666f5c6eb9f1aebca44`  
		Last Modified: Fri, 13 Oct 2023 01:12:35 GMT  
		Size: 121.9 MB (121934228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:574c7a4001f3053b5329e8dfbb9ec27f35b81556feb2060074dc5c5cf5b8f585
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.0 MB (235965732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d0471cccb43aacbdd96d06b51fd8919703bc70d0d12c0803e1b4cdbf4237e92`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 Oct 2023 11:04:09 GMT
ARG RELEASE
# Tue, 03 Oct 2023 11:04:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 11:04:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 11:04:10 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 11:04:16 GMT
ADD file:f70cc2610ea8fcd25e6e9ae727eb9345d5b7198102f6a6d8e458ab8f99efefc3 in / 
# Tue, 03 Oct 2023 11:04:17 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 02:29:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 02:30:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 02:33:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6cba4020c0a193cd551ed8edf368670967e3546345b52c4ec66cb0931436e9b9`  
		Last Modified: Thu, 05 Oct 2023 12:12:17 GMT  
		Size: 27.2 MB (27199503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8f9293c4d270b52b3bc1e56516c484b0006c603f4445a0da0dcd3616f0daf9`  
		Last Modified: Fri, 13 Oct 2023 02:43:18 GMT  
		Size: 11.0 MB (10982407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:527191c7220ec77d3ed7791fedfc7587efea6f1d575a574622faa5bcb12a587e`  
		Last Modified: Fri, 13 Oct 2023 02:43:36 GMT  
		Size: 61.0 MB (61014037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e779168faa14907195729870f4acff9809719c5e3a31a9529a44fec13b6a2c`  
		Last Modified: Fri, 13 Oct 2023 02:43:59 GMT  
		Size: 136.8 MB (136769785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:8ba8ddea9b71cc2251d69f5e8a55ae5e6c9d13075fb8dede76c9df77cb6ab9b6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.5 MB (269488433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:926f600e0a15696dfbaa70229664b65febe27c33212c1e3f9ad7a11994d19c7f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 Oct 2023 11:03:52 GMT
ARG RELEASE
# Tue, 03 Oct 2023 11:03:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 11:03:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 11:03:53 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 11:03:56 GMT
ADD file:ba2394102af0c0584d39af9ec5dd4fa13286293b4607ac7cb9e16d7a2781eef2 in / 
# Tue, 03 Oct 2023 11:03:56 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 06:55:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 06:56:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 07:02:19 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3046919588b0e4a9b202dcd311befda8e46083ce41f424888dcbea91ce8e6e2`  
		Last Modified: Fri, 13 Oct 2023 06:16:08 GMT  
		Size: 33.3 MB (33306424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e14fbec6dc81f63fbfd4d494bd75555c5cd803486e1d753f061b0d3fce81cdc9`  
		Last Modified: Fri, 13 Oct 2023 07:22:17 GMT  
		Size: 12.9 MB (12937951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45cd0c9f0984989e99ef16079e2f5b95f1a20df097939fe992c991233c3e6b72`  
		Last Modified: Fri, 13 Oct 2023 07:22:39 GMT  
		Size: 69.6 MB (69644829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7eb02628173f481bf164e9a0c112a72e5bdea9eda1906464cc8b1bb3d9cfc7`  
		Last Modified: Fri, 13 Oct 2023 07:23:13 GMT  
		Size: 153.6 MB (153599229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:146a4f8c725380eec620a5f6d2f018386dc774ce13692cc79159c2f120c7137a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.6 MB (226607654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed94ac912c0ed9895b3abef8896dee8e605f2bc4e578bb2b29f23932a7ba0bea`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:17:39 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:17:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:17:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:17:39 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:17:41 GMT
ADD file:36efc3ec29bb54e0987fe91be1aa7cc849909b3cd2534af3de2d3d07a03804cf in / 
# Tue, 01 Aug 2023 06:17:41 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 00:08:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 00:09:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 00:11:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:365fa2124eb5f6f369204f3fe0210d9965952628707dfacd4194a8e15caf0420`  
		Last Modified: Thu, 03 Aug 2023 00:03:37 GMT  
		Size: 27.0 MB (27014233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b6082f2457965a87b9693265b680b0a0aa5d30ef936b6df14487a947354b10`  
		Last Modified: Thu, 03 Aug 2023 00:21:05 GMT  
		Size: 10.7 MB (10688615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5764a6c44dcfc11bcbd3dda534db4967a8ffd1443cbe922c189701e996c2c222`  
		Last Modified: Thu, 03 Aug 2023 00:21:19 GMT  
		Size: 60.3 MB (60311530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1c95e4e206b384145bd8128e74027e092da89c7654f4aebfd616735756a6f9`  
		Last Modified: Thu, 03 Aug 2023 00:21:42 GMT  
		Size: 128.6 MB (128593276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:20.04-curl`

```console
$ docker pull buildpack-deps@sha256:b8f274a0d962394e7560a9e6bbe50cdf681b997d8ff76b75dfc16c32366cb9a4
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
$ docker pull buildpack-deps@sha256:199614fe208a7619cdca61ecaf5fd02a9b68698693e7ce08cb12310161add350
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.7 MB (39710141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2297c8acf409d2896d99e9f7b7f2bcafaceb58bca7a1c4c1ff1d8ece2e0f59a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 Oct 2023 10:45:50 GMT
ARG RELEASE
# Tue, 03 Oct 2023 10:45:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 10:45:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 10:45:50 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 10:45:51 GMT
ADD file:4809da414c2d478b4d991cbdaa2df457f2b3d07d0ff6cf673f09a66f90833e81 in / 
# Tue, 03 Oct 2023 10:45:52 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:11:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a2c559011895d255fce249c00396abff5ae7e0c0a92931d0ed493e71de78e3a`  
		Last Modified: Tue, 03 Oct 2023 17:02:08 GMT  
		Size: 28.6 MB (28580681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c93f97937844870a0d591bb295de8f5d1a3c6b7ea71083ccc820afd4282b3a2`  
		Last Modified: Fri, 13 Oct 2023 07:25:30 GMT  
		Size: 11.1 MB (11129460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:62d55d00bdfd031cd04241520627268e72f9785291c812a5241638dda1f4ef2a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.2 MB (34192560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad3e920efdd7794c8223f7269f8035dbf5244950528e86dc0adb8b32ce5bd09e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 Oct 2023 10:47:59 GMT
ARG RELEASE
# Tue, 03 Oct 2023 10:47:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 10:47:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 10:47:59 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 10:48:06 GMT
ADD file:8dffbfada6e0bebb2858525182aef87ac2cbd88c624f32696ec2cb947e71a4f3 in / 
# Tue, 03 Oct 2023 10:48:07 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 00:57:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3b5f1ba1b648ae0824ed6a95ab17335537f8e689df99917fd374af5dd34078eb`  
		Last Modified: Fri, 13 Oct 2023 01:11:42 GMT  
		Size: 24.6 MB (24592174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccfc7436cda39ac35ae7ab16bdcc8269d47169c65ddf58da5fecf28ab6816624`  
		Last Modified: Fri, 13 Oct 2023 01:11:39 GMT  
		Size: 9.6 MB (9600386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:ad462829462c403622fdfcadefd354333067ac8ebf9aae0883a7241e0e27b5cb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38181910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb4d46a93ed4cd4d8d5ebf40b8ddf72eb3a089aa3594f3d51537c78945573ea6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 Oct 2023 11:04:09 GMT
ARG RELEASE
# Tue, 03 Oct 2023 11:04:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 11:04:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 11:04:10 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 11:04:16 GMT
ADD file:f70cc2610ea8fcd25e6e9ae727eb9345d5b7198102f6a6d8e458ab8f99efefc3 in / 
# Tue, 03 Oct 2023 11:04:17 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 02:29:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6cba4020c0a193cd551ed8edf368670967e3546345b52c4ec66cb0931436e9b9`  
		Last Modified: Thu, 05 Oct 2023 12:12:17 GMT  
		Size: 27.2 MB (27199503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8f9293c4d270b52b3bc1e56516c484b0006c603f4445a0da0dcd3616f0daf9`  
		Last Modified: Fri, 13 Oct 2023 02:43:18 GMT  
		Size: 11.0 MB (10982407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:9c2ddc832bd5e7c1caba6736b28c294152b0f8d5f6237e63f698b5acc5b47a04
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.2 MB (46244375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:144ccbf81093f12806a06f937ba5d33d99336e1f72f953180a0fae81473f91b4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 Oct 2023 11:03:52 GMT
ARG RELEASE
# Tue, 03 Oct 2023 11:03:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 11:03:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 11:03:53 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 11:03:56 GMT
ADD file:ba2394102af0c0584d39af9ec5dd4fa13286293b4607ac7cb9e16d7a2781eef2 in / 
# Tue, 03 Oct 2023 11:03:56 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 06:55:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3046919588b0e4a9b202dcd311befda8e46083ce41f424888dcbea91ce8e6e2`  
		Last Modified: Fri, 13 Oct 2023 06:16:08 GMT  
		Size: 33.3 MB (33306424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e14fbec6dc81f63fbfd4d494bd75555c5cd803486e1d753f061b0d3fce81cdc9`  
		Last Modified: Fri, 13 Oct 2023 07:22:17 GMT  
		Size: 12.9 MB (12937951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:028f59f497fa2c8e7f3a358182ef00c601e83780a8c7f9b0fd4e4f0f735ef4cc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37702848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:674186b606991aba08faede7dbb56393ab45900ba8c3e92969a9030076dba1be`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:17:39 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:17:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:17:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:17:39 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:17:41 GMT
ADD file:36efc3ec29bb54e0987fe91be1aa7cc849909b3cd2534af3de2d3d07a03804cf in / 
# Tue, 01 Aug 2023 06:17:41 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 00:08:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:365fa2124eb5f6f369204f3fe0210d9965952628707dfacd4194a8e15caf0420`  
		Last Modified: Thu, 03 Aug 2023 00:03:37 GMT  
		Size: 27.0 MB (27014233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b6082f2457965a87b9693265b680b0a0aa5d30ef936b6df14487a947354b10`  
		Last Modified: Thu, 03 Aug 2023 00:21:05 GMT  
		Size: 10.7 MB (10688615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:20.04-scm`

```console
$ docker pull buildpack-deps@sha256:aa8ad732eec0478a2a39d4674bb6c0688b173b5dda2c8b058d88df485607fe56
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
$ docker pull buildpack-deps@sha256:7ba510d2d414f7f32506b2648e8fae33163f38a95dc9ad53506ddc728fc190d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.6 MB (100634082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d252f65001e3c05b44da7e1571a3fe4ba3665f5da85a30da8ed21e0f01a6550`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 Oct 2023 10:45:50 GMT
ARG RELEASE
# Tue, 03 Oct 2023 10:45:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 10:45:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 10:45:50 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 10:45:51 GMT
ADD file:4809da414c2d478b4d991cbdaa2df457f2b3d07d0ff6cf673f09a66f90833e81 in / 
# Tue, 03 Oct 2023 10:45:52 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:11:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 07:12:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a2c559011895d255fce249c00396abff5ae7e0c0a92931d0ed493e71de78e3a`  
		Last Modified: Tue, 03 Oct 2023 17:02:08 GMT  
		Size: 28.6 MB (28580681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c93f97937844870a0d591bb295de8f5d1a3c6b7ea71083ccc820afd4282b3a2`  
		Last Modified: Fri, 13 Oct 2023 07:25:30 GMT  
		Size: 11.1 MB (11129460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd72b323778a4e704264ff859c0e8ef49d0d285cd057d0781881ee1ca649a67`  
		Last Modified: Fri, 13 Oct 2023 07:25:48 GMT  
		Size: 60.9 MB (60923941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:683c088512efd787bc9a974011eb4710f29b79c298484c32dd5aae263b8fe867
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.0 MB (90016201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3df2135c694ed153481f35d24358fa8df0b07a6ca05006e4b6658177b45c2643`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 Oct 2023 10:47:59 GMT
ARG RELEASE
# Tue, 03 Oct 2023 10:47:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 10:47:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 10:47:59 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 10:48:06 GMT
ADD file:8dffbfada6e0bebb2858525182aef87ac2cbd88c624f32696ec2cb947e71a4f3 in / 
# Tue, 03 Oct 2023 10:48:07 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 00:57:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 00:57:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3b5f1ba1b648ae0824ed6a95ab17335537f8e689df99917fd374af5dd34078eb`  
		Last Modified: Fri, 13 Oct 2023 01:11:42 GMT  
		Size: 24.6 MB (24592174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccfc7436cda39ac35ae7ab16bdcc8269d47169c65ddf58da5fecf28ab6816624`  
		Last Modified: Fri, 13 Oct 2023 01:11:39 GMT  
		Size: 9.6 MB (9600386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2f3dfd8fbd9e1ce1164f9cf7d74790a3955b9019e8988f682380b086407df7`  
		Last Modified: Fri, 13 Oct 2023 01:12:04 GMT  
		Size: 55.8 MB (55823641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:ee4a206dccb175102b3cb2bcf54c4af292f785a26e4c587503957b91512966a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99195947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:297ad753ed84562e345544abda8a38e822dfaad4357141a3af6198c83163c400`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 Oct 2023 11:04:09 GMT
ARG RELEASE
# Tue, 03 Oct 2023 11:04:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 11:04:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 11:04:10 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 11:04:16 GMT
ADD file:f70cc2610ea8fcd25e6e9ae727eb9345d5b7198102f6a6d8e458ab8f99efefc3 in / 
# Tue, 03 Oct 2023 11:04:17 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 02:29:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 02:30:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6cba4020c0a193cd551ed8edf368670967e3546345b52c4ec66cb0931436e9b9`  
		Last Modified: Thu, 05 Oct 2023 12:12:17 GMT  
		Size: 27.2 MB (27199503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8f9293c4d270b52b3bc1e56516c484b0006c603f4445a0da0dcd3616f0daf9`  
		Last Modified: Fri, 13 Oct 2023 02:43:18 GMT  
		Size: 11.0 MB (10982407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:527191c7220ec77d3ed7791fedfc7587efea6f1d575a574622faa5bcb12a587e`  
		Last Modified: Fri, 13 Oct 2023 02:43:36 GMT  
		Size: 61.0 MB (61014037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:9e4691461e8152658a19c6f908b58a8314e928b0fbc6c6da999d39f9655b4154
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.9 MB (115889204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0438293bebad2e61d50f207839478e418b17d5c295b4a9f5c7af55ef6c15f04c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 Oct 2023 11:03:52 GMT
ARG RELEASE
# Tue, 03 Oct 2023 11:03:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 11:03:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 11:03:53 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 11:03:56 GMT
ADD file:ba2394102af0c0584d39af9ec5dd4fa13286293b4607ac7cb9e16d7a2781eef2 in / 
# Tue, 03 Oct 2023 11:03:56 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 06:55:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 06:56:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3046919588b0e4a9b202dcd311befda8e46083ce41f424888dcbea91ce8e6e2`  
		Last Modified: Fri, 13 Oct 2023 06:16:08 GMT  
		Size: 33.3 MB (33306424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e14fbec6dc81f63fbfd4d494bd75555c5cd803486e1d753f061b0d3fce81cdc9`  
		Last Modified: Fri, 13 Oct 2023 07:22:17 GMT  
		Size: 12.9 MB (12937951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45cd0c9f0984989e99ef16079e2f5b95f1a20df097939fe992c991233c3e6b72`  
		Last Modified: Fri, 13 Oct 2023 07:22:39 GMT  
		Size: 69.6 MB (69644829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:079f48635b01d56e2478857b7e0c5fb6212336f9e594e783bbf19cb9dda8b0f2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.0 MB (98014378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2522830f5bbe1d8ea3e120ce6ff28c07dbc6f1a8b7f24c17fbb61b252bbab549`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:17:39 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:17:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:17:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:17:39 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:17:41 GMT
ADD file:36efc3ec29bb54e0987fe91be1aa7cc849909b3cd2534af3de2d3d07a03804cf in / 
# Tue, 01 Aug 2023 06:17:41 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 00:08:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 00:09:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:365fa2124eb5f6f369204f3fe0210d9965952628707dfacd4194a8e15caf0420`  
		Last Modified: Thu, 03 Aug 2023 00:03:37 GMT  
		Size: 27.0 MB (27014233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b6082f2457965a87b9693265b680b0a0aa5d30ef936b6df14487a947354b10`  
		Last Modified: Thu, 03 Aug 2023 00:21:05 GMT  
		Size: 10.7 MB (10688615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5764a6c44dcfc11bcbd3dda534db4967a8ffd1443cbe922c189701e996c2c222`  
		Last Modified: Thu, 03 Aug 2023 00:21:19 GMT  
		Size: 60.3 MB (60311530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.04`

```console
$ docker pull buildpack-deps@sha256:813d299dc3512a6029a8966e92b1080a48d0dda2d6a2f61679b00956b55627e4
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
$ docker pull buildpack-deps@sha256:24fe4235a691b49a8f4c3570eabdbeb2e33f712a7bf05f41717fce9c36bea901
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.0 MB (250049463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9336076452fd84376c39d0382d6478cbea7dbc26b7297b2436651d60a984ce18`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:33:30 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:33:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:33:32 GMT
ADD file:63d5ab3ef0aab308c0e71cb67292c5467f60deafa9b0418cbb220affcd078444 in / 
# Thu, 05 Oct 2023 07:33:32 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:15:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 07:16:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 07:18:52 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:43f89b94cd7df92a2f7e565b8fb1b7f502eff2cd225508cbd7ea2d36a9a3a601`  
		Last Modified: Thu, 05 Oct 2023 08:42:10 GMT  
		Size: 30.4 MB (30439111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c42c1a5016fb63983b7331918ba3251a006a305a7155f887c55ba0310f14ebe4`  
		Last Modified: Fri, 13 Oct 2023 07:26:26 GMT  
		Size: 7.1 MB (7119810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b397bf7f6432393178dcfa275258dfbbf1774183c2bf6d2c376676b1eb9d96ce`  
		Last Modified: Fri, 13 Oct 2023 07:26:41 GMT  
		Size: 39.4 MB (39447269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43f2be70120bd273670e90c14b5caba9a9ed79e5e2195d9fa5751dded927f82`  
		Last Modified: Fri, 13 Oct 2023 07:27:11 GMT  
		Size: 173.0 MB (173043273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:c8c55fc1ddcc289ed750014d5a333d4da1b4c38d9f56e3e28cfc94d75598b64a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.3 MB (217299987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c6ad0546b1c789630d2ab10627fc670a8e959846a0ed9b4d3b0155f252a87bf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:34:56 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:34:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:34:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:34:56 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:35:01 GMT
ADD file:4b9d52f97ed5796b14772a84c1e7213402430d32312d15ae04a2dcc9fc485a52 in / 
# Thu, 05 Oct 2023 07:35:02 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 01:01:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 01:01:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 01:04:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c4f28c22de51200ba6a71d2274daa2f71735946524265b3c45752d2cec53dee0`  
		Last Modified: Fri, 06 Oct 2023 02:02:33 GMT  
		Size: 27.5 MB (27513969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85fc270943bb9c7cfec1343fa169349a26edefb92574ab25cc3c91ba173fac6`  
		Last Modified: Fri, 13 Oct 2023 01:12:46 GMT  
		Size: 7.0 MB (7019227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0b0c5f614ae9b9b0ea44d893e337f282182465a7b811e594df1df46ba55b02`  
		Last Modified: Fri, 13 Oct 2023 01:13:07 GMT  
		Size: 42.2 MB (42240097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c437efecc24744323340d7367e5cf9fe9550f503e10d438a7fedc3c39d0adb53`  
		Last Modified: Fri, 13 Oct 2023 01:13:39 GMT  
		Size: 140.5 MB (140526694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:033f47d0faaf35e3f9a908e8f28aa41349a3c04e7992409d9738936e0b5ace76
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.3 MB (241335805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:878ba0f3fe1ba872439dc5242931f1bea039ea8b923db8db743c9fc3773a7e61`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:32:20 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:32:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:32:22 GMT
ADD file:f8594e26831508c318e42c8dfd9942041031087b8de1bf3fec11fd75b8b30fd4 in / 
# Thu, 05 Oct 2023 07:32:22 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 02:33:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 02:34:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 02:36:52 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:895d322e8e5957c04af3ab7b3431f2a562182d34167c6e159e02044150a66967`  
		Last Modified: Thu, 05 Oct 2023 08:57:30 GMT  
		Size: 28.4 MB (28391939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab98684ba3fe8f55da444be42c97a55fce3f516fbef08145bd1ee5686d63f30`  
		Last Modified: Fri, 13 Oct 2023 02:44:09 GMT  
		Size: 7.1 MB (7066736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:137f888ab5ca54ae228d9aa08792d8dfc0505614071a433dab0b8d64853412d1`  
		Last Modified: Fri, 13 Oct 2023 02:44:24 GMT  
		Size: 39.4 MB (39363322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f636694bf2d25bc6aa577bcca3dc616db456936312afcfea87dbc51426d0892e`  
		Last Modified: Fri, 13 Oct 2023 02:44:49 GMT  
		Size: 166.5 MB (166513808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:672844360fcc6634c2ea76d298bd650eb4ba32f85543816e1f43f814ee105810
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.4 MB (271425284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8f7f46cd62289364aaaed1c58e0b2ae9b323a91f98f9bd611cc8bca32799d56`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:34:18 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:34:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:34:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:34:19 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:34:22 GMT
ADD file:595ff761b2778bdc6bb59cbe8ce51c4a247e0f279ccd59a17b5be6cdeac0b4d2 in / 
# Thu, 05 Oct 2023 07:34:22 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:03:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 07:04:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 07:10:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:589c4cce1daa100afadbdbeda96025d02f85c117e0e60b70801af41b4e618668`  
		Last Modified: Fri, 13 Oct 2023 06:13:20 GMT  
		Size: 35.7 MB (35682793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3915535cd53c34e21aaca3d30c265266ed72ec102dc961ecd9c0616cf6e3df6c`  
		Last Modified: Fri, 13 Oct 2023 07:23:24 GMT  
		Size: 8.3 MB (8253985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7fb2022d4edb92326fe02a877beeae2b46b6b000fb736302f493bec3e625a78`  
		Last Modified: Fri, 13 Oct 2023 07:23:41 GMT  
		Size: 43.8 MB (43764927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff661c5b91d15269c1e42d2b9e38dfe8f206ca2dc9be9069267996663d3f4748`  
		Last Modified: Fri, 13 Oct 2023 07:24:18 GMT  
		Size: 183.7 MB (183723579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:e4399018428c842b4c392e87a36defdb82afeac9551fc87958cfe3d55d3ca0ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.8 MB (223831456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a917d107abf2d33f9279640b659e2f7f812ed5720b724978da723df3da955601`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 25 Sep 2023 10:17:26 GMT
ARG RELEASE
# Mon, 25 Sep 2023 10:17:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 25 Sep 2023 10:17:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 25 Sep 2023 10:17:26 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 25 Sep 2023 10:17:28 GMT
ADD file:78683f2464233172a7cd0d6adc4c7d9fb3ef05fa67ca22e6fbaca0325496a536 in / 
# Mon, 25 Sep 2023 10:17:28 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 08:49:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 08:49:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 08:52:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b6ba488997f9924c9473e547d56b3d4ae74495b1092ca3c613243185ee5d5151`  
		Last Modified: Tue, 03 Oct 2023 08:59:45 GMT  
		Size: 28.7 MB (28651983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63dcb81ab3d8b1a5d99f79f12abeae58d32d80628c914e5b75ac72c82c71adf1`  
		Last Modified: Tue, 03 Oct 2023 08:59:42 GMT  
		Size: 7.0 MB (7033657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05bd5fa6428d58b59c71d06922c39d17e607ab984f737113aea36b3899777d6`  
		Last Modified: Tue, 03 Oct 2023 09:00:17 GMT  
		Size: 39.4 MB (39413935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61eff3bbf0140cf19e8752d02bd7fb1d00a0d33b08b27067a5b9e2b6f6517a64`  
		Last Modified: Tue, 03 Oct 2023 09:00:58 GMT  
		Size: 148.7 MB (148731881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.04-curl`

```console
$ docker pull buildpack-deps@sha256:085a23a57a491311104937fb13c53bf25fad7b201ff429a1ae6815cc84afdddc
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
$ docker pull buildpack-deps@sha256:0f644f5b2afab0d3227b2b34c6a6f129c88ba104f3c07a5ce0b29edfbf6ef91e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37558921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b5f87e49274876d9c93c07c94ec36af2b0f9a55ed8088620181fd55723912c0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:33:30 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:33:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:33:32 GMT
ADD file:63d5ab3ef0aab308c0e71cb67292c5467f60deafa9b0418cbb220affcd078444 in / 
# Thu, 05 Oct 2023 07:33:32 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:15:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:43f89b94cd7df92a2f7e565b8fb1b7f502eff2cd225508cbd7ea2d36a9a3a601`  
		Last Modified: Thu, 05 Oct 2023 08:42:10 GMT  
		Size: 30.4 MB (30439111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c42c1a5016fb63983b7331918ba3251a006a305a7155f887c55ba0310f14ebe4`  
		Last Modified: Fri, 13 Oct 2023 07:26:26 GMT  
		Size: 7.1 MB (7119810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:d1d6a1fcdbc5c3af24c46feea2f9cbf4d8b8fd4e01c3d58bc4b59dee727945b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34533196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18773abeaa0270194048921ebd164d0a4c7a6649da81086097b4e2445330ba1c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:34:56 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:34:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:34:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:34:56 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:35:01 GMT
ADD file:4b9d52f97ed5796b14772a84c1e7213402430d32312d15ae04a2dcc9fc485a52 in / 
# Thu, 05 Oct 2023 07:35:02 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 01:01:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c4f28c22de51200ba6a71d2274daa2f71735946524265b3c45752d2cec53dee0`  
		Last Modified: Fri, 06 Oct 2023 02:02:33 GMT  
		Size: 27.5 MB (27513969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85fc270943bb9c7cfec1343fa169349a26edefb92574ab25cc3c91ba173fac6`  
		Last Modified: Fri, 13 Oct 2023 01:12:46 GMT  
		Size: 7.0 MB (7019227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:549886f44fbb35904c5e8e1c2fea61d8ec12b5caaf0c82cf7efecd82da406a46
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 MB (35458675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58af3f1d094523439bff7af275c13d0b37d05a7f53ef22e92773e3945f20587f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:32:20 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:32:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:32:22 GMT
ADD file:f8594e26831508c318e42c8dfd9942041031087b8de1bf3fec11fd75b8b30fd4 in / 
# Thu, 05 Oct 2023 07:32:22 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 02:33:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:895d322e8e5957c04af3ab7b3431f2a562182d34167c6e159e02044150a66967`  
		Last Modified: Thu, 05 Oct 2023 08:57:30 GMT  
		Size: 28.4 MB (28391939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab98684ba3fe8f55da444be42c97a55fce3f516fbef08145bd1ee5686d63f30`  
		Last Modified: Fri, 13 Oct 2023 02:44:09 GMT  
		Size: 7.1 MB (7066736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d906fc4587e2ecce9c87f730384cc30acca1c1d47298757243269d7924495089
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43936778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c62c64ba3f1b4292cf95704aba38456563dd67309339d32ee6e3e80ab9e890a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:34:18 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:34:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:34:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:34:19 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:34:22 GMT
ADD file:595ff761b2778bdc6bb59cbe8ce51c4a247e0f279ccd59a17b5be6cdeac0b4d2 in / 
# Thu, 05 Oct 2023 07:34:22 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:03:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:589c4cce1daa100afadbdbeda96025d02f85c117e0e60b70801af41b4e618668`  
		Last Modified: Fri, 13 Oct 2023 06:13:20 GMT  
		Size: 35.7 MB (35682793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3915535cd53c34e21aaca3d30c265266ed72ec102dc961ecd9c0616cf6e3df6c`  
		Last Modified: Fri, 13 Oct 2023 07:23:24 GMT  
		Size: 8.3 MB (8253985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:f261ff2241965d50e93901c04a586655af4008f24a94241d1b2ddf8123f0bd26
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35685640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8fe1a2e1659b935c6f8f380bb55c01fe947e5f305337a3f181485a1fe5d7859`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 25 Sep 2023 10:17:26 GMT
ARG RELEASE
# Mon, 25 Sep 2023 10:17:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 25 Sep 2023 10:17:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 25 Sep 2023 10:17:26 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 25 Sep 2023 10:17:28 GMT
ADD file:78683f2464233172a7cd0d6adc4c7d9fb3ef05fa67ca22e6fbaca0325496a536 in / 
# Mon, 25 Sep 2023 10:17:28 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 08:49:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b6ba488997f9924c9473e547d56b3d4ae74495b1092ca3c613243185ee5d5151`  
		Last Modified: Tue, 03 Oct 2023 08:59:45 GMT  
		Size: 28.7 MB (28651983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63dcb81ab3d8b1a5d99f79f12abeae58d32d80628c914e5b75ac72c82c71adf1`  
		Last Modified: Tue, 03 Oct 2023 08:59:42 GMT  
		Size: 7.0 MB (7033657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.04-scm`

```console
$ docker pull buildpack-deps@sha256:f5eb46c4570633bedc3cfa85a592bef312277dd23650e930c58a7c73f9ae8429
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
$ docker pull buildpack-deps@sha256:d24c158fc955083cf096191ae38bbd3cd1ec155e695f4bae2378e78079aa22eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (77006190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dce2ef8e1153a09bce17fbf2148781d63ebe67c1f28767f41a8e6b95a8831f92`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:33:30 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:33:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:33:32 GMT
ADD file:63d5ab3ef0aab308c0e71cb67292c5467f60deafa9b0418cbb220affcd078444 in / 
# Thu, 05 Oct 2023 07:33:32 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:15:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 07:16:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:43f89b94cd7df92a2f7e565b8fb1b7f502eff2cd225508cbd7ea2d36a9a3a601`  
		Last Modified: Thu, 05 Oct 2023 08:42:10 GMT  
		Size: 30.4 MB (30439111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c42c1a5016fb63983b7331918ba3251a006a305a7155f887c55ba0310f14ebe4`  
		Last Modified: Fri, 13 Oct 2023 07:26:26 GMT  
		Size: 7.1 MB (7119810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b397bf7f6432393178dcfa275258dfbbf1774183c2bf6d2c376676b1eb9d96ce`  
		Last Modified: Fri, 13 Oct 2023 07:26:41 GMT  
		Size: 39.4 MB (39447269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:465a04ef4d05ae8daffc7108037ecff2d65c230ab338beaa2a7ca258e2ade9b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76773293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf0e57397bae1b99eb3b196a13dc8e1c4fa6c39d62f3b649961c51c66ee87fc8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:34:56 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:34:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:34:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:34:56 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:35:01 GMT
ADD file:4b9d52f97ed5796b14772a84c1e7213402430d32312d15ae04a2dcc9fc485a52 in / 
# Thu, 05 Oct 2023 07:35:02 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 01:01:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 01:01:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c4f28c22de51200ba6a71d2274daa2f71735946524265b3c45752d2cec53dee0`  
		Last Modified: Fri, 06 Oct 2023 02:02:33 GMT  
		Size: 27.5 MB (27513969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85fc270943bb9c7cfec1343fa169349a26edefb92574ab25cc3c91ba173fac6`  
		Last Modified: Fri, 13 Oct 2023 01:12:46 GMT  
		Size: 7.0 MB (7019227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0b0c5f614ae9b9b0ea44d893e337f282182465a7b811e594df1df46ba55b02`  
		Last Modified: Fri, 13 Oct 2023 01:13:07 GMT  
		Size: 42.2 MB (42240097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:23a410e3dfc5f893887c6f91e3d96a404c7b844d74cb597f0d10483d8200c8bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74821997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dab2960221ba40117786b31739f218f59b91426bb60076b90d952377329f0fd0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:32:20 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:32:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:32:22 GMT
ADD file:f8594e26831508c318e42c8dfd9942041031087b8de1bf3fec11fd75b8b30fd4 in / 
# Thu, 05 Oct 2023 07:32:22 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 02:33:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 02:34:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:895d322e8e5957c04af3ab7b3431f2a562182d34167c6e159e02044150a66967`  
		Last Modified: Thu, 05 Oct 2023 08:57:30 GMT  
		Size: 28.4 MB (28391939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab98684ba3fe8f55da444be42c97a55fce3f516fbef08145bd1ee5686d63f30`  
		Last Modified: Fri, 13 Oct 2023 02:44:09 GMT  
		Size: 7.1 MB (7066736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:137f888ab5ca54ae228d9aa08792d8dfc0505614071a433dab0b8d64853412d1`  
		Last Modified: Fri, 13 Oct 2023 02:44:24 GMT  
		Size: 39.4 MB (39363322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:18932b92e188adb2feac77ff881d8a29babc9805aede5aecf7e2641bd8e80386
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.7 MB (87701705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ac4f1d31d15e96607b82c209778a0051c4dd5a64441fb0258a3267314f9db17`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:34:18 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:34:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:34:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:34:19 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:34:22 GMT
ADD file:595ff761b2778bdc6bb59cbe8ce51c4a247e0f279ccd59a17b5be6cdeac0b4d2 in / 
# Thu, 05 Oct 2023 07:34:22 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:03:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 07:04:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:589c4cce1daa100afadbdbeda96025d02f85c117e0e60b70801af41b4e618668`  
		Last Modified: Fri, 13 Oct 2023 06:13:20 GMT  
		Size: 35.7 MB (35682793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3915535cd53c34e21aaca3d30c265266ed72ec102dc961ecd9c0616cf6e3df6c`  
		Last Modified: Fri, 13 Oct 2023 07:23:24 GMT  
		Size: 8.3 MB (8253985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7fb2022d4edb92326fe02a877beeae2b46b6b000fb736302f493bec3e625a78`  
		Last Modified: Fri, 13 Oct 2023 07:23:41 GMT  
		Size: 43.8 MB (43764927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:f7037c2ca159e27e211e9d3f4c6a04a0a3bf3182edc42d8210a1d965cfe1673d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75099575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34bf07ba4c66ab3817378608226748f1a91d05832c79d5360e4c516bd11c204e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 25 Sep 2023 10:17:26 GMT
ARG RELEASE
# Mon, 25 Sep 2023 10:17:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 25 Sep 2023 10:17:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 25 Sep 2023 10:17:26 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 25 Sep 2023 10:17:28 GMT
ADD file:78683f2464233172a7cd0d6adc4c7d9fb3ef05fa67ca22e6fbaca0325496a536 in / 
# Mon, 25 Sep 2023 10:17:28 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 08:49:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 08:49:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b6ba488997f9924c9473e547d56b3d4ae74495b1092ca3c613243185ee5d5151`  
		Last Modified: Tue, 03 Oct 2023 08:59:45 GMT  
		Size: 28.7 MB (28651983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63dcb81ab3d8b1a5d99f79f12abeae58d32d80628c914e5b75ac72c82c71adf1`  
		Last Modified: Tue, 03 Oct 2023 08:59:42 GMT  
		Size: 7.0 MB (7033657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05bd5fa6428d58b59c71d06922c39d17e607ab984f737113aea36b3899777d6`  
		Last Modified: Tue, 03 Oct 2023 09:00:17 GMT  
		Size: 39.4 MB (39413935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:23.04`

```console
$ docker pull buildpack-deps@sha256:5806596724fa79d84c05c5db171fffd0fb686ce26d6f100d2855b42263c2a739
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
$ docker pull buildpack-deps@sha256:09592b04b0e9b5345a66017fccd2bb575b714fe70d747239889e0abc5b2a581a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.6 MB (268609169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8be3606275e0541fe0c4a3d348ddaadbf8ade3013c418ae2816d332251ba288`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:18:17 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:18:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:18:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:18:18 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:18:19 GMT
ADD file:d4fca0b2b53fa4e2c3e0d721bf983f4095061c5df5fb084d2daf5efad5ee663d in / 
# Wed, 04 Oct 2023 12:18:19 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:19:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 07:20:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 07:24:17 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:850c6621501406ea0aac62d4ae7a001f98fe81b2085449034055ee7ff32622bc`  
		Last Modified: Thu, 05 Oct 2023 03:34:15 GMT  
		Size: 27.7 MB (27654268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c224a085b3b8f6169f29aeb01a19b302e9163e6122211234d56e34c49a1a52`  
		Last Modified: Fri, 13 Oct 2023 07:27:21 GMT  
		Size: 13.7 MB (13745429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415eed8af6d7f694df1de04bb6a2c5eba418319432d2dec5840be186c2df4971`  
		Last Modified: Fri, 13 Oct 2023 07:27:38 GMT  
		Size: 44.4 MB (44389510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed98248655b640aedb599378731535e0a729b6401f26d512f21872ae3f999a0`  
		Last Modified: Fri, 13 Oct 2023 07:28:10 GMT  
		Size: 182.8 MB (182819962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:d10e6715b29dbd0ef1f2ad8e5abf94556ec18422adecbd8bab056d3fc58649b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.4 MB (232441827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c5bfe8d3346fa65b2a65490f89c9d157d50669df53d95f446c6ee5fe8d1690f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:25:21 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:25:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:25:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:25:22 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:25:24 GMT
ADD file:b92305119eab5dd3dfb00f4d83cd84e00c8ae57143739329da5a19aeda55be4e in / 
# Wed, 04 Oct 2023 12:25:24 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 01:05:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 01:06:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 01:10:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0055151e5ef44f81f2355e8073f34f53cc16494749dbc5ba14445ce5edf3d3b6`  
		Last Modified: Fri, 13 Oct 2023 01:13:54 GMT  
		Size: 25.4 MB (25432981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e866c11041f7a46cb12551f8e93dea44f566d63d4fe5e9771fba148287d761c3`  
		Last Modified: Fri, 13 Oct 2023 01:13:51 GMT  
		Size: 12.7 MB (12665364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f378438bc51fcd6e34f3bded8ebdf10b2f56f47951e89908cd028fb60f9d763`  
		Last Modified: Fri, 13 Oct 2023 01:14:13 GMT  
		Size: 48.7 MB (48674522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a87bb08d55e31d0d5845bac5b3d441c3142141dd75d4c02bbf6b036fdc6be30`  
		Last Modified: Fri, 13 Oct 2023 01:14:48 GMT  
		Size: 145.7 MB (145668960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c1669c3bfc03aa349cc7266907fa3c34faeaaf68a9aa3bf7a888b0c4cb59b797
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.1 MB (258146485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:622129654f3cd970d2cb1ad360340c236ca504db8e4dca2544956acc6a1422e0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:23:52 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:23:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:23:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:23:52 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:23:53 GMT
ADD file:c9b1098bc90ac9b887c3bffdffbcff0c32f32e48df9a673041e3aa796296e69b in / 
# Wed, 04 Oct 2023 12:23:54 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 02:37:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 02:38:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 02:41:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6bd86e5a51fe562347e4392a584c2c048e2caf3c855ee2b39d193782482989d0`  
		Last Modified: Fri, 13 Oct 2023 02:45:03 GMT  
		Size: 27.0 MB (27009502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72b644e1b04fb1dbe3643839ab4b6c1c7562eed7fec98b56653bc7526d1f21b8`  
		Last Modified: Fri, 13 Oct 2023 02:45:00 GMT  
		Size: 13.3 MB (13334915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7195734b83041efa5c9550d35f558288d4c59268de32267217d78d00f7cd0dbb`  
		Last Modified: Fri, 13 Oct 2023 02:45:18 GMT  
		Size: 44.2 MB (44238877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73bddc9768e169e64876fcaec439a948c34e36801d337869e2bf980d6c6417a`  
		Last Modified: Fri, 13 Oct 2023 02:45:44 GMT  
		Size: 173.6 MB (173563191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:9186ee4cdc73cd802ff3ce577df5cf354c4b9a52f3afba18edc7725342d769fc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.0 MB (292973666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d17b3a7d6436dea3ef23bcf280cce6a1ed15621fe35c50663b8b5759e7a173c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:08:54 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:08:54 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:08:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:08:55 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:08:57 GMT
ADD file:24bc2f22a395e93a2ebbcfc45da8e5fc7f08e7c03cdc985c997300643d0310ec in / 
# Wed, 04 Oct 2023 12:08:58 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:12:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 07:13:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 07:20:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:56fffb9b8b31e93bce458c1b2532d4e3aabcfa346a00a948fa8702cf6e132f8c`  
		Last Modified: Fri, 13 Oct 2023 07:24:33 GMT  
		Size: 31.9 MB (31886447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a7a715c2447d71e6b94118f081111babef0331bd6104854da882370804c75ae`  
		Last Modified: Fri, 13 Oct 2023 07:24:30 GMT  
		Size: 15.8 MB (15842906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348f4703e93699e4c8ee248cbcc6f18ffaa75e71f9acb2b1a47c6a957a410e6f`  
		Last Modified: Fri, 13 Oct 2023 07:24:51 GMT  
		Size: 49.1 MB (49089842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c5ee703a39bc5a128280f48817e1157579759dcb313dcd3b0332f91493fb95`  
		Last Modified: Fri, 13 Oct 2023 07:25:31 GMT  
		Size: 196.2 MB (196154471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b03c2d5655663b83f6a221f35784d8902b4af4751413f0a874d38b81c25573ad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.2 MB (240157223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df5b35e4a07ed4da761b7644d6c49ad1a8694b981e74aaff067b260dec6c54a8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 04:29:27 GMT
ARG RELEASE
# Wed, 16 Aug 2023 04:29:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 04:29:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 04:29:28 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 16 Aug 2023 04:29:29 GMT
ADD file:14fcf0756fb29b609af54412c31e2ff9acbf4634984ce95bf204c67668706cb5 in / 
# Wed, 16 Aug 2023 04:29:30 GMT
CMD ["/bin/bash"]
# Fri, 01 Sep 2023 23:16:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Sep 2023 23:16:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Sep 2023 23:19:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e9a6157a42893e6f99bd42ba05c70c5313add95c69f61f12e51517c0100470b8`  
		Last Modified: Fri, 01 Sep 2023 23:24:13 GMT  
		Size: 26.2 MB (26223925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f88ef015543162519d8e086a0bb86351d03f27b98218ff39b27f3b8b7bc2cd`  
		Last Modified: Fri, 01 Sep 2023 23:24:12 GMT  
		Size: 14.0 MB (14005753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ad80a5cffb7414f3bd06d5dafc212e2f5a767d3312bead7347e2ba8fae5be35`  
		Last Modified: Fri, 01 Sep 2023 23:24:25 GMT  
		Size: 44.3 MB (44275476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f495142834cd7cf92ea01d1b100c2b74a416627d5613eefc2c858d2b4c774d2`  
		Last Modified: Fri, 01 Sep 2023 23:24:50 GMT  
		Size: 155.7 MB (155652069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:23.04-curl`

```console
$ docker pull buildpack-deps@sha256:072cf6221243181993eae81700993113c3fc12fb299987448794840b33506bc9
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
$ docker pull buildpack-deps@sha256:95e60ea366f0d1dc0c10aedff8863857395287974e218b3f32b0b0d6e98cd7ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.4 MB (41399697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dd67c3192123379e495aa231a49f40ef79982b7d68adc966bfa69e52eaa6d7a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:18:17 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:18:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:18:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:18:18 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:18:19 GMT
ADD file:d4fca0b2b53fa4e2c3e0d721bf983f4095061c5df5fb084d2daf5efad5ee663d in / 
# Wed, 04 Oct 2023 12:18:19 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:19:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:850c6621501406ea0aac62d4ae7a001f98fe81b2085449034055ee7ff32622bc`  
		Last Modified: Thu, 05 Oct 2023 03:34:15 GMT  
		Size: 27.7 MB (27654268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c224a085b3b8f6169f29aeb01a19b302e9163e6122211234d56e34c49a1a52`  
		Last Modified: Fri, 13 Oct 2023 07:27:21 GMT  
		Size: 13.7 MB (13745429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:0ecb3f2788bcf617a9998b5a24be6f6b2a219a05cdc5c8c0f7563ec4e19b4a80
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.1 MB (38098345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:899c18f362f26f3736d179227e6283f562d67fdba75be383e45008ab64e708ca`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:25:21 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:25:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:25:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:25:22 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:25:24 GMT
ADD file:b92305119eab5dd3dfb00f4d83cd84e00c8ae57143739329da5a19aeda55be4e in / 
# Wed, 04 Oct 2023 12:25:24 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 01:05:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0055151e5ef44f81f2355e8073f34f53cc16494749dbc5ba14445ce5edf3d3b6`  
		Last Modified: Fri, 13 Oct 2023 01:13:54 GMT  
		Size: 25.4 MB (25432981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e866c11041f7a46cb12551f8e93dea44f566d63d4fe5e9771fba148287d761c3`  
		Last Modified: Fri, 13 Oct 2023 01:13:51 GMT  
		Size: 12.7 MB (12665364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:e5d87a166e2dad42fa6f525819afb9a640aa0b82b6f7ebf0e5f12e4c65024611
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40344417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e540d2f701ab83d317c63b011be63e392958ad00cce31f3f5f0748db2e0dc8a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:23:52 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:23:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:23:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:23:52 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:23:53 GMT
ADD file:c9b1098bc90ac9b887c3bffdffbcff0c32f32e48df9a673041e3aa796296e69b in / 
# Wed, 04 Oct 2023 12:23:54 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 02:37:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6bd86e5a51fe562347e4392a584c2c048e2caf3c855ee2b39d193782482989d0`  
		Last Modified: Fri, 13 Oct 2023 02:45:03 GMT  
		Size: 27.0 MB (27009502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72b644e1b04fb1dbe3643839ab4b6c1c7562eed7fec98b56653bc7526d1f21b8`  
		Last Modified: Fri, 13 Oct 2023 02:45:00 GMT  
		Size: 13.3 MB (13334915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:72181d85a4df3861bb75602e574739cdd65450d9f1afa978fcecfb324ebf2b82
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.7 MB (47729353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19036cb074a72c8494d631b3bb45bb80bf7b2d181d374dc1c46b8f2bd02b65f0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:08:54 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:08:54 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:08:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:08:55 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:08:57 GMT
ADD file:24bc2f22a395e93a2ebbcfc45da8e5fc7f08e7c03cdc985c997300643d0310ec in / 
# Wed, 04 Oct 2023 12:08:58 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:12:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:56fffb9b8b31e93bce458c1b2532d4e3aabcfa346a00a948fa8702cf6e132f8c`  
		Last Modified: Fri, 13 Oct 2023 07:24:33 GMT  
		Size: 31.9 MB (31886447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a7a715c2447d71e6b94118f081111babef0331bd6104854da882370804c75ae`  
		Last Modified: Fri, 13 Oct 2023 07:24:30 GMT  
		Size: 15.8 MB (15842906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:3e2c1730f17419017837d5f1fc9db6ff833b9dc686ee7b21402e510119d4f4b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40229678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32608e7b5cf27557f6091473da05b6af8a046c450931620144b6162abe38dc78`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 04:29:27 GMT
ARG RELEASE
# Wed, 16 Aug 2023 04:29:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 04:29:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 04:29:28 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 16 Aug 2023 04:29:29 GMT
ADD file:14fcf0756fb29b609af54412c31e2ff9acbf4634984ce95bf204c67668706cb5 in / 
# Wed, 16 Aug 2023 04:29:30 GMT
CMD ["/bin/bash"]
# Fri, 01 Sep 2023 23:16:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e9a6157a42893e6f99bd42ba05c70c5313add95c69f61f12e51517c0100470b8`  
		Last Modified: Fri, 01 Sep 2023 23:24:13 GMT  
		Size: 26.2 MB (26223925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f88ef015543162519d8e086a0bb86351d03f27b98218ff39b27f3b8b7bc2cd`  
		Last Modified: Fri, 01 Sep 2023 23:24:12 GMT  
		Size: 14.0 MB (14005753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:23.04-scm`

```console
$ docker pull buildpack-deps@sha256:9337458ffb6dca2fc2ea67d3c7327ca71f1c6bc4f643d891eb96c8e2968ed8af
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
$ docker pull buildpack-deps@sha256:3476b6f371a5fad9ede92bb3dab111ba19697799847c89c67ffd675834f0a92f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.8 MB (85789207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c1c503d7baadb06f6ca79911e54f8a6167c4eaff6f2ac084de64e505ac9123b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:18:17 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:18:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:18:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:18:18 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:18:19 GMT
ADD file:d4fca0b2b53fa4e2c3e0d721bf983f4095061c5df5fb084d2daf5efad5ee663d in / 
# Wed, 04 Oct 2023 12:18:19 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:19:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 07:20:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:850c6621501406ea0aac62d4ae7a001f98fe81b2085449034055ee7ff32622bc`  
		Last Modified: Thu, 05 Oct 2023 03:34:15 GMT  
		Size: 27.7 MB (27654268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c224a085b3b8f6169f29aeb01a19b302e9163e6122211234d56e34c49a1a52`  
		Last Modified: Fri, 13 Oct 2023 07:27:21 GMT  
		Size: 13.7 MB (13745429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415eed8af6d7f694df1de04bb6a2c5eba418319432d2dec5840be186c2df4971`  
		Last Modified: Fri, 13 Oct 2023 07:27:38 GMT  
		Size: 44.4 MB (44389510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:bc6d4248879ec4a711aa75eade706ef957385237fc45fb1249be243bd0a209b6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.8 MB (86772867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4f5915541d7721f2aa036c93064ae10075f1523f13ff507a800b5d8096b1b82`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:25:21 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:25:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:25:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:25:22 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:25:24 GMT
ADD file:b92305119eab5dd3dfb00f4d83cd84e00c8ae57143739329da5a19aeda55be4e in / 
# Wed, 04 Oct 2023 12:25:24 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 01:05:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 01:06:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0055151e5ef44f81f2355e8073f34f53cc16494749dbc5ba14445ce5edf3d3b6`  
		Last Modified: Fri, 13 Oct 2023 01:13:54 GMT  
		Size: 25.4 MB (25432981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e866c11041f7a46cb12551f8e93dea44f566d63d4fe5e9771fba148287d761c3`  
		Last Modified: Fri, 13 Oct 2023 01:13:51 GMT  
		Size: 12.7 MB (12665364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f378438bc51fcd6e34f3bded8ebdf10b2f56f47951e89908cd028fb60f9d763`  
		Last Modified: Fri, 13 Oct 2023 01:14:13 GMT  
		Size: 48.7 MB (48674522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:5703efee751dc73306c869e77280610707d3d7eb398f10558f4a9f6c52538d3a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.6 MB (84583294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebbfa1bf84c209e495f93ba71668f19434f29ecca4eaabc251d7eba793fcafff`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:23:52 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:23:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:23:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:23:52 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:23:53 GMT
ADD file:c9b1098bc90ac9b887c3bffdffbcff0c32f32e48df9a673041e3aa796296e69b in / 
# Wed, 04 Oct 2023 12:23:54 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 02:37:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 02:38:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6bd86e5a51fe562347e4392a584c2c048e2caf3c855ee2b39d193782482989d0`  
		Last Modified: Fri, 13 Oct 2023 02:45:03 GMT  
		Size: 27.0 MB (27009502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72b644e1b04fb1dbe3643839ab4b6c1c7562eed7fec98b56653bc7526d1f21b8`  
		Last Modified: Fri, 13 Oct 2023 02:45:00 GMT  
		Size: 13.3 MB (13334915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7195734b83041efa5c9550d35f558288d4c59268de32267217d78d00f7cd0dbb`  
		Last Modified: Fri, 13 Oct 2023 02:45:18 GMT  
		Size: 44.2 MB (44238877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:52c33c87b291babb142f130127cb1470b7d82a6145d9aad084a78c88e4c80a2b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.8 MB (96819195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c6787c6550b1e4654d8c1b55c5d617b828335b2ba56fa69d00283241fbecbeb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:08:54 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:08:54 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:08:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:08:55 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:08:57 GMT
ADD file:24bc2f22a395e93a2ebbcfc45da8e5fc7f08e7c03cdc985c997300643d0310ec in / 
# Wed, 04 Oct 2023 12:08:58 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:12:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 07:13:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:56fffb9b8b31e93bce458c1b2532d4e3aabcfa346a00a948fa8702cf6e132f8c`  
		Last Modified: Fri, 13 Oct 2023 07:24:33 GMT  
		Size: 31.9 MB (31886447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a7a715c2447d71e6b94118f081111babef0331bd6104854da882370804c75ae`  
		Last Modified: Fri, 13 Oct 2023 07:24:30 GMT  
		Size: 15.8 MB (15842906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348f4703e93699e4c8ee248cbcc6f18ffaa75e71f9acb2b1a47c6a957a410e6f`  
		Last Modified: Fri, 13 Oct 2023 07:24:51 GMT  
		Size: 49.1 MB (49089842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b2f2a0881286b29de742d50d48259b750a115827b358237c1669ced83f74796e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84505154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7decbe5c1b3961eed7d080573346ae9c054116dc044e81c734abe9ee131cc04d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 04:29:27 GMT
ARG RELEASE
# Wed, 16 Aug 2023 04:29:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 04:29:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 04:29:28 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 16 Aug 2023 04:29:29 GMT
ADD file:14fcf0756fb29b609af54412c31e2ff9acbf4634984ce95bf204c67668706cb5 in / 
# Wed, 16 Aug 2023 04:29:30 GMT
CMD ["/bin/bash"]
# Fri, 01 Sep 2023 23:16:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Sep 2023 23:16:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e9a6157a42893e6f99bd42ba05c70c5313add95c69f61f12e51517c0100470b8`  
		Last Modified: Fri, 01 Sep 2023 23:24:13 GMT  
		Size: 26.2 MB (26223925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f88ef015543162519d8e086a0bb86351d03f27b98218ff39b27f3b8b7bc2cd`  
		Last Modified: Fri, 01 Sep 2023 23:24:12 GMT  
		Size: 14.0 MB (14005753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ad80a5cffb7414f3bd06d5dafc212e2f5a767d3312bead7347e2ba8fae5be35`  
		Last Modified: Fri, 01 Sep 2023 23:24:25 GMT  
		Size: 44.3 MB (44275476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:23.10`

```console
$ docker pull buildpack-deps@sha256:cce4098beee8d4c14a14de9efd05c187c5bc97bdb07a5fa2f4632bbdcf5cb278
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
$ docker pull buildpack-deps@sha256:1ffcc35dc1dfb9751e3339a92471844f54a1b2147c79b4e8a2f45a71137f768d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.1 MB (290073464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bad52367cc0f5c2f3115a8f96c1cb83c0c7bd5fb223d3ff41958867aceb72e3f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 05:03:43 GMT
ARG RELEASE
# Tue, 26 Sep 2023 05:03:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 05:03:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 05:03:43 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 05:03:45 GMT
ADD file:5fb49f260a0c3bf404c0fe31d8f0f812e9c143bd48223c4f15a85168758eb880 in / 
# Tue, 26 Sep 2023 05:03:45 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 05:02:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 05:03:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 05:07:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70c34fc37a9391a001a8d99c74b27823143398763bcd623c3402a790006947ea`  
		Last Modified: Tue, 03 Oct 2023 05:09:43 GMT  
		Size: 28.1 MB (28079281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13daebad235cc5fc75272df7a4cd22cd9e14040be8b10d9ec3764328c7be1ab`  
		Last Modified: Tue, 03 Oct 2023 05:09:41 GMT  
		Size: 13.9 MB (13886180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5024b0813f45b8c3c3d60316917bb453d13c81a8bab8316b17b30ac61156c6`  
		Last Modified: Tue, 03 Oct 2023 05:09:58 GMT  
		Size: 44.8 MB (44761138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd79646f814aefe34908af38903a3d5522c9455086876d9b84dda6633503c1d`  
		Last Modified: Tue, 03 Oct 2023 05:10:33 GMT  
		Size: 203.3 MB (203346865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.10` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:813769c747356c26587f8f75e5e91dc7dfba62b1610307b0c37b2e735245b43e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.4 MB (255352078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8caa1868f243e98eacc3ad77eb6a890dda6b40ba0b8ba30f275d201a970250a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 05:05:03 GMT
ARG RELEASE
# Tue, 26 Sep 2023 05:05:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 05:05:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 05:05:04 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 05:05:08 GMT
ADD file:512405a66f1049a7237c67d9d5776db7f41d5991eceec535260f4d3b7f19e65d in / 
# Tue, 26 Sep 2023 05:05:09 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 06:11:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 06:12:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 06:15:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70fb529e8caade31afb15a43cbaa98da4446d46bd64b25df10259be9a57f0577`  
		Last Modified: Tue, 03 Oct 2023 06:17:59 GMT  
		Size: 26.1 MB (26055984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7003bc3702b787e6176ad194751c3ba0ff76742ea89883d5b9e9bf4a15d93fb`  
		Last Modified: Tue, 03 Oct 2023 06:17:56 GMT  
		Size: 12.7 MB (12713461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fe360aefbe92efc04c5f077bc27baf1ae132ca6e543274ac4e2180efca7507c`  
		Last Modified: Tue, 03 Oct 2023 06:18:16 GMT  
		Size: 48.9 MB (48941849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdde41a257818412d92d75797a26ae9b4eaf5754d92345240d67cabdcba126ca`  
		Last Modified: Tue, 03 Oct 2023 06:18:47 GMT  
		Size: 167.6 MB (167640784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.10` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:14dcc77b25c7b3b5166ab0ef658f1c709bebc6b9b3392c1f144c50d51e7bc5c9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.4 MB (281404865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52326c95116b4ac6d7b8b8a2ee8e3143988a13531ba81915c44bb0a5f02256bd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 05:06:27 GMT
ARG RELEASE
# Tue, 26 Sep 2023 05:06:27 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 05:06:27 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 05:06:27 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 05:06:30 GMT
ADD file:0dbbd4de9483bc32897d525742b94aa13ebd3a6aac7f1844d94d7f4536b2bfb8 in / 
# Tue, 26 Sep 2023 05:06:30 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 06:17:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 06:18:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 06:21:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4259d3adacfee572bed7acadc8e4af2cf679658d229fc94eb25abeb6d662693a`  
		Last Modified: Tue, 03 Oct 2023 06:23:31 GMT  
		Size: 27.3 MB (27315811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56e515aa13e7ac1bba03883084849baef28268d175299a636c354b0e7558af88`  
		Last Modified: Tue, 03 Oct 2023 06:23:28 GMT  
		Size: 13.4 MB (13394041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a515dbb7fdd56d447a83b9c10d1e2ec2fb52e85daf470e09424283d14b5908`  
		Last Modified: Tue, 03 Oct 2023 06:23:44 GMT  
		Size: 44.6 MB (44631383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5870521b137c9f0e7e635cf3385f6c2f67138f6b1620432d51425b77ad10a08`  
		Last Modified: Tue, 03 Oct 2023 06:24:11 GMT  
		Size: 196.1 MB (196063630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.10` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:028eee089be0c465e58258e0093f5277d4e9702ca58ad77f89cedb2c7a8d928d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.0 MB (305008436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a55e4f421197c52b398250bfa25af66d31da985efcde6dbb6b44a2d40305f5b1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 04:52:53 GMT
ARG RELEASE
# Tue, 26 Sep 2023 04:52:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 04:52:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 04:52:54 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 04:52:56 GMT
ADD file:cbeb7f814c9eebdbdc6b8e10fb87ba8334b3f6203ceb166c48f6d7492ab07c4e in / 
# Tue, 26 Sep 2023 04:52:57 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 09:07:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 09:09:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 09:13:48 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:37af6e7cc6b51a4931dbbb51fab85a97161b0e873fc4984f882f48b10b6e52ff`  
		Last Modified: Tue, 03 Oct 2023 09:16:29 GMT  
		Size: 32.3 MB (32340811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5d9e5d675f5b5c56fe9add6cc8a5eb4e0a1d64fbd641984262d3d8e948b074`  
		Last Modified: Tue, 03 Oct 2023 09:16:25 GMT  
		Size: 15.9 MB (15938905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4b5786f2a975233c15614192b6873d23e3731274d109e63aa998b076d7a32f`  
		Last Modified: Tue, 03 Oct 2023 09:16:51 GMT  
		Size: 49.5 MB (49536647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db1518dc6279ec2984f0732cff49e7750b0230e674eb7e39fedd5e2ce7b0bf5b`  
		Last Modified: Tue, 03 Oct 2023 09:17:48 GMT  
		Size: 207.2 MB (207192073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.10` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:452d2d3a6dc77f07166211f76c6055b84c94b6f5e4a06de71349502bcf01ca3b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.5 MB (267507888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e250b3afe33fea9aae901344bb048b329f78d5e15ec826b414308684794425da`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 04:58:19 GMT
ARG RELEASE
# Tue, 26 Sep 2023 04:58:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 04:58:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 04:58:19 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 04:58:21 GMT
ADD file:e86e9b7546a97fa45e9c726cc317a624a7f94b0bd6dd413d89946ff778b18c77 in / 
# Tue, 26 Sep 2023 04:58:21 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 08:54:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 08:54:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 08:57:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:075a43ce09c6e3edbaa35c043b92a1f4c22b8237baa8de4238146e73630250f0`  
		Last Modified: Tue, 03 Oct 2023 09:01:27 GMT  
		Size: 27.6 MB (27623930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b703fa59fe447e054dd8349236278bd073fff635a41311e301569818f07b73b`  
		Last Modified: Tue, 03 Oct 2023 09:01:26 GMT  
		Size: 14.3 MB (14252775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37839377f33f6c3908cfc767a87a21aa81078a4c1959d18de0adab7d94a882d7`  
		Last Modified: Tue, 03 Oct 2023 09:01:50 GMT  
		Size: 45.2 MB (45206881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109a36ba84f6ccbc7952cf40798defc4982c663fa313314706cbfcd75ca2d128`  
		Last Modified: Tue, 03 Oct 2023 09:02:26 GMT  
		Size: 180.4 MB (180424302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:23.10-curl`

```console
$ docker pull buildpack-deps@sha256:f441a6eef343f7751e5dcfa035a98f6b5ccf3c885282d5ddf60c3ba41ed66ee4
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
$ docker pull buildpack-deps@sha256:8f1f81aef045cb4cb1dd04855313ecf0547e82d082914dfa6f5dc608b9f14c66
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (41965461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90765c24b416ae58d6e2266669124bc5049859b2fb076aa733c15a8e524e6e89`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 05:03:43 GMT
ARG RELEASE
# Tue, 26 Sep 2023 05:03:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 05:03:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 05:03:43 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 05:03:45 GMT
ADD file:5fb49f260a0c3bf404c0fe31d8f0f812e9c143bd48223c4f15a85168758eb880 in / 
# Tue, 26 Sep 2023 05:03:45 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 05:02:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70c34fc37a9391a001a8d99c74b27823143398763bcd623c3402a790006947ea`  
		Last Modified: Tue, 03 Oct 2023 05:09:43 GMT  
		Size: 28.1 MB (28079281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13daebad235cc5fc75272df7a4cd22cd9e14040be8b10d9ec3764328c7be1ab`  
		Last Modified: Tue, 03 Oct 2023 05:09:41 GMT  
		Size: 13.9 MB (13886180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.10-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:4f8231c37928bfd6d019f0a4da9fecebbfbe54a3f18b17227fd2da974dccf0e8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38769445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:154aa23af9f19fda735574c488545e91de641bc48dc5e6ccc05d7054dd6c1f27`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 05:05:03 GMT
ARG RELEASE
# Tue, 26 Sep 2023 05:05:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 05:05:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 05:05:04 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 05:05:08 GMT
ADD file:512405a66f1049a7237c67d9d5776db7f41d5991eceec535260f4d3b7f19e65d in / 
# Tue, 26 Sep 2023 05:05:09 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 06:11:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70fb529e8caade31afb15a43cbaa98da4446d46bd64b25df10259be9a57f0577`  
		Last Modified: Tue, 03 Oct 2023 06:17:59 GMT  
		Size: 26.1 MB (26055984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7003bc3702b787e6176ad194751c3ba0ff76742ea89883d5b9e9bf4a15d93fb`  
		Last Modified: Tue, 03 Oct 2023 06:17:56 GMT  
		Size: 12.7 MB (12713461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.10-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f01bdb766fa4849cb4f10a0809a8b5b498d4d0c97c7cc913302bfe7351c7e0ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.7 MB (40709852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72ffd9a6b28e4a8cb359ccf7d53e1f0df441ab57357eb6b0a53dacfcfedaea64`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 05:06:27 GMT
ARG RELEASE
# Tue, 26 Sep 2023 05:06:27 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 05:06:27 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 05:06:27 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 05:06:30 GMT
ADD file:0dbbd4de9483bc32897d525742b94aa13ebd3a6aac7f1844d94d7f4536b2bfb8 in / 
# Tue, 26 Sep 2023 05:06:30 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 06:17:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4259d3adacfee572bed7acadc8e4af2cf679658d229fc94eb25abeb6d662693a`  
		Last Modified: Tue, 03 Oct 2023 06:23:31 GMT  
		Size: 27.3 MB (27315811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56e515aa13e7ac1bba03883084849baef28268d175299a636c354b0e7558af88`  
		Last Modified: Tue, 03 Oct 2023 06:23:28 GMT  
		Size: 13.4 MB (13394041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.10-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:19c8a3b69e40dbebcc75a0a74eb2fccceef5f019bfb07e77681b55a65cd875d6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.3 MB (48279716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb0121e33449b2dd034ad8435b0fd1f59f3e7e5cfdd4f76ab3a8084e34474879`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 04:52:53 GMT
ARG RELEASE
# Tue, 26 Sep 2023 04:52:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 04:52:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 04:52:54 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 04:52:56 GMT
ADD file:cbeb7f814c9eebdbdc6b8e10fb87ba8334b3f6203ceb166c48f6d7492ab07c4e in / 
# Tue, 26 Sep 2023 04:52:57 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 09:07:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:37af6e7cc6b51a4931dbbb51fab85a97161b0e873fc4984f882f48b10b6e52ff`  
		Last Modified: Tue, 03 Oct 2023 09:16:29 GMT  
		Size: 32.3 MB (32340811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5d9e5d675f5b5c56fe9add6cc8a5eb4e0a1d64fbd641984262d3d8e948b074`  
		Last Modified: Tue, 03 Oct 2023 09:16:25 GMT  
		Size: 15.9 MB (15938905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.10-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:3c2543e24855f9466398d6b5283ed99d43c31e6eecb7c8a666fab77844e51f3b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41876705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98f6a5d197679893fff32c1e7e76ceb58cef5345e4214aa24c8a6b1c6e6ec05e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 04:58:19 GMT
ARG RELEASE
# Tue, 26 Sep 2023 04:58:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 04:58:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 04:58:19 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 04:58:21 GMT
ADD file:e86e9b7546a97fa45e9c726cc317a624a7f94b0bd6dd413d89946ff778b18c77 in / 
# Tue, 26 Sep 2023 04:58:21 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 08:54:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:075a43ce09c6e3edbaa35c043b92a1f4c22b8237baa8de4238146e73630250f0`  
		Last Modified: Tue, 03 Oct 2023 09:01:27 GMT  
		Size: 27.6 MB (27623930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b703fa59fe447e054dd8349236278bd073fff635a41311e301569818f07b73b`  
		Last Modified: Tue, 03 Oct 2023 09:01:26 GMT  
		Size: 14.3 MB (14252775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:23.10-scm`

```console
$ docker pull buildpack-deps@sha256:d77e951abdeb73a2dd14ba7bdff99b65cf8868b29fbd2c5bdbceb4ee0f503485
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
$ docker pull buildpack-deps@sha256:7154ee606209e01dfbdb5a98d17f4e66e941f7c1c80af9ba1f3c13303f684b38
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.7 MB (86726599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25d00e70f23db7ea7bb66c70316bc7fdc44a79fb1fd30b985055907d46d8dd27`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 05:03:43 GMT
ARG RELEASE
# Tue, 26 Sep 2023 05:03:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 05:03:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 05:03:43 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 05:03:45 GMT
ADD file:5fb49f260a0c3bf404c0fe31d8f0f812e9c143bd48223c4f15a85168758eb880 in / 
# Tue, 26 Sep 2023 05:03:45 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 05:02:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 05:03:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70c34fc37a9391a001a8d99c74b27823143398763bcd623c3402a790006947ea`  
		Last Modified: Tue, 03 Oct 2023 05:09:43 GMT  
		Size: 28.1 MB (28079281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13daebad235cc5fc75272df7a4cd22cd9e14040be8b10d9ec3764328c7be1ab`  
		Last Modified: Tue, 03 Oct 2023 05:09:41 GMT  
		Size: 13.9 MB (13886180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5024b0813f45b8c3c3d60316917bb453d13c81a8bab8316b17b30ac61156c6`  
		Last Modified: Tue, 03 Oct 2023 05:09:58 GMT  
		Size: 44.8 MB (44761138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.10-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:e198556ecbcc37ab2297352a3ff1845d949b22d85928d97229b1e457431319a4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.7 MB (87711294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09a6f4028f29d6923b5eb801f6947578178f8c808b23aa54095ed940196f8a28`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 05:05:03 GMT
ARG RELEASE
# Tue, 26 Sep 2023 05:05:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 05:05:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 05:05:04 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 05:05:08 GMT
ADD file:512405a66f1049a7237c67d9d5776db7f41d5991eceec535260f4d3b7f19e65d in / 
# Tue, 26 Sep 2023 05:05:09 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 06:11:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 06:12:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70fb529e8caade31afb15a43cbaa98da4446d46bd64b25df10259be9a57f0577`  
		Last Modified: Tue, 03 Oct 2023 06:17:59 GMT  
		Size: 26.1 MB (26055984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7003bc3702b787e6176ad194751c3ba0ff76742ea89883d5b9e9bf4a15d93fb`  
		Last Modified: Tue, 03 Oct 2023 06:17:56 GMT  
		Size: 12.7 MB (12713461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fe360aefbe92efc04c5f077bc27baf1ae132ca6e543274ac4e2180efca7507c`  
		Last Modified: Tue, 03 Oct 2023 06:18:16 GMT  
		Size: 48.9 MB (48941849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.10-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:b90f855ca6f36a58ffa93d51518b716154ce46f2501c052255a4ca69820f5f40
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.3 MB (85341235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1353821bcafbdc837c170ac7e68154a2784c2c9be1397d618829b032d0afd42a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 05:06:27 GMT
ARG RELEASE
# Tue, 26 Sep 2023 05:06:27 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 05:06:27 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 05:06:27 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 05:06:30 GMT
ADD file:0dbbd4de9483bc32897d525742b94aa13ebd3a6aac7f1844d94d7f4536b2bfb8 in / 
# Tue, 26 Sep 2023 05:06:30 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 06:17:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 06:18:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4259d3adacfee572bed7acadc8e4af2cf679658d229fc94eb25abeb6d662693a`  
		Last Modified: Tue, 03 Oct 2023 06:23:31 GMT  
		Size: 27.3 MB (27315811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56e515aa13e7ac1bba03883084849baef28268d175299a636c354b0e7558af88`  
		Last Modified: Tue, 03 Oct 2023 06:23:28 GMT  
		Size: 13.4 MB (13394041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a515dbb7fdd56d447a83b9c10d1e2ec2fb52e85daf470e09424283d14b5908`  
		Last Modified: Tue, 03 Oct 2023 06:23:44 GMT  
		Size: 44.6 MB (44631383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.10-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:acbd20745f2d3bf4eea92a5ae1ac2b8804313963facdce14255800f238f17712
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.8 MB (97816363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbfadc597734b0797716241519be9e98eea7bb25158e76398d42c3fb1d0366c3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 04:52:53 GMT
ARG RELEASE
# Tue, 26 Sep 2023 04:52:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 04:52:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 04:52:54 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 04:52:56 GMT
ADD file:cbeb7f814c9eebdbdc6b8e10fb87ba8334b3f6203ceb166c48f6d7492ab07c4e in / 
# Tue, 26 Sep 2023 04:52:57 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 09:07:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 09:09:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:37af6e7cc6b51a4931dbbb51fab85a97161b0e873fc4984f882f48b10b6e52ff`  
		Last Modified: Tue, 03 Oct 2023 09:16:29 GMT  
		Size: 32.3 MB (32340811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5d9e5d675f5b5c56fe9add6cc8a5eb4e0a1d64fbd641984262d3d8e948b074`  
		Last Modified: Tue, 03 Oct 2023 09:16:25 GMT  
		Size: 15.9 MB (15938905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4b5786f2a975233c15614192b6873d23e3731274d109e63aa998b076d7a32f`  
		Last Modified: Tue, 03 Oct 2023 09:16:51 GMT  
		Size: 49.5 MB (49536647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.10-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:7ba205206c01993460abc949cb42dd5a14f530a2a21cdd5b3c733d628d0d3546
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.1 MB (87083586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a73fb50f78e1bb0c4a8281876e5d8202f69f3bd80ec2901e296e2a620b18304`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 04:58:19 GMT
ARG RELEASE
# Tue, 26 Sep 2023 04:58:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 04:58:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 04:58:19 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 04:58:21 GMT
ADD file:e86e9b7546a97fa45e9c726cc317a624a7f94b0bd6dd413d89946ff778b18c77 in / 
# Tue, 26 Sep 2023 04:58:21 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 08:54:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 08:54:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:075a43ce09c6e3edbaa35c043b92a1f4c22b8237baa8de4238146e73630250f0`  
		Last Modified: Tue, 03 Oct 2023 09:01:27 GMT  
		Size: 27.6 MB (27623930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b703fa59fe447e054dd8349236278bd073fff635a41311e301569818f07b73b`  
		Last Modified: Tue, 03 Oct 2023 09:01:26 GMT  
		Size: 14.3 MB (14252775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37839377f33f6c3908cfc767a87a21aa81078a4c1959d18de0adab7d94a882d7`  
		Last Modified: Tue, 03 Oct 2023 09:01:50 GMT  
		Size: 45.2 MB (45206881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bookworm`

```console
$ docker pull buildpack-deps@sha256:584ae312404463556590dbd340dc888147030cb3c8cbaec1ae7fc474ac453fdd
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
$ docker pull buildpack-deps@sha256:e5e5c80b6c13eb1ac931b319d5b2dda3a67473c085edc2ef5212ee628f4ee6bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.8 MB (348827828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c9f4bf96c80ab0bd24165e83092eab60265322c4575d970deaae7e8a4742ea3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:37 GMT
ADD file:1e4dd5dab602337b5d5ef8d84b8dbe8b1ac62225f077b29b27d045842486d8e2 in / 
# Wed, 11 Oct 2023 18:34:37 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:19:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:19:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:20:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0a9573503463fd3166b5b1f34a7720dac28609e98d731e50e7068f92e79b8545`  
		Last Modified: Wed, 11 Oct 2023 18:39:10 GMT  
		Size: 49.6 MB (49582224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ccc26d841b4acc2562483bf393ce1cf8bc358ced09ccd825425226827c79c92`  
		Last Modified: Thu, 12 Oct 2023 03:28:45 GMT  
		Size: 24.1 MB (24051259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800d84653581fc119cd75cd572fa190d3b813d49221b9e5ee463e3560e2cb342`  
		Last Modified: Thu, 12 Oct 2023 03:29:04 GMT  
		Size: 64.1 MB (64130287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c632e57ea62ea950c367f484f52cdcfd2adb12060a31f5c413f40db9822e96e`  
		Last Modified: Thu, 12 Oct 2023 03:29:40 GMT  
		Size: 211.1 MB (211064058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:86d28c1e87df6d4e3309e403a9ced8594ad1380ffb29db3cbb99ee65245d77e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.0 MB (316030711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f61c441d8080fa400d21357cb9170445e8b0e150d15c350be1e20d0849837a84`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:37:30 GMT
ADD file:c07cf5c750a3e3c7ff84a3a3b8fc6087c9c5e0639d7bf638f0556d0a94309919 in / 
# Wed, 11 Oct 2023 17:37:35 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:04:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:05:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:06:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b7ec6536594e6c45ab234eecb51aacd85440ddc0e6da5873de23938ff146b5ec`  
		Last Modified: Wed, 11 Oct 2023 17:40:19 GMT  
		Size: 47.4 MB (47355749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ec943df1872e82ab3efa51bd5b2d7aac598550123e6db67156283ade7509d1`  
		Last Modified: Wed, 11 Oct 2023 18:14:31 GMT  
		Size: 22.7 MB (22729282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9f5c18924658cf6e03e52e00ddbf230cb1925aa017edb92b3cd508ec76293f`  
		Last Modified: Wed, 11 Oct 2023 18:14:54 GMT  
		Size: 61.6 MB (61561678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7670741713d795c2814eacfe8b75187f28e3485379b6fb2770c71d163e26127`  
		Last Modified: Wed, 11 Oct 2023 18:15:37 GMT  
		Size: 184.4 MB (184384002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:28ad6736c4c7a5c78602a4c42becc99de682ba5927aa95ad9f5105294d099a8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.4 MB (301449230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43d67f8c14cfd8cddba9828203d94136bcc749df068cfbc834ba011ede605f79`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:41:59 GMT
ADD file:914e8a43f38c44fe9a6aabf05bbf3ebad5530966a354c8e7bb873c0842d35256 in / 
# Wed, 11 Oct 2023 17:42:00 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:45:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:45:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:46:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:65b9f3344eccdad2292cc7eec885befe05a52ec1136e145130c849441428eee6`  
		Last Modified: Wed, 11 Oct 2023 17:45:56 GMT  
		Size: 45.2 MB (45180287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbdddb82776e8c5901a821d5034c82b0fcba2993014440cd080d0592cd49616`  
		Last Modified: Thu, 12 Oct 2023 03:55:58 GMT  
		Size: 22.0 MB (21953833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f9d9ae792bc9a3749049ab80543cfddbda8910bcaffc9c95c7db4feb9e625a6`  
		Last Modified: Thu, 12 Oct 2023 03:56:18 GMT  
		Size: 59.3 MB (59266472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9912e09bb3246583228b0aa9f45499f60d04bbb57d5db9e63d50fd5585cc0c20`  
		Last Modified: Thu, 12 Oct 2023 03:56:58 GMT  
		Size: 175.0 MB (175048638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:1217daf5693bf080affa2383e80682e4ed80fa25c7b6889924e21e401abfef07
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.6 MB (339643434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13543f9c2ab23caf4e23f3900fa93f86e7a0d57bbfb3dfb296c3985b777511b8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:43 GMT
ADD file:bf4264671bd91eb30c67d512144ebcf7f5c55a3e490ebe7876fa9b20d433bf7b in / 
# Wed, 11 Oct 2023 18:24:44 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:44:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:45:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:46:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e720f94321d63ecb6efa873b294dce7eaa1c3a5ddcd5bf7daddf375b955669a4`  
		Last Modified: Wed, 11 Oct 2023 18:28:04 GMT  
		Size: 49.6 MB (49612578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7541d83e7b8c0f5f6cacacddfcf5fdd942793f13418bc4645203b4ab4f3de3`  
		Last Modified: Wed, 11 Oct 2023 19:53:48 GMT  
		Size: 23.6 MB (23588086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a653d69b7b96df6835b157d043d7b926f776531e96c9263f4c7dae0033514d`  
		Last Modified: Wed, 11 Oct 2023 19:54:07 GMT  
		Size: 64.0 MB (63994319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c02d5d50082e4632f070b715dfd5d3a3680e35e0434a1281edbcfdc3cdff52dc`  
		Last Modified: Wed, 11 Oct 2023 19:54:39 GMT  
		Size: 202.4 MB (202448451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:1a6a219086627846d966e869a8d56fd78994fb747da91f49e6a46a674ef778c6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.5 MB (351462994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f4402f88a53734d262ec398d9da3786d89072972edfbbc52175a078d23b80d0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:40:29 GMT
ADD file:0b6fc66d778d0cd8ae8b17b92945d98cc34f9c7008cda864ed0a54b5e40b9cb0 in / 
# Wed, 11 Oct 2023 17:40:32 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:09:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:10:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:11:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:501a599c15b6def048b2e00cfdf6c658061c00a504305ef2075fb1009a62c1e2`  
		Last Modified: Wed, 11 Oct 2023 17:45:01 GMT  
		Size: 50.6 MB (50600791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf9d6abbf47f32cac71cefb6f7233e5f700d4f6f941ca631e29947c5f1df955`  
		Last Modified: Wed, 11 Oct 2023 18:21:57 GMT  
		Size: 24.9 MB (24887201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1693c4d42b110c48ad84138aa8c91e1aeffbed6ca630f12495f711b89609823`  
		Last Modified: Wed, 11 Oct 2023 18:22:27 GMT  
		Size: 66.0 MB (65984002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d61ba44e3cf60d5c6195ef4448de7160aff21051156b51d78755d19cb401055`  
		Last Modified: Wed, 11 Oct 2023 18:23:24 GMT  
		Size: 210.0 MB (209991000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:b585c2f0cfabe530c3905bb95c637eb6339c7663273b893ede5b4d8cacd9233b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.6 MB (325624324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01ae125d4ffa592dfd3716595bf2806c88e2b3b84e7cdc94482338771a440d1c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:48:50 GMT
ADD file:b081db8d48290ef5b5f477edb85d8f04d62a6995ec09bdb516d66dbe19b98137 in / 
# Wed, 11 Oct 2023 17:48:55 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:19:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:20:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:26:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:54dda4e4d31846b7324172a7fda3d0bdc7d8a2105ab27e9a92c2db43f35f9e5d`  
		Last Modified: Wed, 11 Oct 2023 17:59:53 GMT  
		Size: 49.6 MB (49569257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370a64ae3420fd85a23128ef46431df034f9038821764a14bb436272a1345505`  
		Last Modified: Wed, 11 Oct 2023 23:55:20 GMT  
		Size: 23.4 MB (23439567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c19b06553268b2cbcf576e075fdb1ac8c430154167258bcd4f925d5938117659`  
		Last Modified: Wed, 11 Oct 2023 23:56:13 GMT  
		Size: 63.0 MB (62962779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe7e7187a4f54c6c9e49f439f18fe1ae7a7f06894b24eae29001a71e03340c5`  
		Last Modified: Wed, 11 Oct 2023 23:58:22 GMT  
		Size: 189.7 MB (189652721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:12b9dc56603f357d0e68e2cd0927be121561f588bc3f728ed3a1fb3dc0ec9ded
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **363.0 MB (362953503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7467ffe1bf70430528cbbee8f716bd707ff747ee7ff42c2f77578884a1c214d6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:44:01 GMT
ADD file:ed515e1aef8321271c6544e30cbeb31257e9640979e8f68a9e490cb25d3525fd in / 
# Wed, 11 Oct 2023 17:44:04 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:14:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:15:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:19:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f137383853e717724a59e86aa526d31eabb4a5d45a259cd1ade68d93b3f45ae9`  
		Last Modified: Wed, 11 Oct 2023 17:49:27 GMT  
		Size: 53.6 MB (53575984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da754908592cac64ca75d9cdc8c43a4a396901108de4adae61bd92937de4f65`  
		Last Modified: Wed, 11 Oct 2023 18:36:14 GMT  
		Size: 25.7 MB (25700026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524b67dc97fb52dd33f61fe12da424874443bb200789c7cfde14425f85938f54`  
		Last Modified: Wed, 11 Oct 2023 18:36:46 GMT  
		Size: 69.6 MB (69584544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7449a547606da3836fd2405c85ed15e48ed96b7936fe9dfcbb8c69e21475738e`  
		Last Modified: Wed, 11 Oct 2023 18:37:46 GMT  
		Size: 214.1 MB (214092949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:eb83643215e451aa8409fe1fec979764362831916fa9a2955baa57c263d6631f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.2 MB (318222519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42abbfd998057c2e0c5d1c31d39f5a383b5ce7201d011ae9066f0214cd94321c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:50:07 GMT
ADD file:2dc117136732884ad4b058065700dd66cc49d6ce56b0fdbb672915e3ad8adb84 in / 
# Wed, 11 Oct 2023 17:50:10 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:51:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:52:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:58:19 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ad5e374600bf40a929dfe51e52737e4ca04aba83f499656760ba938841fb6552`  
		Last Modified: Wed, 11 Oct 2023 17:55:18 GMT  
		Size: 47.9 MB (47942934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6344f505670ce139b1b3f472749240f33304ec7535daae4a72913a6da08f304f`  
		Last Modified: Thu, 12 Oct 2023 00:33:20 GMT  
		Size: 24.0 MB (24046768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf2b4ce0798e7985dd88d10311ea2a2730812d4e10c9a8f24f564875c6cb617`  
		Last Modified: Thu, 12 Oct 2023 00:33:56 GMT  
		Size: 63.1 MB (63132898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317490e394e1c9331e54c7c33215628d4d08a8cd9d2191cb3d294d0b021a18f9`  
		Last Modified: Thu, 12 Oct 2023 00:34:47 GMT  
		Size: 183.1 MB (183099919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bookworm-curl`

```console
$ docker pull buildpack-deps@sha256:ce8ea34dd6046d5bd7bc423fbee3460e246b576dcd581e5ba6583f3535b55fcd
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
$ docker pull buildpack-deps@sha256:977f8a0eade986703e1379ef96d1c106c53eccfef6eb0dace01f3f404dd41db3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73633483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6190da4faf36a08749338aa0f80e05ce0f4a16fc3164c506cc7cd23b0b6e665c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:37 GMT
ADD file:1e4dd5dab602337b5d5ef8d84b8dbe8b1ac62225f077b29b27d045842486d8e2 in / 
# Wed, 11 Oct 2023 18:34:37 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:19:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0a9573503463fd3166b5b1f34a7720dac28609e98d731e50e7068f92e79b8545`  
		Last Modified: Wed, 11 Oct 2023 18:39:10 GMT  
		Size: 49.6 MB (49582224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ccc26d841b4acc2562483bf393ce1cf8bc358ced09ccd825425226827c79c92`  
		Last Modified: Thu, 12 Oct 2023 03:28:45 GMT  
		Size: 24.1 MB (24051259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:26df1627a60457168bc3b15d71211f6b2233409c7dcd192decbae29947006323
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.1 MB (70085031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ef4b4f6796a04df75ac23eda97d56908155655aca64a22dceb52210e8ef9956`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:37:30 GMT
ADD file:c07cf5c750a3e3c7ff84a3a3b8fc6087c9c5e0639d7bf638f0556d0a94309919 in / 
# Wed, 11 Oct 2023 17:37:35 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:04:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b7ec6536594e6c45ab234eecb51aacd85440ddc0e6da5873de23938ff146b5ec`  
		Last Modified: Wed, 11 Oct 2023 17:40:19 GMT  
		Size: 47.4 MB (47355749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ec943df1872e82ab3efa51bd5b2d7aac598550123e6db67156283ade7509d1`  
		Last Modified: Wed, 11 Oct 2023 18:14:31 GMT  
		Size: 22.7 MB (22729282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:c88279d74fb84bd9e91e1631a6f8be701529d90987a5bd1877a7c1741aaddf11
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67134120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:922f8718561dcde238f85464ae864269e429eda3b44a3124b8a1c955d881c183`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:41:59 GMT
ADD file:914e8a43f38c44fe9a6aabf05bbf3ebad5530966a354c8e7bb873c0842d35256 in / 
# Wed, 11 Oct 2023 17:42:00 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:45:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:65b9f3344eccdad2292cc7eec885befe05a52ec1136e145130c849441428eee6`  
		Last Modified: Wed, 11 Oct 2023 17:45:56 GMT  
		Size: 45.2 MB (45180287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbdddb82776e8c5901a821d5034c82b0fcba2993014440cd080d0592cd49616`  
		Last Modified: Thu, 12 Oct 2023 03:55:58 GMT  
		Size: 22.0 MB (21953833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3336852231c4838575dca42d951ad5ef02897709b046c708ab77d49bf73af01c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73200664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a61350e5fd6e43ba2eafdd779f92c81d1adcc19b9614cd2c2a8a88b2f7ff2b7e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:43 GMT
ADD file:bf4264671bd91eb30c67d512144ebcf7f5c55a3e490ebe7876fa9b20d433bf7b in / 
# Wed, 11 Oct 2023 18:24:44 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:44:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e720f94321d63ecb6efa873b294dce7eaa1c3a5ddcd5bf7daddf375b955669a4`  
		Last Modified: Wed, 11 Oct 2023 18:28:04 GMT  
		Size: 49.6 MB (49612578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7541d83e7b8c0f5f6cacacddfcf5fdd942793f13418bc4645203b4ab4f3de3`  
		Last Modified: Wed, 11 Oct 2023 19:53:48 GMT  
		Size: 23.6 MB (23588086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:af61129a918d7d5a838f84a53e5c4187bfad03a62baf89b590e2eee9e0ccbd15
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.5 MB (75487992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8222a221a97a3218fabbfecba1af542b4002d5b5999bdcecc8a82f8e724c78a7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:40:29 GMT
ADD file:0b6fc66d778d0cd8ae8b17b92945d98cc34f9c7008cda864ed0a54b5e40b9cb0 in / 
# Wed, 11 Oct 2023 17:40:32 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:09:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:501a599c15b6def048b2e00cfdf6c658061c00a504305ef2075fb1009a62c1e2`  
		Last Modified: Wed, 11 Oct 2023 17:45:01 GMT  
		Size: 50.6 MB (50600791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf9d6abbf47f32cac71cefb6f7233e5f700d4f6f941ca631e29947c5f1df955`  
		Last Modified: Wed, 11 Oct 2023 18:21:57 GMT  
		Size: 24.9 MB (24887201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:5019b5e06e6411dc6681b042d91c4166bda9f959281d3afb18a28b2c51859fe1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (73008824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a14c97aa10bb55fcde7d0ab1936a74404ebc81297baed7f34e394b13f6e1be9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:48:50 GMT
ADD file:b081db8d48290ef5b5f477edb85d8f04d62a6995ec09bdb516d66dbe19b98137 in / 
# Wed, 11 Oct 2023 17:48:55 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:19:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:54dda4e4d31846b7324172a7fda3d0bdc7d8a2105ab27e9a92c2db43f35f9e5d`  
		Last Modified: Wed, 11 Oct 2023 17:59:53 GMT  
		Size: 49.6 MB (49569257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370a64ae3420fd85a23128ef46431df034f9038821764a14bb436272a1345505`  
		Last Modified: Wed, 11 Oct 2023 23:55:20 GMT  
		Size: 23.4 MB (23439567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:744a14b7351b264caa5f532c9e2ddd30adb33c3aff32aa63acc7cf5b82a9400d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.3 MB (79276010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79aafe4e34b99dcfea8074db94ea73e75d2fd2d71b38493a1d9fb2b1d31e811f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:44:01 GMT
ADD file:ed515e1aef8321271c6544e30cbeb31257e9640979e8f68a9e490cb25d3525fd in / 
# Wed, 11 Oct 2023 17:44:04 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:14:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f137383853e717724a59e86aa526d31eabb4a5d45a259cd1ade68d93b3f45ae9`  
		Last Modified: Wed, 11 Oct 2023 17:49:27 GMT  
		Size: 53.6 MB (53575984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da754908592cac64ca75d9cdc8c43a4a396901108de4adae61bd92937de4f65`  
		Last Modified: Wed, 11 Oct 2023 18:36:14 GMT  
		Size: 25.7 MB (25700026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b8e20019afbeea6704a1315aac08a0971e357e86421fea4eadddb139a30796db
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.0 MB (71989702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:547b709e2a6beabff89cf0efea20a9713d1b7b7b7a3d67ecd5bdef17c2ff16fc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:50:07 GMT
ADD file:2dc117136732884ad4b058065700dd66cc49d6ce56b0fdbb672915e3ad8adb84 in / 
# Wed, 11 Oct 2023 17:50:10 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:51:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ad5e374600bf40a929dfe51e52737e4ca04aba83f499656760ba938841fb6552`  
		Last Modified: Wed, 11 Oct 2023 17:55:18 GMT  
		Size: 47.9 MB (47942934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6344f505670ce139b1b3f472749240f33304ec7535daae4a72913a6da08f304f`  
		Last Modified: Thu, 12 Oct 2023 00:33:20 GMT  
		Size: 24.0 MB (24046768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bookworm-scm`

```console
$ docker pull buildpack-deps@sha256:9b04ada2d533a254f9a3a4a4599a2a887717355d3963f1348b5908be6c0fc814
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
$ docker pull buildpack-deps@sha256:034daef4bd975190007ca9ea04206a70a50f0c94a22c31c69fb45266caf27bc3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.8 MB (137763770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7603bf6905c2f4d377ec3583bac5ca95d9600d3ad513c8f3e18ca0bc0a1459ca`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:37 GMT
ADD file:1e4dd5dab602337b5d5ef8d84b8dbe8b1ac62225f077b29b27d045842486d8e2 in / 
# Wed, 11 Oct 2023 18:34:37 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:19:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:19:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0a9573503463fd3166b5b1f34a7720dac28609e98d731e50e7068f92e79b8545`  
		Last Modified: Wed, 11 Oct 2023 18:39:10 GMT  
		Size: 49.6 MB (49582224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ccc26d841b4acc2562483bf393ce1cf8bc358ced09ccd825425226827c79c92`  
		Last Modified: Thu, 12 Oct 2023 03:28:45 GMT  
		Size: 24.1 MB (24051259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800d84653581fc119cd75cd572fa190d3b813d49221b9e5ee463e3560e2cb342`  
		Last Modified: Thu, 12 Oct 2023 03:29:04 GMT  
		Size: 64.1 MB (64130287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:3f6585039e542b0e19a291d5b489ba1d3647b261627e2c2467209933bd6424e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.6 MB (131646709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3619e24c9c6a8902a9cef46ec89de341f0bb65f1bb2c8e5f914176c890aa0259`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:37:30 GMT
ADD file:c07cf5c750a3e3c7ff84a3a3b8fc6087c9c5e0639d7bf638f0556d0a94309919 in / 
# Wed, 11 Oct 2023 17:37:35 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:04:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:05:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b7ec6536594e6c45ab234eecb51aacd85440ddc0e6da5873de23938ff146b5ec`  
		Last Modified: Wed, 11 Oct 2023 17:40:19 GMT  
		Size: 47.4 MB (47355749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ec943df1872e82ab3efa51bd5b2d7aac598550123e6db67156283ade7509d1`  
		Last Modified: Wed, 11 Oct 2023 18:14:31 GMT  
		Size: 22.7 MB (22729282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9f5c18924658cf6e03e52e00ddbf230cb1925aa017edb92b3cd508ec76293f`  
		Last Modified: Wed, 11 Oct 2023 18:14:54 GMT  
		Size: 61.6 MB (61561678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:5c80e22ca4ce0fc1769cad578ca3c0ec2d6020358bee0e0708ad8a7a4e1890eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.4 MB (126400592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c19fe7e4dbcb60f0b62f9d2258c1b8367310a78105eeac8cf15a871a70b0f97b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:41:59 GMT
ADD file:914e8a43f38c44fe9a6aabf05bbf3ebad5530966a354c8e7bb873c0842d35256 in / 
# Wed, 11 Oct 2023 17:42:00 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:45:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:45:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:65b9f3344eccdad2292cc7eec885befe05a52ec1136e145130c849441428eee6`  
		Last Modified: Wed, 11 Oct 2023 17:45:56 GMT  
		Size: 45.2 MB (45180287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbdddb82776e8c5901a821d5034c82b0fcba2993014440cd080d0592cd49616`  
		Last Modified: Thu, 12 Oct 2023 03:55:58 GMT  
		Size: 22.0 MB (21953833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f9d9ae792bc9a3749049ab80543cfddbda8910bcaffc9c95c7db4feb9e625a6`  
		Last Modified: Thu, 12 Oct 2023 03:56:18 GMT  
		Size: 59.3 MB (59266472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:ece8d9aa98c4e2ac79b982df68ee2ac9b4ae41a08fb3d92800f7124578ffffc8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.2 MB (137194983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0674043e7c55a6a4fc06506c806c8d8dab00a6ab67719922aa473372777950aa`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:43 GMT
ADD file:bf4264671bd91eb30c67d512144ebcf7f5c55a3e490ebe7876fa9b20d433bf7b in / 
# Wed, 11 Oct 2023 18:24:44 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:44:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:45:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e720f94321d63ecb6efa873b294dce7eaa1c3a5ddcd5bf7daddf375b955669a4`  
		Last Modified: Wed, 11 Oct 2023 18:28:04 GMT  
		Size: 49.6 MB (49612578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7541d83e7b8c0f5f6cacacddfcf5fdd942793f13418bc4645203b4ab4f3de3`  
		Last Modified: Wed, 11 Oct 2023 19:53:48 GMT  
		Size: 23.6 MB (23588086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a653d69b7b96df6835b157d043d7b926f776531e96c9263f4c7dae0033514d`  
		Last Modified: Wed, 11 Oct 2023 19:54:07 GMT  
		Size: 64.0 MB (63994319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:0225376ebdabef6ebca5adfd31d8e251c589b21de778ff4d6eb5f4435c87b92e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.5 MB (141471994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4557670d1bf5012131b762bb020c0f608408deca580a2b2638a6a0794046695`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:40:29 GMT
ADD file:0b6fc66d778d0cd8ae8b17b92945d98cc34f9c7008cda864ed0a54b5e40b9cb0 in / 
# Wed, 11 Oct 2023 17:40:32 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:09:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:10:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:501a599c15b6def048b2e00cfdf6c658061c00a504305ef2075fb1009a62c1e2`  
		Last Modified: Wed, 11 Oct 2023 17:45:01 GMT  
		Size: 50.6 MB (50600791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf9d6abbf47f32cac71cefb6f7233e5f700d4f6f941ca631e29947c5f1df955`  
		Last Modified: Wed, 11 Oct 2023 18:21:57 GMT  
		Size: 24.9 MB (24887201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1693c4d42b110c48ad84138aa8c91e1aeffbed6ca630f12495f711b89609823`  
		Last Modified: Wed, 11 Oct 2023 18:22:27 GMT  
		Size: 66.0 MB (65984002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:978fa0881d84f169ef3b182a55614b8c003440bfc7daff138acec86929b33f45
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.0 MB (135971603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:399ffe5bc61d49dc80a6a20678665009b14d5784ffd8ec66bd758ded95515def`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:48:50 GMT
ADD file:b081db8d48290ef5b5f477edb85d8f04d62a6995ec09bdb516d66dbe19b98137 in / 
# Wed, 11 Oct 2023 17:48:55 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:19:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:20:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:54dda4e4d31846b7324172a7fda3d0bdc7d8a2105ab27e9a92c2db43f35f9e5d`  
		Last Modified: Wed, 11 Oct 2023 17:59:53 GMT  
		Size: 49.6 MB (49569257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370a64ae3420fd85a23128ef46431df034f9038821764a14bb436272a1345505`  
		Last Modified: Wed, 11 Oct 2023 23:55:20 GMT  
		Size: 23.4 MB (23439567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c19b06553268b2cbcf576e075fdb1ac8c430154167258bcd4f925d5938117659`  
		Last Modified: Wed, 11 Oct 2023 23:56:13 GMT  
		Size: 63.0 MB (62962779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:e7774041231cd8297000ad9f73ba035a8098f870ab9e5935bf9e659d61dd0b02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.9 MB (148860554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eff06503f2fa76d78d36cfb0c68c5ebb59ed3780f372aec67e688ba57c8afda9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:44:01 GMT
ADD file:ed515e1aef8321271c6544e30cbeb31257e9640979e8f68a9e490cb25d3525fd in / 
# Wed, 11 Oct 2023 17:44:04 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:14:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:15:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f137383853e717724a59e86aa526d31eabb4a5d45a259cd1ade68d93b3f45ae9`  
		Last Modified: Wed, 11 Oct 2023 17:49:27 GMT  
		Size: 53.6 MB (53575984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da754908592cac64ca75d9cdc8c43a4a396901108de4adae61bd92937de4f65`  
		Last Modified: Wed, 11 Oct 2023 18:36:14 GMT  
		Size: 25.7 MB (25700026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524b67dc97fb52dd33f61fe12da424874443bb200789c7cfde14425f85938f54`  
		Last Modified: Wed, 11 Oct 2023 18:36:46 GMT  
		Size: 69.6 MB (69584544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:198224f3809fdab1ffa595ddb0d788d97dec1c41556a1a5e913b711ec6ccdaab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.1 MB (135122600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8fda4e35a32e1c513adb4a70b998c8a77f96ac52d6a7c94f6f085b1d1995b8e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:50:07 GMT
ADD file:2dc117136732884ad4b058065700dd66cc49d6ce56b0fdbb672915e3ad8adb84 in / 
# Wed, 11 Oct 2023 17:50:10 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:51:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:52:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ad5e374600bf40a929dfe51e52737e4ca04aba83f499656760ba938841fb6552`  
		Last Modified: Wed, 11 Oct 2023 17:55:18 GMT  
		Size: 47.9 MB (47942934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6344f505670ce139b1b3f472749240f33304ec7535daae4a72913a6da08f304f`  
		Last Modified: Thu, 12 Oct 2023 00:33:20 GMT  
		Size: 24.0 MB (24046768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf2b4ce0798e7985dd88d10311ea2a2730812d4e10c9a8f24f564875c6cb617`  
		Last Modified: Thu, 12 Oct 2023 00:33:56 GMT  
		Size: 63.1 MB (63132898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bullseye`

```console
$ docker pull buildpack-deps@sha256:e5587c367e13ef9c01dede7c4085056a65e24caa7257a53c303c6c074fe6034e
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
$ docker pull buildpack-deps@sha256:bb08d7e7738400cf38ca527441821b7215d53edb756a895846f813ea1638f1b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.3 MB (322297429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bd9f475bf39e63db0ab9a574f52a6174c3a1d300c551ce995495ff132286ab2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:01 GMT
ADD file:8a9222387b89a9ac763fd72610ce01ab17f64387cbfde30a6af1861a82030aad in / 
# Wed, 11 Oct 2023 18:35:01 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:20:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:21:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:22:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:69b3efbf67c2d9a46fdfdc8480b5a03ef73e9999a53aad57213447784f01eb6e`  
		Last Modified: Wed, 11 Oct 2023 18:39:54 GMT  
		Size: 55.1 MB (55058028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dedceb9c21c46986231d9dfb896b37cfc470d67799e7e919a641ac54dcc9eed`  
		Last Modified: Thu, 12 Oct 2023 03:29:53 GMT  
		Size: 15.8 MB (15764226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98dfe1ecd6ba8d7f42ee14ec8a64da6ba633ed96ac9c58f6c5a0028ce6908916`  
		Last Modified: Thu, 12 Oct 2023 03:30:09 GMT  
		Size: 54.6 MB (54595813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d198e46b4004b646fce783c4378d6841632c0fb7fb2360927673d788abfda172`  
		Last Modified: Thu, 12 Oct 2023 03:30:42 GMT  
		Size: 196.9 MB (196879362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:04535164c424cb704b73bb1a19096a7e575863c4dbc9adb873d833e366628ccd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.4 MB (295372008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a5f995269b01b9f80a154b38cb65347aa8df4e33c664107279723056ea8c8e9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:37:51 GMT
ADD file:dd011733a11e4681328b2d45bbfc478e1dab88a95554fe817e238ef27b1865c2 in / 
# Wed, 11 Oct 2023 17:37:51 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:06:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:07:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:08:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d310e2405531cf391481a06c9f4d0fc75165ad8e3025e4035c6be5245b6cc754`  
		Last Modified: Wed, 11 Oct 2023 17:41:07 GMT  
		Size: 52.6 MB (52563098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c07441895e6cb16dc8222813db91b971828ec10cafdde9634c13ad69f7723b`  
		Last Modified: Wed, 11 Oct 2023 18:15:51 GMT  
		Size: 15.4 MB (15374683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36086464e7a231c171f28068f405baccff6fe849ecc79fba7ed52c6ebfdba6f9`  
		Last Modified: Wed, 11 Oct 2023 18:16:08 GMT  
		Size: 52.3 MB (52331039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcfedfb2a62724677848265f66d1519ef423f3440998f0a2ce6a01dc498f2b22`  
		Last Modified: Wed, 11 Oct 2023 18:16:43 GMT  
		Size: 175.1 MB (175103188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:e4e482d959b44f9fe93c58da44f823f57a6c75f8f1ac90b76f88d71420aae7a9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.8 MB (282800401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5067c84592299d066e5e61cdeca7db4d8ddd0cfd8d1012de6c767b147e0af26`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:19 GMT
ADD file:684f3634c6b747a4caad8f9f820cc02b53a2122591fe215935c5497ec234c3ad in / 
# Wed, 11 Oct 2023 17:42:20 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:47:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:47:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:48:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:33d0c7672db93e653471872c639cd6129ec25c168942e15a008c4920cafe62d7`  
		Last Modified: Wed, 11 Oct 2023 17:46:42 GMT  
		Size: 50.2 MB (50215704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe33e05af9470f2356c8047560fded363dda4990bb2d70e9194f0dca496bb82`  
		Last Modified: Thu, 12 Oct 2023 03:57:11 GMT  
		Size: 14.9 MB (14879720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0953bb94dc6fcb1dee741e8bfc886a0671f4516a04fbf1a92527c2bb1598e1dd`  
		Last Modified: Thu, 12 Oct 2023 03:57:33 GMT  
		Size: 50.4 MB (50353136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783a8cf6b572fdf6838ef5ecf60b5713b7139f7f8e554b1ccd61d56a597e3cf7`  
		Last Modified: Thu, 12 Oct 2023 03:58:11 GMT  
		Size: 167.4 MB (167351841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:00ffaa1775df7aa605c2ced1697ead01a9b21693aae4289cfe39e23f12001037
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.0 MB (313959291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62c1e77e85cc31b53ae5fb1cf23802ccb5e6e8394bc753361cf259672e530e5b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:58 GMT
ADD file:e1a6c6c976e5e7c53eb2a7343a7a763b46e56828588535f4c79e63d6ec08198d in / 
# Wed, 11 Oct 2023 18:24:58 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:46:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:46:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:47:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dd0dc10f921f4b3b65b17f20d367374079e6cb4e26531624ee64caaaf4adcc28`  
		Last Modified: Wed, 11 Oct 2023 18:28:45 GMT  
		Size: 53.7 MB (53707810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7a630df11a812111dd2b7f5b819a692f2350ad055fab0cd3e60b322c2eead5`  
		Last Modified: Wed, 11 Oct 2023 19:54:57 GMT  
		Size: 15.7 MB (15749899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9c8e3bce435b9fb78d2fd6a8f0ce18ddecff51902c10074a9da4287cb35963b`  
		Last Modified: Wed, 11 Oct 2023 19:55:14 GMT  
		Size: 54.7 MB (54700074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda70d4f1c4310da8eb56a83b481a5bda9d57efa32a6ef6d7915a7cf487c8ba6`  
		Last Modified: Wed, 11 Oct 2023 19:55:43 GMT  
		Size: 189.8 MB (189801508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; 386

```console
$ docker pull buildpack-deps@sha256:027c2ac7b7fa9f7c2154a9a29054feac38fc193959a31cf73c35f363d04ef38a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.0 MB (328045308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:384002c0f12bf18ca0f3797b1f0a18d7a84a7ed8720b3688b2b735b291d8ce4e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:40:52 GMT
ADD file:a3c1e94bb116d940a614a5275c69bacbac46e00da2070b5c7a561e64b975acc6 in / 
# Wed, 11 Oct 2023 17:40:53 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:12:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:13:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:081c634ff059d5636b4292d84d0b49429030b3dca70ca56828543b295adb9d47`  
		Last Modified: Wed, 11 Oct 2023 17:45:55 GMT  
		Size: 56.0 MB (56046358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c55d0c1747845e146fb76750b201af94d841ddeee081fcbdefcc5353c17f2e`  
		Last Modified: Wed, 11 Oct 2023 18:23:38 GMT  
		Size: 16.3 MB (16268212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:049e1171db56ce9d453ea26b1abcc12e301ef98dda47be8250cb0ced74ec097a`  
		Last Modified: Wed, 11 Oct 2023 18:24:01 GMT  
		Size: 55.9 MB (55936762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e77fa153db9b2a24390633ef303b38a33f84bbe4d12c7490cfcc8e12554868d`  
		Last Modified: Wed, 11 Oct 2023 18:24:50 GMT  
		Size: 199.8 MB (199793976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:e5f03b8a3612aa16737fb4f085988cd8bba30d0a048cb95c65b85fedf27c9418
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.1 MB (301123558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f13213c1ead0656fc3dcddc0a9823684c244f11c9e87c31973becaccd971048`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:50:06 GMT
ADD file:c4be7fca661f2a8181ee1e05fda057c18a2d7c1ae0e08ab63b2c5567ef9cc0a7 in / 
# Wed, 11 Oct 2023 17:50:12 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:27:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:29:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:34:59 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d237f50a9f05adf465246bef37e194e1d7a226224c7f90ae7b55925c5b509d15`  
		Last Modified: Wed, 11 Oct 2023 18:01:27 GMT  
		Size: 53.3 MB (53289043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a8381daee3205699bef24f6e7ee0bd6b3621924baae8f1b0b0026007cfe3b4`  
		Last Modified: Wed, 11 Oct 2023 23:58:42 GMT  
		Size: 15.5 MB (15529612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9e6da5ca3b34590abe253ac60b2000d9724ff3d9572311ded53ba9d66e58de`  
		Last Modified: Wed, 11 Oct 2023 23:59:27 GMT  
		Size: 53.3 MB (53302304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2632af27ef8e60c2473640fa869c1560b9bc160073d3db4db8c120329ad58ba3`  
		Last Modified: Thu, 12 Oct 2023 00:01:26 GMT  
		Size: 179.0 MB (179002599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:958d63f118f9541a5d8261b37e6ea3047bb2c96deb9af2464690bec55b58dcbb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.8 MB (330810785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1f7cd93d79e43a628cbf38352b5a20938139f8968c227d5a0b718d6b34fc765`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:44:35 GMT
ADD file:d59326770edede2ba1d2005697bf41540a3d76a4bae883b91fede9b68018630c in / 
# Wed, 11 Oct 2023 17:44:38 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:20:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:21:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:24:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6613fa9f09034273d2b35a47386f8d53c77953a73e561b9f189ffa43ea17bd54`  
		Last Modified: Wed, 11 Oct 2023 17:50:25 GMT  
		Size: 58.9 MB (58929717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565fd5d2ec4119e0cef3217e4496512c36e4adc4e98567f565f105e684e80c4e`  
		Last Modified: Wed, 11 Oct 2023 18:38:00 GMT  
		Size: 16.8 MB (16765485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac6ae11620e817afc07c304ae67f21276148cc99a42e4ac56d481faceb27146`  
		Last Modified: Wed, 11 Oct 2023 18:38:24 GMT  
		Size: 58.9 MB (58866926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e868ed372aa88cb7b1880038e68bff4def65e8692014745f7a779d67797a8527`  
		Last Modified: Wed, 11 Oct 2023 18:39:18 GMT  
		Size: 196.2 MB (196248657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:c508b62b26cf4c3e78a3a679727268f9c89cf031809913639114575bed3387f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.9 MB (295893977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2030b0af1fd8ca97341a629b714304bddce2ff9594cb68f4483fdcccafced6d4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:50:40 GMT
ADD file:bb3ee20a7ddf364b23163c517132146872491e85ef2f1465bf7fd2ed33f94827 in / 
# Wed, 11 Oct 2023 17:50:44 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:58:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:59:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 00:03:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e651436ffb848f56da62cd2c80f206a288b94da8113c4c23a7e5502fb597ce23`  
		Last Modified: Wed, 11 Oct 2023 17:56:38 GMT  
		Size: 53.3 MB (53296378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a52fe3127c9c85c0c5e50b52a035e6bcee230e0c38db795abfee4b60522f157`  
		Last Modified: Thu, 12 Oct 2023 00:35:16 GMT  
		Size: 15.6 MB (15640232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58e9fa5eede43b49ed76d5e09e5c978ac8b2296773dad3161eae081bba447e45`  
		Last Modified: Thu, 12 Oct 2023 00:35:44 GMT  
		Size: 54.1 MB (54066239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d404a1f00add5fb24f6224adfac012cf688caba0fb9eb52c82c499b84498b414`  
		Last Modified: Thu, 12 Oct 2023 00:36:17 GMT  
		Size: 172.9 MB (172891128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bullseye-curl`

```console
$ docker pull buildpack-deps@sha256:a1cf2b85c16ce2dcef6d5b5e603d6dcc208287ba0c02cb856e117837b3dbd700
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
$ docker pull buildpack-deps@sha256:ee1320245c18c32018ab7c9b5930a007c1cdd617ef894def34d8b9a97edfed2e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.8 MB (70822254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9144300bda2ab6cd167ac7386e562115d65c96297fbf92f5bf92e98784a5b25`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:01 GMT
ADD file:8a9222387b89a9ac763fd72610ce01ab17f64387cbfde30a6af1861a82030aad in / 
# Wed, 11 Oct 2023 18:35:01 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:20:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:69b3efbf67c2d9a46fdfdc8480b5a03ef73e9999a53aad57213447784f01eb6e`  
		Last Modified: Wed, 11 Oct 2023 18:39:54 GMT  
		Size: 55.1 MB (55058028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dedceb9c21c46986231d9dfb896b37cfc470d67799e7e919a641ac54dcc9eed`  
		Last Modified: Thu, 12 Oct 2023 03:29:53 GMT  
		Size: 15.8 MB (15764226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:370bfb2b7dc382e63da82b4ba78d9717baf16f82f20e7c43723e804e0b344a4a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.9 MB (67937781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0979f1da4edd11481372e6d0be81bd79af79fc236117439dceddbef0c454bc8b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:37:51 GMT
ADD file:dd011733a11e4681328b2d45bbfc478e1dab88a95554fe817e238ef27b1865c2 in / 
# Wed, 11 Oct 2023 17:37:51 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:06:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d310e2405531cf391481a06c9f4d0fc75165ad8e3025e4035c6be5245b6cc754`  
		Last Modified: Wed, 11 Oct 2023 17:41:07 GMT  
		Size: 52.6 MB (52563098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c07441895e6cb16dc8222813db91b971828ec10cafdde9634c13ad69f7723b`  
		Last Modified: Wed, 11 Oct 2023 18:15:51 GMT  
		Size: 15.4 MB (15374683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:84e96a20434a3a6eb8d0a4e7237e11ad8d690fc89f01d5c16f68f9ceb0e55758
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.1 MB (65095424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56fe78d093f425564326f7db7157a9c30ececd23a260999492e51a77ef946ab6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:19 GMT
ADD file:684f3634c6b747a4caad8f9f820cc02b53a2122591fe215935c5497ec234c3ad in / 
# Wed, 11 Oct 2023 17:42:20 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:47:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:33d0c7672db93e653471872c639cd6129ec25c168942e15a008c4920cafe62d7`  
		Last Modified: Wed, 11 Oct 2023 17:46:42 GMT  
		Size: 50.2 MB (50215704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe33e05af9470f2356c8047560fded363dda4990bb2d70e9194f0dca496bb82`  
		Last Modified: Thu, 12 Oct 2023 03:57:11 GMT  
		Size: 14.9 MB (14879720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:58b83690d392c116335e8fd9b2c275091639d089b8f7f847f4d377a6d82b7378
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69457709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bcc8243d9507636e5a3dea0b7fed7e96bda7eafbdd181c94760a568fc989ba5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:58 GMT
ADD file:e1a6c6c976e5e7c53eb2a7343a7a763b46e56828588535f4c79e63d6ec08198d in / 
# Wed, 11 Oct 2023 18:24:58 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:46:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dd0dc10f921f4b3b65b17f20d367374079e6cb4e26531624ee64caaaf4adcc28`  
		Last Modified: Wed, 11 Oct 2023 18:28:45 GMT  
		Size: 53.7 MB (53707810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7a630df11a812111dd2b7f5b819a692f2350ad055fab0cd3e60b322c2eead5`  
		Last Modified: Wed, 11 Oct 2023 19:54:57 GMT  
		Size: 15.7 MB (15749899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:e1c572c67ccecd84db4824b91544f67cf96d1898da9f2d2e8082d02a28156ee4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.3 MB (72314570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1a1649cccdfb82a9509f903fefa311a0cbe4efa7c06904483e262c6ef68cd43`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:40:52 GMT
ADD file:a3c1e94bb116d940a614a5275c69bacbac46e00da2070b5c7a561e64b975acc6 in / 
# Wed, 11 Oct 2023 17:40:53 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:12:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:081c634ff059d5636b4292d84d0b49429030b3dca70ca56828543b295adb9d47`  
		Last Modified: Wed, 11 Oct 2023 17:45:55 GMT  
		Size: 56.0 MB (56046358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c55d0c1747845e146fb76750b201af94d841ddeee081fcbdefcc5353c17f2e`  
		Last Modified: Wed, 11 Oct 2023 18:23:38 GMT  
		Size: 16.3 MB (16268212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:d36ab6ccd5a69d80d30a12899ec690d3465ffbe7f79c9959256ff964a8013b19
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68818655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59e679dfa36ed42066347b3a7c55c9e0fe065971e0f4b551e37944ff83892c9d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:50:06 GMT
ADD file:c4be7fca661f2a8181ee1e05fda057c18a2d7c1ae0e08ab63b2c5567ef9cc0a7 in / 
# Wed, 11 Oct 2023 17:50:12 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:27:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d237f50a9f05adf465246bef37e194e1d7a226224c7f90ae7b55925c5b509d15`  
		Last Modified: Wed, 11 Oct 2023 18:01:27 GMT  
		Size: 53.3 MB (53289043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a8381daee3205699bef24f6e7ee0bd6b3621924baae8f1b0b0026007cfe3b4`  
		Last Modified: Wed, 11 Oct 2023 23:58:42 GMT  
		Size: 15.5 MB (15529612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:a8f64ada08912d3bc6055dfb5556580bdc6e31a2b9d852fb97e443e7967bc125
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75695202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dab5dd6afc653a6bf54d9046c1376d631f18b2de419b34a6eebaecd1c1c9e0e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:44:35 GMT
ADD file:d59326770edede2ba1d2005697bf41540a3d76a4bae883b91fede9b68018630c in / 
# Wed, 11 Oct 2023 17:44:38 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:20:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6613fa9f09034273d2b35a47386f8d53c77953a73e561b9f189ffa43ea17bd54`  
		Last Modified: Wed, 11 Oct 2023 17:50:25 GMT  
		Size: 58.9 MB (58929717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565fd5d2ec4119e0cef3217e4496512c36e4adc4e98567f565f105e684e80c4e`  
		Last Modified: Wed, 11 Oct 2023 18:38:00 GMT  
		Size: 16.8 MB (16765485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:22bb4a69e38d7e27b147c422662a4fd498271358a64a316a4955c9ae4087f7da
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68936610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:493442157276cd80e2ea1efa06c399eb8d575ca91cf4d33c6ea2e217d2cd5e57`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:50:40 GMT
ADD file:bb3ee20a7ddf364b23163c517132146872491e85ef2f1465bf7fd2ed33f94827 in / 
# Wed, 11 Oct 2023 17:50:44 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:58:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e651436ffb848f56da62cd2c80f206a288b94da8113c4c23a7e5502fb597ce23`  
		Last Modified: Wed, 11 Oct 2023 17:56:38 GMT  
		Size: 53.3 MB (53296378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a52fe3127c9c85c0c5e50b52a035e6bcee230e0c38db795abfee4b60522f157`  
		Last Modified: Thu, 12 Oct 2023 00:35:16 GMT  
		Size: 15.6 MB (15640232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bullseye-scm`

```console
$ docker pull buildpack-deps@sha256:bac055b211a05a57b5e3ecef13ebf2467489801508aa142627e76621976a6ee9
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
$ docker pull buildpack-deps@sha256:253d4cf8241a2eff590b5ac562692d9e115c7537c1981afde7c0bb9f50651076
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.4 MB (125418067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01459750910db9c5ab8b473b3d05da74886a0b37bc6665134abdce8e1a17bf19`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:01 GMT
ADD file:8a9222387b89a9ac763fd72610ce01ab17f64387cbfde30a6af1861a82030aad in / 
# Wed, 11 Oct 2023 18:35:01 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:20:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:21:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:69b3efbf67c2d9a46fdfdc8480b5a03ef73e9999a53aad57213447784f01eb6e`  
		Last Modified: Wed, 11 Oct 2023 18:39:54 GMT  
		Size: 55.1 MB (55058028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dedceb9c21c46986231d9dfb896b37cfc470d67799e7e919a641ac54dcc9eed`  
		Last Modified: Thu, 12 Oct 2023 03:29:53 GMT  
		Size: 15.8 MB (15764226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98dfe1ecd6ba8d7f42ee14ec8a64da6ba633ed96ac9c58f6c5a0028ce6908916`  
		Last Modified: Thu, 12 Oct 2023 03:30:09 GMT  
		Size: 54.6 MB (54595813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:011f6927755aeeb83705407dd0b8b44593b9134ddf0d0ee7ef5cec32418d1b6d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.3 MB (120268820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b18801b1c50fa7588edecb59d16649ecbcec14a4478b91085817f3fb7ca1da5c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:37:51 GMT
ADD file:dd011733a11e4681328b2d45bbfc478e1dab88a95554fe817e238ef27b1865c2 in / 
# Wed, 11 Oct 2023 17:37:51 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:06:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:07:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d310e2405531cf391481a06c9f4d0fc75165ad8e3025e4035c6be5245b6cc754`  
		Last Modified: Wed, 11 Oct 2023 17:41:07 GMT  
		Size: 52.6 MB (52563098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c07441895e6cb16dc8222813db91b971828ec10cafdde9634c13ad69f7723b`  
		Last Modified: Wed, 11 Oct 2023 18:15:51 GMT  
		Size: 15.4 MB (15374683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36086464e7a231c171f28068f405baccff6fe849ecc79fba7ed52c6ebfdba6f9`  
		Last Modified: Wed, 11 Oct 2023 18:16:08 GMT  
		Size: 52.3 MB (52331039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:c53c90800fe4cf9897c502d7711674d1a1066c078d1b97b72b5c798ddada0128
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115448560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecdf47b0ce17fefb017abd99216cc417cc7afb93963a744c684e0994829f6da9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:19 GMT
ADD file:684f3634c6b747a4caad8f9f820cc02b53a2122591fe215935c5497ec234c3ad in / 
# Wed, 11 Oct 2023 17:42:20 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:47:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:47:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:33d0c7672db93e653471872c639cd6129ec25c168942e15a008c4920cafe62d7`  
		Last Modified: Wed, 11 Oct 2023 17:46:42 GMT  
		Size: 50.2 MB (50215704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe33e05af9470f2356c8047560fded363dda4990bb2d70e9194f0dca496bb82`  
		Last Modified: Thu, 12 Oct 2023 03:57:11 GMT  
		Size: 14.9 MB (14879720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0953bb94dc6fcb1dee741e8bfc886a0671f4516a04fbf1a92527c2bb1598e1dd`  
		Last Modified: Thu, 12 Oct 2023 03:57:33 GMT  
		Size: 50.4 MB (50353136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:ced5e59499a3da882d04714d3b138662087510ae912a4a3f67e07091d779be56
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124157783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b274c20cfd411a3b40df383bdd201e2c6b0b2793e2aab1604083557f0fb5edb1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:58 GMT
ADD file:e1a6c6c976e5e7c53eb2a7343a7a763b46e56828588535f4c79e63d6ec08198d in / 
# Wed, 11 Oct 2023 18:24:58 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:46:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:46:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dd0dc10f921f4b3b65b17f20d367374079e6cb4e26531624ee64caaaf4adcc28`  
		Last Modified: Wed, 11 Oct 2023 18:28:45 GMT  
		Size: 53.7 MB (53707810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7a630df11a812111dd2b7f5b819a692f2350ad055fab0cd3e60b322c2eead5`  
		Last Modified: Wed, 11 Oct 2023 19:54:57 GMT  
		Size: 15.7 MB (15749899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9c8e3bce435b9fb78d2fd6a8f0ce18ddecff51902c10074a9da4287cb35963b`  
		Last Modified: Wed, 11 Oct 2023 19:55:14 GMT  
		Size: 54.7 MB (54700074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:a09e5525965252b12dd52923b5273449114a15e10408a8ad5b56775c47c27211
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128251332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa3a761c17f979ab85a035b0000b43ff140b4e3759ad1a3fe42ae6bad59afa14`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:40:52 GMT
ADD file:a3c1e94bb116d940a614a5275c69bacbac46e00da2070b5c7a561e64b975acc6 in / 
# Wed, 11 Oct 2023 17:40:53 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:12:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:081c634ff059d5636b4292d84d0b49429030b3dca70ca56828543b295adb9d47`  
		Last Modified: Wed, 11 Oct 2023 17:45:55 GMT  
		Size: 56.0 MB (56046358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c55d0c1747845e146fb76750b201af94d841ddeee081fcbdefcc5353c17f2e`  
		Last Modified: Wed, 11 Oct 2023 18:23:38 GMT  
		Size: 16.3 MB (16268212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:049e1171db56ce9d453ea26b1abcc12e301ef98dda47be8250cb0ced74ec097a`  
		Last Modified: Wed, 11 Oct 2023 18:24:01 GMT  
		Size: 55.9 MB (55936762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:78a2985bb49a2845f3145c2470d4fc56a0d5c9a1b2cc8b8530d1f76b0249e136
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122120959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7a5579be6befdd5b737e228200c04b041ee9277c42609f172d9cd187c395a48`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:50:06 GMT
ADD file:c4be7fca661f2a8181ee1e05fda057c18a2d7c1ae0e08ab63b2c5567ef9cc0a7 in / 
# Wed, 11 Oct 2023 17:50:12 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:27:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:29:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d237f50a9f05adf465246bef37e194e1d7a226224c7f90ae7b55925c5b509d15`  
		Last Modified: Wed, 11 Oct 2023 18:01:27 GMT  
		Size: 53.3 MB (53289043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a8381daee3205699bef24f6e7ee0bd6b3621924baae8f1b0b0026007cfe3b4`  
		Last Modified: Wed, 11 Oct 2023 23:58:42 GMT  
		Size: 15.5 MB (15529612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9e6da5ca3b34590abe253ac60b2000d9724ff3d9572311ded53ba9d66e58de`  
		Last Modified: Wed, 11 Oct 2023 23:59:27 GMT  
		Size: 53.3 MB (53302304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:c2a2624d91648d9bff279829625cbbf4355423f43ccf91431c0d3d3fbea2583d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.6 MB (134562128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:518eca7155957889e092f55b3815b4670c5db7a907113bc9fd64683bc7c719a9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:44:35 GMT
ADD file:d59326770edede2ba1d2005697bf41540a3d76a4bae883b91fede9b68018630c in / 
# Wed, 11 Oct 2023 17:44:38 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:20:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:21:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6613fa9f09034273d2b35a47386f8d53c77953a73e561b9f189ffa43ea17bd54`  
		Last Modified: Wed, 11 Oct 2023 17:50:25 GMT  
		Size: 58.9 MB (58929717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565fd5d2ec4119e0cef3217e4496512c36e4adc4e98567f565f105e684e80c4e`  
		Last Modified: Wed, 11 Oct 2023 18:38:00 GMT  
		Size: 16.8 MB (16765485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac6ae11620e817afc07c304ae67f21276148cc99a42e4ac56d481faceb27146`  
		Last Modified: Wed, 11 Oct 2023 18:38:24 GMT  
		Size: 58.9 MB (58866926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:4e549af12fe7ffa2d33939608ee823e50b8c02fbfe3fe7ad6542e9ca78ce985b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123002849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56de25e9482f0b3b8dd9d90c7bb9e4fc63c09768465c3b79a95301dbfe9205fc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:50:40 GMT
ADD file:bb3ee20a7ddf364b23163c517132146872491e85ef2f1465bf7fd2ed33f94827 in / 
# Wed, 11 Oct 2023 17:50:44 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:58:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:59:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e651436ffb848f56da62cd2c80f206a288b94da8113c4c23a7e5502fb597ce23`  
		Last Modified: Wed, 11 Oct 2023 17:56:38 GMT  
		Size: 53.3 MB (53296378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a52fe3127c9c85c0c5e50b52a035e6bcee230e0c38db795abfee4b60522f157`  
		Last Modified: Thu, 12 Oct 2023 00:35:16 GMT  
		Size: 15.6 MB (15640232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58e9fa5eede43b49ed76d5e09e5c978ac8b2296773dad3161eae081bba447e45`  
		Last Modified: Thu, 12 Oct 2023 00:35:44 GMT  
		Size: 54.1 MB (54066239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:buster`

```console
$ docker pull buildpack-deps@sha256:82e25c1dea159632964a4c576380aa6ae9fd1d28c42b1f967d5474167ee4f6a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:buster` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:3cce8b99c877ede9a61de5d6c26b7812ff14240940a8d5b022acee4ecbe4407b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.9 MB (311864851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:812562bb54bb3b4a8d34fffe7cb7523e1d58d69c7e6f3f31ca19c5e280e54922`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:23 GMT
ADD file:1efe9845e057e7029a1c2c26c148e6dc1bd9c65d0cbbb23cb49c86295d1f1f48 in / 
# Wed, 11 Oct 2023 18:35:23 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:22:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:22:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:24:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99db33be616a9a2a0b0b1bc913b548317bab7bd11cb6968d357457e201c44077`  
		Last Modified: Wed, 11 Oct 2023 18:40:37 GMT  
		Size: 50.5 MB (50499400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4df9fde773e0c195208a941f5c813fcae5310dfa340b1092a91ca3dca2f0997`  
		Last Modified: Thu, 12 Oct 2023 03:30:53 GMT  
		Size: 17.6 MB (17580739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47c0008f57ffcdd8594227fc498eec4c4660fd627978baa26cf04a9a18908391`  
		Last Modified: Thu, 12 Oct 2023 03:31:09 GMT  
		Size: 51.9 MB (51874135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:640e2c66b8c0a79112068e7e0c50721ca969cdf94a73740fabd8230930e835ae`  
		Last Modified: Thu, 12 Oct 2023 03:31:41 GMT  
		Size: 191.9 MB (191910577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:17038db490bbb33ff709999f26a89753069ad0d2b167e56adf06474c2f8b9512
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.7 MB (277692858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02bb7e9c592bddbb15c614d9057cb8a1518aee94b14b7a7f746972df6779d573`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:37 GMT
ADD file:90492dd68d097af40a6208353165e1b7e2bc04a31cd2270232e085416f6e940e in / 
# Wed, 11 Oct 2023 17:42:38 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:48:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:49:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:50:19 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2ecd2705b9dde659b853da74fbe8d7227d02acd96f1d34766d44193b82468b37`  
		Last Modified: Wed, 11 Oct 2023 17:47:27 GMT  
		Size: 46.0 MB (45966353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2548d6bcf8bfe2322ed1ed9f56eeab4afd1b65e4c4a62d0be4d602f14dafc992`  
		Last Modified: Thu, 12 Oct 2023 03:58:22 GMT  
		Size: 16.2 MB (16213670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:423a7661d20a90498af23198b35b85c16af055a76453a7e8392ce97b5f4e398c`  
		Last Modified: Thu, 12 Oct 2023 03:58:40 GMT  
		Size: 47.4 MB (47410916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aa54b7711ac968a604b4e2ef193e8298d78d435fd3241931a711bc5ccce47e1`  
		Last Modified: Thu, 12 Oct 2023 03:59:13 GMT  
		Size: 168.1 MB (168101919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f8e53ff95899f67abb3aa35ec671c43f119ca559ee8b0e519a0ece7cfe03c0fc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.4 MB (302434057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ab5f1e32878a2fe74760a4cb35219c1d3828050ae2f605403539b5a27473351`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:12 GMT
ADD file:d97d8c89883987c89b2150923abea982086030e71970f5473a534e95252b4972 in / 
# Wed, 11 Oct 2023 18:25:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:47:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:48:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:49:16 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6a7acee270b8289bdc6bb8836f1a4899f794d60337a0cdc46b58a717bd27ba89`  
		Last Modified: Wed, 11 Oct 2023 18:29:25 GMT  
		Size: 49.3 MB (49291086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d43a8471c221305b41e4a48fe1a36d8d976208b182f048b98aa6dc81e6fec8`  
		Last Modified: Wed, 11 Oct 2023 19:55:54 GMT  
		Size: 17.5 MB (17451818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a82d27a09b100de4594fbc9e341ab946a39a8d635f12e633b1341a1c7aaa4b`  
		Last Modified: Wed, 11 Oct 2023 19:56:09 GMT  
		Size: 52.2 MB (52208642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb224d9b0fd6283df35335f4979c2c54bdc5609ca8473220d5d9924a91a0e11`  
		Last Modified: Wed, 11 Oct 2023 19:56:34 GMT  
		Size: 183.5 MB (183482511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; 386

```console
$ docker pull buildpack-deps@sha256:e2ca1129326f210b765c3fc489de34d0c965072bdb15a62cf1b72ab756fa27b3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.3 MB (321272799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:138b172705b3f04788d90ae5fdf81f014877dfb0f9d4e808fba131bc14519f3d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:41:14 GMT
ADD file:47cece2eff96bf7383dd2a9c5632f0ad7bb31b3a459677530f77a78e22658e98 in / 
# Wed, 11 Oct 2023 17:41:14 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:14:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:14:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:16:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:62bc68699d611f4c048328a0468ebc10de528260c7823c8938796da30db31a17`  
		Last Modified: Wed, 11 Oct 2023 17:46:45 GMT  
		Size: 51.3 MB (51256071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a664405fd519ae385ebac7659c355b2c380dd5c84037f38e6d3673b2bd9795c5`  
		Last Modified: Wed, 11 Oct 2023 18:25:03 GMT  
		Size: 18.1 MB (18097310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c138636d1c51e715c73bdb28e49fb18fc2d82cca0a21d5641a911f48cd3ff695`  
		Last Modified: Wed, 11 Oct 2023 18:25:25 GMT  
		Size: 53.5 MB (53487954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31fb7080416fbc4aee5e058de75799128cbeb8d55130f29854b8e5d7666fca0c`  
		Last Modified: Wed, 11 Oct 2023 18:26:09 GMT  
		Size: 198.4 MB (198431464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:buster-curl`

```console
$ docker pull buildpack-deps@sha256:d8e623f145ced0b674077746d2384f6e7f4adc64f84389a951e9acccf7a2ca40
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:buster-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:fb59272c01f331c27bbf043917330de01941dbf342ed54f26343cb9ac8d31b13
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68080139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf521dae41c7d61f7dc44e641032d2e238a024f227c62d1e5fe1a5c4889449ad`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:23 GMT
ADD file:1efe9845e057e7029a1c2c26c148e6dc1bd9c65d0cbbb23cb49c86295d1f1f48 in / 
# Wed, 11 Oct 2023 18:35:23 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:22:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99db33be616a9a2a0b0b1bc913b548317bab7bd11cb6968d357457e201c44077`  
		Last Modified: Wed, 11 Oct 2023 18:40:37 GMT  
		Size: 50.5 MB (50499400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4df9fde773e0c195208a941f5c813fcae5310dfa340b1092a91ca3dca2f0997`  
		Last Modified: Thu, 12 Oct 2023 03:30:53 GMT  
		Size: 17.6 MB (17580739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:d480bc746f923acad671d7592a0318d59b3d00cff454e730e20b9e915a3e4752
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62180023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0eca085d0fa4d2ab3f440a605762d5eab83321b1edfb729fab09fc20f6bdea5c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:37 GMT
ADD file:90492dd68d097af40a6208353165e1b7e2bc04a31cd2270232e085416f6e940e in / 
# Wed, 11 Oct 2023 17:42:38 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:48:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2ecd2705b9dde659b853da74fbe8d7227d02acd96f1d34766d44193b82468b37`  
		Last Modified: Wed, 11 Oct 2023 17:47:27 GMT  
		Size: 46.0 MB (45966353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2548d6bcf8bfe2322ed1ed9f56eeab4afd1b65e4c4a62d0be4d602f14dafc992`  
		Last Modified: Thu, 12 Oct 2023 03:58:22 GMT  
		Size: 16.2 MB (16213670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f93b04aec507910fbaa9a45dcff734fa880323618be3ee146dc70f885a285af1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66742904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c330d4af463f1493cf1f188470d0d1445f9d11bf3ace6545f44b18cf2f1f8d5e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:12 GMT
ADD file:d97d8c89883987c89b2150923abea982086030e71970f5473a534e95252b4972 in / 
# Wed, 11 Oct 2023 18:25:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:47:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6a7acee270b8289bdc6bb8836f1a4899f794d60337a0cdc46b58a717bd27ba89`  
		Last Modified: Wed, 11 Oct 2023 18:29:25 GMT  
		Size: 49.3 MB (49291086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d43a8471c221305b41e4a48fe1a36d8d976208b182f048b98aa6dc81e6fec8`  
		Last Modified: Wed, 11 Oct 2023 19:55:54 GMT  
		Size: 17.5 MB (17451818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:32c7184a162ee94fdac9984a9cef58f1bcf15f4c0a1acd21082769162bd02990
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.4 MB (69353381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:885698803969612184270761585a946f4b430a1383c328ab4924a3f6c7f6a410`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:41:14 GMT
ADD file:47cece2eff96bf7383dd2a9c5632f0ad7bb31b3a459677530f77a78e22658e98 in / 
# Wed, 11 Oct 2023 17:41:14 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:14:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:62bc68699d611f4c048328a0468ebc10de528260c7823c8938796da30db31a17`  
		Last Modified: Wed, 11 Oct 2023 17:46:45 GMT  
		Size: 51.3 MB (51256071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a664405fd519ae385ebac7659c355b2c380dd5c84037f38e6d3673b2bd9795c5`  
		Last Modified: Wed, 11 Oct 2023 18:25:03 GMT  
		Size: 18.1 MB (18097310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:buster-scm`

```console
$ docker pull buildpack-deps@sha256:2437a1e2cad84091b2e8393d0a736af68e46f377f6c499327516e4815feea613
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:buster-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:00b0f3aca41e1135dc391f626f66f5b6a086ee260c995f37805f27164957691d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.0 MB (119954274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06dd589d27b2d2d0733d458cb149600accc2ea5f8f818c903bddb738204c8426`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:23 GMT
ADD file:1efe9845e057e7029a1c2c26c148e6dc1bd9c65d0cbbb23cb49c86295d1f1f48 in / 
# Wed, 11 Oct 2023 18:35:23 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:22:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:22:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99db33be616a9a2a0b0b1bc913b548317bab7bd11cb6968d357457e201c44077`  
		Last Modified: Wed, 11 Oct 2023 18:40:37 GMT  
		Size: 50.5 MB (50499400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4df9fde773e0c195208a941f5c813fcae5310dfa340b1092a91ca3dca2f0997`  
		Last Modified: Thu, 12 Oct 2023 03:30:53 GMT  
		Size: 17.6 MB (17580739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47c0008f57ffcdd8594227fc498eec4c4660fd627978baa26cf04a9a18908391`  
		Last Modified: Thu, 12 Oct 2023 03:31:09 GMT  
		Size: 51.9 MB (51874135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:23fa82b6ce62d4459c91ba9cd6a119c8132666e0e84b1bccdbc46652fdd4fa8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109590939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:419a7b84b078554b5177dd14ef6a12e1a6696df651c438b2bcf3f8761077497c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:37 GMT
ADD file:90492dd68d097af40a6208353165e1b7e2bc04a31cd2270232e085416f6e940e in / 
# Wed, 11 Oct 2023 17:42:38 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:48:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:49:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2ecd2705b9dde659b853da74fbe8d7227d02acd96f1d34766d44193b82468b37`  
		Last Modified: Wed, 11 Oct 2023 17:47:27 GMT  
		Size: 46.0 MB (45966353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2548d6bcf8bfe2322ed1ed9f56eeab4afd1b65e4c4a62d0be4d602f14dafc992`  
		Last Modified: Thu, 12 Oct 2023 03:58:22 GMT  
		Size: 16.2 MB (16213670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:423a7661d20a90498af23198b35b85c16af055a76453a7e8392ce97b5f4e398c`  
		Last Modified: Thu, 12 Oct 2023 03:58:40 GMT  
		Size: 47.4 MB (47410916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:142a54e609ce722402983f6daa77ee12ec5baf50a191b64ef7f9a4c85262597c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.0 MB (118951546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b138e1d073c5b16678192fbfb7949d838e13e95902b21affb91b17aed7e9f89`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:12 GMT
ADD file:d97d8c89883987c89b2150923abea982086030e71970f5473a534e95252b4972 in / 
# Wed, 11 Oct 2023 18:25:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:47:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:48:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6a7acee270b8289bdc6bb8836f1a4899f794d60337a0cdc46b58a717bd27ba89`  
		Last Modified: Wed, 11 Oct 2023 18:29:25 GMT  
		Size: 49.3 MB (49291086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d43a8471c221305b41e4a48fe1a36d8d976208b182f048b98aa6dc81e6fec8`  
		Last Modified: Wed, 11 Oct 2023 19:55:54 GMT  
		Size: 17.5 MB (17451818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a82d27a09b100de4594fbc9e341ab946a39a8d635f12e633b1341a1c7aaa4b`  
		Last Modified: Wed, 11 Oct 2023 19:56:09 GMT  
		Size: 52.2 MB (52208642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:b9714a557ba551d0e25530e69b9c38752fec848204c2e0791697c79dacbd1d67
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.8 MB (122841335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ce745aed3b333b25b3e5c0db30d1014e3561c2f1044192ec0991f69bb7cecf8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:41:14 GMT
ADD file:47cece2eff96bf7383dd2a9c5632f0ad7bb31b3a459677530f77a78e22658e98 in / 
# Wed, 11 Oct 2023 17:41:14 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:14:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:14:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:62bc68699d611f4c048328a0468ebc10de528260c7823c8938796da30db31a17`  
		Last Modified: Wed, 11 Oct 2023 17:46:45 GMT  
		Size: 51.3 MB (51256071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a664405fd519ae385ebac7659c355b2c380dd5c84037f38e6d3673b2bd9795c5`  
		Last Modified: Wed, 11 Oct 2023 18:25:03 GMT  
		Size: 18.1 MB (18097310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c138636d1c51e715c73bdb28e49fb18fc2d82cca0a21d5641a911f48cd3ff695`  
		Last Modified: Wed, 11 Oct 2023 18:25:25 GMT  
		Size: 53.5 MB (53487954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:curl`

```console
$ docker pull buildpack-deps@sha256:ce8ea34dd6046d5bd7bc423fbee3460e246b576dcd581e5ba6583f3535b55fcd
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
$ docker pull buildpack-deps@sha256:977f8a0eade986703e1379ef96d1c106c53eccfef6eb0dace01f3f404dd41db3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73633483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6190da4faf36a08749338aa0f80e05ce0f4a16fc3164c506cc7cd23b0b6e665c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:37 GMT
ADD file:1e4dd5dab602337b5d5ef8d84b8dbe8b1ac62225f077b29b27d045842486d8e2 in / 
# Wed, 11 Oct 2023 18:34:37 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:19:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0a9573503463fd3166b5b1f34a7720dac28609e98d731e50e7068f92e79b8545`  
		Last Modified: Wed, 11 Oct 2023 18:39:10 GMT  
		Size: 49.6 MB (49582224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ccc26d841b4acc2562483bf393ce1cf8bc358ced09ccd825425226827c79c92`  
		Last Modified: Thu, 12 Oct 2023 03:28:45 GMT  
		Size: 24.1 MB (24051259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:26df1627a60457168bc3b15d71211f6b2233409c7dcd192decbae29947006323
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.1 MB (70085031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ef4b4f6796a04df75ac23eda97d56908155655aca64a22dceb52210e8ef9956`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:37:30 GMT
ADD file:c07cf5c750a3e3c7ff84a3a3b8fc6087c9c5e0639d7bf638f0556d0a94309919 in / 
# Wed, 11 Oct 2023 17:37:35 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:04:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b7ec6536594e6c45ab234eecb51aacd85440ddc0e6da5873de23938ff146b5ec`  
		Last Modified: Wed, 11 Oct 2023 17:40:19 GMT  
		Size: 47.4 MB (47355749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ec943df1872e82ab3efa51bd5b2d7aac598550123e6db67156283ade7509d1`  
		Last Modified: Wed, 11 Oct 2023 18:14:31 GMT  
		Size: 22.7 MB (22729282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:c88279d74fb84bd9e91e1631a6f8be701529d90987a5bd1877a7c1741aaddf11
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67134120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:922f8718561dcde238f85464ae864269e429eda3b44a3124b8a1c955d881c183`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:41:59 GMT
ADD file:914e8a43f38c44fe9a6aabf05bbf3ebad5530966a354c8e7bb873c0842d35256 in / 
# Wed, 11 Oct 2023 17:42:00 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:45:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:65b9f3344eccdad2292cc7eec885befe05a52ec1136e145130c849441428eee6`  
		Last Modified: Wed, 11 Oct 2023 17:45:56 GMT  
		Size: 45.2 MB (45180287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbdddb82776e8c5901a821d5034c82b0fcba2993014440cd080d0592cd49616`  
		Last Modified: Thu, 12 Oct 2023 03:55:58 GMT  
		Size: 22.0 MB (21953833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3336852231c4838575dca42d951ad5ef02897709b046c708ab77d49bf73af01c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73200664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a61350e5fd6e43ba2eafdd779f92c81d1adcc19b9614cd2c2a8a88b2f7ff2b7e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:43 GMT
ADD file:bf4264671bd91eb30c67d512144ebcf7f5c55a3e490ebe7876fa9b20d433bf7b in / 
# Wed, 11 Oct 2023 18:24:44 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:44:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e720f94321d63ecb6efa873b294dce7eaa1c3a5ddcd5bf7daddf375b955669a4`  
		Last Modified: Wed, 11 Oct 2023 18:28:04 GMT  
		Size: 49.6 MB (49612578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7541d83e7b8c0f5f6cacacddfcf5fdd942793f13418bc4645203b4ab4f3de3`  
		Last Modified: Wed, 11 Oct 2023 19:53:48 GMT  
		Size: 23.6 MB (23588086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:af61129a918d7d5a838f84a53e5c4187bfad03a62baf89b590e2eee9e0ccbd15
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.5 MB (75487992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8222a221a97a3218fabbfecba1af542b4002d5b5999bdcecc8a82f8e724c78a7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:40:29 GMT
ADD file:0b6fc66d778d0cd8ae8b17b92945d98cc34f9c7008cda864ed0a54b5e40b9cb0 in / 
# Wed, 11 Oct 2023 17:40:32 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:09:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:501a599c15b6def048b2e00cfdf6c658061c00a504305ef2075fb1009a62c1e2`  
		Last Modified: Wed, 11 Oct 2023 17:45:01 GMT  
		Size: 50.6 MB (50600791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf9d6abbf47f32cac71cefb6f7233e5f700d4f6f941ca631e29947c5f1df955`  
		Last Modified: Wed, 11 Oct 2023 18:21:57 GMT  
		Size: 24.9 MB (24887201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:5019b5e06e6411dc6681b042d91c4166bda9f959281d3afb18a28b2c51859fe1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (73008824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a14c97aa10bb55fcde7d0ab1936a74404ebc81297baed7f34e394b13f6e1be9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:48:50 GMT
ADD file:b081db8d48290ef5b5f477edb85d8f04d62a6995ec09bdb516d66dbe19b98137 in / 
# Wed, 11 Oct 2023 17:48:55 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:19:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:54dda4e4d31846b7324172a7fda3d0bdc7d8a2105ab27e9a92c2db43f35f9e5d`  
		Last Modified: Wed, 11 Oct 2023 17:59:53 GMT  
		Size: 49.6 MB (49569257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370a64ae3420fd85a23128ef46431df034f9038821764a14bb436272a1345505`  
		Last Modified: Wed, 11 Oct 2023 23:55:20 GMT  
		Size: 23.4 MB (23439567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:744a14b7351b264caa5f532c9e2ddd30adb33c3aff32aa63acc7cf5b82a9400d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.3 MB (79276010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79aafe4e34b99dcfea8074db94ea73e75d2fd2d71b38493a1d9fb2b1d31e811f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:44:01 GMT
ADD file:ed515e1aef8321271c6544e30cbeb31257e9640979e8f68a9e490cb25d3525fd in / 
# Wed, 11 Oct 2023 17:44:04 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:14:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f137383853e717724a59e86aa526d31eabb4a5d45a259cd1ade68d93b3f45ae9`  
		Last Modified: Wed, 11 Oct 2023 17:49:27 GMT  
		Size: 53.6 MB (53575984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da754908592cac64ca75d9cdc8c43a4a396901108de4adae61bd92937de4f65`  
		Last Modified: Wed, 11 Oct 2023 18:36:14 GMT  
		Size: 25.7 MB (25700026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b8e20019afbeea6704a1315aac08a0971e357e86421fea4eadddb139a30796db
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.0 MB (71989702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:547b709e2a6beabff89cf0efea20a9713d1b7b7b7a3d67ecd5bdef17c2ff16fc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:50:07 GMT
ADD file:2dc117136732884ad4b058065700dd66cc49d6ce56b0fdbb672915e3ad8adb84 in / 
# Wed, 11 Oct 2023 17:50:10 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:51:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ad5e374600bf40a929dfe51e52737e4ca04aba83f499656760ba938841fb6552`  
		Last Modified: Wed, 11 Oct 2023 17:55:18 GMT  
		Size: 47.9 MB (47942934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6344f505670ce139b1b3f472749240f33304ec7535daae4a72913a6da08f304f`  
		Last Modified: Thu, 12 Oct 2023 00:33:20 GMT  
		Size: 24.0 MB (24046768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:focal`

```console
$ docker pull buildpack-deps@sha256:bfdf1ac658ab3c2da2a75ca6e60428056f2478e3eba675f2b5639eb96957a711
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
$ docker pull buildpack-deps@sha256:b5fde3cb8a892f44fcc5cd00f64984c2dfbc1f716ae0f3102cd4e87be3075da8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.8 MB (245752605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d936a0f2edffab8e89ae578c7ac39d7c7d57edd069dc932d27927c98628a571f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 Oct 2023 10:45:50 GMT
ARG RELEASE
# Tue, 03 Oct 2023 10:45:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 10:45:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 10:45:50 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 10:45:51 GMT
ADD file:4809da414c2d478b4d991cbdaa2df457f2b3d07d0ff6cf673f09a66f90833e81 in / 
# Tue, 03 Oct 2023 10:45:52 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:11:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 07:12:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 07:15:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a2c559011895d255fce249c00396abff5ae7e0c0a92931d0ed493e71de78e3a`  
		Last Modified: Tue, 03 Oct 2023 17:02:08 GMT  
		Size: 28.6 MB (28580681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c93f97937844870a0d591bb295de8f5d1a3c6b7ea71083ccc820afd4282b3a2`  
		Last Modified: Fri, 13 Oct 2023 07:25:30 GMT  
		Size: 11.1 MB (11129460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd72b323778a4e704264ff859c0e8ef49d0d285cd057d0781881ee1ca649a67`  
		Last Modified: Fri, 13 Oct 2023 07:25:48 GMT  
		Size: 60.9 MB (60923941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f14c4b8174ea549d7ff9050fe9d305f59153eddecfae52c56d0f0c7821e6d4`  
		Last Modified: Fri, 13 Oct 2023 07:26:16 GMT  
		Size: 145.1 MB (145118523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:72e23dbcf10bc3d9f43d4e5f6481fc5724226a4bb3e74ad540729cad2db4e985
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.0 MB (211950429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b3706a3084dfe4471fcf5717dd0c407744133880c98f0a940274260275eb2ae`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 Oct 2023 10:47:59 GMT
ARG RELEASE
# Tue, 03 Oct 2023 10:47:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 10:47:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 10:47:59 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 10:48:06 GMT
ADD file:8dffbfada6e0bebb2858525182aef87ac2cbd88c624f32696ec2cb947e71a4f3 in / 
# Tue, 03 Oct 2023 10:48:07 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 00:57:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 00:57:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 01:00:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3b5f1ba1b648ae0824ed6a95ab17335537f8e689df99917fd374af5dd34078eb`  
		Last Modified: Fri, 13 Oct 2023 01:11:42 GMT  
		Size: 24.6 MB (24592174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccfc7436cda39ac35ae7ab16bdcc8269d47169c65ddf58da5fecf28ab6816624`  
		Last Modified: Fri, 13 Oct 2023 01:11:39 GMT  
		Size: 9.6 MB (9600386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2f3dfd8fbd9e1ce1164f9cf7d74790a3955b9019e8988f682380b086407df7`  
		Last Modified: Fri, 13 Oct 2023 01:12:04 GMT  
		Size: 55.8 MB (55823641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3aa5772d8f961cf51ee5a3fda8e29375c98387fc11a666f5c6eb9f1aebca44`  
		Last Modified: Fri, 13 Oct 2023 01:12:35 GMT  
		Size: 121.9 MB (121934228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:574c7a4001f3053b5329e8dfbb9ec27f35b81556feb2060074dc5c5cf5b8f585
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.0 MB (235965732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d0471cccb43aacbdd96d06b51fd8919703bc70d0d12c0803e1b4cdbf4237e92`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 Oct 2023 11:04:09 GMT
ARG RELEASE
# Tue, 03 Oct 2023 11:04:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 11:04:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 11:04:10 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 11:04:16 GMT
ADD file:f70cc2610ea8fcd25e6e9ae727eb9345d5b7198102f6a6d8e458ab8f99efefc3 in / 
# Tue, 03 Oct 2023 11:04:17 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 02:29:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 02:30:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 02:33:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6cba4020c0a193cd551ed8edf368670967e3546345b52c4ec66cb0931436e9b9`  
		Last Modified: Thu, 05 Oct 2023 12:12:17 GMT  
		Size: 27.2 MB (27199503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8f9293c4d270b52b3bc1e56516c484b0006c603f4445a0da0dcd3616f0daf9`  
		Last Modified: Fri, 13 Oct 2023 02:43:18 GMT  
		Size: 11.0 MB (10982407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:527191c7220ec77d3ed7791fedfc7587efea6f1d575a574622faa5bcb12a587e`  
		Last Modified: Fri, 13 Oct 2023 02:43:36 GMT  
		Size: 61.0 MB (61014037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e779168faa14907195729870f4acff9809719c5e3a31a9529a44fec13b6a2c`  
		Last Modified: Fri, 13 Oct 2023 02:43:59 GMT  
		Size: 136.8 MB (136769785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:8ba8ddea9b71cc2251d69f5e8a55ae5e6c9d13075fb8dede76c9df77cb6ab9b6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.5 MB (269488433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:926f600e0a15696dfbaa70229664b65febe27c33212c1e3f9ad7a11994d19c7f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 Oct 2023 11:03:52 GMT
ARG RELEASE
# Tue, 03 Oct 2023 11:03:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 11:03:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 11:03:53 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 11:03:56 GMT
ADD file:ba2394102af0c0584d39af9ec5dd4fa13286293b4607ac7cb9e16d7a2781eef2 in / 
# Tue, 03 Oct 2023 11:03:56 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 06:55:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 06:56:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 07:02:19 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3046919588b0e4a9b202dcd311befda8e46083ce41f424888dcbea91ce8e6e2`  
		Last Modified: Fri, 13 Oct 2023 06:16:08 GMT  
		Size: 33.3 MB (33306424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e14fbec6dc81f63fbfd4d494bd75555c5cd803486e1d753f061b0d3fce81cdc9`  
		Last Modified: Fri, 13 Oct 2023 07:22:17 GMT  
		Size: 12.9 MB (12937951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45cd0c9f0984989e99ef16079e2f5b95f1a20df097939fe992c991233c3e6b72`  
		Last Modified: Fri, 13 Oct 2023 07:22:39 GMT  
		Size: 69.6 MB (69644829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7eb02628173f481bf164e9a0c112a72e5bdea9eda1906464cc8b1bb3d9cfc7`  
		Last Modified: Fri, 13 Oct 2023 07:23:13 GMT  
		Size: 153.6 MB (153599229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:146a4f8c725380eec620a5f6d2f018386dc774ce13692cc79159c2f120c7137a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.6 MB (226607654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed94ac912c0ed9895b3abef8896dee8e605f2bc4e578bb2b29f23932a7ba0bea`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:17:39 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:17:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:17:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:17:39 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:17:41 GMT
ADD file:36efc3ec29bb54e0987fe91be1aa7cc849909b3cd2534af3de2d3d07a03804cf in / 
# Tue, 01 Aug 2023 06:17:41 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 00:08:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 00:09:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 00:11:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:365fa2124eb5f6f369204f3fe0210d9965952628707dfacd4194a8e15caf0420`  
		Last Modified: Thu, 03 Aug 2023 00:03:37 GMT  
		Size: 27.0 MB (27014233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b6082f2457965a87b9693265b680b0a0aa5d30ef936b6df14487a947354b10`  
		Last Modified: Thu, 03 Aug 2023 00:21:05 GMT  
		Size: 10.7 MB (10688615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5764a6c44dcfc11bcbd3dda534db4967a8ffd1443cbe922c189701e996c2c222`  
		Last Modified: Thu, 03 Aug 2023 00:21:19 GMT  
		Size: 60.3 MB (60311530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1c95e4e206b384145bd8128e74027e092da89c7654f4aebfd616735756a6f9`  
		Last Modified: Thu, 03 Aug 2023 00:21:42 GMT  
		Size: 128.6 MB (128593276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:focal-curl`

```console
$ docker pull buildpack-deps@sha256:b8f274a0d962394e7560a9e6bbe50cdf681b997d8ff76b75dfc16c32366cb9a4
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
$ docker pull buildpack-deps@sha256:199614fe208a7619cdca61ecaf5fd02a9b68698693e7ce08cb12310161add350
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.7 MB (39710141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2297c8acf409d2896d99e9f7b7f2bcafaceb58bca7a1c4c1ff1d8ece2e0f59a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 Oct 2023 10:45:50 GMT
ARG RELEASE
# Tue, 03 Oct 2023 10:45:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 10:45:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 10:45:50 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 10:45:51 GMT
ADD file:4809da414c2d478b4d991cbdaa2df457f2b3d07d0ff6cf673f09a66f90833e81 in / 
# Tue, 03 Oct 2023 10:45:52 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:11:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a2c559011895d255fce249c00396abff5ae7e0c0a92931d0ed493e71de78e3a`  
		Last Modified: Tue, 03 Oct 2023 17:02:08 GMT  
		Size: 28.6 MB (28580681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c93f97937844870a0d591bb295de8f5d1a3c6b7ea71083ccc820afd4282b3a2`  
		Last Modified: Fri, 13 Oct 2023 07:25:30 GMT  
		Size: 11.1 MB (11129460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:62d55d00bdfd031cd04241520627268e72f9785291c812a5241638dda1f4ef2a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.2 MB (34192560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad3e920efdd7794c8223f7269f8035dbf5244950528e86dc0adb8b32ce5bd09e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 Oct 2023 10:47:59 GMT
ARG RELEASE
# Tue, 03 Oct 2023 10:47:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 10:47:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 10:47:59 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 10:48:06 GMT
ADD file:8dffbfada6e0bebb2858525182aef87ac2cbd88c624f32696ec2cb947e71a4f3 in / 
# Tue, 03 Oct 2023 10:48:07 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 00:57:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3b5f1ba1b648ae0824ed6a95ab17335537f8e689df99917fd374af5dd34078eb`  
		Last Modified: Fri, 13 Oct 2023 01:11:42 GMT  
		Size: 24.6 MB (24592174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccfc7436cda39ac35ae7ab16bdcc8269d47169c65ddf58da5fecf28ab6816624`  
		Last Modified: Fri, 13 Oct 2023 01:11:39 GMT  
		Size: 9.6 MB (9600386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:ad462829462c403622fdfcadefd354333067ac8ebf9aae0883a7241e0e27b5cb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38181910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb4d46a93ed4cd4d8d5ebf40b8ddf72eb3a089aa3594f3d51537c78945573ea6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 Oct 2023 11:04:09 GMT
ARG RELEASE
# Tue, 03 Oct 2023 11:04:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 11:04:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 11:04:10 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 11:04:16 GMT
ADD file:f70cc2610ea8fcd25e6e9ae727eb9345d5b7198102f6a6d8e458ab8f99efefc3 in / 
# Tue, 03 Oct 2023 11:04:17 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 02:29:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6cba4020c0a193cd551ed8edf368670967e3546345b52c4ec66cb0931436e9b9`  
		Last Modified: Thu, 05 Oct 2023 12:12:17 GMT  
		Size: 27.2 MB (27199503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8f9293c4d270b52b3bc1e56516c484b0006c603f4445a0da0dcd3616f0daf9`  
		Last Modified: Fri, 13 Oct 2023 02:43:18 GMT  
		Size: 11.0 MB (10982407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:9c2ddc832bd5e7c1caba6736b28c294152b0f8d5f6237e63f698b5acc5b47a04
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.2 MB (46244375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:144ccbf81093f12806a06f937ba5d33d99336e1f72f953180a0fae81473f91b4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 Oct 2023 11:03:52 GMT
ARG RELEASE
# Tue, 03 Oct 2023 11:03:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 11:03:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 11:03:53 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 11:03:56 GMT
ADD file:ba2394102af0c0584d39af9ec5dd4fa13286293b4607ac7cb9e16d7a2781eef2 in / 
# Tue, 03 Oct 2023 11:03:56 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 06:55:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3046919588b0e4a9b202dcd311befda8e46083ce41f424888dcbea91ce8e6e2`  
		Last Modified: Fri, 13 Oct 2023 06:16:08 GMT  
		Size: 33.3 MB (33306424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e14fbec6dc81f63fbfd4d494bd75555c5cd803486e1d753f061b0d3fce81cdc9`  
		Last Modified: Fri, 13 Oct 2023 07:22:17 GMT  
		Size: 12.9 MB (12937951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:028f59f497fa2c8e7f3a358182ef00c601e83780a8c7f9b0fd4e4f0f735ef4cc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37702848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:674186b606991aba08faede7dbb56393ab45900ba8c3e92969a9030076dba1be`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:17:39 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:17:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:17:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:17:39 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:17:41 GMT
ADD file:36efc3ec29bb54e0987fe91be1aa7cc849909b3cd2534af3de2d3d07a03804cf in / 
# Tue, 01 Aug 2023 06:17:41 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 00:08:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:365fa2124eb5f6f369204f3fe0210d9965952628707dfacd4194a8e15caf0420`  
		Last Modified: Thu, 03 Aug 2023 00:03:37 GMT  
		Size: 27.0 MB (27014233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b6082f2457965a87b9693265b680b0a0aa5d30ef936b6df14487a947354b10`  
		Last Modified: Thu, 03 Aug 2023 00:21:05 GMT  
		Size: 10.7 MB (10688615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:focal-scm`

```console
$ docker pull buildpack-deps@sha256:aa8ad732eec0478a2a39d4674bb6c0688b173b5dda2c8b058d88df485607fe56
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
$ docker pull buildpack-deps@sha256:7ba510d2d414f7f32506b2648e8fae33163f38a95dc9ad53506ddc728fc190d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.6 MB (100634082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d252f65001e3c05b44da7e1571a3fe4ba3665f5da85a30da8ed21e0f01a6550`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 Oct 2023 10:45:50 GMT
ARG RELEASE
# Tue, 03 Oct 2023 10:45:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 10:45:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 10:45:50 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 10:45:51 GMT
ADD file:4809da414c2d478b4d991cbdaa2df457f2b3d07d0ff6cf673f09a66f90833e81 in / 
# Tue, 03 Oct 2023 10:45:52 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:11:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 07:12:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a2c559011895d255fce249c00396abff5ae7e0c0a92931d0ed493e71de78e3a`  
		Last Modified: Tue, 03 Oct 2023 17:02:08 GMT  
		Size: 28.6 MB (28580681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c93f97937844870a0d591bb295de8f5d1a3c6b7ea71083ccc820afd4282b3a2`  
		Last Modified: Fri, 13 Oct 2023 07:25:30 GMT  
		Size: 11.1 MB (11129460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd72b323778a4e704264ff859c0e8ef49d0d285cd057d0781881ee1ca649a67`  
		Last Modified: Fri, 13 Oct 2023 07:25:48 GMT  
		Size: 60.9 MB (60923941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:683c088512efd787bc9a974011eb4710f29b79c298484c32dd5aae263b8fe867
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.0 MB (90016201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3df2135c694ed153481f35d24358fa8df0b07a6ca05006e4b6658177b45c2643`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 Oct 2023 10:47:59 GMT
ARG RELEASE
# Tue, 03 Oct 2023 10:47:59 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 10:47:59 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 10:47:59 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 10:48:06 GMT
ADD file:8dffbfada6e0bebb2858525182aef87ac2cbd88c624f32696ec2cb947e71a4f3 in / 
# Tue, 03 Oct 2023 10:48:07 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 00:57:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 00:57:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3b5f1ba1b648ae0824ed6a95ab17335537f8e689df99917fd374af5dd34078eb`  
		Last Modified: Fri, 13 Oct 2023 01:11:42 GMT  
		Size: 24.6 MB (24592174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccfc7436cda39ac35ae7ab16bdcc8269d47169c65ddf58da5fecf28ab6816624`  
		Last Modified: Fri, 13 Oct 2023 01:11:39 GMT  
		Size: 9.6 MB (9600386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b2f3dfd8fbd9e1ce1164f9cf7d74790a3955b9019e8988f682380b086407df7`  
		Last Modified: Fri, 13 Oct 2023 01:12:04 GMT  
		Size: 55.8 MB (55823641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:ee4a206dccb175102b3cb2bcf54c4af292f785a26e4c587503957b91512966a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99195947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:297ad753ed84562e345544abda8a38e822dfaad4357141a3af6198c83163c400`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 Oct 2023 11:04:09 GMT
ARG RELEASE
# Tue, 03 Oct 2023 11:04:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 11:04:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 11:04:10 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 11:04:16 GMT
ADD file:f70cc2610ea8fcd25e6e9ae727eb9345d5b7198102f6a6d8e458ab8f99efefc3 in / 
# Tue, 03 Oct 2023 11:04:17 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 02:29:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 02:30:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6cba4020c0a193cd551ed8edf368670967e3546345b52c4ec66cb0931436e9b9`  
		Last Modified: Thu, 05 Oct 2023 12:12:17 GMT  
		Size: 27.2 MB (27199503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8f9293c4d270b52b3bc1e56516c484b0006c603f4445a0da0dcd3616f0daf9`  
		Last Modified: Fri, 13 Oct 2023 02:43:18 GMT  
		Size: 11.0 MB (10982407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:527191c7220ec77d3ed7791fedfc7587efea6f1d575a574622faa5bcb12a587e`  
		Last Modified: Fri, 13 Oct 2023 02:43:36 GMT  
		Size: 61.0 MB (61014037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:9e4691461e8152658a19c6f908b58a8314e928b0fbc6c6da999d39f9655b4154
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.9 MB (115889204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0438293bebad2e61d50f207839478e418b17d5c295b4a9f5c7af55ef6c15f04c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 Oct 2023 11:03:52 GMT
ARG RELEASE
# Tue, 03 Oct 2023 11:03:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 11:03:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 11:03:53 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 11:03:56 GMT
ADD file:ba2394102af0c0584d39af9ec5dd4fa13286293b4607ac7cb9e16d7a2781eef2 in / 
# Tue, 03 Oct 2023 11:03:56 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 06:55:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 06:56:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f3046919588b0e4a9b202dcd311befda8e46083ce41f424888dcbea91ce8e6e2`  
		Last Modified: Fri, 13 Oct 2023 06:16:08 GMT  
		Size: 33.3 MB (33306424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e14fbec6dc81f63fbfd4d494bd75555c5cd803486e1d753f061b0d3fce81cdc9`  
		Last Modified: Fri, 13 Oct 2023 07:22:17 GMT  
		Size: 12.9 MB (12937951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45cd0c9f0984989e99ef16079e2f5b95f1a20df097939fe992c991233c3e6b72`  
		Last Modified: Fri, 13 Oct 2023 07:22:39 GMT  
		Size: 69.6 MB (69644829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:079f48635b01d56e2478857b7e0c5fb6212336f9e594e783bbf19cb9dda8b0f2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.0 MB (98014378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2522830f5bbe1d8ea3e120ce6ff28c07dbc6f1a8b7f24c17fbb61b252bbab549`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:17:39 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:17:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:17:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:17:39 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:17:41 GMT
ADD file:36efc3ec29bb54e0987fe91be1aa7cc849909b3cd2534af3de2d3d07a03804cf in / 
# Tue, 01 Aug 2023 06:17:41 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 00:08:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 00:09:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:365fa2124eb5f6f369204f3fe0210d9965952628707dfacd4194a8e15caf0420`  
		Last Modified: Thu, 03 Aug 2023 00:03:37 GMT  
		Size: 27.0 MB (27014233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b6082f2457965a87b9693265b680b0a0aa5d30ef936b6df14487a947354b10`  
		Last Modified: Thu, 03 Aug 2023 00:21:05 GMT  
		Size: 10.7 MB (10688615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5764a6c44dcfc11bcbd3dda534db4967a8ffd1443cbe922c189701e996c2c222`  
		Last Modified: Thu, 03 Aug 2023 00:21:19 GMT  
		Size: 60.3 MB (60311530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:jammy`

```console
$ docker pull buildpack-deps@sha256:813d299dc3512a6029a8966e92b1080a48d0dda2d6a2f61679b00956b55627e4
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
$ docker pull buildpack-deps@sha256:24fe4235a691b49a8f4c3570eabdbeb2e33f712a7bf05f41717fce9c36bea901
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.0 MB (250049463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9336076452fd84376c39d0382d6478cbea7dbc26b7297b2436651d60a984ce18`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:33:30 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:33:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:33:32 GMT
ADD file:63d5ab3ef0aab308c0e71cb67292c5467f60deafa9b0418cbb220affcd078444 in / 
# Thu, 05 Oct 2023 07:33:32 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:15:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 07:16:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 07:18:52 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:43f89b94cd7df92a2f7e565b8fb1b7f502eff2cd225508cbd7ea2d36a9a3a601`  
		Last Modified: Thu, 05 Oct 2023 08:42:10 GMT  
		Size: 30.4 MB (30439111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c42c1a5016fb63983b7331918ba3251a006a305a7155f887c55ba0310f14ebe4`  
		Last Modified: Fri, 13 Oct 2023 07:26:26 GMT  
		Size: 7.1 MB (7119810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b397bf7f6432393178dcfa275258dfbbf1774183c2bf6d2c376676b1eb9d96ce`  
		Last Modified: Fri, 13 Oct 2023 07:26:41 GMT  
		Size: 39.4 MB (39447269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43f2be70120bd273670e90c14b5caba9a9ed79e5e2195d9fa5751dded927f82`  
		Last Modified: Fri, 13 Oct 2023 07:27:11 GMT  
		Size: 173.0 MB (173043273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:c8c55fc1ddcc289ed750014d5a333d4da1b4c38d9f56e3e28cfc94d75598b64a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.3 MB (217299987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c6ad0546b1c789630d2ab10627fc670a8e959846a0ed9b4d3b0155f252a87bf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:34:56 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:34:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:34:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:34:56 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:35:01 GMT
ADD file:4b9d52f97ed5796b14772a84c1e7213402430d32312d15ae04a2dcc9fc485a52 in / 
# Thu, 05 Oct 2023 07:35:02 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 01:01:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 01:01:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 01:04:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c4f28c22de51200ba6a71d2274daa2f71735946524265b3c45752d2cec53dee0`  
		Last Modified: Fri, 06 Oct 2023 02:02:33 GMT  
		Size: 27.5 MB (27513969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85fc270943bb9c7cfec1343fa169349a26edefb92574ab25cc3c91ba173fac6`  
		Last Modified: Fri, 13 Oct 2023 01:12:46 GMT  
		Size: 7.0 MB (7019227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0b0c5f614ae9b9b0ea44d893e337f282182465a7b811e594df1df46ba55b02`  
		Last Modified: Fri, 13 Oct 2023 01:13:07 GMT  
		Size: 42.2 MB (42240097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c437efecc24744323340d7367e5cf9fe9550f503e10d438a7fedc3c39d0adb53`  
		Last Modified: Fri, 13 Oct 2023 01:13:39 GMT  
		Size: 140.5 MB (140526694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:033f47d0faaf35e3f9a908e8f28aa41349a3c04e7992409d9738936e0b5ace76
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.3 MB (241335805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:878ba0f3fe1ba872439dc5242931f1bea039ea8b923db8db743c9fc3773a7e61`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:32:20 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:32:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:32:22 GMT
ADD file:f8594e26831508c318e42c8dfd9942041031087b8de1bf3fec11fd75b8b30fd4 in / 
# Thu, 05 Oct 2023 07:32:22 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 02:33:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 02:34:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 02:36:52 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:895d322e8e5957c04af3ab7b3431f2a562182d34167c6e159e02044150a66967`  
		Last Modified: Thu, 05 Oct 2023 08:57:30 GMT  
		Size: 28.4 MB (28391939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab98684ba3fe8f55da444be42c97a55fce3f516fbef08145bd1ee5686d63f30`  
		Last Modified: Fri, 13 Oct 2023 02:44:09 GMT  
		Size: 7.1 MB (7066736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:137f888ab5ca54ae228d9aa08792d8dfc0505614071a433dab0b8d64853412d1`  
		Last Modified: Fri, 13 Oct 2023 02:44:24 GMT  
		Size: 39.4 MB (39363322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f636694bf2d25bc6aa577bcca3dc616db456936312afcfea87dbc51426d0892e`  
		Last Modified: Fri, 13 Oct 2023 02:44:49 GMT  
		Size: 166.5 MB (166513808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:672844360fcc6634c2ea76d298bd650eb4ba32f85543816e1f43f814ee105810
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.4 MB (271425284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8f7f46cd62289364aaaed1c58e0b2ae9b323a91f98f9bd611cc8bca32799d56`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:34:18 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:34:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:34:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:34:19 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:34:22 GMT
ADD file:595ff761b2778bdc6bb59cbe8ce51c4a247e0f279ccd59a17b5be6cdeac0b4d2 in / 
# Thu, 05 Oct 2023 07:34:22 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:03:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 07:04:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 07:10:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:589c4cce1daa100afadbdbeda96025d02f85c117e0e60b70801af41b4e618668`  
		Last Modified: Fri, 13 Oct 2023 06:13:20 GMT  
		Size: 35.7 MB (35682793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3915535cd53c34e21aaca3d30c265266ed72ec102dc961ecd9c0616cf6e3df6c`  
		Last Modified: Fri, 13 Oct 2023 07:23:24 GMT  
		Size: 8.3 MB (8253985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7fb2022d4edb92326fe02a877beeae2b46b6b000fb736302f493bec3e625a78`  
		Last Modified: Fri, 13 Oct 2023 07:23:41 GMT  
		Size: 43.8 MB (43764927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff661c5b91d15269c1e42d2b9e38dfe8f206ca2dc9be9069267996663d3f4748`  
		Last Modified: Fri, 13 Oct 2023 07:24:18 GMT  
		Size: 183.7 MB (183723579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:e4399018428c842b4c392e87a36defdb82afeac9551fc87958cfe3d55d3ca0ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.8 MB (223831456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a917d107abf2d33f9279640b659e2f7f812ed5720b724978da723df3da955601`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 25 Sep 2023 10:17:26 GMT
ARG RELEASE
# Mon, 25 Sep 2023 10:17:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 25 Sep 2023 10:17:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 25 Sep 2023 10:17:26 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 25 Sep 2023 10:17:28 GMT
ADD file:78683f2464233172a7cd0d6adc4c7d9fb3ef05fa67ca22e6fbaca0325496a536 in / 
# Mon, 25 Sep 2023 10:17:28 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 08:49:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 08:49:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 08:52:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b6ba488997f9924c9473e547d56b3d4ae74495b1092ca3c613243185ee5d5151`  
		Last Modified: Tue, 03 Oct 2023 08:59:45 GMT  
		Size: 28.7 MB (28651983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63dcb81ab3d8b1a5d99f79f12abeae58d32d80628c914e5b75ac72c82c71adf1`  
		Last Modified: Tue, 03 Oct 2023 08:59:42 GMT  
		Size: 7.0 MB (7033657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05bd5fa6428d58b59c71d06922c39d17e607ab984f737113aea36b3899777d6`  
		Last Modified: Tue, 03 Oct 2023 09:00:17 GMT  
		Size: 39.4 MB (39413935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61eff3bbf0140cf19e8752d02bd7fb1d00a0d33b08b27067a5b9e2b6f6517a64`  
		Last Modified: Tue, 03 Oct 2023 09:00:58 GMT  
		Size: 148.7 MB (148731881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:jammy-curl`

```console
$ docker pull buildpack-deps@sha256:085a23a57a491311104937fb13c53bf25fad7b201ff429a1ae6815cc84afdddc
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
$ docker pull buildpack-deps@sha256:0f644f5b2afab0d3227b2b34c6a6f129c88ba104f3c07a5ce0b29edfbf6ef91e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37558921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b5f87e49274876d9c93c07c94ec36af2b0f9a55ed8088620181fd55723912c0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:33:30 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:33:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:33:32 GMT
ADD file:63d5ab3ef0aab308c0e71cb67292c5467f60deafa9b0418cbb220affcd078444 in / 
# Thu, 05 Oct 2023 07:33:32 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:15:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:43f89b94cd7df92a2f7e565b8fb1b7f502eff2cd225508cbd7ea2d36a9a3a601`  
		Last Modified: Thu, 05 Oct 2023 08:42:10 GMT  
		Size: 30.4 MB (30439111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c42c1a5016fb63983b7331918ba3251a006a305a7155f887c55ba0310f14ebe4`  
		Last Modified: Fri, 13 Oct 2023 07:26:26 GMT  
		Size: 7.1 MB (7119810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:d1d6a1fcdbc5c3af24c46feea2f9cbf4d8b8fd4e01c3d58bc4b59dee727945b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 MB (34533196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18773abeaa0270194048921ebd164d0a4c7a6649da81086097b4e2445330ba1c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:34:56 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:34:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:34:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:34:56 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:35:01 GMT
ADD file:4b9d52f97ed5796b14772a84c1e7213402430d32312d15ae04a2dcc9fc485a52 in / 
# Thu, 05 Oct 2023 07:35:02 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 01:01:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c4f28c22de51200ba6a71d2274daa2f71735946524265b3c45752d2cec53dee0`  
		Last Modified: Fri, 06 Oct 2023 02:02:33 GMT  
		Size: 27.5 MB (27513969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85fc270943bb9c7cfec1343fa169349a26edefb92574ab25cc3c91ba173fac6`  
		Last Modified: Fri, 13 Oct 2023 01:12:46 GMT  
		Size: 7.0 MB (7019227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:549886f44fbb35904c5e8e1c2fea61d8ec12b5caaf0c82cf7efecd82da406a46
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 MB (35458675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58af3f1d094523439bff7af275c13d0b37d05a7f53ef22e92773e3945f20587f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:32:20 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:32:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:32:22 GMT
ADD file:f8594e26831508c318e42c8dfd9942041031087b8de1bf3fec11fd75b8b30fd4 in / 
# Thu, 05 Oct 2023 07:32:22 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 02:33:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:895d322e8e5957c04af3ab7b3431f2a562182d34167c6e159e02044150a66967`  
		Last Modified: Thu, 05 Oct 2023 08:57:30 GMT  
		Size: 28.4 MB (28391939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab98684ba3fe8f55da444be42c97a55fce3f516fbef08145bd1ee5686d63f30`  
		Last Modified: Fri, 13 Oct 2023 02:44:09 GMT  
		Size: 7.1 MB (7066736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d906fc4587e2ecce9c87f730384cc30acca1c1d47298757243269d7924495089
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43936778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c62c64ba3f1b4292cf95704aba38456563dd67309339d32ee6e3e80ab9e890a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:34:18 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:34:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:34:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:34:19 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:34:22 GMT
ADD file:595ff761b2778bdc6bb59cbe8ce51c4a247e0f279ccd59a17b5be6cdeac0b4d2 in / 
# Thu, 05 Oct 2023 07:34:22 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:03:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:589c4cce1daa100afadbdbeda96025d02f85c117e0e60b70801af41b4e618668`  
		Last Modified: Fri, 13 Oct 2023 06:13:20 GMT  
		Size: 35.7 MB (35682793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3915535cd53c34e21aaca3d30c265266ed72ec102dc961ecd9c0616cf6e3df6c`  
		Last Modified: Fri, 13 Oct 2023 07:23:24 GMT  
		Size: 8.3 MB (8253985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:f261ff2241965d50e93901c04a586655af4008f24a94241d1b2ddf8123f0bd26
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35685640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8fe1a2e1659b935c6f8f380bb55c01fe947e5f305337a3f181485a1fe5d7859`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 25 Sep 2023 10:17:26 GMT
ARG RELEASE
# Mon, 25 Sep 2023 10:17:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 25 Sep 2023 10:17:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 25 Sep 2023 10:17:26 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 25 Sep 2023 10:17:28 GMT
ADD file:78683f2464233172a7cd0d6adc4c7d9fb3ef05fa67ca22e6fbaca0325496a536 in / 
# Mon, 25 Sep 2023 10:17:28 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 08:49:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b6ba488997f9924c9473e547d56b3d4ae74495b1092ca3c613243185ee5d5151`  
		Last Modified: Tue, 03 Oct 2023 08:59:45 GMT  
		Size: 28.7 MB (28651983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63dcb81ab3d8b1a5d99f79f12abeae58d32d80628c914e5b75ac72c82c71adf1`  
		Last Modified: Tue, 03 Oct 2023 08:59:42 GMT  
		Size: 7.0 MB (7033657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:jammy-scm`

```console
$ docker pull buildpack-deps@sha256:f5eb46c4570633bedc3cfa85a592bef312277dd23650e930c58a7c73f9ae8429
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
$ docker pull buildpack-deps@sha256:d24c158fc955083cf096191ae38bbd3cd1ec155e695f4bae2378e78079aa22eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (77006190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dce2ef8e1153a09bce17fbf2148781d63ebe67c1f28767f41a8e6b95a8831f92`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:33:30 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:33:30 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:33:30 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:33:32 GMT
ADD file:63d5ab3ef0aab308c0e71cb67292c5467f60deafa9b0418cbb220affcd078444 in / 
# Thu, 05 Oct 2023 07:33:32 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:15:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 07:16:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:43f89b94cd7df92a2f7e565b8fb1b7f502eff2cd225508cbd7ea2d36a9a3a601`  
		Last Modified: Thu, 05 Oct 2023 08:42:10 GMT  
		Size: 30.4 MB (30439111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c42c1a5016fb63983b7331918ba3251a006a305a7155f887c55ba0310f14ebe4`  
		Last Modified: Fri, 13 Oct 2023 07:26:26 GMT  
		Size: 7.1 MB (7119810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b397bf7f6432393178dcfa275258dfbbf1774183c2bf6d2c376676b1eb9d96ce`  
		Last Modified: Fri, 13 Oct 2023 07:26:41 GMT  
		Size: 39.4 MB (39447269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:465a04ef4d05ae8daffc7108037ecff2d65c230ab338beaa2a7ca258e2ade9b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.8 MB (76773293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf0e57397bae1b99eb3b196a13dc8e1c4fa6c39d62f3b649961c51c66ee87fc8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:34:56 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:34:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:34:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:34:56 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:35:01 GMT
ADD file:4b9d52f97ed5796b14772a84c1e7213402430d32312d15ae04a2dcc9fc485a52 in / 
# Thu, 05 Oct 2023 07:35:02 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 01:01:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 01:01:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c4f28c22de51200ba6a71d2274daa2f71735946524265b3c45752d2cec53dee0`  
		Last Modified: Fri, 06 Oct 2023 02:02:33 GMT  
		Size: 27.5 MB (27513969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85fc270943bb9c7cfec1343fa169349a26edefb92574ab25cc3c91ba173fac6`  
		Last Modified: Fri, 13 Oct 2023 01:12:46 GMT  
		Size: 7.0 MB (7019227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0b0c5f614ae9b9b0ea44d893e337f282182465a7b811e594df1df46ba55b02`  
		Last Modified: Fri, 13 Oct 2023 01:13:07 GMT  
		Size: 42.2 MB (42240097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:23a410e3dfc5f893887c6f91e3d96a404c7b844d74cb597f0d10483d8200c8bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74821997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dab2960221ba40117786b31739f218f59b91426bb60076b90d952377329f0fd0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:32:20 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:32:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:32:21 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:32:22 GMT
ADD file:f8594e26831508c318e42c8dfd9942041031087b8de1bf3fec11fd75b8b30fd4 in / 
# Thu, 05 Oct 2023 07:32:22 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 02:33:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 02:34:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:895d322e8e5957c04af3ab7b3431f2a562182d34167c6e159e02044150a66967`  
		Last Modified: Thu, 05 Oct 2023 08:57:30 GMT  
		Size: 28.4 MB (28391939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab98684ba3fe8f55da444be42c97a55fce3f516fbef08145bd1ee5686d63f30`  
		Last Modified: Fri, 13 Oct 2023 02:44:09 GMT  
		Size: 7.1 MB (7066736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:137f888ab5ca54ae228d9aa08792d8dfc0505614071a433dab0b8d64853412d1`  
		Last Modified: Fri, 13 Oct 2023 02:44:24 GMT  
		Size: 39.4 MB (39363322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:18932b92e188adb2feac77ff881d8a29babc9805aede5aecf7e2641bd8e80386
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.7 MB (87701705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ac4f1d31d15e96607b82c209778a0051c4dd5a64441fb0258a3267314f9db17`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:34:18 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:34:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:34:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:34:19 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:34:22 GMT
ADD file:595ff761b2778bdc6bb59cbe8ce51c4a247e0f279ccd59a17b5be6cdeac0b4d2 in / 
# Thu, 05 Oct 2023 07:34:22 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:03:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 07:04:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:589c4cce1daa100afadbdbeda96025d02f85c117e0e60b70801af41b4e618668`  
		Last Modified: Fri, 13 Oct 2023 06:13:20 GMT  
		Size: 35.7 MB (35682793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3915535cd53c34e21aaca3d30c265266ed72ec102dc961ecd9c0616cf6e3df6c`  
		Last Modified: Fri, 13 Oct 2023 07:23:24 GMT  
		Size: 8.3 MB (8253985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7fb2022d4edb92326fe02a877beeae2b46b6b000fb736302f493bec3e625a78`  
		Last Modified: Fri, 13 Oct 2023 07:23:41 GMT  
		Size: 43.8 MB (43764927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:f7037c2ca159e27e211e9d3f4c6a04a0a3bf3182edc42d8210a1d965cfe1673d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75099575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34bf07ba4c66ab3817378608226748f1a91d05832c79d5360e4c516bd11c204e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 25 Sep 2023 10:17:26 GMT
ARG RELEASE
# Mon, 25 Sep 2023 10:17:26 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 25 Sep 2023 10:17:26 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 25 Sep 2023 10:17:26 GMT
LABEL org.opencontainers.image.version=22.04
# Mon, 25 Sep 2023 10:17:28 GMT
ADD file:78683f2464233172a7cd0d6adc4c7d9fb3ef05fa67ca22e6fbaca0325496a536 in / 
# Mon, 25 Sep 2023 10:17:28 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 08:49:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 08:49:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b6ba488997f9924c9473e547d56b3d4ae74495b1092ca3c613243185ee5d5151`  
		Last Modified: Tue, 03 Oct 2023 08:59:45 GMT  
		Size: 28.7 MB (28651983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63dcb81ab3d8b1a5d99f79f12abeae58d32d80628c914e5b75ac72c82c71adf1`  
		Last Modified: Tue, 03 Oct 2023 08:59:42 GMT  
		Size: 7.0 MB (7033657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05bd5fa6428d58b59c71d06922c39d17e607ab984f737113aea36b3899777d6`  
		Last Modified: Tue, 03 Oct 2023 09:00:17 GMT  
		Size: 39.4 MB (39413935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:latest`

```console
$ docker pull buildpack-deps@sha256:584ae312404463556590dbd340dc888147030cb3c8cbaec1ae7fc474ac453fdd
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
$ docker pull buildpack-deps@sha256:e5e5c80b6c13eb1ac931b319d5b2dda3a67473c085edc2ef5212ee628f4ee6bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.8 MB (348827828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c9f4bf96c80ab0bd24165e83092eab60265322c4575d970deaae7e8a4742ea3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:37 GMT
ADD file:1e4dd5dab602337b5d5ef8d84b8dbe8b1ac62225f077b29b27d045842486d8e2 in / 
# Wed, 11 Oct 2023 18:34:37 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:19:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:19:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:20:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0a9573503463fd3166b5b1f34a7720dac28609e98d731e50e7068f92e79b8545`  
		Last Modified: Wed, 11 Oct 2023 18:39:10 GMT  
		Size: 49.6 MB (49582224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ccc26d841b4acc2562483bf393ce1cf8bc358ced09ccd825425226827c79c92`  
		Last Modified: Thu, 12 Oct 2023 03:28:45 GMT  
		Size: 24.1 MB (24051259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800d84653581fc119cd75cd572fa190d3b813d49221b9e5ee463e3560e2cb342`  
		Last Modified: Thu, 12 Oct 2023 03:29:04 GMT  
		Size: 64.1 MB (64130287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c632e57ea62ea950c367f484f52cdcfd2adb12060a31f5c413f40db9822e96e`  
		Last Modified: Thu, 12 Oct 2023 03:29:40 GMT  
		Size: 211.1 MB (211064058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:86d28c1e87df6d4e3309e403a9ced8594ad1380ffb29db3cbb99ee65245d77e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.0 MB (316030711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f61c441d8080fa400d21357cb9170445e8b0e150d15c350be1e20d0849837a84`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:37:30 GMT
ADD file:c07cf5c750a3e3c7ff84a3a3b8fc6087c9c5e0639d7bf638f0556d0a94309919 in / 
# Wed, 11 Oct 2023 17:37:35 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:04:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:05:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:06:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b7ec6536594e6c45ab234eecb51aacd85440ddc0e6da5873de23938ff146b5ec`  
		Last Modified: Wed, 11 Oct 2023 17:40:19 GMT  
		Size: 47.4 MB (47355749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ec943df1872e82ab3efa51bd5b2d7aac598550123e6db67156283ade7509d1`  
		Last Modified: Wed, 11 Oct 2023 18:14:31 GMT  
		Size: 22.7 MB (22729282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9f5c18924658cf6e03e52e00ddbf230cb1925aa017edb92b3cd508ec76293f`  
		Last Modified: Wed, 11 Oct 2023 18:14:54 GMT  
		Size: 61.6 MB (61561678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7670741713d795c2814eacfe8b75187f28e3485379b6fb2770c71d163e26127`  
		Last Modified: Wed, 11 Oct 2023 18:15:37 GMT  
		Size: 184.4 MB (184384002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:28ad6736c4c7a5c78602a4c42becc99de682ba5927aa95ad9f5105294d099a8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.4 MB (301449230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43d67f8c14cfd8cddba9828203d94136bcc749df068cfbc834ba011ede605f79`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:41:59 GMT
ADD file:914e8a43f38c44fe9a6aabf05bbf3ebad5530966a354c8e7bb873c0842d35256 in / 
# Wed, 11 Oct 2023 17:42:00 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:45:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:45:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:46:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:65b9f3344eccdad2292cc7eec885befe05a52ec1136e145130c849441428eee6`  
		Last Modified: Wed, 11 Oct 2023 17:45:56 GMT  
		Size: 45.2 MB (45180287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbdddb82776e8c5901a821d5034c82b0fcba2993014440cd080d0592cd49616`  
		Last Modified: Thu, 12 Oct 2023 03:55:58 GMT  
		Size: 22.0 MB (21953833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f9d9ae792bc9a3749049ab80543cfddbda8910bcaffc9c95c7db4feb9e625a6`  
		Last Modified: Thu, 12 Oct 2023 03:56:18 GMT  
		Size: 59.3 MB (59266472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9912e09bb3246583228b0aa9f45499f60d04bbb57d5db9e63d50fd5585cc0c20`  
		Last Modified: Thu, 12 Oct 2023 03:56:58 GMT  
		Size: 175.0 MB (175048638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:1217daf5693bf080affa2383e80682e4ed80fa25c7b6889924e21e401abfef07
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.6 MB (339643434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13543f9c2ab23caf4e23f3900fa93f86e7a0d57bbfb3dfb296c3985b777511b8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:43 GMT
ADD file:bf4264671bd91eb30c67d512144ebcf7f5c55a3e490ebe7876fa9b20d433bf7b in / 
# Wed, 11 Oct 2023 18:24:44 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:44:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:45:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:46:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e720f94321d63ecb6efa873b294dce7eaa1c3a5ddcd5bf7daddf375b955669a4`  
		Last Modified: Wed, 11 Oct 2023 18:28:04 GMT  
		Size: 49.6 MB (49612578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7541d83e7b8c0f5f6cacacddfcf5fdd942793f13418bc4645203b4ab4f3de3`  
		Last Modified: Wed, 11 Oct 2023 19:53:48 GMT  
		Size: 23.6 MB (23588086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a653d69b7b96df6835b157d043d7b926f776531e96c9263f4c7dae0033514d`  
		Last Modified: Wed, 11 Oct 2023 19:54:07 GMT  
		Size: 64.0 MB (63994319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c02d5d50082e4632f070b715dfd5d3a3680e35e0434a1281edbcfdc3cdff52dc`  
		Last Modified: Wed, 11 Oct 2023 19:54:39 GMT  
		Size: 202.4 MB (202448451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; 386

```console
$ docker pull buildpack-deps@sha256:1a6a219086627846d966e869a8d56fd78994fb747da91f49e6a46a674ef778c6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.5 MB (351462994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f4402f88a53734d262ec398d9da3786d89072972edfbbc52175a078d23b80d0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:40:29 GMT
ADD file:0b6fc66d778d0cd8ae8b17b92945d98cc34f9c7008cda864ed0a54b5e40b9cb0 in / 
# Wed, 11 Oct 2023 17:40:32 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:09:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:10:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:11:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:501a599c15b6def048b2e00cfdf6c658061c00a504305ef2075fb1009a62c1e2`  
		Last Modified: Wed, 11 Oct 2023 17:45:01 GMT  
		Size: 50.6 MB (50600791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf9d6abbf47f32cac71cefb6f7233e5f700d4f6f941ca631e29947c5f1df955`  
		Last Modified: Wed, 11 Oct 2023 18:21:57 GMT  
		Size: 24.9 MB (24887201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1693c4d42b110c48ad84138aa8c91e1aeffbed6ca630f12495f711b89609823`  
		Last Modified: Wed, 11 Oct 2023 18:22:27 GMT  
		Size: 66.0 MB (65984002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d61ba44e3cf60d5c6195ef4448de7160aff21051156b51d78755d19cb401055`  
		Last Modified: Wed, 11 Oct 2023 18:23:24 GMT  
		Size: 210.0 MB (209991000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:b585c2f0cfabe530c3905bb95c637eb6339c7663273b893ede5b4d8cacd9233b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.6 MB (325624324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01ae125d4ffa592dfd3716595bf2806c88e2b3b84e7cdc94482338771a440d1c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:48:50 GMT
ADD file:b081db8d48290ef5b5f477edb85d8f04d62a6995ec09bdb516d66dbe19b98137 in / 
# Wed, 11 Oct 2023 17:48:55 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:19:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:20:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:26:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:54dda4e4d31846b7324172a7fda3d0bdc7d8a2105ab27e9a92c2db43f35f9e5d`  
		Last Modified: Wed, 11 Oct 2023 17:59:53 GMT  
		Size: 49.6 MB (49569257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370a64ae3420fd85a23128ef46431df034f9038821764a14bb436272a1345505`  
		Last Modified: Wed, 11 Oct 2023 23:55:20 GMT  
		Size: 23.4 MB (23439567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c19b06553268b2cbcf576e075fdb1ac8c430154167258bcd4f925d5938117659`  
		Last Modified: Wed, 11 Oct 2023 23:56:13 GMT  
		Size: 63.0 MB (62962779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe7e7187a4f54c6c9e49f439f18fe1ae7a7f06894b24eae29001a71e03340c5`  
		Last Modified: Wed, 11 Oct 2023 23:58:22 GMT  
		Size: 189.7 MB (189652721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:12b9dc56603f357d0e68e2cd0927be121561f588bc3f728ed3a1fb3dc0ec9ded
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **363.0 MB (362953503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7467ffe1bf70430528cbbee8f716bd707ff747ee7ff42c2f77578884a1c214d6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:44:01 GMT
ADD file:ed515e1aef8321271c6544e30cbeb31257e9640979e8f68a9e490cb25d3525fd in / 
# Wed, 11 Oct 2023 17:44:04 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:14:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:15:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:19:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f137383853e717724a59e86aa526d31eabb4a5d45a259cd1ade68d93b3f45ae9`  
		Last Modified: Wed, 11 Oct 2023 17:49:27 GMT  
		Size: 53.6 MB (53575984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da754908592cac64ca75d9cdc8c43a4a396901108de4adae61bd92937de4f65`  
		Last Modified: Wed, 11 Oct 2023 18:36:14 GMT  
		Size: 25.7 MB (25700026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524b67dc97fb52dd33f61fe12da424874443bb200789c7cfde14425f85938f54`  
		Last Modified: Wed, 11 Oct 2023 18:36:46 GMT  
		Size: 69.6 MB (69584544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7449a547606da3836fd2405c85ed15e48ed96b7936fe9dfcbb8c69e21475738e`  
		Last Modified: Wed, 11 Oct 2023 18:37:46 GMT  
		Size: 214.1 MB (214092949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:eb83643215e451aa8409fe1fec979764362831916fa9a2955baa57c263d6631f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.2 MB (318222519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42abbfd998057c2e0c5d1c31d39f5a383b5ce7201d011ae9066f0214cd94321c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:50:07 GMT
ADD file:2dc117136732884ad4b058065700dd66cc49d6ce56b0fdbb672915e3ad8adb84 in / 
# Wed, 11 Oct 2023 17:50:10 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:51:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:52:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:58:19 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ad5e374600bf40a929dfe51e52737e4ca04aba83f499656760ba938841fb6552`  
		Last Modified: Wed, 11 Oct 2023 17:55:18 GMT  
		Size: 47.9 MB (47942934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6344f505670ce139b1b3f472749240f33304ec7535daae4a72913a6da08f304f`  
		Last Modified: Thu, 12 Oct 2023 00:33:20 GMT  
		Size: 24.0 MB (24046768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf2b4ce0798e7985dd88d10311ea2a2730812d4e10c9a8f24f564875c6cb617`  
		Last Modified: Thu, 12 Oct 2023 00:33:56 GMT  
		Size: 63.1 MB (63132898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317490e394e1c9331e54c7c33215628d4d08a8cd9d2191cb3d294d0b021a18f9`  
		Last Modified: Thu, 12 Oct 2023 00:34:47 GMT  
		Size: 183.1 MB (183099919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:lunar`

```console
$ docker pull buildpack-deps@sha256:5806596724fa79d84c05c5db171fffd0fb686ce26d6f100d2855b42263c2a739
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
$ docker pull buildpack-deps@sha256:09592b04b0e9b5345a66017fccd2bb575b714fe70d747239889e0abc5b2a581a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.6 MB (268609169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8be3606275e0541fe0c4a3d348ddaadbf8ade3013c418ae2816d332251ba288`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:18:17 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:18:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:18:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:18:18 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:18:19 GMT
ADD file:d4fca0b2b53fa4e2c3e0d721bf983f4095061c5df5fb084d2daf5efad5ee663d in / 
# Wed, 04 Oct 2023 12:18:19 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:19:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 07:20:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 07:24:17 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:850c6621501406ea0aac62d4ae7a001f98fe81b2085449034055ee7ff32622bc`  
		Last Modified: Thu, 05 Oct 2023 03:34:15 GMT  
		Size: 27.7 MB (27654268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c224a085b3b8f6169f29aeb01a19b302e9163e6122211234d56e34c49a1a52`  
		Last Modified: Fri, 13 Oct 2023 07:27:21 GMT  
		Size: 13.7 MB (13745429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415eed8af6d7f694df1de04bb6a2c5eba418319432d2dec5840be186c2df4971`  
		Last Modified: Fri, 13 Oct 2023 07:27:38 GMT  
		Size: 44.4 MB (44389510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed98248655b640aedb599378731535e0a729b6401f26d512f21872ae3f999a0`  
		Last Modified: Fri, 13 Oct 2023 07:28:10 GMT  
		Size: 182.8 MB (182819962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:d10e6715b29dbd0ef1f2ad8e5abf94556ec18422adecbd8bab056d3fc58649b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.4 MB (232441827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c5bfe8d3346fa65b2a65490f89c9d157d50669df53d95f446c6ee5fe8d1690f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:25:21 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:25:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:25:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:25:22 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:25:24 GMT
ADD file:b92305119eab5dd3dfb00f4d83cd84e00c8ae57143739329da5a19aeda55be4e in / 
# Wed, 04 Oct 2023 12:25:24 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 01:05:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 01:06:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 01:10:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0055151e5ef44f81f2355e8073f34f53cc16494749dbc5ba14445ce5edf3d3b6`  
		Last Modified: Fri, 13 Oct 2023 01:13:54 GMT  
		Size: 25.4 MB (25432981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e866c11041f7a46cb12551f8e93dea44f566d63d4fe5e9771fba148287d761c3`  
		Last Modified: Fri, 13 Oct 2023 01:13:51 GMT  
		Size: 12.7 MB (12665364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f378438bc51fcd6e34f3bded8ebdf10b2f56f47951e89908cd028fb60f9d763`  
		Last Modified: Fri, 13 Oct 2023 01:14:13 GMT  
		Size: 48.7 MB (48674522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a87bb08d55e31d0d5845bac5b3d441c3142141dd75d4c02bbf6b036fdc6be30`  
		Last Modified: Fri, 13 Oct 2023 01:14:48 GMT  
		Size: 145.7 MB (145668960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c1669c3bfc03aa349cc7266907fa3c34faeaaf68a9aa3bf7a888b0c4cb59b797
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.1 MB (258146485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:622129654f3cd970d2cb1ad360340c236ca504db8e4dca2544956acc6a1422e0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:23:52 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:23:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:23:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:23:52 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:23:53 GMT
ADD file:c9b1098bc90ac9b887c3bffdffbcff0c32f32e48df9a673041e3aa796296e69b in / 
# Wed, 04 Oct 2023 12:23:54 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 02:37:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 02:38:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 02:41:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6bd86e5a51fe562347e4392a584c2c048e2caf3c855ee2b39d193782482989d0`  
		Last Modified: Fri, 13 Oct 2023 02:45:03 GMT  
		Size: 27.0 MB (27009502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72b644e1b04fb1dbe3643839ab4b6c1c7562eed7fec98b56653bc7526d1f21b8`  
		Last Modified: Fri, 13 Oct 2023 02:45:00 GMT  
		Size: 13.3 MB (13334915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7195734b83041efa5c9550d35f558288d4c59268de32267217d78d00f7cd0dbb`  
		Last Modified: Fri, 13 Oct 2023 02:45:18 GMT  
		Size: 44.2 MB (44238877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73bddc9768e169e64876fcaec439a948c34e36801d337869e2bf980d6c6417a`  
		Last Modified: Fri, 13 Oct 2023 02:45:44 GMT  
		Size: 173.6 MB (173563191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:9186ee4cdc73cd802ff3ce577df5cf354c4b9a52f3afba18edc7725342d769fc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.0 MB (292973666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d17b3a7d6436dea3ef23bcf280cce6a1ed15621fe35c50663b8b5759e7a173c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:08:54 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:08:54 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:08:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:08:55 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:08:57 GMT
ADD file:24bc2f22a395e93a2ebbcfc45da8e5fc7f08e7c03cdc985c997300643d0310ec in / 
# Wed, 04 Oct 2023 12:08:58 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:12:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 07:13:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 07:20:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:56fffb9b8b31e93bce458c1b2532d4e3aabcfa346a00a948fa8702cf6e132f8c`  
		Last Modified: Fri, 13 Oct 2023 07:24:33 GMT  
		Size: 31.9 MB (31886447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a7a715c2447d71e6b94118f081111babef0331bd6104854da882370804c75ae`  
		Last Modified: Fri, 13 Oct 2023 07:24:30 GMT  
		Size: 15.8 MB (15842906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348f4703e93699e4c8ee248cbcc6f18ffaa75e71f9acb2b1a47c6a957a410e6f`  
		Last Modified: Fri, 13 Oct 2023 07:24:51 GMT  
		Size: 49.1 MB (49089842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c5ee703a39bc5a128280f48817e1157579759dcb313dcd3b0332f91493fb95`  
		Last Modified: Fri, 13 Oct 2023 07:25:31 GMT  
		Size: 196.2 MB (196154471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b03c2d5655663b83f6a221f35784d8902b4af4751413f0a874d38b81c25573ad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.2 MB (240157223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df5b35e4a07ed4da761b7644d6c49ad1a8694b981e74aaff067b260dec6c54a8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 04:29:27 GMT
ARG RELEASE
# Wed, 16 Aug 2023 04:29:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 04:29:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 04:29:28 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 16 Aug 2023 04:29:29 GMT
ADD file:14fcf0756fb29b609af54412c31e2ff9acbf4634984ce95bf204c67668706cb5 in / 
# Wed, 16 Aug 2023 04:29:30 GMT
CMD ["/bin/bash"]
# Fri, 01 Sep 2023 23:16:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Sep 2023 23:16:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 01 Sep 2023 23:19:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e9a6157a42893e6f99bd42ba05c70c5313add95c69f61f12e51517c0100470b8`  
		Last Modified: Fri, 01 Sep 2023 23:24:13 GMT  
		Size: 26.2 MB (26223925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f88ef015543162519d8e086a0bb86351d03f27b98218ff39b27f3b8b7bc2cd`  
		Last Modified: Fri, 01 Sep 2023 23:24:12 GMT  
		Size: 14.0 MB (14005753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ad80a5cffb7414f3bd06d5dafc212e2f5a767d3312bead7347e2ba8fae5be35`  
		Last Modified: Fri, 01 Sep 2023 23:24:25 GMT  
		Size: 44.3 MB (44275476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f495142834cd7cf92ea01d1b100c2b74a416627d5613eefc2c858d2b4c774d2`  
		Last Modified: Fri, 01 Sep 2023 23:24:50 GMT  
		Size: 155.7 MB (155652069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:lunar-curl`

```console
$ docker pull buildpack-deps@sha256:072cf6221243181993eae81700993113c3fc12fb299987448794840b33506bc9
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
$ docker pull buildpack-deps@sha256:95e60ea366f0d1dc0c10aedff8863857395287974e218b3f32b0b0d6e98cd7ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.4 MB (41399697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8dd67c3192123379e495aa231a49f40ef79982b7d68adc966bfa69e52eaa6d7a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:18:17 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:18:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:18:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:18:18 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:18:19 GMT
ADD file:d4fca0b2b53fa4e2c3e0d721bf983f4095061c5df5fb084d2daf5efad5ee663d in / 
# Wed, 04 Oct 2023 12:18:19 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:19:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:850c6621501406ea0aac62d4ae7a001f98fe81b2085449034055ee7ff32622bc`  
		Last Modified: Thu, 05 Oct 2023 03:34:15 GMT  
		Size: 27.7 MB (27654268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c224a085b3b8f6169f29aeb01a19b302e9163e6122211234d56e34c49a1a52`  
		Last Modified: Fri, 13 Oct 2023 07:27:21 GMT  
		Size: 13.7 MB (13745429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:0ecb3f2788bcf617a9998b5a24be6f6b2a219a05cdc5c8c0f7563ec4e19b4a80
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.1 MB (38098345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:899c18f362f26f3736d179227e6283f562d67fdba75be383e45008ab64e708ca`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:25:21 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:25:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:25:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:25:22 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:25:24 GMT
ADD file:b92305119eab5dd3dfb00f4d83cd84e00c8ae57143739329da5a19aeda55be4e in / 
# Wed, 04 Oct 2023 12:25:24 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 01:05:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0055151e5ef44f81f2355e8073f34f53cc16494749dbc5ba14445ce5edf3d3b6`  
		Last Modified: Fri, 13 Oct 2023 01:13:54 GMT  
		Size: 25.4 MB (25432981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e866c11041f7a46cb12551f8e93dea44f566d63d4fe5e9771fba148287d761c3`  
		Last Modified: Fri, 13 Oct 2023 01:13:51 GMT  
		Size: 12.7 MB (12665364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:e5d87a166e2dad42fa6f525819afb9a640aa0b82b6f7ebf0e5f12e4c65024611
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.3 MB (40344417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e540d2f701ab83d317c63b011be63e392958ad00cce31f3f5f0748db2e0dc8a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:23:52 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:23:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:23:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:23:52 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:23:53 GMT
ADD file:c9b1098bc90ac9b887c3bffdffbcff0c32f32e48df9a673041e3aa796296e69b in / 
# Wed, 04 Oct 2023 12:23:54 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 02:37:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6bd86e5a51fe562347e4392a584c2c048e2caf3c855ee2b39d193782482989d0`  
		Last Modified: Fri, 13 Oct 2023 02:45:03 GMT  
		Size: 27.0 MB (27009502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72b644e1b04fb1dbe3643839ab4b6c1c7562eed7fec98b56653bc7526d1f21b8`  
		Last Modified: Fri, 13 Oct 2023 02:45:00 GMT  
		Size: 13.3 MB (13334915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:72181d85a4df3861bb75602e574739cdd65450d9f1afa978fcecfb324ebf2b82
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.7 MB (47729353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19036cb074a72c8494d631b3bb45bb80bf7b2d181d374dc1c46b8f2bd02b65f0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:08:54 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:08:54 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:08:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:08:55 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:08:57 GMT
ADD file:24bc2f22a395e93a2ebbcfc45da8e5fc7f08e7c03cdc985c997300643d0310ec in / 
# Wed, 04 Oct 2023 12:08:58 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:12:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:56fffb9b8b31e93bce458c1b2532d4e3aabcfa346a00a948fa8702cf6e132f8c`  
		Last Modified: Fri, 13 Oct 2023 07:24:33 GMT  
		Size: 31.9 MB (31886447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a7a715c2447d71e6b94118f081111babef0331bd6104854da882370804c75ae`  
		Last Modified: Fri, 13 Oct 2023 07:24:30 GMT  
		Size: 15.8 MB (15842906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:3e2c1730f17419017837d5f1fc9db6ff833b9dc686ee7b21402e510119d4f4b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40229678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32608e7b5cf27557f6091473da05b6af8a046c450931620144b6162abe38dc78`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 04:29:27 GMT
ARG RELEASE
# Wed, 16 Aug 2023 04:29:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 04:29:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 04:29:28 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 16 Aug 2023 04:29:29 GMT
ADD file:14fcf0756fb29b609af54412c31e2ff9acbf4634984ce95bf204c67668706cb5 in / 
# Wed, 16 Aug 2023 04:29:30 GMT
CMD ["/bin/bash"]
# Fri, 01 Sep 2023 23:16:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e9a6157a42893e6f99bd42ba05c70c5313add95c69f61f12e51517c0100470b8`  
		Last Modified: Fri, 01 Sep 2023 23:24:13 GMT  
		Size: 26.2 MB (26223925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f88ef015543162519d8e086a0bb86351d03f27b98218ff39b27f3b8b7bc2cd`  
		Last Modified: Fri, 01 Sep 2023 23:24:12 GMT  
		Size: 14.0 MB (14005753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:lunar-scm`

```console
$ docker pull buildpack-deps@sha256:9337458ffb6dca2fc2ea67d3c7327ca71f1c6bc4f643d891eb96c8e2968ed8af
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
$ docker pull buildpack-deps@sha256:3476b6f371a5fad9ede92bb3dab111ba19697799847c89c67ffd675834f0a92f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.8 MB (85789207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c1c503d7baadb06f6ca79911e54f8a6167c4eaff6f2ac084de64e505ac9123b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:18:17 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:18:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:18:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:18:18 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:18:19 GMT
ADD file:d4fca0b2b53fa4e2c3e0d721bf983f4095061c5df5fb084d2daf5efad5ee663d in / 
# Wed, 04 Oct 2023 12:18:19 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:19:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 07:20:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:850c6621501406ea0aac62d4ae7a001f98fe81b2085449034055ee7ff32622bc`  
		Last Modified: Thu, 05 Oct 2023 03:34:15 GMT  
		Size: 27.7 MB (27654268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c224a085b3b8f6169f29aeb01a19b302e9163e6122211234d56e34c49a1a52`  
		Last Modified: Fri, 13 Oct 2023 07:27:21 GMT  
		Size: 13.7 MB (13745429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415eed8af6d7f694df1de04bb6a2c5eba418319432d2dec5840be186c2df4971`  
		Last Modified: Fri, 13 Oct 2023 07:27:38 GMT  
		Size: 44.4 MB (44389510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:bc6d4248879ec4a711aa75eade706ef957385237fc45fb1249be243bd0a209b6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.8 MB (86772867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4f5915541d7721f2aa036c93064ae10075f1523f13ff507a800b5d8096b1b82`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:25:21 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:25:21 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:25:21 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:25:22 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:25:24 GMT
ADD file:b92305119eab5dd3dfb00f4d83cd84e00c8ae57143739329da5a19aeda55be4e in / 
# Wed, 04 Oct 2023 12:25:24 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 01:05:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 01:06:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0055151e5ef44f81f2355e8073f34f53cc16494749dbc5ba14445ce5edf3d3b6`  
		Last Modified: Fri, 13 Oct 2023 01:13:54 GMT  
		Size: 25.4 MB (25432981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e866c11041f7a46cb12551f8e93dea44f566d63d4fe5e9771fba148287d761c3`  
		Last Modified: Fri, 13 Oct 2023 01:13:51 GMT  
		Size: 12.7 MB (12665364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f378438bc51fcd6e34f3bded8ebdf10b2f56f47951e89908cd028fb60f9d763`  
		Last Modified: Fri, 13 Oct 2023 01:14:13 GMT  
		Size: 48.7 MB (48674522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:5703efee751dc73306c869e77280610707d3d7eb398f10558f4a9f6c52538d3a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.6 MB (84583294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebbfa1bf84c209e495f93ba71668f19434f29ecca4eaabc251d7eba793fcafff`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:23:52 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:23:52 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:23:52 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:23:52 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:23:53 GMT
ADD file:c9b1098bc90ac9b887c3bffdffbcff0c32f32e48df9a673041e3aa796296e69b in / 
# Wed, 04 Oct 2023 12:23:54 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 02:37:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 02:38:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6bd86e5a51fe562347e4392a584c2c048e2caf3c855ee2b39d193782482989d0`  
		Last Modified: Fri, 13 Oct 2023 02:45:03 GMT  
		Size: 27.0 MB (27009502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72b644e1b04fb1dbe3643839ab4b6c1c7562eed7fec98b56653bc7526d1f21b8`  
		Last Modified: Fri, 13 Oct 2023 02:45:00 GMT  
		Size: 13.3 MB (13334915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7195734b83041efa5c9550d35f558288d4c59268de32267217d78d00f7cd0dbb`  
		Last Modified: Fri, 13 Oct 2023 02:45:18 GMT  
		Size: 44.2 MB (44238877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:52c33c87b291babb142f130127cb1470b7d82a6145d9aad084a78c88e4c80a2b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.8 MB (96819195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c6787c6550b1e4654d8c1b55c5d617b828335b2ba56fa69d00283241fbecbeb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:08:54 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:08:54 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:08:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:08:55 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:08:57 GMT
ADD file:24bc2f22a395e93a2ebbcfc45da8e5fc7f08e7c03cdc985c997300643d0310ec in / 
# Wed, 04 Oct 2023 12:08:58 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 07:12:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 07:13:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:56fffb9b8b31e93bce458c1b2532d4e3aabcfa346a00a948fa8702cf6e132f8c`  
		Last Modified: Fri, 13 Oct 2023 07:24:33 GMT  
		Size: 31.9 MB (31886447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a7a715c2447d71e6b94118f081111babef0331bd6104854da882370804c75ae`  
		Last Modified: Fri, 13 Oct 2023 07:24:30 GMT  
		Size: 15.8 MB (15842906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:348f4703e93699e4c8ee248cbcc6f18ffaa75e71f9acb2b1a47c6a957a410e6f`  
		Last Modified: Fri, 13 Oct 2023 07:24:51 GMT  
		Size: 49.1 MB (49089842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b2f2a0881286b29de742d50d48259b750a115827b358237c1669ced83f74796e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84505154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7decbe5c1b3961eed7d080573346ae9c054116dc044e81c734abe9ee131cc04d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 16 Aug 2023 04:29:27 GMT
ARG RELEASE
# Wed, 16 Aug 2023 04:29:28 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 16 Aug 2023 04:29:28 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 16 Aug 2023 04:29:28 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 16 Aug 2023 04:29:29 GMT
ADD file:14fcf0756fb29b609af54412c31e2ff9acbf4634984ce95bf204c67668706cb5 in / 
# Wed, 16 Aug 2023 04:29:30 GMT
CMD ["/bin/bash"]
# Fri, 01 Sep 2023 23:16:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Sep 2023 23:16:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e9a6157a42893e6f99bd42ba05c70c5313add95c69f61f12e51517c0100470b8`  
		Last Modified: Fri, 01 Sep 2023 23:24:13 GMT  
		Size: 26.2 MB (26223925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f88ef015543162519d8e086a0bb86351d03f27b98218ff39b27f3b8b7bc2cd`  
		Last Modified: Fri, 01 Sep 2023 23:24:12 GMT  
		Size: 14.0 MB (14005753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ad80a5cffb7414f3bd06d5dafc212e2f5a767d3312bead7347e2ba8fae5be35`  
		Last Modified: Fri, 01 Sep 2023 23:24:25 GMT  
		Size: 44.3 MB (44275476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:mantic`

```console
$ docker pull buildpack-deps@sha256:cce4098beee8d4c14a14de9efd05c187c5bc97bdb07a5fa2f4632bbdcf5cb278
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
$ docker pull buildpack-deps@sha256:1ffcc35dc1dfb9751e3339a92471844f54a1b2147c79b4e8a2f45a71137f768d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.1 MB (290073464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bad52367cc0f5c2f3115a8f96c1cb83c0c7bd5fb223d3ff41958867aceb72e3f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 05:03:43 GMT
ARG RELEASE
# Tue, 26 Sep 2023 05:03:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 05:03:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 05:03:43 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 05:03:45 GMT
ADD file:5fb49f260a0c3bf404c0fe31d8f0f812e9c143bd48223c4f15a85168758eb880 in / 
# Tue, 26 Sep 2023 05:03:45 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 05:02:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 05:03:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 05:07:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70c34fc37a9391a001a8d99c74b27823143398763bcd623c3402a790006947ea`  
		Last Modified: Tue, 03 Oct 2023 05:09:43 GMT  
		Size: 28.1 MB (28079281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13daebad235cc5fc75272df7a4cd22cd9e14040be8b10d9ec3764328c7be1ab`  
		Last Modified: Tue, 03 Oct 2023 05:09:41 GMT  
		Size: 13.9 MB (13886180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5024b0813f45b8c3c3d60316917bb453d13c81a8bab8316b17b30ac61156c6`  
		Last Modified: Tue, 03 Oct 2023 05:09:58 GMT  
		Size: 44.8 MB (44761138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd79646f814aefe34908af38903a3d5522c9455086876d9b84dda6633503c1d`  
		Last Modified: Tue, 03 Oct 2023 05:10:33 GMT  
		Size: 203.3 MB (203346865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:813769c747356c26587f8f75e5e91dc7dfba62b1610307b0c37b2e735245b43e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **255.4 MB (255352078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8caa1868f243e98eacc3ad77eb6a890dda6b40ba0b8ba30f275d201a970250a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 05:05:03 GMT
ARG RELEASE
# Tue, 26 Sep 2023 05:05:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 05:05:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 05:05:04 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 05:05:08 GMT
ADD file:512405a66f1049a7237c67d9d5776db7f41d5991eceec535260f4d3b7f19e65d in / 
# Tue, 26 Sep 2023 05:05:09 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 06:11:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 06:12:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 06:15:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70fb529e8caade31afb15a43cbaa98da4446d46bd64b25df10259be9a57f0577`  
		Last Modified: Tue, 03 Oct 2023 06:17:59 GMT  
		Size: 26.1 MB (26055984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7003bc3702b787e6176ad194751c3ba0ff76742ea89883d5b9e9bf4a15d93fb`  
		Last Modified: Tue, 03 Oct 2023 06:17:56 GMT  
		Size: 12.7 MB (12713461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fe360aefbe92efc04c5f077bc27baf1ae132ca6e543274ac4e2180efca7507c`  
		Last Modified: Tue, 03 Oct 2023 06:18:16 GMT  
		Size: 48.9 MB (48941849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdde41a257818412d92d75797a26ae9b4eaf5754d92345240d67cabdcba126ca`  
		Last Modified: Tue, 03 Oct 2023 06:18:47 GMT  
		Size: 167.6 MB (167640784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:14dcc77b25c7b3b5166ab0ef658f1c709bebc6b9b3392c1f144c50d51e7bc5c9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **281.4 MB (281404865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52326c95116b4ac6d7b8b8a2ee8e3143988a13531ba81915c44bb0a5f02256bd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 05:06:27 GMT
ARG RELEASE
# Tue, 26 Sep 2023 05:06:27 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 05:06:27 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 05:06:27 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 05:06:30 GMT
ADD file:0dbbd4de9483bc32897d525742b94aa13ebd3a6aac7f1844d94d7f4536b2bfb8 in / 
# Tue, 26 Sep 2023 05:06:30 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 06:17:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 06:18:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 06:21:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4259d3adacfee572bed7acadc8e4af2cf679658d229fc94eb25abeb6d662693a`  
		Last Modified: Tue, 03 Oct 2023 06:23:31 GMT  
		Size: 27.3 MB (27315811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56e515aa13e7ac1bba03883084849baef28268d175299a636c354b0e7558af88`  
		Last Modified: Tue, 03 Oct 2023 06:23:28 GMT  
		Size: 13.4 MB (13394041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a515dbb7fdd56d447a83b9c10d1e2ec2fb52e85daf470e09424283d14b5908`  
		Last Modified: Tue, 03 Oct 2023 06:23:44 GMT  
		Size: 44.6 MB (44631383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5870521b137c9f0e7e635cf3385f6c2f67138f6b1620432d51425b77ad10a08`  
		Last Modified: Tue, 03 Oct 2023 06:24:11 GMT  
		Size: 196.1 MB (196063630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:028eee089be0c465e58258e0093f5277d4e9702ca58ad77f89cedb2c7a8d928d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.0 MB (305008436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a55e4f421197c52b398250bfa25af66d31da985efcde6dbb6b44a2d40305f5b1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 04:52:53 GMT
ARG RELEASE
# Tue, 26 Sep 2023 04:52:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 04:52:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 04:52:54 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 04:52:56 GMT
ADD file:cbeb7f814c9eebdbdc6b8e10fb87ba8334b3f6203ceb166c48f6d7492ab07c4e in / 
# Tue, 26 Sep 2023 04:52:57 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 09:07:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 09:09:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 09:13:48 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:37af6e7cc6b51a4931dbbb51fab85a97161b0e873fc4984f882f48b10b6e52ff`  
		Last Modified: Tue, 03 Oct 2023 09:16:29 GMT  
		Size: 32.3 MB (32340811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5d9e5d675f5b5c56fe9add6cc8a5eb4e0a1d64fbd641984262d3d8e948b074`  
		Last Modified: Tue, 03 Oct 2023 09:16:25 GMT  
		Size: 15.9 MB (15938905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4b5786f2a975233c15614192b6873d23e3731274d109e63aa998b076d7a32f`  
		Last Modified: Tue, 03 Oct 2023 09:16:51 GMT  
		Size: 49.5 MB (49536647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db1518dc6279ec2984f0732cff49e7750b0230e674eb7e39fedd5e2ce7b0bf5b`  
		Last Modified: Tue, 03 Oct 2023 09:17:48 GMT  
		Size: 207.2 MB (207192073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:452d2d3a6dc77f07166211f76c6055b84c94b6f5e4a06de71349502bcf01ca3b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **267.5 MB (267507888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e250b3afe33fea9aae901344bb048b329f78d5e15ec826b414308684794425da`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 04:58:19 GMT
ARG RELEASE
# Tue, 26 Sep 2023 04:58:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 04:58:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 04:58:19 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 04:58:21 GMT
ADD file:e86e9b7546a97fa45e9c726cc317a624a7f94b0bd6dd413d89946ff778b18c77 in / 
# Tue, 26 Sep 2023 04:58:21 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 08:54:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 08:54:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 08:57:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:075a43ce09c6e3edbaa35c043b92a1f4c22b8237baa8de4238146e73630250f0`  
		Last Modified: Tue, 03 Oct 2023 09:01:27 GMT  
		Size: 27.6 MB (27623930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b703fa59fe447e054dd8349236278bd073fff635a41311e301569818f07b73b`  
		Last Modified: Tue, 03 Oct 2023 09:01:26 GMT  
		Size: 14.3 MB (14252775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37839377f33f6c3908cfc767a87a21aa81078a4c1959d18de0adab7d94a882d7`  
		Last Modified: Tue, 03 Oct 2023 09:01:50 GMT  
		Size: 45.2 MB (45206881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109a36ba84f6ccbc7952cf40798defc4982c663fa313314706cbfcd75ca2d128`  
		Last Modified: Tue, 03 Oct 2023 09:02:26 GMT  
		Size: 180.4 MB (180424302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:mantic-curl`

```console
$ docker pull buildpack-deps@sha256:f441a6eef343f7751e5dcfa035a98f6b5ccf3c885282d5ddf60c3ba41ed66ee4
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
$ docker pull buildpack-deps@sha256:8f1f81aef045cb4cb1dd04855313ecf0547e82d082914dfa6f5dc608b9f14c66
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (41965461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90765c24b416ae58d6e2266669124bc5049859b2fb076aa733c15a8e524e6e89`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 05:03:43 GMT
ARG RELEASE
# Tue, 26 Sep 2023 05:03:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 05:03:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 05:03:43 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 05:03:45 GMT
ADD file:5fb49f260a0c3bf404c0fe31d8f0f812e9c143bd48223c4f15a85168758eb880 in / 
# Tue, 26 Sep 2023 05:03:45 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 05:02:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70c34fc37a9391a001a8d99c74b27823143398763bcd623c3402a790006947ea`  
		Last Modified: Tue, 03 Oct 2023 05:09:43 GMT  
		Size: 28.1 MB (28079281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13daebad235cc5fc75272df7a4cd22cd9e14040be8b10d9ec3764328c7be1ab`  
		Last Modified: Tue, 03 Oct 2023 05:09:41 GMT  
		Size: 13.9 MB (13886180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:4f8231c37928bfd6d019f0a4da9fecebbfbe54a3f18b17227fd2da974dccf0e8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38769445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:154aa23af9f19fda735574c488545e91de641bc48dc5e6ccc05d7054dd6c1f27`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 05:05:03 GMT
ARG RELEASE
# Tue, 26 Sep 2023 05:05:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 05:05:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 05:05:04 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 05:05:08 GMT
ADD file:512405a66f1049a7237c67d9d5776db7f41d5991eceec535260f4d3b7f19e65d in / 
# Tue, 26 Sep 2023 05:05:09 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 06:11:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70fb529e8caade31afb15a43cbaa98da4446d46bd64b25df10259be9a57f0577`  
		Last Modified: Tue, 03 Oct 2023 06:17:59 GMT  
		Size: 26.1 MB (26055984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7003bc3702b787e6176ad194751c3ba0ff76742ea89883d5b9e9bf4a15d93fb`  
		Last Modified: Tue, 03 Oct 2023 06:17:56 GMT  
		Size: 12.7 MB (12713461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f01bdb766fa4849cb4f10a0809a8b5b498d4d0c97c7cc913302bfe7351c7e0ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.7 MB (40709852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72ffd9a6b28e4a8cb359ccf7d53e1f0df441ab57357eb6b0a53dacfcfedaea64`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 05:06:27 GMT
ARG RELEASE
# Tue, 26 Sep 2023 05:06:27 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 05:06:27 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 05:06:27 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 05:06:30 GMT
ADD file:0dbbd4de9483bc32897d525742b94aa13ebd3a6aac7f1844d94d7f4536b2bfb8 in / 
# Tue, 26 Sep 2023 05:06:30 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 06:17:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4259d3adacfee572bed7acadc8e4af2cf679658d229fc94eb25abeb6d662693a`  
		Last Modified: Tue, 03 Oct 2023 06:23:31 GMT  
		Size: 27.3 MB (27315811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56e515aa13e7ac1bba03883084849baef28268d175299a636c354b0e7558af88`  
		Last Modified: Tue, 03 Oct 2023 06:23:28 GMT  
		Size: 13.4 MB (13394041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:19c8a3b69e40dbebcc75a0a74eb2fccceef5f019bfb07e77681b55a65cd875d6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.3 MB (48279716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb0121e33449b2dd034ad8435b0fd1f59f3e7e5cfdd4f76ab3a8084e34474879`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 04:52:53 GMT
ARG RELEASE
# Tue, 26 Sep 2023 04:52:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 04:52:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 04:52:54 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 04:52:56 GMT
ADD file:cbeb7f814c9eebdbdc6b8e10fb87ba8334b3f6203ceb166c48f6d7492ab07c4e in / 
# Tue, 26 Sep 2023 04:52:57 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 09:07:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:37af6e7cc6b51a4931dbbb51fab85a97161b0e873fc4984f882f48b10b6e52ff`  
		Last Modified: Tue, 03 Oct 2023 09:16:29 GMT  
		Size: 32.3 MB (32340811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5d9e5d675f5b5c56fe9add6cc8a5eb4e0a1d64fbd641984262d3d8e948b074`  
		Last Modified: Tue, 03 Oct 2023 09:16:25 GMT  
		Size: 15.9 MB (15938905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:3c2543e24855f9466398d6b5283ed99d43c31e6eecb7c8a666fab77844e51f3b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.9 MB (41876705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98f6a5d197679893fff32c1e7e76ceb58cef5345e4214aa24c8a6b1c6e6ec05e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 04:58:19 GMT
ARG RELEASE
# Tue, 26 Sep 2023 04:58:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 04:58:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 04:58:19 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 04:58:21 GMT
ADD file:e86e9b7546a97fa45e9c726cc317a624a7f94b0bd6dd413d89946ff778b18c77 in / 
# Tue, 26 Sep 2023 04:58:21 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 08:54:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:075a43ce09c6e3edbaa35c043b92a1f4c22b8237baa8de4238146e73630250f0`  
		Last Modified: Tue, 03 Oct 2023 09:01:27 GMT  
		Size: 27.6 MB (27623930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b703fa59fe447e054dd8349236278bd073fff635a41311e301569818f07b73b`  
		Last Modified: Tue, 03 Oct 2023 09:01:26 GMT  
		Size: 14.3 MB (14252775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:mantic-scm`

```console
$ docker pull buildpack-deps@sha256:d77e951abdeb73a2dd14ba7bdff99b65cf8868b29fbd2c5bdbceb4ee0f503485
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
$ docker pull buildpack-deps@sha256:7154ee606209e01dfbdb5a98d17f4e66e941f7c1c80af9ba1f3c13303f684b38
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.7 MB (86726599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25d00e70f23db7ea7bb66c70316bc7fdc44a79fb1fd30b985055907d46d8dd27`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 05:03:43 GMT
ARG RELEASE
# Tue, 26 Sep 2023 05:03:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 05:03:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 05:03:43 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 05:03:45 GMT
ADD file:5fb49f260a0c3bf404c0fe31d8f0f812e9c143bd48223c4f15a85168758eb880 in / 
# Tue, 26 Sep 2023 05:03:45 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 05:02:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 05:03:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70c34fc37a9391a001a8d99c74b27823143398763bcd623c3402a790006947ea`  
		Last Modified: Tue, 03 Oct 2023 05:09:43 GMT  
		Size: 28.1 MB (28079281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13daebad235cc5fc75272df7a4cd22cd9e14040be8b10d9ec3764328c7be1ab`  
		Last Modified: Tue, 03 Oct 2023 05:09:41 GMT  
		Size: 13.9 MB (13886180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5024b0813f45b8c3c3d60316917bb453d13c81a8bab8316b17b30ac61156c6`  
		Last Modified: Tue, 03 Oct 2023 05:09:58 GMT  
		Size: 44.8 MB (44761138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:e198556ecbcc37ab2297352a3ff1845d949b22d85928d97229b1e457431319a4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.7 MB (87711294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09a6f4028f29d6923b5eb801f6947578178f8c808b23aa54095ed940196f8a28`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 05:05:03 GMT
ARG RELEASE
# Tue, 26 Sep 2023 05:05:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 05:05:04 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 05:05:04 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 05:05:08 GMT
ADD file:512405a66f1049a7237c67d9d5776db7f41d5991eceec535260f4d3b7f19e65d in / 
# Tue, 26 Sep 2023 05:05:09 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 06:11:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 06:12:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70fb529e8caade31afb15a43cbaa98da4446d46bd64b25df10259be9a57f0577`  
		Last Modified: Tue, 03 Oct 2023 06:17:59 GMT  
		Size: 26.1 MB (26055984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7003bc3702b787e6176ad194751c3ba0ff76742ea89883d5b9e9bf4a15d93fb`  
		Last Modified: Tue, 03 Oct 2023 06:17:56 GMT  
		Size: 12.7 MB (12713461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fe360aefbe92efc04c5f077bc27baf1ae132ca6e543274ac4e2180efca7507c`  
		Last Modified: Tue, 03 Oct 2023 06:18:16 GMT  
		Size: 48.9 MB (48941849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:b90f855ca6f36a58ffa93d51518b716154ce46f2501c052255a4ca69820f5f40
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.3 MB (85341235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1353821bcafbdc837c170ac7e68154a2784c2c9be1397d618829b032d0afd42a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 05:06:27 GMT
ARG RELEASE
# Tue, 26 Sep 2023 05:06:27 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 05:06:27 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 05:06:27 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 05:06:30 GMT
ADD file:0dbbd4de9483bc32897d525742b94aa13ebd3a6aac7f1844d94d7f4536b2bfb8 in / 
# Tue, 26 Sep 2023 05:06:30 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 06:17:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 06:18:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4259d3adacfee572bed7acadc8e4af2cf679658d229fc94eb25abeb6d662693a`  
		Last Modified: Tue, 03 Oct 2023 06:23:31 GMT  
		Size: 27.3 MB (27315811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56e515aa13e7ac1bba03883084849baef28268d175299a636c354b0e7558af88`  
		Last Modified: Tue, 03 Oct 2023 06:23:28 GMT  
		Size: 13.4 MB (13394041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a515dbb7fdd56d447a83b9c10d1e2ec2fb52e85daf470e09424283d14b5908`  
		Last Modified: Tue, 03 Oct 2023 06:23:44 GMT  
		Size: 44.6 MB (44631383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:acbd20745f2d3bf4eea92a5ae1ac2b8804313963facdce14255800f238f17712
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.8 MB (97816363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbfadc597734b0797716241519be9e98eea7bb25158e76398d42c3fb1d0366c3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 04:52:53 GMT
ARG RELEASE
# Tue, 26 Sep 2023 04:52:53 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 04:52:53 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 04:52:54 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 04:52:56 GMT
ADD file:cbeb7f814c9eebdbdc6b8e10fb87ba8334b3f6203ceb166c48f6d7492ab07c4e in / 
# Tue, 26 Sep 2023 04:52:57 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 09:07:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 09:09:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:37af6e7cc6b51a4931dbbb51fab85a97161b0e873fc4984f882f48b10b6e52ff`  
		Last Modified: Tue, 03 Oct 2023 09:16:29 GMT  
		Size: 32.3 MB (32340811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b5d9e5d675f5b5c56fe9add6cc8a5eb4e0a1d64fbd641984262d3d8e948b074`  
		Last Modified: Tue, 03 Oct 2023 09:16:25 GMT  
		Size: 15.9 MB (15938905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4b5786f2a975233c15614192b6873d23e3731274d109e63aa998b076d7a32f`  
		Last Modified: Tue, 03 Oct 2023 09:16:51 GMT  
		Size: 49.5 MB (49536647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:7ba205206c01993460abc949cb42dd5a14f530a2a21cdd5b3c733d628d0d3546
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.1 MB (87083586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a73fb50f78e1bb0c4a8281876e5d8202f69f3bd80ec2901e296e2a620b18304`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 04:58:19 GMT
ARG RELEASE
# Tue, 26 Sep 2023 04:58:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 04:58:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 04:58:19 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 04:58:21 GMT
ADD file:e86e9b7546a97fa45e9c726cc317a624a7f94b0bd6dd413d89946ff778b18c77 in / 
# Tue, 26 Sep 2023 04:58:21 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 08:54:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 08:54:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:075a43ce09c6e3edbaa35c043b92a1f4c22b8237baa8de4238146e73630250f0`  
		Last Modified: Tue, 03 Oct 2023 09:01:27 GMT  
		Size: 27.6 MB (27623930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b703fa59fe447e054dd8349236278bd073fff635a41311e301569818f07b73b`  
		Last Modified: Tue, 03 Oct 2023 09:01:26 GMT  
		Size: 14.3 MB (14252775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37839377f33f6c3908cfc767a87a21aa81078a4c1959d18de0adab7d94a882d7`  
		Last Modified: Tue, 03 Oct 2023 09:01:50 GMT  
		Size: 45.2 MB (45206881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldoldstable`

```console
$ docker pull buildpack-deps@sha256:82e25c1dea159632964a4c576380aa6ae9fd1d28c42b1f967d5474167ee4f6a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:oldoldstable` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:3cce8b99c877ede9a61de5d6c26b7812ff14240940a8d5b022acee4ecbe4407b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.9 MB (311864851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:812562bb54bb3b4a8d34fffe7cb7523e1d58d69c7e6f3f31ca19c5e280e54922`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:23 GMT
ADD file:1efe9845e057e7029a1c2c26c148e6dc1bd9c65d0cbbb23cb49c86295d1f1f48 in / 
# Wed, 11 Oct 2023 18:35:23 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:22:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:22:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:24:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99db33be616a9a2a0b0b1bc913b548317bab7bd11cb6968d357457e201c44077`  
		Last Modified: Wed, 11 Oct 2023 18:40:37 GMT  
		Size: 50.5 MB (50499400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4df9fde773e0c195208a941f5c813fcae5310dfa340b1092a91ca3dca2f0997`  
		Last Modified: Thu, 12 Oct 2023 03:30:53 GMT  
		Size: 17.6 MB (17580739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47c0008f57ffcdd8594227fc498eec4c4660fd627978baa26cf04a9a18908391`  
		Last Modified: Thu, 12 Oct 2023 03:31:09 GMT  
		Size: 51.9 MB (51874135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:640e2c66b8c0a79112068e7e0c50721ca969cdf94a73740fabd8230930e835ae`  
		Last Modified: Thu, 12 Oct 2023 03:31:41 GMT  
		Size: 191.9 MB (191910577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:17038db490bbb33ff709999f26a89753069ad0d2b167e56adf06474c2f8b9512
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.7 MB (277692858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02bb7e9c592bddbb15c614d9057cb8a1518aee94b14b7a7f746972df6779d573`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:37 GMT
ADD file:90492dd68d097af40a6208353165e1b7e2bc04a31cd2270232e085416f6e940e in / 
# Wed, 11 Oct 2023 17:42:38 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:48:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:49:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:50:19 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2ecd2705b9dde659b853da74fbe8d7227d02acd96f1d34766d44193b82468b37`  
		Last Modified: Wed, 11 Oct 2023 17:47:27 GMT  
		Size: 46.0 MB (45966353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2548d6bcf8bfe2322ed1ed9f56eeab4afd1b65e4c4a62d0be4d602f14dafc992`  
		Last Modified: Thu, 12 Oct 2023 03:58:22 GMT  
		Size: 16.2 MB (16213670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:423a7661d20a90498af23198b35b85c16af055a76453a7e8392ce97b5f4e398c`  
		Last Modified: Thu, 12 Oct 2023 03:58:40 GMT  
		Size: 47.4 MB (47410916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aa54b7711ac968a604b4e2ef193e8298d78d435fd3241931a711bc5ccce47e1`  
		Last Modified: Thu, 12 Oct 2023 03:59:13 GMT  
		Size: 168.1 MB (168101919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f8e53ff95899f67abb3aa35ec671c43f119ca559ee8b0e519a0ece7cfe03c0fc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.4 MB (302434057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ab5f1e32878a2fe74760a4cb35219c1d3828050ae2f605403539b5a27473351`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:12 GMT
ADD file:d97d8c89883987c89b2150923abea982086030e71970f5473a534e95252b4972 in / 
# Wed, 11 Oct 2023 18:25:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:47:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:48:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:49:16 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6a7acee270b8289bdc6bb8836f1a4899f794d60337a0cdc46b58a717bd27ba89`  
		Last Modified: Wed, 11 Oct 2023 18:29:25 GMT  
		Size: 49.3 MB (49291086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d43a8471c221305b41e4a48fe1a36d8d976208b182f048b98aa6dc81e6fec8`  
		Last Modified: Wed, 11 Oct 2023 19:55:54 GMT  
		Size: 17.5 MB (17451818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a82d27a09b100de4594fbc9e341ab946a39a8d635f12e633b1341a1c7aaa4b`  
		Last Modified: Wed, 11 Oct 2023 19:56:09 GMT  
		Size: 52.2 MB (52208642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb224d9b0fd6283df35335f4979c2c54bdc5609ca8473220d5d9924a91a0e11`  
		Last Modified: Wed, 11 Oct 2023 19:56:34 GMT  
		Size: 183.5 MB (183482511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:e2ca1129326f210b765c3fc489de34d0c965072bdb15a62cf1b72ab756fa27b3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.3 MB (321272799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:138b172705b3f04788d90ae5fdf81f014877dfb0f9d4e808fba131bc14519f3d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:41:14 GMT
ADD file:47cece2eff96bf7383dd2a9c5632f0ad7bb31b3a459677530f77a78e22658e98 in / 
# Wed, 11 Oct 2023 17:41:14 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:14:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:14:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:16:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:62bc68699d611f4c048328a0468ebc10de528260c7823c8938796da30db31a17`  
		Last Modified: Wed, 11 Oct 2023 17:46:45 GMT  
		Size: 51.3 MB (51256071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a664405fd519ae385ebac7659c355b2c380dd5c84037f38e6d3673b2bd9795c5`  
		Last Modified: Wed, 11 Oct 2023 18:25:03 GMT  
		Size: 18.1 MB (18097310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c138636d1c51e715c73bdb28e49fb18fc2d82cca0a21d5641a911f48cd3ff695`  
		Last Modified: Wed, 11 Oct 2023 18:25:25 GMT  
		Size: 53.5 MB (53487954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31fb7080416fbc4aee5e058de75799128cbeb8d55130f29854b8e5d7666fca0c`  
		Last Modified: Wed, 11 Oct 2023 18:26:09 GMT  
		Size: 198.4 MB (198431464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldoldstable-curl`

```console
$ docker pull buildpack-deps@sha256:d8e623f145ced0b674077746d2384f6e7f4adc64f84389a951e9acccf7a2ca40
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:oldoldstable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:fb59272c01f331c27bbf043917330de01941dbf342ed54f26343cb9ac8d31b13
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68080139 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf521dae41c7d61f7dc44e641032d2e238a024f227c62d1e5fe1a5c4889449ad`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:23 GMT
ADD file:1efe9845e057e7029a1c2c26c148e6dc1bd9c65d0cbbb23cb49c86295d1f1f48 in / 
# Wed, 11 Oct 2023 18:35:23 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:22:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99db33be616a9a2a0b0b1bc913b548317bab7bd11cb6968d357457e201c44077`  
		Last Modified: Wed, 11 Oct 2023 18:40:37 GMT  
		Size: 50.5 MB (50499400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4df9fde773e0c195208a941f5c813fcae5310dfa340b1092a91ca3dca2f0997`  
		Last Modified: Thu, 12 Oct 2023 03:30:53 GMT  
		Size: 17.6 MB (17580739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:d480bc746f923acad671d7592a0318d59b3d00cff454e730e20b9e915a3e4752
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62180023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0eca085d0fa4d2ab3f440a605762d5eab83321b1edfb729fab09fc20f6bdea5c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:37 GMT
ADD file:90492dd68d097af40a6208353165e1b7e2bc04a31cd2270232e085416f6e940e in / 
# Wed, 11 Oct 2023 17:42:38 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:48:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2ecd2705b9dde659b853da74fbe8d7227d02acd96f1d34766d44193b82468b37`  
		Last Modified: Wed, 11 Oct 2023 17:47:27 GMT  
		Size: 46.0 MB (45966353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2548d6bcf8bfe2322ed1ed9f56eeab4afd1b65e4c4a62d0be4d602f14dafc992`  
		Last Modified: Thu, 12 Oct 2023 03:58:22 GMT  
		Size: 16.2 MB (16213670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f93b04aec507910fbaa9a45dcff734fa880323618be3ee146dc70f885a285af1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66742904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c330d4af463f1493cf1f188470d0d1445f9d11bf3ace6545f44b18cf2f1f8d5e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:12 GMT
ADD file:d97d8c89883987c89b2150923abea982086030e71970f5473a534e95252b4972 in / 
# Wed, 11 Oct 2023 18:25:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:47:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6a7acee270b8289bdc6bb8836f1a4899f794d60337a0cdc46b58a717bd27ba89`  
		Last Modified: Wed, 11 Oct 2023 18:29:25 GMT  
		Size: 49.3 MB (49291086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d43a8471c221305b41e4a48fe1a36d8d976208b182f048b98aa6dc81e6fec8`  
		Last Modified: Wed, 11 Oct 2023 19:55:54 GMT  
		Size: 17.5 MB (17451818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:32c7184a162ee94fdac9984a9cef58f1bcf15f4c0a1acd21082769162bd02990
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.4 MB (69353381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:885698803969612184270761585a946f4b430a1383c328ab4924a3f6c7f6a410`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:41:14 GMT
ADD file:47cece2eff96bf7383dd2a9c5632f0ad7bb31b3a459677530f77a78e22658e98 in / 
# Wed, 11 Oct 2023 17:41:14 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:14:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:62bc68699d611f4c048328a0468ebc10de528260c7823c8938796da30db31a17`  
		Last Modified: Wed, 11 Oct 2023 17:46:45 GMT  
		Size: 51.3 MB (51256071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a664405fd519ae385ebac7659c355b2c380dd5c84037f38e6d3673b2bd9795c5`  
		Last Modified: Wed, 11 Oct 2023 18:25:03 GMT  
		Size: 18.1 MB (18097310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldoldstable-scm`

```console
$ docker pull buildpack-deps@sha256:2437a1e2cad84091b2e8393d0a736af68e46f377f6c499327516e4815feea613
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:oldoldstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:00b0f3aca41e1135dc391f626f66f5b6a086ee260c995f37805f27164957691d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.0 MB (119954274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06dd589d27b2d2d0733d458cb149600accc2ea5f8f818c903bddb738204c8426`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:23 GMT
ADD file:1efe9845e057e7029a1c2c26c148e6dc1bd9c65d0cbbb23cb49c86295d1f1f48 in / 
# Wed, 11 Oct 2023 18:35:23 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:22:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:22:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:99db33be616a9a2a0b0b1bc913b548317bab7bd11cb6968d357457e201c44077`  
		Last Modified: Wed, 11 Oct 2023 18:40:37 GMT  
		Size: 50.5 MB (50499400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4df9fde773e0c195208a941f5c813fcae5310dfa340b1092a91ca3dca2f0997`  
		Last Modified: Thu, 12 Oct 2023 03:30:53 GMT  
		Size: 17.6 MB (17580739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47c0008f57ffcdd8594227fc498eec4c4660fd627978baa26cf04a9a18908391`  
		Last Modified: Thu, 12 Oct 2023 03:31:09 GMT  
		Size: 51.9 MB (51874135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:23fa82b6ce62d4459c91ba9cd6a119c8132666e0e84b1bccdbc46652fdd4fa8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109590939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:419a7b84b078554b5177dd14ef6a12e1a6696df651c438b2bcf3f8761077497c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:37 GMT
ADD file:90492dd68d097af40a6208353165e1b7e2bc04a31cd2270232e085416f6e940e in / 
# Wed, 11 Oct 2023 17:42:38 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:48:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:49:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2ecd2705b9dde659b853da74fbe8d7227d02acd96f1d34766d44193b82468b37`  
		Last Modified: Wed, 11 Oct 2023 17:47:27 GMT  
		Size: 46.0 MB (45966353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2548d6bcf8bfe2322ed1ed9f56eeab4afd1b65e4c4a62d0be4d602f14dafc992`  
		Last Modified: Thu, 12 Oct 2023 03:58:22 GMT  
		Size: 16.2 MB (16213670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:423a7661d20a90498af23198b35b85c16af055a76453a7e8392ce97b5f4e398c`  
		Last Modified: Thu, 12 Oct 2023 03:58:40 GMT  
		Size: 47.4 MB (47410916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:142a54e609ce722402983f6daa77ee12ec5baf50a191b64ef7f9a4c85262597c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.0 MB (118951546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b138e1d073c5b16678192fbfb7949d838e13e95902b21affb91b17aed7e9f89`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:12 GMT
ADD file:d97d8c89883987c89b2150923abea982086030e71970f5473a534e95252b4972 in / 
# Wed, 11 Oct 2023 18:25:13 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:47:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:48:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6a7acee270b8289bdc6bb8836f1a4899f794d60337a0cdc46b58a717bd27ba89`  
		Last Modified: Wed, 11 Oct 2023 18:29:25 GMT  
		Size: 49.3 MB (49291086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d43a8471c221305b41e4a48fe1a36d8d976208b182f048b98aa6dc81e6fec8`  
		Last Modified: Wed, 11 Oct 2023 19:55:54 GMT  
		Size: 17.5 MB (17451818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a82d27a09b100de4594fbc9e341ab946a39a8d635f12e633b1341a1c7aaa4b`  
		Last Modified: Wed, 11 Oct 2023 19:56:09 GMT  
		Size: 52.2 MB (52208642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:b9714a557ba551d0e25530e69b9c38752fec848204c2e0791697c79dacbd1d67
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.8 MB (122841335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ce745aed3b333b25b3e5c0db30d1014e3561c2f1044192ec0991f69bb7cecf8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:41:14 GMT
ADD file:47cece2eff96bf7383dd2a9c5632f0ad7bb31b3a459677530f77a78e22658e98 in / 
# Wed, 11 Oct 2023 17:41:14 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:14:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:14:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:62bc68699d611f4c048328a0468ebc10de528260c7823c8938796da30db31a17`  
		Last Modified: Wed, 11 Oct 2023 17:46:45 GMT  
		Size: 51.3 MB (51256071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a664405fd519ae385ebac7659c355b2c380dd5c84037f38e6d3673b2bd9795c5`  
		Last Modified: Wed, 11 Oct 2023 18:25:03 GMT  
		Size: 18.1 MB (18097310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c138636d1c51e715c73bdb28e49fb18fc2d82cca0a21d5641a911f48cd3ff695`  
		Last Modified: Wed, 11 Oct 2023 18:25:25 GMT  
		Size: 53.5 MB (53487954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldstable`

```console
$ docker pull buildpack-deps@sha256:e5587c367e13ef9c01dede7c4085056a65e24caa7257a53c303c6c074fe6034e
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
$ docker pull buildpack-deps@sha256:bb08d7e7738400cf38ca527441821b7215d53edb756a895846f813ea1638f1b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.3 MB (322297429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bd9f475bf39e63db0ab9a574f52a6174c3a1d300c551ce995495ff132286ab2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:01 GMT
ADD file:8a9222387b89a9ac763fd72610ce01ab17f64387cbfde30a6af1861a82030aad in / 
# Wed, 11 Oct 2023 18:35:01 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:20:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:21:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:22:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:69b3efbf67c2d9a46fdfdc8480b5a03ef73e9999a53aad57213447784f01eb6e`  
		Last Modified: Wed, 11 Oct 2023 18:39:54 GMT  
		Size: 55.1 MB (55058028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dedceb9c21c46986231d9dfb896b37cfc470d67799e7e919a641ac54dcc9eed`  
		Last Modified: Thu, 12 Oct 2023 03:29:53 GMT  
		Size: 15.8 MB (15764226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98dfe1ecd6ba8d7f42ee14ec8a64da6ba633ed96ac9c58f6c5a0028ce6908916`  
		Last Modified: Thu, 12 Oct 2023 03:30:09 GMT  
		Size: 54.6 MB (54595813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d198e46b4004b646fce783c4378d6841632c0fb7fb2360927673d788abfda172`  
		Last Modified: Thu, 12 Oct 2023 03:30:42 GMT  
		Size: 196.9 MB (196879362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:04535164c424cb704b73bb1a19096a7e575863c4dbc9adb873d833e366628ccd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.4 MB (295372008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a5f995269b01b9f80a154b38cb65347aa8df4e33c664107279723056ea8c8e9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:37:51 GMT
ADD file:dd011733a11e4681328b2d45bbfc478e1dab88a95554fe817e238ef27b1865c2 in / 
# Wed, 11 Oct 2023 17:37:51 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:06:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:07:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:08:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d310e2405531cf391481a06c9f4d0fc75165ad8e3025e4035c6be5245b6cc754`  
		Last Modified: Wed, 11 Oct 2023 17:41:07 GMT  
		Size: 52.6 MB (52563098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c07441895e6cb16dc8222813db91b971828ec10cafdde9634c13ad69f7723b`  
		Last Modified: Wed, 11 Oct 2023 18:15:51 GMT  
		Size: 15.4 MB (15374683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36086464e7a231c171f28068f405baccff6fe849ecc79fba7ed52c6ebfdba6f9`  
		Last Modified: Wed, 11 Oct 2023 18:16:08 GMT  
		Size: 52.3 MB (52331039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcfedfb2a62724677848265f66d1519ef423f3440998f0a2ce6a01dc498f2b22`  
		Last Modified: Wed, 11 Oct 2023 18:16:43 GMT  
		Size: 175.1 MB (175103188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:e4e482d959b44f9fe93c58da44f823f57a6c75f8f1ac90b76f88d71420aae7a9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.8 MB (282800401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5067c84592299d066e5e61cdeca7db4d8ddd0cfd8d1012de6c767b147e0af26`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:19 GMT
ADD file:684f3634c6b747a4caad8f9f820cc02b53a2122591fe215935c5497ec234c3ad in / 
# Wed, 11 Oct 2023 17:42:20 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:47:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:47:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:48:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:33d0c7672db93e653471872c639cd6129ec25c168942e15a008c4920cafe62d7`  
		Last Modified: Wed, 11 Oct 2023 17:46:42 GMT  
		Size: 50.2 MB (50215704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe33e05af9470f2356c8047560fded363dda4990bb2d70e9194f0dca496bb82`  
		Last Modified: Thu, 12 Oct 2023 03:57:11 GMT  
		Size: 14.9 MB (14879720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0953bb94dc6fcb1dee741e8bfc886a0671f4516a04fbf1a92527c2bb1598e1dd`  
		Last Modified: Thu, 12 Oct 2023 03:57:33 GMT  
		Size: 50.4 MB (50353136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783a8cf6b572fdf6838ef5ecf60b5713b7139f7f8e554b1ccd61d56a597e3cf7`  
		Last Modified: Thu, 12 Oct 2023 03:58:11 GMT  
		Size: 167.4 MB (167351841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:00ffaa1775df7aa605c2ced1697ead01a9b21693aae4289cfe39e23f12001037
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.0 MB (313959291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62c1e77e85cc31b53ae5fb1cf23802ccb5e6e8394bc753361cf259672e530e5b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:58 GMT
ADD file:e1a6c6c976e5e7c53eb2a7343a7a763b46e56828588535f4c79e63d6ec08198d in / 
# Wed, 11 Oct 2023 18:24:58 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:46:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:46:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:47:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dd0dc10f921f4b3b65b17f20d367374079e6cb4e26531624ee64caaaf4adcc28`  
		Last Modified: Wed, 11 Oct 2023 18:28:45 GMT  
		Size: 53.7 MB (53707810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7a630df11a812111dd2b7f5b819a692f2350ad055fab0cd3e60b322c2eead5`  
		Last Modified: Wed, 11 Oct 2023 19:54:57 GMT  
		Size: 15.7 MB (15749899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9c8e3bce435b9fb78d2fd6a8f0ce18ddecff51902c10074a9da4287cb35963b`  
		Last Modified: Wed, 11 Oct 2023 19:55:14 GMT  
		Size: 54.7 MB (54700074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda70d4f1c4310da8eb56a83b481a5bda9d57efa32a6ef6d7915a7cf487c8ba6`  
		Last Modified: Wed, 11 Oct 2023 19:55:43 GMT  
		Size: 189.8 MB (189801508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:027c2ac7b7fa9f7c2154a9a29054feac38fc193959a31cf73c35f363d04ef38a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.0 MB (328045308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:384002c0f12bf18ca0f3797b1f0a18d7a84a7ed8720b3688b2b735b291d8ce4e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:40:52 GMT
ADD file:a3c1e94bb116d940a614a5275c69bacbac46e00da2070b5c7a561e64b975acc6 in / 
# Wed, 11 Oct 2023 17:40:53 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:12:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:13:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:081c634ff059d5636b4292d84d0b49429030b3dca70ca56828543b295adb9d47`  
		Last Modified: Wed, 11 Oct 2023 17:45:55 GMT  
		Size: 56.0 MB (56046358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c55d0c1747845e146fb76750b201af94d841ddeee081fcbdefcc5353c17f2e`  
		Last Modified: Wed, 11 Oct 2023 18:23:38 GMT  
		Size: 16.3 MB (16268212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:049e1171db56ce9d453ea26b1abcc12e301ef98dda47be8250cb0ced74ec097a`  
		Last Modified: Wed, 11 Oct 2023 18:24:01 GMT  
		Size: 55.9 MB (55936762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e77fa153db9b2a24390633ef303b38a33f84bbe4d12c7490cfcc8e12554868d`  
		Last Modified: Wed, 11 Oct 2023 18:24:50 GMT  
		Size: 199.8 MB (199793976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:e5f03b8a3612aa16737fb4f085988cd8bba30d0a048cb95c65b85fedf27c9418
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.1 MB (301123558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f13213c1ead0656fc3dcddc0a9823684c244f11c9e87c31973becaccd971048`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:50:06 GMT
ADD file:c4be7fca661f2a8181ee1e05fda057c18a2d7c1ae0e08ab63b2c5567ef9cc0a7 in / 
# Wed, 11 Oct 2023 17:50:12 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:27:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:29:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:34:59 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d237f50a9f05adf465246bef37e194e1d7a226224c7f90ae7b55925c5b509d15`  
		Last Modified: Wed, 11 Oct 2023 18:01:27 GMT  
		Size: 53.3 MB (53289043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a8381daee3205699bef24f6e7ee0bd6b3621924baae8f1b0b0026007cfe3b4`  
		Last Modified: Wed, 11 Oct 2023 23:58:42 GMT  
		Size: 15.5 MB (15529612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9e6da5ca3b34590abe253ac60b2000d9724ff3d9572311ded53ba9d66e58de`  
		Last Modified: Wed, 11 Oct 2023 23:59:27 GMT  
		Size: 53.3 MB (53302304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2632af27ef8e60c2473640fa869c1560b9bc160073d3db4db8c120329ad58ba3`  
		Last Modified: Thu, 12 Oct 2023 00:01:26 GMT  
		Size: 179.0 MB (179002599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:958d63f118f9541a5d8261b37e6ea3047bb2c96deb9af2464690bec55b58dcbb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.8 MB (330810785 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1f7cd93d79e43a628cbf38352b5a20938139f8968c227d5a0b718d6b34fc765`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:44:35 GMT
ADD file:d59326770edede2ba1d2005697bf41540a3d76a4bae883b91fede9b68018630c in / 
# Wed, 11 Oct 2023 17:44:38 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:20:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:21:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:24:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6613fa9f09034273d2b35a47386f8d53c77953a73e561b9f189ffa43ea17bd54`  
		Last Modified: Wed, 11 Oct 2023 17:50:25 GMT  
		Size: 58.9 MB (58929717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565fd5d2ec4119e0cef3217e4496512c36e4adc4e98567f565f105e684e80c4e`  
		Last Modified: Wed, 11 Oct 2023 18:38:00 GMT  
		Size: 16.8 MB (16765485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac6ae11620e817afc07c304ae67f21276148cc99a42e4ac56d481faceb27146`  
		Last Modified: Wed, 11 Oct 2023 18:38:24 GMT  
		Size: 58.9 MB (58866926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e868ed372aa88cb7b1880038e68bff4def65e8692014745f7a779d67797a8527`  
		Last Modified: Wed, 11 Oct 2023 18:39:18 GMT  
		Size: 196.2 MB (196248657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:c508b62b26cf4c3e78a3a679727268f9c89cf031809913639114575bed3387f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.9 MB (295893977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2030b0af1fd8ca97341a629b714304bddce2ff9594cb68f4483fdcccafced6d4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:50:40 GMT
ADD file:bb3ee20a7ddf364b23163c517132146872491e85ef2f1465bf7fd2ed33f94827 in / 
# Wed, 11 Oct 2023 17:50:44 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:58:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:59:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 00:03:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e651436ffb848f56da62cd2c80f206a288b94da8113c4c23a7e5502fb597ce23`  
		Last Modified: Wed, 11 Oct 2023 17:56:38 GMT  
		Size: 53.3 MB (53296378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a52fe3127c9c85c0c5e50b52a035e6bcee230e0c38db795abfee4b60522f157`  
		Last Modified: Thu, 12 Oct 2023 00:35:16 GMT  
		Size: 15.6 MB (15640232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58e9fa5eede43b49ed76d5e09e5c978ac8b2296773dad3161eae081bba447e45`  
		Last Modified: Thu, 12 Oct 2023 00:35:44 GMT  
		Size: 54.1 MB (54066239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d404a1f00add5fb24f6224adfac012cf688caba0fb9eb52c82c499b84498b414`  
		Last Modified: Thu, 12 Oct 2023 00:36:17 GMT  
		Size: 172.9 MB (172891128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldstable-curl`

```console
$ docker pull buildpack-deps@sha256:a1cf2b85c16ce2dcef6d5b5e603d6dcc208287ba0c02cb856e117837b3dbd700
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
$ docker pull buildpack-deps@sha256:ee1320245c18c32018ab7c9b5930a007c1cdd617ef894def34d8b9a97edfed2e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.8 MB (70822254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9144300bda2ab6cd167ac7386e562115d65c96297fbf92f5bf92e98784a5b25`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:01 GMT
ADD file:8a9222387b89a9ac763fd72610ce01ab17f64387cbfde30a6af1861a82030aad in / 
# Wed, 11 Oct 2023 18:35:01 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:20:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:69b3efbf67c2d9a46fdfdc8480b5a03ef73e9999a53aad57213447784f01eb6e`  
		Last Modified: Wed, 11 Oct 2023 18:39:54 GMT  
		Size: 55.1 MB (55058028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dedceb9c21c46986231d9dfb896b37cfc470d67799e7e919a641ac54dcc9eed`  
		Last Modified: Thu, 12 Oct 2023 03:29:53 GMT  
		Size: 15.8 MB (15764226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:370bfb2b7dc382e63da82b4ba78d9717baf16f82f20e7c43723e804e0b344a4a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.9 MB (67937781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0979f1da4edd11481372e6d0be81bd79af79fc236117439dceddbef0c454bc8b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:37:51 GMT
ADD file:dd011733a11e4681328b2d45bbfc478e1dab88a95554fe817e238ef27b1865c2 in / 
# Wed, 11 Oct 2023 17:37:51 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:06:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d310e2405531cf391481a06c9f4d0fc75165ad8e3025e4035c6be5245b6cc754`  
		Last Modified: Wed, 11 Oct 2023 17:41:07 GMT  
		Size: 52.6 MB (52563098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c07441895e6cb16dc8222813db91b971828ec10cafdde9634c13ad69f7723b`  
		Last Modified: Wed, 11 Oct 2023 18:15:51 GMT  
		Size: 15.4 MB (15374683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:84e96a20434a3a6eb8d0a4e7237e11ad8d690fc89f01d5c16f68f9ceb0e55758
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.1 MB (65095424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56fe78d093f425564326f7db7157a9c30ececd23a260999492e51a77ef946ab6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:19 GMT
ADD file:684f3634c6b747a4caad8f9f820cc02b53a2122591fe215935c5497ec234c3ad in / 
# Wed, 11 Oct 2023 17:42:20 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:47:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:33d0c7672db93e653471872c639cd6129ec25c168942e15a008c4920cafe62d7`  
		Last Modified: Wed, 11 Oct 2023 17:46:42 GMT  
		Size: 50.2 MB (50215704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe33e05af9470f2356c8047560fded363dda4990bb2d70e9194f0dca496bb82`  
		Last Modified: Thu, 12 Oct 2023 03:57:11 GMT  
		Size: 14.9 MB (14879720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:58b83690d392c116335e8fd9b2c275091639d089b8f7f847f4d377a6d82b7378
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69457709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2bcc8243d9507636e5a3dea0b7fed7e96bda7eafbdd181c94760a568fc989ba5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:58 GMT
ADD file:e1a6c6c976e5e7c53eb2a7343a7a763b46e56828588535f4c79e63d6ec08198d in / 
# Wed, 11 Oct 2023 18:24:58 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:46:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dd0dc10f921f4b3b65b17f20d367374079e6cb4e26531624ee64caaaf4adcc28`  
		Last Modified: Wed, 11 Oct 2023 18:28:45 GMT  
		Size: 53.7 MB (53707810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7a630df11a812111dd2b7f5b819a692f2350ad055fab0cd3e60b322c2eead5`  
		Last Modified: Wed, 11 Oct 2023 19:54:57 GMT  
		Size: 15.7 MB (15749899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:e1c572c67ccecd84db4824b91544f67cf96d1898da9f2d2e8082d02a28156ee4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.3 MB (72314570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1a1649cccdfb82a9509f903fefa311a0cbe4efa7c06904483e262c6ef68cd43`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:40:52 GMT
ADD file:a3c1e94bb116d940a614a5275c69bacbac46e00da2070b5c7a561e64b975acc6 in / 
# Wed, 11 Oct 2023 17:40:53 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:12:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:081c634ff059d5636b4292d84d0b49429030b3dca70ca56828543b295adb9d47`  
		Last Modified: Wed, 11 Oct 2023 17:45:55 GMT  
		Size: 56.0 MB (56046358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c55d0c1747845e146fb76750b201af94d841ddeee081fcbdefcc5353c17f2e`  
		Last Modified: Wed, 11 Oct 2023 18:23:38 GMT  
		Size: 16.3 MB (16268212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:d36ab6ccd5a69d80d30a12899ec690d3465ffbe7f79c9959256ff964a8013b19
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68818655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59e679dfa36ed42066347b3a7c55c9e0fe065971e0f4b551e37944ff83892c9d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:50:06 GMT
ADD file:c4be7fca661f2a8181ee1e05fda057c18a2d7c1ae0e08ab63b2c5567ef9cc0a7 in / 
# Wed, 11 Oct 2023 17:50:12 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:27:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d237f50a9f05adf465246bef37e194e1d7a226224c7f90ae7b55925c5b509d15`  
		Last Modified: Wed, 11 Oct 2023 18:01:27 GMT  
		Size: 53.3 MB (53289043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a8381daee3205699bef24f6e7ee0bd6b3621924baae8f1b0b0026007cfe3b4`  
		Last Modified: Wed, 11 Oct 2023 23:58:42 GMT  
		Size: 15.5 MB (15529612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:a8f64ada08912d3bc6055dfb5556580bdc6e31a2b9d852fb97e443e7967bc125
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75695202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dab5dd6afc653a6bf54d9046c1376d631f18b2de419b34a6eebaecd1c1c9e0e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:44:35 GMT
ADD file:d59326770edede2ba1d2005697bf41540a3d76a4bae883b91fede9b68018630c in / 
# Wed, 11 Oct 2023 17:44:38 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:20:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6613fa9f09034273d2b35a47386f8d53c77953a73e561b9f189ffa43ea17bd54`  
		Last Modified: Wed, 11 Oct 2023 17:50:25 GMT  
		Size: 58.9 MB (58929717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565fd5d2ec4119e0cef3217e4496512c36e4adc4e98567f565f105e684e80c4e`  
		Last Modified: Wed, 11 Oct 2023 18:38:00 GMT  
		Size: 16.8 MB (16765485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:22bb4a69e38d7e27b147c422662a4fd498271358a64a316a4955c9ae4087f7da
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68936610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:493442157276cd80e2ea1efa06c399eb8d575ca91cf4d33c6ea2e217d2cd5e57`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:50:40 GMT
ADD file:bb3ee20a7ddf364b23163c517132146872491e85ef2f1465bf7fd2ed33f94827 in / 
# Wed, 11 Oct 2023 17:50:44 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:58:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e651436ffb848f56da62cd2c80f206a288b94da8113c4c23a7e5502fb597ce23`  
		Last Modified: Wed, 11 Oct 2023 17:56:38 GMT  
		Size: 53.3 MB (53296378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a52fe3127c9c85c0c5e50b52a035e6bcee230e0c38db795abfee4b60522f157`  
		Last Modified: Thu, 12 Oct 2023 00:35:16 GMT  
		Size: 15.6 MB (15640232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldstable-scm`

```console
$ docker pull buildpack-deps@sha256:bac055b211a05a57b5e3ecef13ebf2467489801508aa142627e76621976a6ee9
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
$ docker pull buildpack-deps@sha256:253d4cf8241a2eff590b5ac562692d9e115c7537c1981afde7c0bb9f50651076
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.4 MB (125418067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01459750910db9c5ab8b473b3d05da74886a0b37bc6665134abdce8e1a17bf19`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:01 GMT
ADD file:8a9222387b89a9ac763fd72610ce01ab17f64387cbfde30a6af1861a82030aad in / 
# Wed, 11 Oct 2023 18:35:01 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:20:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:21:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:69b3efbf67c2d9a46fdfdc8480b5a03ef73e9999a53aad57213447784f01eb6e`  
		Last Modified: Wed, 11 Oct 2023 18:39:54 GMT  
		Size: 55.1 MB (55058028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dedceb9c21c46986231d9dfb896b37cfc470d67799e7e919a641ac54dcc9eed`  
		Last Modified: Thu, 12 Oct 2023 03:29:53 GMT  
		Size: 15.8 MB (15764226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98dfe1ecd6ba8d7f42ee14ec8a64da6ba633ed96ac9c58f6c5a0028ce6908916`  
		Last Modified: Thu, 12 Oct 2023 03:30:09 GMT  
		Size: 54.6 MB (54595813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:011f6927755aeeb83705407dd0b8b44593b9134ddf0d0ee7ef5cec32418d1b6d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.3 MB (120268820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b18801b1c50fa7588edecb59d16649ecbcec14a4478b91085817f3fb7ca1da5c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:37:51 GMT
ADD file:dd011733a11e4681328b2d45bbfc478e1dab88a95554fe817e238ef27b1865c2 in / 
# Wed, 11 Oct 2023 17:37:51 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:06:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:07:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d310e2405531cf391481a06c9f4d0fc75165ad8e3025e4035c6be5245b6cc754`  
		Last Modified: Wed, 11 Oct 2023 17:41:07 GMT  
		Size: 52.6 MB (52563098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c07441895e6cb16dc8222813db91b971828ec10cafdde9634c13ad69f7723b`  
		Last Modified: Wed, 11 Oct 2023 18:15:51 GMT  
		Size: 15.4 MB (15374683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36086464e7a231c171f28068f405baccff6fe849ecc79fba7ed52c6ebfdba6f9`  
		Last Modified: Wed, 11 Oct 2023 18:16:08 GMT  
		Size: 52.3 MB (52331039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:c53c90800fe4cf9897c502d7711674d1a1066c078d1b97b72b5c798ddada0128
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115448560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecdf47b0ce17fefb017abd99216cc417cc7afb93963a744c684e0994829f6da9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:19 GMT
ADD file:684f3634c6b747a4caad8f9f820cc02b53a2122591fe215935c5497ec234c3ad in / 
# Wed, 11 Oct 2023 17:42:20 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:47:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:47:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:33d0c7672db93e653471872c639cd6129ec25c168942e15a008c4920cafe62d7`  
		Last Modified: Wed, 11 Oct 2023 17:46:42 GMT  
		Size: 50.2 MB (50215704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe33e05af9470f2356c8047560fded363dda4990bb2d70e9194f0dca496bb82`  
		Last Modified: Thu, 12 Oct 2023 03:57:11 GMT  
		Size: 14.9 MB (14879720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0953bb94dc6fcb1dee741e8bfc886a0671f4516a04fbf1a92527c2bb1598e1dd`  
		Last Modified: Thu, 12 Oct 2023 03:57:33 GMT  
		Size: 50.4 MB (50353136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:ced5e59499a3da882d04714d3b138662087510ae912a4a3f67e07091d779be56
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124157783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b274c20cfd411a3b40df383bdd201e2c6b0b2793e2aab1604083557f0fb5edb1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:58 GMT
ADD file:e1a6c6c976e5e7c53eb2a7343a7a763b46e56828588535f4c79e63d6ec08198d in / 
# Wed, 11 Oct 2023 18:24:58 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:46:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:46:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dd0dc10f921f4b3b65b17f20d367374079e6cb4e26531624ee64caaaf4adcc28`  
		Last Modified: Wed, 11 Oct 2023 18:28:45 GMT  
		Size: 53.7 MB (53707810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7a630df11a812111dd2b7f5b819a692f2350ad055fab0cd3e60b322c2eead5`  
		Last Modified: Wed, 11 Oct 2023 19:54:57 GMT  
		Size: 15.7 MB (15749899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9c8e3bce435b9fb78d2fd6a8f0ce18ddecff51902c10074a9da4287cb35963b`  
		Last Modified: Wed, 11 Oct 2023 19:55:14 GMT  
		Size: 54.7 MB (54700074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:a09e5525965252b12dd52923b5273449114a15e10408a8ad5b56775c47c27211
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128251332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa3a761c17f979ab85a035b0000b43ff140b4e3759ad1a3fe42ae6bad59afa14`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:40:52 GMT
ADD file:a3c1e94bb116d940a614a5275c69bacbac46e00da2070b5c7a561e64b975acc6 in / 
# Wed, 11 Oct 2023 17:40:53 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:12:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:12:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:081c634ff059d5636b4292d84d0b49429030b3dca70ca56828543b295adb9d47`  
		Last Modified: Wed, 11 Oct 2023 17:45:55 GMT  
		Size: 56.0 MB (56046358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6c55d0c1747845e146fb76750b201af94d841ddeee081fcbdefcc5353c17f2e`  
		Last Modified: Wed, 11 Oct 2023 18:23:38 GMT  
		Size: 16.3 MB (16268212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:049e1171db56ce9d453ea26b1abcc12e301ef98dda47be8250cb0ced74ec097a`  
		Last Modified: Wed, 11 Oct 2023 18:24:01 GMT  
		Size: 55.9 MB (55936762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:78a2985bb49a2845f3145c2470d4fc56a0d5c9a1b2cc8b8530d1f76b0249e136
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122120959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7a5579be6befdd5b737e228200c04b041ee9277c42609f172d9cd187c395a48`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:50:06 GMT
ADD file:c4be7fca661f2a8181ee1e05fda057c18a2d7c1ae0e08ab63b2c5567ef9cc0a7 in / 
# Wed, 11 Oct 2023 17:50:12 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:27:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:29:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d237f50a9f05adf465246bef37e194e1d7a226224c7f90ae7b55925c5b509d15`  
		Last Modified: Wed, 11 Oct 2023 18:01:27 GMT  
		Size: 53.3 MB (53289043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a8381daee3205699bef24f6e7ee0bd6b3621924baae8f1b0b0026007cfe3b4`  
		Last Modified: Wed, 11 Oct 2023 23:58:42 GMT  
		Size: 15.5 MB (15529612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9e6da5ca3b34590abe253ac60b2000d9724ff3d9572311ded53ba9d66e58de`  
		Last Modified: Wed, 11 Oct 2023 23:59:27 GMT  
		Size: 53.3 MB (53302304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:c2a2624d91648d9bff279829625cbbf4355423f43ccf91431c0d3d3fbea2583d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.6 MB (134562128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:518eca7155957889e092f55b3815b4670c5db7a907113bc9fd64683bc7c719a9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:44:35 GMT
ADD file:d59326770edede2ba1d2005697bf41540a3d76a4bae883b91fede9b68018630c in / 
# Wed, 11 Oct 2023 17:44:38 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:20:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:21:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6613fa9f09034273d2b35a47386f8d53c77953a73e561b9f189ffa43ea17bd54`  
		Last Modified: Wed, 11 Oct 2023 17:50:25 GMT  
		Size: 58.9 MB (58929717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565fd5d2ec4119e0cef3217e4496512c36e4adc4e98567f565f105e684e80c4e`  
		Last Modified: Wed, 11 Oct 2023 18:38:00 GMT  
		Size: 16.8 MB (16765485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac6ae11620e817afc07c304ae67f21276148cc99a42e4ac56d481faceb27146`  
		Last Modified: Wed, 11 Oct 2023 18:38:24 GMT  
		Size: 58.9 MB (58866926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:4e549af12fe7ffa2d33939608ee823e50b8c02fbfe3fe7ad6542e9ca78ce985b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123002849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56de25e9482f0b3b8dd9d90c7bb9e4fc63c09768465c3b79a95301dbfe9205fc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:50:40 GMT
ADD file:bb3ee20a7ddf364b23163c517132146872491e85ef2f1465bf7fd2ed33f94827 in / 
# Wed, 11 Oct 2023 17:50:44 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:58:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:59:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e651436ffb848f56da62cd2c80f206a288b94da8113c4c23a7e5502fb597ce23`  
		Last Modified: Wed, 11 Oct 2023 17:56:38 GMT  
		Size: 53.3 MB (53296378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a52fe3127c9c85c0c5e50b52a035e6bcee230e0c38db795abfee4b60522f157`  
		Last Modified: Thu, 12 Oct 2023 00:35:16 GMT  
		Size: 15.6 MB (15640232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58e9fa5eede43b49ed76d5e09e5c978ac8b2296773dad3161eae081bba447e45`  
		Last Modified: Thu, 12 Oct 2023 00:35:44 GMT  
		Size: 54.1 MB (54066239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:scm`

```console
$ docker pull buildpack-deps@sha256:9b04ada2d533a254f9a3a4a4599a2a887717355d3963f1348b5908be6c0fc814
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
$ docker pull buildpack-deps@sha256:034daef4bd975190007ca9ea04206a70a50f0c94a22c31c69fb45266caf27bc3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.8 MB (137763770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7603bf6905c2f4d377ec3583bac5ca95d9600d3ad513c8f3e18ca0bc0a1459ca`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:37 GMT
ADD file:1e4dd5dab602337b5d5ef8d84b8dbe8b1ac62225f077b29b27d045842486d8e2 in / 
# Wed, 11 Oct 2023 18:34:37 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:19:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:19:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0a9573503463fd3166b5b1f34a7720dac28609e98d731e50e7068f92e79b8545`  
		Last Modified: Wed, 11 Oct 2023 18:39:10 GMT  
		Size: 49.6 MB (49582224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ccc26d841b4acc2562483bf393ce1cf8bc358ced09ccd825425226827c79c92`  
		Last Modified: Thu, 12 Oct 2023 03:28:45 GMT  
		Size: 24.1 MB (24051259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800d84653581fc119cd75cd572fa190d3b813d49221b9e5ee463e3560e2cb342`  
		Last Modified: Thu, 12 Oct 2023 03:29:04 GMT  
		Size: 64.1 MB (64130287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:3f6585039e542b0e19a291d5b489ba1d3647b261627e2c2467209933bd6424e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.6 MB (131646709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3619e24c9c6a8902a9cef46ec89de341f0bb65f1bb2c8e5f914176c890aa0259`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:37:30 GMT
ADD file:c07cf5c750a3e3c7ff84a3a3b8fc6087c9c5e0639d7bf638f0556d0a94309919 in / 
# Wed, 11 Oct 2023 17:37:35 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:04:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:05:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b7ec6536594e6c45ab234eecb51aacd85440ddc0e6da5873de23938ff146b5ec`  
		Last Modified: Wed, 11 Oct 2023 17:40:19 GMT  
		Size: 47.4 MB (47355749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ec943df1872e82ab3efa51bd5b2d7aac598550123e6db67156283ade7509d1`  
		Last Modified: Wed, 11 Oct 2023 18:14:31 GMT  
		Size: 22.7 MB (22729282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9f5c18924658cf6e03e52e00ddbf230cb1925aa017edb92b3cd508ec76293f`  
		Last Modified: Wed, 11 Oct 2023 18:14:54 GMT  
		Size: 61.6 MB (61561678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:5c80e22ca4ce0fc1769cad578ca3c0ec2d6020358bee0e0708ad8a7a4e1890eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.4 MB (126400592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c19fe7e4dbcb60f0b62f9d2258c1b8367310a78105eeac8cf15a871a70b0f97b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:41:59 GMT
ADD file:914e8a43f38c44fe9a6aabf05bbf3ebad5530966a354c8e7bb873c0842d35256 in / 
# Wed, 11 Oct 2023 17:42:00 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:45:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:45:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:65b9f3344eccdad2292cc7eec885befe05a52ec1136e145130c849441428eee6`  
		Last Modified: Wed, 11 Oct 2023 17:45:56 GMT  
		Size: 45.2 MB (45180287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbdddb82776e8c5901a821d5034c82b0fcba2993014440cd080d0592cd49616`  
		Last Modified: Thu, 12 Oct 2023 03:55:58 GMT  
		Size: 22.0 MB (21953833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f9d9ae792bc9a3749049ab80543cfddbda8910bcaffc9c95c7db4feb9e625a6`  
		Last Modified: Thu, 12 Oct 2023 03:56:18 GMT  
		Size: 59.3 MB (59266472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:ece8d9aa98c4e2ac79b982df68ee2ac9b4ae41a08fb3d92800f7124578ffffc8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.2 MB (137194983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0674043e7c55a6a4fc06506c806c8d8dab00a6ab67719922aa473372777950aa`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:43 GMT
ADD file:bf4264671bd91eb30c67d512144ebcf7f5c55a3e490ebe7876fa9b20d433bf7b in / 
# Wed, 11 Oct 2023 18:24:44 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:44:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:45:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e720f94321d63ecb6efa873b294dce7eaa1c3a5ddcd5bf7daddf375b955669a4`  
		Last Modified: Wed, 11 Oct 2023 18:28:04 GMT  
		Size: 49.6 MB (49612578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7541d83e7b8c0f5f6cacacddfcf5fdd942793f13418bc4645203b4ab4f3de3`  
		Last Modified: Wed, 11 Oct 2023 19:53:48 GMT  
		Size: 23.6 MB (23588086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a653d69b7b96df6835b157d043d7b926f776531e96c9263f4c7dae0033514d`  
		Last Modified: Wed, 11 Oct 2023 19:54:07 GMT  
		Size: 64.0 MB (63994319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:0225376ebdabef6ebca5adfd31d8e251c589b21de778ff4d6eb5f4435c87b92e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.5 MB (141471994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4557670d1bf5012131b762bb020c0f608408deca580a2b2638a6a0794046695`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:40:29 GMT
ADD file:0b6fc66d778d0cd8ae8b17b92945d98cc34f9c7008cda864ed0a54b5e40b9cb0 in / 
# Wed, 11 Oct 2023 17:40:32 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:09:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:10:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:501a599c15b6def048b2e00cfdf6c658061c00a504305ef2075fb1009a62c1e2`  
		Last Modified: Wed, 11 Oct 2023 17:45:01 GMT  
		Size: 50.6 MB (50600791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf9d6abbf47f32cac71cefb6f7233e5f700d4f6f941ca631e29947c5f1df955`  
		Last Modified: Wed, 11 Oct 2023 18:21:57 GMT  
		Size: 24.9 MB (24887201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1693c4d42b110c48ad84138aa8c91e1aeffbed6ca630f12495f711b89609823`  
		Last Modified: Wed, 11 Oct 2023 18:22:27 GMT  
		Size: 66.0 MB (65984002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:978fa0881d84f169ef3b182a55614b8c003440bfc7daff138acec86929b33f45
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.0 MB (135971603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:399ffe5bc61d49dc80a6a20678665009b14d5784ffd8ec66bd758ded95515def`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:48:50 GMT
ADD file:b081db8d48290ef5b5f477edb85d8f04d62a6995ec09bdb516d66dbe19b98137 in / 
# Wed, 11 Oct 2023 17:48:55 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:19:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:20:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:54dda4e4d31846b7324172a7fda3d0bdc7d8a2105ab27e9a92c2db43f35f9e5d`  
		Last Modified: Wed, 11 Oct 2023 17:59:53 GMT  
		Size: 49.6 MB (49569257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370a64ae3420fd85a23128ef46431df034f9038821764a14bb436272a1345505`  
		Last Modified: Wed, 11 Oct 2023 23:55:20 GMT  
		Size: 23.4 MB (23439567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c19b06553268b2cbcf576e075fdb1ac8c430154167258bcd4f925d5938117659`  
		Last Modified: Wed, 11 Oct 2023 23:56:13 GMT  
		Size: 63.0 MB (62962779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:e7774041231cd8297000ad9f73ba035a8098f870ab9e5935bf9e659d61dd0b02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.9 MB (148860554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eff06503f2fa76d78d36cfb0c68c5ebb59ed3780f372aec67e688ba57c8afda9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:44:01 GMT
ADD file:ed515e1aef8321271c6544e30cbeb31257e9640979e8f68a9e490cb25d3525fd in / 
# Wed, 11 Oct 2023 17:44:04 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:14:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:15:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f137383853e717724a59e86aa526d31eabb4a5d45a259cd1ade68d93b3f45ae9`  
		Last Modified: Wed, 11 Oct 2023 17:49:27 GMT  
		Size: 53.6 MB (53575984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da754908592cac64ca75d9cdc8c43a4a396901108de4adae61bd92937de4f65`  
		Last Modified: Wed, 11 Oct 2023 18:36:14 GMT  
		Size: 25.7 MB (25700026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524b67dc97fb52dd33f61fe12da424874443bb200789c7cfde14425f85938f54`  
		Last Modified: Wed, 11 Oct 2023 18:36:46 GMT  
		Size: 69.6 MB (69584544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:198224f3809fdab1ffa595ddb0d788d97dec1c41556a1a5e913b711ec6ccdaab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.1 MB (135122600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8fda4e35a32e1c513adb4a70b998c8a77f96ac52d6a7c94f6f085b1d1995b8e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:50:07 GMT
ADD file:2dc117136732884ad4b058065700dd66cc49d6ce56b0fdbb672915e3ad8adb84 in / 
# Wed, 11 Oct 2023 17:50:10 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:51:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:52:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ad5e374600bf40a929dfe51e52737e4ca04aba83f499656760ba938841fb6552`  
		Last Modified: Wed, 11 Oct 2023 17:55:18 GMT  
		Size: 47.9 MB (47942934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6344f505670ce139b1b3f472749240f33304ec7535daae4a72913a6da08f304f`  
		Last Modified: Thu, 12 Oct 2023 00:33:20 GMT  
		Size: 24.0 MB (24046768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf2b4ce0798e7985dd88d10311ea2a2730812d4e10c9a8f24f564875c6cb617`  
		Last Modified: Thu, 12 Oct 2023 00:33:56 GMT  
		Size: 63.1 MB (63132898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:sid`

```console
$ docker pull buildpack-deps@sha256:8815033d9170f0e05af5c2cd68e7f754eb3aa01c893f5d61a2396a59e668a5bb
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
$ docker pull buildpack-deps@sha256:2d20963c232d6971a6a39af931571eb1d5e7fba7c4bcdaf0088977bfc6844a83
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **379.9 MB (379943549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59354cbe9e3cad45620c2a2218d362d004025667786b9e7ebfa732437af1daef`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:36:29 GMT
ADD file:0301a32b2b2f0af81dd4277b61ab0069818663e8ad39e59dec42f2a74e027eda in / 
# Wed, 11 Oct 2023 18:36:29 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:24:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:24:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:25:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3997a52aa0dcbfc5a01686dece23fdbb32f74ea998359451f16034544761414c`  
		Last Modified: Wed, 11 Oct 2023 18:42:29 GMT  
		Size: 49.5 MB (49503645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0b8297fd30d70e6a01a348e7e07badb169eb034e4f609afaa217cab587d8b9`  
		Last Modified: Thu, 12 Oct 2023 03:31:53 GMT  
		Size: 24.3 MB (24334751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6e5521f78eb644a7a00e353d6c3a5f1799c951272b0b5ec79a44243d51a462`  
		Last Modified: Thu, 12 Oct 2023 03:32:12 GMT  
		Size: 65.5 MB (65492596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af279c69b25af9b0d882b06462ffef0299fb0aa7628e001b6b2607baca6c6b94`  
		Last Modified: Thu, 12 Oct 2023 03:32:50 GMT  
		Size: 240.6 MB (240612557 bytes)  
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

## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:e9e3226aca93195d4f816612bce1cd5fb77e540c1269e6a3629c11235c9d9859
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
$ docker pull buildpack-deps@sha256:93d69ad7c2dba69a9f03d997bc80b11965a717a955bad0dbc9e73930c0fec227
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.8 MB (73838396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0aead4e0ede50e21f0bb6b06b316d7bf4b26320273def7c2d20529ceb8d60a57`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:36:29 GMT
ADD file:0301a32b2b2f0af81dd4277b61ab0069818663e8ad39e59dec42f2a74e027eda in / 
# Wed, 11 Oct 2023 18:36:29 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:24:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3997a52aa0dcbfc5a01686dece23fdbb32f74ea998359451f16034544761414c`  
		Last Modified: Wed, 11 Oct 2023 18:42:29 GMT  
		Size: 49.5 MB (49503645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0b8297fd30d70e6a01a348e7e07badb169eb034e4f609afaa217cab587d8b9`  
		Last Modified: Thu, 12 Oct 2023 03:31:53 GMT  
		Size: 24.3 MB (24334751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:2facb29855ce778449935650ad0bf8f05285f5bc037e27c0abc545731ade43e0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70157877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e3ce55c97d64bebc6d52e5b52a1e5ec90df23921d54256da45d2978fabdcf44`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:38:22 GMT
ADD file:32bc859b55e9b4aada411b379418b1cd95da1e1f72e89ade7698d0132f8edafd in / 
# Wed, 11 Oct 2023 17:38:22 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:09:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
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

### `buildpack-deps:sid-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:2a3ac98b13e5c0b84e8a96c479d489b7281c2542c75032fdcd02dda6af1de78e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67168379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d21e5bc073011f98455f4bb3cf2cf376f08857422f623a0610bbb271406d9f9c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:43:32 GMT
ADD file:e83473ecad5aa9a153d02c535c6e40e22679b973268fdd74a0f5bd86b004222a in / 
# Wed, 11 Oct 2023 17:43:33 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:50:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
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

### `buildpack-deps:sid-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:fce215ecb937435e92000bf5dfe52f3717f5dca30b710c5064233ef875426f43
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.4 MB (73391816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2d378acba0577367ce6a31afd366988b2b397f9537de3a47b965ec3899cb758`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:56 GMT
ADD file:c18e09bd64c99d045a504c333efaa05322c76b488039b206edcf75aa2a1a3812 in / 
# Wed, 11 Oct 2023 18:25:57 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:49:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
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

### `buildpack-deps:sid-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:6c5a3c841432a3311b27c5d3b9ab74fbfd33f1fc8c9c5570adcbd1a3449f301c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75645770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b139468ba853f4e64f72ad3a626476ad17acf6b17286e5b697e458ab16986cd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:19 GMT
ADD file:e8e1c13db04ddce5a6b3f4e29283e75eeecf85f213c2433ccb342a253457abc1 in / 
# Wed, 11 Oct 2023 17:42:20 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:16:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
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

### `buildpack-deps:sid-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:630fa9a87431d5ef63ba0403e35b1d13078e44716350c2f7f626b79644299959
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73189227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4f8b088028ae199b72c712652c50ff8948c76437c673b92447dcdf542c35ff8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:52:38 GMT
ADD file:b80f07fa17341655abce58a1824ae94b2623d66b3f37a58194b8a738cf645945 in / 
# Wed, 11 Oct 2023 17:52:44 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:36:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
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

### `buildpack-deps:sid-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:cd232f49802d24b109a6845c69de40da722b1c48414c6b7198c904425c111923
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.4 MB (79394432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dff07d1542982f90245cadfde4cf3d10fe51356a3b06794d5b5de4fb83cb01e2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:45:44 GMT
ADD file:5f062baf648f8cba61d84347ebedbe11eca129a318a8146b4c7c30586cbf0436 in / 
# Wed, 11 Oct 2023 17:45:47 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:25:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
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

### `buildpack-deps:sid-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:463277650cb87ff963c4f3e246c78101c2bf595bfdcfda04fb4db350e9dc1592
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69007846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a46d4dea6048745e0f58711f73e97cfebd76971edb90fbbf0cf7dc14a24ec144`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:09:51 GMT
ADD file:fdcff160dcad587bb28b0cba721c24193be4ab5de90a2d503cba3d329b78797b in / 
# Thu, 27 Jul 2023 23:09:54 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:32:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
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

### `buildpack-deps:sid-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:43c6868e1269e7652a2de8a9524ef2cfdc486ebee9b841c762abc68d593b7c7b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.5 MB (73502003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cbc0b99dfdb875d8a7fc97b0162f802cadba9a8045b9077107c5592300b2f65`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:51:43 GMT
ADD file:66653f97d007e397b8dbcdca1bbb32bd8039456ae5b2cae3e049382489afb265 in / 
# Wed, 11 Oct 2023 17:51:47 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 00:05:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
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

## `buildpack-deps:sid-scm`

```console
$ docker pull buildpack-deps@sha256:718fec922b4a6871329a1bbf1c6d9da309a17f8aac5af9743fdda459d5fb3a85
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
$ docker pull buildpack-deps@sha256:0b2f3bd1cc4c7815a7e596fb753fc38a233e70c90ecf2bed32ecdcf28e5a74a2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.3 MB (139330992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6908eca674268f2a8c937287486ca0fb7661d00ec8e725e0ede07b0970b7ee1b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:36:29 GMT
ADD file:0301a32b2b2f0af81dd4277b61ab0069818663e8ad39e59dec42f2a74e027eda in / 
# Wed, 11 Oct 2023 18:36:29 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:24:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:24:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3997a52aa0dcbfc5a01686dece23fdbb32f74ea998359451f16034544761414c`  
		Last Modified: Wed, 11 Oct 2023 18:42:29 GMT  
		Size: 49.5 MB (49503645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0b8297fd30d70e6a01a348e7e07badb169eb034e4f609afaa217cab587d8b9`  
		Last Modified: Thu, 12 Oct 2023 03:31:53 GMT  
		Size: 24.3 MB (24334751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6e5521f78eb644a7a00e353d6c3a5f1799c951272b0b5ec79a44243d51a462`  
		Last Modified: Thu, 12 Oct 2023 03:32:12 GMT  
		Size: 65.5 MB (65492596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:6e5665d5853aa13b18e4bc33e2e74ccd3fd4299bbee0d5638a8edfd8811fd31d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.2 MB (133155810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82733bdae381c5738d0e28f4d4a7b2e23a488cf237028a2f9d7340ed42a2de6a`
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

### `buildpack-deps:sid-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:0241422c180b52449cebfb843511a622b3db62b876adcb35f83687d33338ebd0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127780532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e47cd5dfc4c910b811a8be1f25b280a059fbcfd20276ea41ecb9d61a43415c5`
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

### `buildpack-deps:sid-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:944bdc970d6ca598d11e588a54f084da0fb8a9ba812e762a9214eabe87384929
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.0 MB (138977761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1834be5b56b00292a42bceb02448a4a30da604bc1654bd80098dd463aa4b5e12`
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

### `buildpack-deps:sid-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:db6becb86617eec873cc1f2cbc1f8c0abd30edc8936fe15da22884a7c262b25f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.9 MB (142912216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5170e1fe625abd2d29e37453c2b4b9ba4255f5b27a6f1e529629d4b96d54a95`
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

### `buildpack-deps:sid-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:89df672a2eae0669920f05fcd19c0581e1dece33f0bb2a1d319e25e9d2537059
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137502013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e3b055ef2c6b884b963271c3f7fbb51f1913f3ac0ad28460eb6d5a0d022fb30`
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

### `buildpack-deps:sid-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:bfd905fe06deae4a397b28f46fa0b93ebc6e0f31d8de7f7d64f20a01c3510614
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.3 MB (150311356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc0c94e86ebe4c6d3673f604832571ce2c2f31974dc5f67beeb360a926f3aa03`
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

### `buildpack-deps:sid-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:82b54224e16141b3d128a2c7213a413e390b1216abe389f923a2eaf497c751af
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.4 MB (129394231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4d1a4d2d9108164c640ce2247e18e16b8a958c777fd7a7181f424ddb829d083`
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

### `buildpack-deps:sid-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:60c63e0e0ad978fcf73dd18012240127fcb631a7993d05b3f9d3ddabab132675
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.9 MB (139893138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f3debda305b48b4c96aeca9c4076cb44864a7a588e3041b287ddf0f78757147`
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

## `buildpack-deps:stable`

```console
$ docker pull buildpack-deps@sha256:584ae312404463556590dbd340dc888147030cb3c8cbaec1ae7fc474ac453fdd
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
$ docker pull buildpack-deps@sha256:e5e5c80b6c13eb1ac931b319d5b2dda3a67473c085edc2ef5212ee628f4ee6bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.8 MB (348827828 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c9f4bf96c80ab0bd24165e83092eab60265322c4575d970deaae7e8a4742ea3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:37 GMT
ADD file:1e4dd5dab602337b5d5ef8d84b8dbe8b1ac62225f077b29b27d045842486d8e2 in / 
# Wed, 11 Oct 2023 18:34:37 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:19:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:19:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:20:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0a9573503463fd3166b5b1f34a7720dac28609e98d731e50e7068f92e79b8545`  
		Last Modified: Wed, 11 Oct 2023 18:39:10 GMT  
		Size: 49.6 MB (49582224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ccc26d841b4acc2562483bf393ce1cf8bc358ced09ccd825425226827c79c92`  
		Last Modified: Thu, 12 Oct 2023 03:28:45 GMT  
		Size: 24.1 MB (24051259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800d84653581fc119cd75cd572fa190d3b813d49221b9e5ee463e3560e2cb342`  
		Last Modified: Thu, 12 Oct 2023 03:29:04 GMT  
		Size: 64.1 MB (64130287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c632e57ea62ea950c367f484f52cdcfd2adb12060a31f5c413f40db9822e96e`  
		Last Modified: Thu, 12 Oct 2023 03:29:40 GMT  
		Size: 211.1 MB (211064058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:86d28c1e87df6d4e3309e403a9ced8594ad1380ffb29db3cbb99ee65245d77e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.0 MB (316030711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f61c441d8080fa400d21357cb9170445e8b0e150d15c350be1e20d0849837a84`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:37:30 GMT
ADD file:c07cf5c750a3e3c7ff84a3a3b8fc6087c9c5e0639d7bf638f0556d0a94309919 in / 
# Wed, 11 Oct 2023 17:37:35 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:04:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:05:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:06:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b7ec6536594e6c45ab234eecb51aacd85440ddc0e6da5873de23938ff146b5ec`  
		Last Modified: Wed, 11 Oct 2023 17:40:19 GMT  
		Size: 47.4 MB (47355749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ec943df1872e82ab3efa51bd5b2d7aac598550123e6db67156283ade7509d1`  
		Last Modified: Wed, 11 Oct 2023 18:14:31 GMT  
		Size: 22.7 MB (22729282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9f5c18924658cf6e03e52e00ddbf230cb1925aa017edb92b3cd508ec76293f`  
		Last Modified: Wed, 11 Oct 2023 18:14:54 GMT  
		Size: 61.6 MB (61561678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7670741713d795c2814eacfe8b75187f28e3485379b6fb2770c71d163e26127`  
		Last Modified: Wed, 11 Oct 2023 18:15:37 GMT  
		Size: 184.4 MB (184384002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:28ad6736c4c7a5c78602a4c42becc99de682ba5927aa95ad9f5105294d099a8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.4 MB (301449230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43d67f8c14cfd8cddba9828203d94136bcc749df068cfbc834ba011ede605f79`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:41:59 GMT
ADD file:914e8a43f38c44fe9a6aabf05bbf3ebad5530966a354c8e7bb873c0842d35256 in / 
# Wed, 11 Oct 2023 17:42:00 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:45:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:45:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:46:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:65b9f3344eccdad2292cc7eec885befe05a52ec1136e145130c849441428eee6`  
		Last Modified: Wed, 11 Oct 2023 17:45:56 GMT  
		Size: 45.2 MB (45180287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbdddb82776e8c5901a821d5034c82b0fcba2993014440cd080d0592cd49616`  
		Last Modified: Thu, 12 Oct 2023 03:55:58 GMT  
		Size: 22.0 MB (21953833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f9d9ae792bc9a3749049ab80543cfddbda8910bcaffc9c95c7db4feb9e625a6`  
		Last Modified: Thu, 12 Oct 2023 03:56:18 GMT  
		Size: 59.3 MB (59266472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9912e09bb3246583228b0aa9f45499f60d04bbb57d5db9e63d50fd5585cc0c20`  
		Last Modified: Thu, 12 Oct 2023 03:56:58 GMT  
		Size: 175.0 MB (175048638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:1217daf5693bf080affa2383e80682e4ed80fa25c7b6889924e21e401abfef07
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.6 MB (339643434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13543f9c2ab23caf4e23f3900fa93f86e7a0d57bbfb3dfb296c3985b777511b8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:43 GMT
ADD file:bf4264671bd91eb30c67d512144ebcf7f5c55a3e490ebe7876fa9b20d433bf7b in / 
# Wed, 11 Oct 2023 18:24:44 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:44:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:45:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:46:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e720f94321d63ecb6efa873b294dce7eaa1c3a5ddcd5bf7daddf375b955669a4`  
		Last Modified: Wed, 11 Oct 2023 18:28:04 GMT  
		Size: 49.6 MB (49612578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7541d83e7b8c0f5f6cacacddfcf5fdd942793f13418bc4645203b4ab4f3de3`  
		Last Modified: Wed, 11 Oct 2023 19:53:48 GMT  
		Size: 23.6 MB (23588086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a653d69b7b96df6835b157d043d7b926f776531e96c9263f4c7dae0033514d`  
		Last Modified: Wed, 11 Oct 2023 19:54:07 GMT  
		Size: 64.0 MB (63994319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c02d5d50082e4632f070b715dfd5d3a3680e35e0434a1281edbcfdc3cdff52dc`  
		Last Modified: Wed, 11 Oct 2023 19:54:39 GMT  
		Size: 202.4 MB (202448451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:1a6a219086627846d966e869a8d56fd78994fb747da91f49e6a46a674ef778c6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.5 MB (351462994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f4402f88a53734d262ec398d9da3786d89072972edfbbc52175a078d23b80d0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:40:29 GMT
ADD file:0b6fc66d778d0cd8ae8b17b92945d98cc34f9c7008cda864ed0a54b5e40b9cb0 in / 
# Wed, 11 Oct 2023 17:40:32 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:09:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:10:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:11:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:501a599c15b6def048b2e00cfdf6c658061c00a504305ef2075fb1009a62c1e2`  
		Last Modified: Wed, 11 Oct 2023 17:45:01 GMT  
		Size: 50.6 MB (50600791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf9d6abbf47f32cac71cefb6f7233e5f700d4f6f941ca631e29947c5f1df955`  
		Last Modified: Wed, 11 Oct 2023 18:21:57 GMT  
		Size: 24.9 MB (24887201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1693c4d42b110c48ad84138aa8c91e1aeffbed6ca630f12495f711b89609823`  
		Last Modified: Wed, 11 Oct 2023 18:22:27 GMT  
		Size: 66.0 MB (65984002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d61ba44e3cf60d5c6195ef4448de7160aff21051156b51d78755d19cb401055`  
		Last Modified: Wed, 11 Oct 2023 18:23:24 GMT  
		Size: 210.0 MB (209991000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:b585c2f0cfabe530c3905bb95c637eb6339c7663273b893ede5b4d8cacd9233b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.6 MB (325624324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01ae125d4ffa592dfd3716595bf2806c88e2b3b84e7cdc94482338771a440d1c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:48:50 GMT
ADD file:b081db8d48290ef5b5f477edb85d8f04d62a6995ec09bdb516d66dbe19b98137 in / 
# Wed, 11 Oct 2023 17:48:55 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:19:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:20:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:26:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:54dda4e4d31846b7324172a7fda3d0bdc7d8a2105ab27e9a92c2db43f35f9e5d`  
		Last Modified: Wed, 11 Oct 2023 17:59:53 GMT  
		Size: 49.6 MB (49569257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370a64ae3420fd85a23128ef46431df034f9038821764a14bb436272a1345505`  
		Last Modified: Wed, 11 Oct 2023 23:55:20 GMT  
		Size: 23.4 MB (23439567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c19b06553268b2cbcf576e075fdb1ac8c430154167258bcd4f925d5938117659`  
		Last Modified: Wed, 11 Oct 2023 23:56:13 GMT  
		Size: 63.0 MB (62962779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe7e7187a4f54c6c9e49f439f18fe1ae7a7f06894b24eae29001a71e03340c5`  
		Last Modified: Wed, 11 Oct 2023 23:58:22 GMT  
		Size: 189.7 MB (189652721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:12b9dc56603f357d0e68e2cd0927be121561f588bc3f728ed3a1fb3dc0ec9ded
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **363.0 MB (362953503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7467ffe1bf70430528cbbee8f716bd707ff747ee7ff42c2f77578884a1c214d6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:44:01 GMT
ADD file:ed515e1aef8321271c6544e30cbeb31257e9640979e8f68a9e490cb25d3525fd in / 
# Wed, 11 Oct 2023 17:44:04 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:14:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:15:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:19:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f137383853e717724a59e86aa526d31eabb4a5d45a259cd1ade68d93b3f45ae9`  
		Last Modified: Wed, 11 Oct 2023 17:49:27 GMT  
		Size: 53.6 MB (53575984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da754908592cac64ca75d9cdc8c43a4a396901108de4adae61bd92937de4f65`  
		Last Modified: Wed, 11 Oct 2023 18:36:14 GMT  
		Size: 25.7 MB (25700026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524b67dc97fb52dd33f61fe12da424874443bb200789c7cfde14425f85938f54`  
		Last Modified: Wed, 11 Oct 2023 18:36:46 GMT  
		Size: 69.6 MB (69584544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7449a547606da3836fd2405c85ed15e48ed96b7936fe9dfcbb8c69e21475738e`  
		Last Modified: Wed, 11 Oct 2023 18:37:46 GMT  
		Size: 214.1 MB (214092949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:eb83643215e451aa8409fe1fec979764362831916fa9a2955baa57c263d6631f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.2 MB (318222519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42abbfd998057c2e0c5d1c31d39f5a383b5ce7201d011ae9066f0214cd94321c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:50:07 GMT
ADD file:2dc117136732884ad4b058065700dd66cc49d6ce56b0fdbb672915e3ad8adb84 in / 
# Wed, 11 Oct 2023 17:50:10 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:51:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:52:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:58:19 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ad5e374600bf40a929dfe51e52737e4ca04aba83f499656760ba938841fb6552`  
		Last Modified: Wed, 11 Oct 2023 17:55:18 GMT  
		Size: 47.9 MB (47942934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6344f505670ce139b1b3f472749240f33304ec7535daae4a72913a6da08f304f`  
		Last Modified: Thu, 12 Oct 2023 00:33:20 GMT  
		Size: 24.0 MB (24046768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf2b4ce0798e7985dd88d10311ea2a2730812d4e10c9a8f24f564875c6cb617`  
		Last Modified: Thu, 12 Oct 2023 00:33:56 GMT  
		Size: 63.1 MB (63132898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317490e394e1c9331e54c7c33215628d4d08a8cd9d2191cb3d294d0b021a18f9`  
		Last Modified: Thu, 12 Oct 2023 00:34:47 GMT  
		Size: 183.1 MB (183099919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stable-curl`

```console
$ docker pull buildpack-deps@sha256:ce8ea34dd6046d5bd7bc423fbee3460e246b576dcd581e5ba6583f3535b55fcd
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
$ docker pull buildpack-deps@sha256:977f8a0eade986703e1379ef96d1c106c53eccfef6eb0dace01f3f404dd41db3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73633483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6190da4faf36a08749338aa0f80e05ce0f4a16fc3164c506cc7cd23b0b6e665c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:37 GMT
ADD file:1e4dd5dab602337b5d5ef8d84b8dbe8b1ac62225f077b29b27d045842486d8e2 in / 
# Wed, 11 Oct 2023 18:34:37 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:19:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0a9573503463fd3166b5b1f34a7720dac28609e98d731e50e7068f92e79b8545`  
		Last Modified: Wed, 11 Oct 2023 18:39:10 GMT  
		Size: 49.6 MB (49582224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ccc26d841b4acc2562483bf393ce1cf8bc358ced09ccd825425226827c79c92`  
		Last Modified: Thu, 12 Oct 2023 03:28:45 GMT  
		Size: 24.1 MB (24051259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:26df1627a60457168bc3b15d71211f6b2233409c7dcd192decbae29947006323
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.1 MB (70085031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ef4b4f6796a04df75ac23eda97d56908155655aca64a22dceb52210e8ef9956`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:37:30 GMT
ADD file:c07cf5c750a3e3c7ff84a3a3b8fc6087c9c5e0639d7bf638f0556d0a94309919 in / 
# Wed, 11 Oct 2023 17:37:35 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:04:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b7ec6536594e6c45ab234eecb51aacd85440ddc0e6da5873de23938ff146b5ec`  
		Last Modified: Wed, 11 Oct 2023 17:40:19 GMT  
		Size: 47.4 MB (47355749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ec943df1872e82ab3efa51bd5b2d7aac598550123e6db67156283ade7509d1`  
		Last Modified: Wed, 11 Oct 2023 18:14:31 GMT  
		Size: 22.7 MB (22729282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:c88279d74fb84bd9e91e1631a6f8be701529d90987a5bd1877a7c1741aaddf11
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67134120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:922f8718561dcde238f85464ae864269e429eda3b44a3124b8a1c955d881c183`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:41:59 GMT
ADD file:914e8a43f38c44fe9a6aabf05bbf3ebad5530966a354c8e7bb873c0842d35256 in / 
# Wed, 11 Oct 2023 17:42:00 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:45:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:65b9f3344eccdad2292cc7eec885befe05a52ec1136e145130c849441428eee6`  
		Last Modified: Wed, 11 Oct 2023 17:45:56 GMT  
		Size: 45.2 MB (45180287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbdddb82776e8c5901a821d5034c82b0fcba2993014440cd080d0592cd49616`  
		Last Modified: Thu, 12 Oct 2023 03:55:58 GMT  
		Size: 22.0 MB (21953833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3336852231c4838575dca42d951ad5ef02897709b046c708ab77d49bf73af01c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73200664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a61350e5fd6e43ba2eafdd779f92c81d1adcc19b9614cd2c2a8a88b2f7ff2b7e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:43 GMT
ADD file:bf4264671bd91eb30c67d512144ebcf7f5c55a3e490ebe7876fa9b20d433bf7b in / 
# Wed, 11 Oct 2023 18:24:44 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:44:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e720f94321d63ecb6efa873b294dce7eaa1c3a5ddcd5bf7daddf375b955669a4`  
		Last Modified: Wed, 11 Oct 2023 18:28:04 GMT  
		Size: 49.6 MB (49612578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7541d83e7b8c0f5f6cacacddfcf5fdd942793f13418bc4645203b4ab4f3de3`  
		Last Modified: Wed, 11 Oct 2023 19:53:48 GMT  
		Size: 23.6 MB (23588086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:af61129a918d7d5a838f84a53e5c4187bfad03a62baf89b590e2eee9e0ccbd15
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.5 MB (75487992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8222a221a97a3218fabbfecba1af542b4002d5b5999bdcecc8a82f8e724c78a7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:40:29 GMT
ADD file:0b6fc66d778d0cd8ae8b17b92945d98cc34f9c7008cda864ed0a54b5e40b9cb0 in / 
# Wed, 11 Oct 2023 17:40:32 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:09:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:501a599c15b6def048b2e00cfdf6c658061c00a504305ef2075fb1009a62c1e2`  
		Last Modified: Wed, 11 Oct 2023 17:45:01 GMT  
		Size: 50.6 MB (50600791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf9d6abbf47f32cac71cefb6f7233e5f700d4f6f941ca631e29947c5f1df955`  
		Last Modified: Wed, 11 Oct 2023 18:21:57 GMT  
		Size: 24.9 MB (24887201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:5019b5e06e6411dc6681b042d91c4166bda9f959281d3afb18a28b2c51859fe1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (73008824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a14c97aa10bb55fcde7d0ab1936a74404ebc81297baed7f34e394b13f6e1be9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:48:50 GMT
ADD file:b081db8d48290ef5b5f477edb85d8f04d62a6995ec09bdb516d66dbe19b98137 in / 
# Wed, 11 Oct 2023 17:48:55 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:19:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:54dda4e4d31846b7324172a7fda3d0bdc7d8a2105ab27e9a92c2db43f35f9e5d`  
		Last Modified: Wed, 11 Oct 2023 17:59:53 GMT  
		Size: 49.6 MB (49569257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370a64ae3420fd85a23128ef46431df034f9038821764a14bb436272a1345505`  
		Last Modified: Wed, 11 Oct 2023 23:55:20 GMT  
		Size: 23.4 MB (23439567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:744a14b7351b264caa5f532c9e2ddd30adb33c3aff32aa63acc7cf5b82a9400d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.3 MB (79276010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79aafe4e34b99dcfea8074db94ea73e75d2fd2d71b38493a1d9fb2b1d31e811f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:44:01 GMT
ADD file:ed515e1aef8321271c6544e30cbeb31257e9640979e8f68a9e490cb25d3525fd in / 
# Wed, 11 Oct 2023 17:44:04 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:14:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f137383853e717724a59e86aa526d31eabb4a5d45a259cd1ade68d93b3f45ae9`  
		Last Modified: Wed, 11 Oct 2023 17:49:27 GMT  
		Size: 53.6 MB (53575984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da754908592cac64ca75d9cdc8c43a4a396901108de4adae61bd92937de4f65`  
		Last Modified: Wed, 11 Oct 2023 18:36:14 GMT  
		Size: 25.7 MB (25700026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b8e20019afbeea6704a1315aac08a0971e357e86421fea4eadddb139a30796db
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.0 MB (71989702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:547b709e2a6beabff89cf0efea20a9713d1b7b7b7a3d67ecd5bdef17c2ff16fc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:50:07 GMT
ADD file:2dc117136732884ad4b058065700dd66cc49d6ce56b0fdbb672915e3ad8adb84 in / 
# Wed, 11 Oct 2023 17:50:10 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:51:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ad5e374600bf40a929dfe51e52737e4ca04aba83f499656760ba938841fb6552`  
		Last Modified: Wed, 11 Oct 2023 17:55:18 GMT  
		Size: 47.9 MB (47942934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6344f505670ce139b1b3f472749240f33304ec7535daae4a72913a6da08f304f`  
		Last Modified: Thu, 12 Oct 2023 00:33:20 GMT  
		Size: 24.0 MB (24046768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stable-scm`

```console
$ docker pull buildpack-deps@sha256:9b04ada2d533a254f9a3a4a4599a2a887717355d3963f1348b5908be6c0fc814
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
$ docker pull buildpack-deps@sha256:034daef4bd975190007ca9ea04206a70a50f0c94a22c31c69fb45266caf27bc3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.8 MB (137763770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7603bf6905c2f4d377ec3583bac5ca95d9600d3ad513c8f3e18ca0bc0a1459ca`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:34:37 GMT
ADD file:1e4dd5dab602337b5d5ef8d84b8dbe8b1ac62225f077b29b27d045842486d8e2 in / 
# Wed, 11 Oct 2023 18:34:37 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:19:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:19:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0a9573503463fd3166b5b1f34a7720dac28609e98d731e50e7068f92e79b8545`  
		Last Modified: Wed, 11 Oct 2023 18:39:10 GMT  
		Size: 49.6 MB (49582224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ccc26d841b4acc2562483bf393ce1cf8bc358ced09ccd825425226827c79c92`  
		Last Modified: Thu, 12 Oct 2023 03:28:45 GMT  
		Size: 24.1 MB (24051259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800d84653581fc119cd75cd572fa190d3b813d49221b9e5ee463e3560e2cb342`  
		Last Modified: Thu, 12 Oct 2023 03:29:04 GMT  
		Size: 64.1 MB (64130287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:3f6585039e542b0e19a291d5b489ba1d3647b261627e2c2467209933bd6424e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.6 MB (131646709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3619e24c9c6a8902a9cef46ec89de341f0bb65f1bb2c8e5f914176c890aa0259`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:37:30 GMT
ADD file:c07cf5c750a3e3c7ff84a3a3b8fc6087c9c5e0639d7bf638f0556d0a94309919 in / 
# Wed, 11 Oct 2023 17:37:35 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:04:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:05:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b7ec6536594e6c45ab234eecb51aacd85440ddc0e6da5873de23938ff146b5ec`  
		Last Modified: Wed, 11 Oct 2023 17:40:19 GMT  
		Size: 47.4 MB (47355749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ec943df1872e82ab3efa51bd5b2d7aac598550123e6db67156283ade7509d1`  
		Last Modified: Wed, 11 Oct 2023 18:14:31 GMT  
		Size: 22.7 MB (22729282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9f5c18924658cf6e03e52e00ddbf230cb1925aa017edb92b3cd508ec76293f`  
		Last Modified: Wed, 11 Oct 2023 18:14:54 GMT  
		Size: 61.6 MB (61561678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:5c80e22ca4ce0fc1769cad578ca3c0ec2d6020358bee0e0708ad8a7a4e1890eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.4 MB (126400592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c19fe7e4dbcb60f0b62f9d2258c1b8367310a78105eeac8cf15a871a70b0f97b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:41:59 GMT
ADD file:914e8a43f38c44fe9a6aabf05bbf3ebad5530966a354c8e7bb873c0842d35256 in / 
# Wed, 11 Oct 2023 17:42:00 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:45:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:45:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:65b9f3344eccdad2292cc7eec885befe05a52ec1136e145130c849441428eee6`  
		Last Modified: Wed, 11 Oct 2023 17:45:56 GMT  
		Size: 45.2 MB (45180287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbdddb82776e8c5901a821d5034c82b0fcba2993014440cd080d0592cd49616`  
		Last Modified: Thu, 12 Oct 2023 03:55:58 GMT  
		Size: 22.0 MB (21953833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f9d9ae792bc9a3749049ab80543cfddbda8910bcaffc9c95c7db4feb9e625a6`  
		Last Modified: Thu, 12 Oct 2023 03:56:18 GMT  
		Size: 59.3 MB (59266472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:ece8d9aa98c4e2ac79b982df68ee2ac9b4ae41a08fb3d92800f7124578ffffc8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.2 MB (137194983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0674043e7c55a6a4fc06506c806c8d8dab00a6ab67719922aa473372777950aa`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:24:43 GMT
ADD file:bf4264671bd91eb30c67d512144ebcf7f5c55a3e490ebe7876fa9b20d433bf7b in / 
# Wed, 11 Oct 2023 18:24:44 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:44:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:45:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e720f94321d63ecb6efa873b294dce7eaa1c3a5ddcd5bf7daddf375b955669a4`  
		Last Modified: Wed, 11 Oct 2023 18:28:04 GMT  
		Size: 49.6 MB (49612578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7541d83e7b8c0f5f6cacacddfcf5fdd942793f13418bc4645203b4ab4f3de3`  
		Last Modified: Wed, 11 Oct 2023 19:53:48 GMT  
		Size: 23.6 MB (23588086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a653d69b7b96df6835b157d043d7b926f776531e96c9263f4c7dae0033514d`  
		Last Modified: Wed, 11 Oct 2023 19:54:07 GMT  
		Size: 64.0 MB (63994319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:0225376ebdabef6ebca5adfd31d8e251c589b21de778ff4d6eb5f4435c87b92e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.5 MB (141471994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4557670d1bf5012131b762bb020c0f608408deca580a2b2638a6a0794046695`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:40:29 GMT
ADD file:0b6fc66d778d0cd8ae8b17b92945d98cc34f9c7008cda864ed0a54b5e40b9cb0 in / 
# Wed, 11 Oct 2023 17:40:32 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:09:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:10:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:501a599c15b6def048b2e00cfdf6c658061c00a504305ef2075fb1009a62c1e2`  
		Last Modified: Wed, 11 Oct 2023 17:45:01 GMT  
		Size: 50.6 MB (50600791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf9d6abbf47f32cac71cefb6f7233e5f700d4f6f941ca631e29947c5f1df955`  
		Last Modified: Wed, 11 Oct 2023 18:21:57 GMT  
		Size: 24.9 MB (24887201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1693c4d42b110c48ad84138aa8c91e1aeffbed6ca630f12495f711b89609823`  
		Last Modified: Wed, 11 Oct 2023 18:22:27 GMT  
		Size: 66.0 MB (65984002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:978fa0881d84f169ef3b182a55614b8c003440bfc7daff138acec86929b33f45
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.0 MB (135971603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:399ffe5bc61d49dc80a6a20678665009b14d5784ffd8ec66bd758ded95515def`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:48:50 GMT
ADD file:b081db8d48290ef5b5f477edb85d8f04d62a6995ec09bdb516d66dbe19b98137 in / 
# Wed, 11 Oct 2023 17:48:55 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:19:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:20:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:54dda4e4d31846b7324172a7fda3d0bdc7d8a2105ab27e9a92c2db43f35f9e5d`  
		Last Modified: Wed, 11 Oct 2023 17:59:53 GMT  
		Size: 49.6 MB (49569257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370a64ae3420fd85a23128ef46431df034f9038821764a14bb436272a1345505`  
		Last Modified: Wed, 11 Oct 2023 23:55:20 GMT  
		Size: 23.4 MB (23439567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c19b06553268b2cbcf576e075fdb1ac8c430154167258bcd4f925d5938117659`  
		Last Modified: Wed, 11 Oct 2023 23:56:13 GMT  
		Size: 63.0 MB (62962779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:e7774041231cd8297000ad9f73ba035a8098f870ab9e5935bf9e659d61dd0b02
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.9 MB (148860554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eff06503f2fa76d78d36cfb0c68c5ebb59ed3780f372aec67e688ba57c8afda9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:44:01 GMT
ADD file:ed515e1aef8321271c6544e30cbeb31257e9640979e8f68a9e490cb25d3525fd in / 
# Wed, 11 Oct 2023 17:44:04 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:14:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:15:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f137383853e717724a59e86aa526d31eabb4a5d45a259cd1ade68d93b3f45ae9`  
		Last Modified: Wed, 11 Oct 2023 17:49:27 GMT  
		Size: 53.6 MB (53575984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da754908592cac64ca75d9cdc8c43a4a396901108de4adae61bd92937de4f65`  
		Last Modified: Wed, 11 Oct 2023 18:36:14 GMT  
		Size: 25.7 MB (25700026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524b67dc97fb52dd33f61fe12da424874443bb200789c7cfde14425f85938f54`  
		Last Modified: Wed, 11 Oct 2023 18:36:46 GMT  
		Size: 69.6 MB (69584544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:198224f3809fdab1ffa595ddb0d788d97dec1c41556a1a5e913b711ec6ccdaab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.1 MB (135122600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8fda4e35a32e1c513adb4a70b998c8a77f96ac52d6a7c94f6f085b1d1995b8e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:50:07 GMT
ADD file:2dc117136732884ad4b058065700dd66cc49d6ce56b0fdbb672915e3ad8adb84 in / 
# Wed, 11 Oct 2023 17:50:10 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:51:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:52:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ad5e374600bf40a929dfe51e52737e4ca04aba83f499656760ba938841fb6552`  
		Last Modified: Wed, 11 Oct 2023 17:55:18 GMT  
		Size: 47.9 MB (47942934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6344f505670ce139b1b3f472749240f33304ec7535daae4a72913a6da08f304f`  
		Last Modified: Thu, 12 Oct 2023 00:33:20 GMT  
		Size: 24.0 MB (24046768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf2b4ce0798e7985dd88d10311ea2a2730812d4e10c9a8f24f564875c6cb617`  
		Last Modified: Thu, 12 Oct 2023 00:33:56 GMT  
		Size: 63.1 MB (63132898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:testing`

```console
$ docker pull buildpack-deps@sha256:8239859a271daf7278851d4c3cd498f74df238578a8e8520edd70989b2e41af0
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

### `buildpack-deps:testing` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:edb95280582c7f8e752a73d574ca1abc342e5bc5a5f2ef92081a4954d9792cea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **372.3 MB (372298722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1a943436b3fd42fef5e0c371807c92484ce675d9a6a64a80933eb3a37d93fa7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:37:30 GMT
ADD file:3c195cef0a6014fed28aeda30d2b0d0be58874ffbe451542fe4e63c3eedc06fc in / 
# Wed, 11 Oct 2023 18:37:31 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:26:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:26:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:27:21 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:af8900f491294a73f9d7586b4543b5c4231f20bf6977df5d89b7834baefa83db`  
		Last Modified: Wed, 11 Oct 2023 18:44:07 GMT  
		Size: 49.5 MB (49502119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9860fefe1e6f4f965e383c52355a47c3ede6024b0d14e721534d67d8e2f60c`  
		Last Modified: Thu, 12 Oct 2023 03:33:01 GMT  
		Size: 20.3 MB (20306460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c363cc8f9e708c06b320264321cf82790bbb5c5a0bcb7a2086eb0ad55100b76a`  
		Last Modified: Thu, 12 Oct 2023 03:33:19 GMT  
		Size: 65.3 MB (65319749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c9f6e673079413c621f78218ebf233447d31573fe408e0819d045255561f22`  
		Last Modified: Thu, 12 Oct 2023 03:33:56 GMT  
		Size: 237.2 MB (237170394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:b6b4d49af1a135a0b9700d1b31cbfe1fda5885fc88085318d20c6f5677f4c267
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **341.7 MB (341744224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94edfebf8754105d0b1e2b17ab0f403de0d9b5e649ba4c9796e5ddb66e339895`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:39:06 GMT
ADD file:a7de42b73a4591d75c2ea2f44cdd15d34ce24fa78ca8e57ac62e4fd3ffe2019d in / 
# Wed, 11 Oct 2023 17:39:07 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:12:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:12:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:13:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5a100e11229dc40f9cdcd25e779cd1f10bb500c44c5b9ae24abec0b01f4b26b1`  
		Last Modified: Wed, 11 Oct 2023 17:44:09 GMT  
		Size: 47.2 MB (47166046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13f41504078ef3db4155843c88e3eb49d76721ce77692685bb502799200ff810`  
		Last Modified: Wed, 11 Oct 2023 18:18:08 GMT  
		Size: 19.4 MB (19369976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262dceb7106ef55dcd198f1f5e689fd8eb7e9ed58de15831f3c0c75dfd041123`  
		Last Modified: Wed, 11 Oct 2023 18:18:28 GMT  
		Size: 62.8 MB (62838690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d46f6f51ff369aa4d880bd7e8a20e601a1c90225ae57a890f12a2a25e5f49ec`  
		Last Modified: Wed, 11 Oct 2023 18:19:07 GMT  
		Size: 212.4 MB (212369512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:2b6c7c93e9e7018fe73d1e0209fcdef997f21e5ee223861d822faf96b4c83a76
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.0 MB (323027351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dd3fee9a11cbd37c0b83b1cfa97cb93a0cfe42e4b7ee8430aacd624b64f0714`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:44:26 GMT
ADD file:69ac67070b211f2a7980ec82da00c1d97d41dc6fe979f892e741ce9b7c566a85 in / 
# Wed, 11 Oct 2023 17:44:26 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:53:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:53:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:54:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:53634a2dc8fdfb2e0bde3647302a9fd6183101ae18e9a9c89ec4d54909761e25`  
		Last Modified: Wed, 11 Oct 2023 17:50:55 GMT  
		Size: 45.0 MB (44954093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2152d48e2ff44fb8710e1613ee9c264a844d0354cce2b66cb656364b0908e2`  
		Last Modified: Thu, 12 Oct 2023 04:00:35 GMT  
		Size: 18.6 MB (18638360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f80ce051fa36ff87ccad2188b21b904002f911e804126f90381e2bfe700e56`  
		Last Modified: Thu, 12 Oct 2023 04:00:54 GMT  
		Size: 60.4 MB (60436364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a5d2e8e2e71cd8cbc1b0978188876c25d2401bddd94c865e96ef9fa522386c`  
		Last Modified: Thu, 12 Oct 2023 04:01:32 GMT  
		Size: 199.0 MB (198998534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:080672a6e364a27dc74f4ec29e73403740d0faa2676e8c119a74d82d8156d9a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **363.5 MB (363518845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7225dc2374bb409fec886a4babdb54f6e8707be41fd604029d5b36036471ecda`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:26:37 GMT
ADD file:ae967b7faba93d8a00f97f28b4d720835a90a27fe53b2f278072893f4cdaa8e7 in / 
# Wed, 11 Oct 2023 18:26:38 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:51:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:51:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:52:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ddf19dd473b427de200cf2b123540cd1dce2dcb51aeeb4a1359b7f954dc951ba`  
		Last Modified: Wed, 11 Oct 2023 18:32:45 GMT  
		Size: 49.5 MB (49505530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3234e169293a5a7c5d4630e4d414fffc649556678901730a692ba3b43cd5e618`  
		Last Modified: Wed, 11 Oct 2023 19:57:45 GMT  
		Size: 20.1 MB (20110046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71bac299e7b4e42a2756046d77fc625e1dc632615808cd1ec6bbcc2d48bf4f5`  
		Last Modified: Wed, 11 Oct 2023 19:58:01 GMT  
		Size: 65.4 MB (65405981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd31d1b7c77e861f5a1738daaf94715bed1e46ce9d29312378210f37d36a0041`  
		Last Modified: Wed, 11 Oct 2023 19:58:31 GMT  
		Size: 228.5 MB (228497288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; 386

```console
$ docker pull buildpack-deps@sha256:994ef7ea0528ecf13af562253a56f73215611d917ab27a646754b376219684c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **377.6 MB (377583489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8687b806f3edf6acdd139dc20b84f6944f4c0dd93ccea4d071e0dfd78397f5b5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:43:20 GMT
ADD file:ad97acda5f74778001aece2a9e280f0e58d2953cf8fdbd4740a049c4a595a225 in / 
# Wed, 11 Oct 2023 17:43:20 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:19:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:19:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:21:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce8ed34eaeffdeb7ac49225c6093f421b0005558aedb2b9c429731032d156621`  
		Last Modified: Wed, 11 Oct 2023 17:50:59 GMT  
		Size: 50.5 MB (50485846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f94c813421107d5ab710ec3329c2cd90f1b42da6b64e3d4ea8428fc7802b293`  
		Last Modified: Wed, 11 Oct 2023 18:27:57 GMT  
		Size: 20.9 MB (20886277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f264142306efbcccd3638b5a3b7788249da917c198eab1e97f89a7fb7178050`  
		Last Modified: Wed, 11 Oct 2023 18:28:21 GMT  
		Size: 67.1 MB (67089139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cdd865dd18cf6d9d37c1cf2104e99f5152965c92be6435b3e986f215cf6dc6`  
		Last Modified: Wed, 11 Oct 2023 18:29:15 GMT  
		Size: 239.1 MB (239122227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:842b71b4caf420c4377b561cf00b97cc6a8197bc33d15a4737e15b31abe79e34
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.0 MB (349022097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df4ec66a4877ae141ac96c8cbd31f79462471d543cd6361ed56e2ed57e1e7f8e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:56:15 GMT
ADD file:29bed270e296c5a95f2141f114580e0f25c1040c03609fa632757a8e48ec43fd in / 
# Wed, 11 Oct 2023 17:56:22 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:46:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:48:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:54:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f0d54eafe706e7144ea10a18a0abaa975cb4f7f92fd40e292f388c2b1321a794`  
		Last Modified: Wed, 11 Oct 2023 18:07:41 GMT  
		Size: 49.3 MB (49301729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5204f5199336e47ca287487c83b254ad7b0260c5bf568e92c8927077786ee91c`  
		Last Modified: Thu, 12 Oct 2023 00:05:30 GMT  
		Size: 19.6 MB (19593645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf370881cf98cc9a8acbbacf482b90a7a2d7f3a1d96216bd4d6b824f2814f5c`  
		Last Modified: Thu, 12 Oct 2023 00:06:22 GMT  
		Size: 64.1 MB (64135686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a05c74c2f9b1e7dbea41a67c427a2bbb28c1d0773bb04df36a32be1367db1717`  
		Last Modified: Thu, 12 Oct 2023 00:08:49 GMT  
		Size: 216.0 MB (215991037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:309bfd6b1b1b3855702980edcb586bc26ba049db4463943b23153879f9c6eeec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **384.4 MB (384351616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:751aaaeb8b4738691d1aaf012e3cb97d29e306dac0ff37ad139457c8d1c8c919`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:47:23 GMT
ADD file:24d4df221ce118a8059e0559a8bb2d715512fa6f5b15cd1397dbc177ceaa1bfd in / 
# Wed, 11 Oct 2023 17:47:26 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:30:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:31:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:34:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:93b578febbe769059c90eaa91e9dc027d172e6088856c2c52dc3e26dfdf01d4c`  
		Last Modified: Wed, 11 Oct 2023 17:54:24 GMT  
		Size: 53.4 MB (53418134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:576f9c6569231cdc2bf492ed27ab8c980261301252c26c4d6fcf8dec4fa4de9b`  
		Last Modified: Wed, 11 Oct 2023 18:41:22 GMT  
		Size: 21.6 MB (21644083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86429c6121c1cef63b4087b6359567a0aa3be523db5603dc673793266a48e8c4`  
		Last Modified: Wed, 11 Oct 2023 18:41:50 GMT  
		Size: 70.8 MB (70768983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61d96d5ef85833f9afe41198588301802855414f4a727cccf6ccd0e7de39ad1`  
		Last Modified: Wed, 11 Oct 2023 18:42:56 GMT  
		Size: 238.5 MB (238520416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:ba95984ed5c555b2ad5623c370c426debc4e8604fd1dafd24b572c0b4457b046
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **345.1 MB (345094462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a45d57e5a00a8e982793da9cfda9e0c832626c573f7c77e3dc87604cf44eb4c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:53:11 GMT
ADD file:7f7d0fe596110ed400f2bbc2fe6edf5716a5a62332062c86009df0df0cc0a257 in / 
# Wed, 11 Oct 2023 17:53:14 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 00:25:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 00:26:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 00:30:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3f47ccc9a5d62eac06dcd9bcbdf51b3bf5f494156a2c21d58d93d11f5261baf4`  
		Last Modified: Wed, 11 Oct 2023 18:01:45 GMT  
		Size: 48.9 MB (48924346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:659ce526b11a7e72319632cba55fb2631fe06f2d042501bcb6fd357be98825e4`  
		Last Modified: Thu, 12 Oct 2023 00:38:24 GMT  
		Size: 20.0 MB (20041463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb87df3b4ff93b8ee1589ac6dee47871cab5b94a7b2b411694cada1830b9793`  
		Last Modified: Thu, 12 Oct 2023 00:38:56 GMT  
		Size: 66.2 MB (66208891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adbe22ce87c5d9b87e39f49a34b4eae9702adf68f91c79686c409a142dd8f816`  
		Last Modified: Thu, 12 Oct 2023 00:39:28 GMT  
		Size: 209.9 MB (209919762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:testing-curl`

```console
$ docker pull buildpack-deps@sha256:e23b3798e79c0cea4f4b6f51364aa68a70db6b9e03c6204d8ff820469b71d4ce
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

### `buildpack-deps:testing-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:b3748cda7b913aacef884543e86a9509f7b67b5573ad6b7d7fd1f46ed6c11097
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69808579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f2619a9a35cd4544f71519954bc9a964c5e4bb775a0af8292af79b8d260c331`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:37:30 GMT
ADD file:3c195cef0a6014fed28aeda30d2b0d0be58874ffbe451542fe4e63c3eedc06fc in / 
# Wed, 11 Oct 2023 18:37:31 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:26:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:af8900f491294a73f9d7586b4543b5c4231f20bf6977df5d89b7834baefa83db`  
		Last Modified: Wed, 11 Oct 2023 18:44:07 GMT  
		Size: 49.5 MB (49502119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9860fefe1e6f4f965e383c52355a47c3ede6024b0d14e721534d67d8e2f60c`  
		Last Modified: Thu, 12 Oct 2023 03:33:01 GMT  
		Size: 20.3 MB (20306460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:031cbfec3788de366368b6700cf07f976ca32f81b5388f71e97a642ceaf17d99
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66536022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfeb4d63e6a42cebf132eda2fade400016c56515b7ccc382acb28f0ffaf96207`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:39:06 GMT
ADD file:a7de42b73a4591d75c2ea2f44cdd15d34ce24fa78ca8e57ac62e4fd3ffe2019d in / 
# Wed, 11 Oct 2023 17:39:07 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:12:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5a100e11229dc40f9cdcd25e779cd1f10bb500c44c5b9ae24abec0b01f4b26b1`  
		Last Modified: Wed, 11 Oct 2023 17:44:09 GMT  
		Size: 47.2 MB (47166046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13f41504078ef3db4155843c88e3eb49d76721ce77692685bb502799200ff810`  
		Last Modified: Wed, 11 Oct 2023 18:18:08 GMT  
		Size: 19.4 MB (19369976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:0341d48d95c3e5a4d2c5a756bf9c02be5ac68c3f91d4d25430cb7e2b39f87798
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.6 MB (63592453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec3154dd1baa055cc85e3cde172b24a55a63577750ffcf2919f520810dfa4bc8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:44:26 GMT
ADD file:69ac67070b211f2a7980ec82da00c1d97d41dc6fe979f892e741ce9b7c566a85 in / 
# Wed, 11 Oct 2023 17:44:26 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:53:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:53634a2dc8fdfb2e0bde3647302a9fd6183101ae18e9a9c89ec4d54909761e25`  
		Last Modified: Wed, 11 Oct 2023 17:50:55 GMT  
		Size: 45.0 MB (44954093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2152d48e2ff44fb8710e1613ee9c264a844d0354cce2b66cb656364b0908e2`  
		Last Modified: Thu, 12 Oct 2023 04:00:35 GMT  
		Size: 18.6 MB (18638360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:9fbda31bfbc609c550daf14bef5f22d3f176104c0821d8ddfe4582837d5a85ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69615576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab0b60c14a1ee8b098f27d569ee70427ec60d1436140bb21e61e1e3ce0735f75`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:26:37 GMT
ADD file:ae967b7faba93d8a00f97f28b4d720835a90a27fe53b2f278072893f4cdaa8e7 in / 
# Wed, 11 Oct 2023 18:26:38 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:51:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ddf19dd473b427de200cf2b123540cd1dce2dcb51aeeb4a1359b7f954dc951ba`  
		Last Modified: Wed, 11 Oct 2023 18:32:45 GMT  
		Size: 49.5 MB (49505530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3234e169293a5a7c5d4630e4d414fffc649556678901730a692ba3b43cd5e618`  
		Last Modified: Wed, 11 Oct 2023 19:57:45 GMT  
		Size: 20.1 MB (20110046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:805dd0cb6d20f9293082e2731dee26c4189ba2e05e33a9f191a996164477f318
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.4 MB (71372123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92b67991ebfd3a67bfb234e83a7242703653494aeefd5471beb24c4e239b52a8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:43:20 GMT
ADD file:ad97acda5f74778001aece2a9e280f0e58d2953cf8fdbd4740a049c4a595a225 in / 
# Wed, 11 Oct 2023 17:43:20 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:19:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce8ed34eaeffdeb7ac49225c6093f421b0005558aedb2b9c429731032d156621`  
		Last Modified: Wed, 11 Oct 2023 17:50:59 GMT  
		Size: 50.5 MB (50485846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f94c813421107d5ab710ec3329c2cd90f1b42da6b64e3d4ea8428fc7802b293`  
		Last Modified: Wed, 11 Oct 2023 18:27:57 GMT  
		Size: 20.9 MB (20886277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:2f51f1238b9640b9e5ee718926672d0df20e00b0acbf2c2b311248148673bbc6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68895374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5db4384cd0f6fbbde63af84a9a7aba48e7ca88a8045c743733eb4c43414eed70`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:56:15 GMT
ADD file:29bed270e296c5a95f2141f114580e0f25c1040c03609fa632757a8e48ec43fd in / 
# Wed, 11 Oct 2023 17:56:22 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:46:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f0d54eafe706e7144ea10a18a0abaa975cb4f7f92fd40e292f388c2b1321a794`  
		Last Modified: Wed, 11 Oct 2023 18:07:41 GMT  
		Size: 49.3 MB (49301729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5204f5199336e47ca287487c83b254ad7b0260c5bf568e92c8927077786ee91c`  
		Last Modified: Thu, 12 Oct 2023 00:05:30 GMT  
		Size: 19.6 MB (19593645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:591e2f9c3b9c350ed8dba9ca0614e4c7b44b3610c178f9e4448c57ad5e3133b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75062217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdae9eab9b095c3c61aa347d6635f9ce2117099144c8bea9931d276e481f2711`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:47:23 GMT
ADD file:24d4df221ce118a8059e0559a8bb2d715512fa6f5b15cd1397dbc177ceaa1bfd in / 
# Wed, 11 Oct 2023 17:47:26 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:30:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:93b578febbe769059c90eaa91e9dc027d172e6088856c2c52dc3e26dfdf01d4c`  
		Last Modified: Wed, 11 Oct 2023 17:54:24 GMT  
		Size: 53.4 MB (53418134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:576f9c6569231cdc2bf492ed27ab8c980261301252c26c4d6fcf8dec4fa4de9b`  
		Last Modified: Wed, 11 Oct 2023 18:41:22 GMT  
		Size: 21.6 MB (21644083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:dce98873fc650b5ee64351ca6ac11454fe20bca0ec37aeca46e3f5eaebabcafd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (68965809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3887383a692e4e80043fe7ea299b03d5845a16f8d443c12d78177cdea73045e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:53:11 GMT
ADD file:7f7d0fe596110ed400f2bbc2fe6edf5716a5a62332062c86009df0df0cc0a257 in / 
# Wed, 11 Oct 2023 17:53:14 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 00:25:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3f47ccc9a5d62eac06dcd9bcbdf51b3bf5f494156a2c21d58d93d11f5261baf4`  
		Last Modified: Wed, 11 Oct 2023 18:01:45 GMT  
		Size: 48.9 MB (48924346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:659ce526b11a7e72319632cba55fb2631fe06f2d042501bcb6fd357be98825e4`  
		Last Modified: Thu, 12 Oct 2023 00:38:24 GMT  
		Size: 20.0 MB (20041463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:testing-scm`

```console
$ docker pull buildpack-deps@sha256:44ba27103cdeb4abe69f7e404555306ce5248a4f51d16a72418af0bfdd537a12
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

### `buildpack-deps:testing-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:bd7500ebabf1abc10b5af503dad44aa3b05f3f6eca4ef72caeeb8fda16485a94
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.1 MB (135128328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f347a88d4cc94ea5906a30d6318baef6923feaf2317fb5b5750ae55348560d52`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:37:30 GMT
ADD file:3c195cef0a6014fed28aeda30d2b0d0be58874ffbe451542fe4e63c3eedc06fc in / 
# Wed, 11 Oct 2023 18:37:31 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:26:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:26:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:af8900f491294a73f9d7586b4543b5c4231f20bf6977df5d89b7834baefa83db`  
		Last Modified: Wed, 11 Oct 2023 18:44:07 GMT  
		Size: 49.5 MB (49502119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9860fefe1e6f4f965e383c52355a47c3ede6024b0d14e721534d67d8e2f60c`  
		Last Modified: Thu, 12 Oct 2023 03:33:01 GMT  
		Size: 20.3 MB (20306460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c363cc8f9e708c06b320264321cf82790bbb5c5a0bcb7a2086eb0ad55100b76a`  
		Last Modified: Thu, 12 Oct 2023 03:33:19 GMT  
		Size: 65.3 MB (65319749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:0ebff169c1476a3a84b0ddec9c0d87c66ee5c9c7c790880727c23c2e387be6f8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.4 MB (129374712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bed6de9127d38f8a91bb4e3baec0e807c69c85ec95b3eb85617c79e5dfc8b6b2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:39:06 GMT
ADD file:a7de42b73a4591d75c2ea2f44cdd15d34ce24fa78ca8e57ac62e4fd3ffe2019d in / 
# Wed, 11 Oct 2023 17:39:07 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:12:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:12:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5a100e11229dc40f9cdcd25e779cd1f10bb500c44c5b9ae24abec0b01f4b26b1`  
		Last Modified: Wed, 11 Oct 2023 17:44:09 GMT  
		Size: 47.2 MB (47166046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13f41504078ef3db4155843c88e3eb49d76721ce77692685bb502799200ff810`  
		Last Modified: Wed, 11 Oct 2023 18:18:08 GMT  
		Size: 19.4 MB (19369976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262dceb7106ef55dcd198f1f5e689fd8eb7e9ed58de15831f3c0c75dfd041123`  
		Last Modified: Wed, 11 Oct 2023 18:18:28 GMT  
		Size: 62.8 MB (62838690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:85b21ba969054c1b0ab1fc5db729f54a2b8ef9e62258344568f916698d9947a8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.0 MB (124028817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89fe0a557548aa01429458a69c202a28e1d3771485ab683b5452453f2ecca967`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:44:26 GMT
ADD file:69ac67070b211f2a7980ec82da00c1d97d41dc6fe979f892e741ce9b7c566a85 in / 
# Wed, 11 Oct 2023 17:44:26 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:53:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:53:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:53634a2dc8fdfb2e0bde3647302a9fd6183101ae18e9a9c89ec4d54909761e25`  
		Last Modified: Wed, 11 Oct 2023 17:50:55 GMT  
		Size: 45.0 MB (44954093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2152d48e2ff44fb8710e1613ee9c264a844d0354cce2b66cb656364b0908e2`  
		Last Modified: Thu, 12 Oct 2023 04:00:35 GMT  
		Size: 18.6 MB (18638360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f80ce051fa36ff87ccad2188b21b904002f911e804126f90381e2bfe700e56`  
		Last Modified: Thu, 12 Oct 2023 04:00:54 GMT  
		Size: 60.4 MB (60436364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:5d9bcecf36028c9169e4f22dcfb0789845cf6523bd944dd55eab22dd5d4ba9aa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.0 MB (135021557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82b7c1249c50f4b3449269dc5abe7ee5c404db73aead5b7fe4b25aff61f441f6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:26:37 GMT
ADD file:ae967b7faba93d8a00f97f28b4d720835a90a27fe53b2f278072893f4cdaa8e7 in / 
# Wed, 11 Oct 2023 18:26:38 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:51:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:51:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ddf19dd473b427de200cf2b123540cd1dce2dcb51aeeb4a1359b7f954dc951ba`  
		Last Modified: Wed, 11 Oct 2023 18:32:45 GMT  
		Size: 49.5 MB (49505530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3234e169293a5a7c5d4630e4d414fffc649556678901730a692ba3b43cd5e618`  
		Last Modified: Wed, 11 Oct 2023 19:57:45 GMT  
		Size: 20.1 MB (20110046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71bac299e7b4e42a2756046d77fc625e1dc632615808cd1ec6bbcc2d48bf4f5`  
		Last Modified: Wed, 11 Oct 2023 19:58:01 GMT  
		Size: 65.4 MB (65405981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:c68a447d1f8f8a57fc43e7455aaaabda87e8fe5f7bb01f584d260efac38c75b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.5 MB (138461262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e178f98ad66d50e8c497cf5503dcda5d92cae0a761c41df1e7a2d0905b93549e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:43:20 GMT
ADD file:ad97acda5f74778001aece2a9e280f0e58d2953cf8fdbd4740a049c4a595a225 in / 
# Wed, 11 Oct 2023 17:43:20 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:19:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:19:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce8ed34eaeffdeb7ac49225c6093f421b0005558aedb2b9c429731032d156621`  
		Last Modified: Wed, 11 Oct 2023 17:50:59 GMT  
		Size: 50.5 MB (50485846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f94c813421107d5ab710ec3329c2cd90f1b42da6b64e3d4ea8428fc7802b293`  
		Last Modified: Wed, 11 Oct 2023 18:27:57 GMT  
		Size: 20.9 MB (20886277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f264142306efbcccd3638b5a3b7788249da917c198eab1e97f89a7fb7178050`  
		Last Modified: Wed, 11 Oct 2023 18:28:21 GMT  
		Size: 67.1 MB (67089139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:30a2cdeea3d62c9dd4c0e562792d7aa77f1039eed2ee98069e6905a96ca15261
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.0 MB (133031060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36fb20dd0a09ce4ea2be6a3e98e09f84f36053e6646b0f5e76821b4998265f5c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:56:15 GMT
ADD file:29bed270e296c5a95f2141f114580e0f25c1040c03609fa632757a8e48ec43fd in / 
# Wed, 11 Oct 2023 17:56:22 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:46:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:48:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f0d54eafe706e7144ea10a18a0abaa975cb4f7f92fd40e292f388c2b1321a794`  
		Last Modified: Wed, 11 Oct 2023 18:07:41 GMT  
		Size: 49.3 MB (49301729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5204f5199336e47ca287487c83b254ad7b0260c5bf568e92c8927077786ee91c`  
		Last Modified: Thu, 12 Oct 2023 00:05:30 GMT  
		Size: 19.6 MB (19593645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf370881cf98cc9a8acbbacf482b90a7a2d7f3a1d96216bd4d6b824f2814f5c`  
		Last Modified: Thu, 12 Oct 2023 00:06:22 GMT  
		Size: 64.1 MB (64135686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d2b8ff9957833a55d2e2a2acb81c8ded45ed8f7cfdf2e9256ef9a8a8e4b699c5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.8 MB (145831200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f52eb015b31afb09fcb86b0b390e24b827066a43b906b3574e645b2a65406697`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:47:23 GMT
ADD file:24d4df221ce118a8059e0559a8bb2d715512fa6f5b15cd1397dbc177ceaa1bfd in / 
# Wed, 11 Oct 2023 17:47:26 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:30:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:31:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:93b578febbe769059c90eaa91e9dc027d172e6088856c2c52dc3e26dfdf01d4c`  
		Last Modified: Wed, 11 Oct 2023 17:54:24 GMT  
		Size: 53.4 MB (53418134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:576f9c6569231cdc2bf492ed27ab8c980261301252c26c4d6fcf8dec4fa4de9b`  
		Last Modified: Wed, 11 Oct 2023 18:41:22 GMT  
		Size: 21.6 MB (21644083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86429c6121c1cef63b4087b6359567a0aa3be523db5603dc673793266a48e8c4`  
		Last Modified: Wed, 11 Oct 2023 18:41:50 GMT  
		Size: 70.8 MB (70768983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:d56b43941a28de4537dd79f70f50cdf39dd28ebab1806ed5a4fddf6ffabcbe5e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.2 MB (135174700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5db68d1b36c00eab98e91d36cd34783d7f739259d8c82262bada484ee4590aa9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:53:11 GMT
ADD file:7f7d0fe596110ed400f2bbc2fe6edf5716a5a62332062c86009df0df0cc0a257 in / 
# Wed, 11 Oct 2023 17:53:14 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 00:25:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 00:26:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3f47ccc9a5d62eac06dcd9bcbdf51b3bf5f494156a2c21d58d93d11f5261baf4`  
		Last Modified: Wed, 11 Oct 2023 18:01:45 GMT  
		Size: 48.9 MB (48924346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:659ce526b11a7e72319632cba55fb2631fe06f2d042501bcb6fd357be98825e4`  
		Last Modified: Thu, 12 Oct 2023 00:38:24 GMT  
		Size: 20.0 MB (20041463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb87df3b4ff93b8ee1589ac6dee47871cab5b94a7b2b411694cada1830b9793`  
		Last Modified: Thu, 12 Oct 2023 00:38:56 GMT  
		Size: 66.2 MB (66208891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:trixie`

```console
$ docker pull buildpack-deps@sha256:8239859a271daf7278851d4c3cd498f74df238578a8e8520edd70989b2e41af0
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
$ docker pull buildpack-deps@sha256:edb95280582c7f8e752a73d574ca1abc342e5bc5a5f2ef92081a4954d9792cea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **372.3 MB (372298722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1a943436b3fd42fef5e0c371807c92484ce675d9a6a64a80933eb3a37d93fa7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:37:30 GMT
ADD file:3c195cef0a6014fed28aeda30d2b0d0be58874ffbe451542fe4e63c3eedc06fc in / 
# Wed, 11 Oct 2023 18:37:31 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:26:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:26:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:27:21 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:af8900f491294a73f9d7586b4543b5c4231f20bf6977df5d89b7834baefa83db`  
		Last Modified: Wed, 11 Oct 2023 18:44:07 GMT  
		Size: 49.5 MB (49502119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9860fefe1e6f4f965e383c52355a47c3ede6024b0d14e721534d67d8e2f60c`  
		Last Modified: Thu, 12 Oct 2023 03:33:01 GMT  
		Size: 20.3 MB (20306460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c363cc8f9e708c06b320264321cf82790bbb5c5a0bcb7a2086eb0ad55100b76a`  
		Last Modified: Thu, 12 Oct 2023 03:33:19 GMT  
		Size: 65.3 MB (65319749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c9f6e673079413c621f78218ebf233447d31573fe408e0819d045255561f22`  
		Last Modified: Thu, 12 Oct 2023 03:33:56 GMT  
		Size: 237.2 MB (237170394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:b6b4d49af1a135a0b9700d1b31cbfe1fda5885fc88085318d20c6f5677f4c267
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **341.7 MB (341744224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94edfebf8754105d0b1e2b17ab0f403de0d9b5e649ba4c9796e5ddb66e339895`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:39:06 GMT
ADD file:a7de42b73a4591d75c2ea2f44cdd15d34ce24fa78ca8e57ac62e4fd3ffe2019d in / 
# Wed, 11 Oct 2023 17:39:07 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:12:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:12:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:13:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5a100e11229dc40f9cdcd25e779cd1f10bb500c44c5b9ae24abec0b01f4b26b1`  
		Last Modified: Wed, 11 Oct 2023 17:44:09 GMT  
		Size: 47.2 MB (47166046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13f41504078ef3db4155843c88e3eb49d76721ce77692685bb502799200ff810`  
		Last Modified: Wed, 11 Oct 2023 18:18:08 GMT  
		Size: 19.4 MB (19369976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262dceb7106ef55dcd198f1f5e689fd8eb7e9ed58de15831f3c0c75dfd041123`  
		Last Modified: Wed, 11 Oct 2023 18:18:28 GMT  
		Size: 62.8 MB (62838690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d46f6f51ff369aa4d880bd7e8a20e601a1c90225ae57a890f12a2a25e5f49ec`  
		Last Modified: Wed, 11 Oct 2023 18:19:07 GMT  
		Size: 212.4 MB (212369512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:2b6c7c93e9e7018fe73d1e0209fcdef997f21e5ee223861d822faf96b4c83a76
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.0 MB (323027351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7dd3fee9a11cbd37c0b83b1cfa97cb93a0cfe42e4b7ee8430aacd624b64f0714`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:44:26 GMT
ADD file:69ac67070b211f2a7980ec82da00c1d97d41dc6fe979f892e741ce9b7c566a85 in / 
# Wed, 11 Oct 2023 17:44:26 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:53:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:53:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:54:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:53634a2dc8fdfb2e0bde3647302a9fd6183101ae18e9a9c89ec4d54909761e25`  
		Last Modified: Wed, 11 Oct 2023 17:50:55 GMT  
		Size: 45.0 MB (44954093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2152d48e2ff44fb8710e1613ee9c264a844d0354cce2b66cb656364b0908e2`  
		Last Modified: Thu, 12 Oct 2023 04:00:35 GMT  
		Size: 18.6 MB (18638360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f80ce051fa36ff87ccad2188b21b904002f911e804126f90381e2bfe700e56`  
		Last Modified: Thu, 12 Oct 2023 04:00:54 GMT  
		Size: 60.4 MB (60436364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a5d2e8e2e71cd8cbc1b0978188876c25d2401bddd94c865e96ef9fa522386c`  
		Last Modified: Thu, 12 Oct 2023 04:01:32 GMT  
		Size: 199.0 MB (198998534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:080672a6e364a27dc74f4ec29e73403740d0faa2676e8c119a74d82d8156d9a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **363.5 MB (363518845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7225dc2374bb409fec886a4babdb54f6e8707be41fd604029d5b36036471ecda`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:26:37 GMT
ADD file:ae967b7faba93d8a00f97f28b4d720835a90a27fe53b2f278072893f4cdaa8e7 in / 
# Wed, 11 Oct 2023 18:26:38 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:51:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:51:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:52:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ddf19dd473b427de200cf2b123540cd1dce2dcb51aeeb4a1359b7f954dc951ba`  
		Last Modified: Wed, 11 Oct 2023 18:32:45 GMT  
		Size: 49.5 MB (49505530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3234e169293a5a7c5d4630e4d414fffc649556678901730a692ba3b43cd5e618`  
		Last Modified: Wed, 11 Oct 2023 19:57:45 GMT  
		Size: 20.1 MB (20110046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71bac299e7b4e42a2756046d77fc625e1dc632615808cd1ec6bbcc2d48bf4f5`  
		Last Modified: Wed, 11 Oct 2023 19:58:01 GMT  
		Size: 65.4 MB (65405981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd31d1b7c77e861f5a1738daaf94715bed1e46ce9d29312378210f37d36a0041`  
		Last Modified: Wed, 11 Oct 2023 19:58:31 GMT  
		Size: 228.5 MB (228497288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie` - linux; 386

```console
$ docker pull buildpack-deps@sha256:994ef7ea0528ecf13af562253a56f73215611d917ab27a646754b376219684c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **377.6 MB (377583489 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8687b806f3edf6acdd139dc20b84f6944f4c0dd93ccea4d071e0dfd78397f5b5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:43:20 GMT
ADD file:ad97acda5f74778001aece2a9e280f0e58d2953cf8fdbd4740a049c4a595a225 in / 
# Wed, 11 Oct 2023 17:43:20 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:19:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:19:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:21:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce8ed34eaeffdeb7ac49225c6093f421b0005558aedb2b9c429731032d156621`  
		Last Modified: Wed, 11 Oct 2023 17:50:59 GMT  
		Size: 50.5 MB (50485846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f94c813421107d5ab710ec3329c2cd90f1b42da6b64e3d4ea8428fc7802b293`  
		Last Modified: Wed, 11 Oct 2023 18:27:57 GMT  
		Size: 20.9 MB (20886277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f264142306efbcccd3638b5a3b7788249da917c198eab1e97f89a7fb7178050`  
		Last Modified: Wed, 11 Oct 2023 18:28:21 GMT  
		Size: 67.1 MB (67089139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27cdd865dd18cf6d9d37c1cf2104e99f5152965c92be6435b3e986f215cf6dc6`  
		Last Modified: Wed, 11 Oct 2023 18:29:15 GMT  
		Size: 239.1 MB (239122227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:842b71b4caf420c4377b561cf00b97cc6a8197bc33d15a4737e15b31abe79e34
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.0 MB (349022097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df4ec66a4877ae141ac96c8cbd31f79462471d543cd6361ed56e2ed57e1e7f8e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:56:15 GMT
ADD file:29bed270e296c5a95f2141f114580e0f25c1040c03609fa632757a8e48ec43fd in / 
# Wed, 11 Oct 2023 17:56:22 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:46:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:48:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:54:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f0d54eafe706e7144ea10a18a0abaa975cb4f7f92fd40e292f388c2b1321a794`  
		Last Modified: Wed, 11 Oct 2023 18:07:41 GMT  
		Size: 49.3 MB (49301729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5204f5199336e47ca287487c83b254ad7b0260c5bf568e92c8927077786ee91c`  
		Last Modified: Thu, 12 Oct 2023 00:05:30 GMT  
		Size: 19.6 MB (19593645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf370881cf98cc9a8acbbacf482b90a7a2d7f3a1d96216bd4d6b824f2814f5c`  
		Last Modified: Thu, 12 Oct 2023 00:06:22 GMT  
		Size: 64.1 MB (64135686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a05c74c2f9b1e7dbea41a67c427a2bbb28c1d0773bb04df36a32be1367db1717`  
		Last Modified: Thu, 12 Oct 2023 00:08:49 GMT  
		Size: 216.0 MB (215991037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:309bfd6b1b1b3855702980edcb586bc26ba049db4463943b23153879f9c6eeec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **384.4 MB (384351616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:751aaaeb8b4738691d1aaf012e3cb97d29e306dac0ff37ad139457c8d1c8c919`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:47:23 GMT
ADD file:24d4df221ce118a8059e0559a8bb2d715512fa6f5b15cd1397dbc177ceaa1bfd in / 
# Wed, 11 Oct 2023 17:47:26 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:30:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:31:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:34:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:93b578febbe769059c90eaa91e9dc027d172e6088856c2c52dc3e26dfdf01d4c`  
		Last Modified: Wed, 11 Oct 2023 17:54:24 GMT  
		Size: 53.4 MB (53418134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:576f9c6569231cdc2bf492ed27ab8c980261301252c26c4d6fcf8dec4fa4de9b`  
		Last Modified: Wed, 11 Oct 2023 18:41:22 GMT  
		Size: 21.6 MB (21644083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86429c6121c1cef63b4087b6359567a0aa3be523db5603dc673793266a48e8c4`  
		Last Modified: Wed, 11 Oct 2023 18:41:50 GMT  
		Size: 70.8 MB (70768983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61d96d5ef85833f9afe41198588301802855414f4a727cccf6ccd0e7de39ad1`  
		Last Modified: Wed, 11 Oct 2023 18:42:56 GMT  
		Size: 238.5 MB (238520416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:ba95984ed5c555b2ad5623c370c426debc4e8604fd1dafd24b572c0b4457b046
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **345.1 MB (345094462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a45d57e5a00a8e982793da9cfda9e0c832626c573f7c77e3dc87604cf44eb4c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:53:11 GMT
ADD file:7f7d0fe596110ed400f2bbc2fe6edf5716a5a62332062c86009df0df0cc0a257 in / 
# Wed, 11 Oct 2023 17:53:14 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 00:25:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 00:26:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 00:30:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3f47ccc9a5d62eac06dcd9bcbdf51b3bf5f494156a2c21d58d93d11f5261baf4`  
		Last Modified: Wed, 11 Oct 2023 18:01:45 GMT  
		Size: 48.9 MB (48924346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:659ce526b11a7e72319632cba55fb2631fe06f2d042501bcb6fd357be98825e4`  
		Last Modified: Thu, 12 Oct 2023 00:38:24 GMT  
		Size: 20.0 MB (20041463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb87df3b4ff93b8ee1589ac6dee47871cab5b94a7b2b411694cada1830b9793`  
		Last Modified: Thu, 12 Oct 2023 00:38:56 GMT  
		Size: 66.2 MB (66208891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adbe22ce87c5d9b87e39f49a34b4eae9702adf68f91c79686c409a142dd8f816`  
		Last Modified: Thu, 12 Oct 2023 00:39:28 GMT  
		Size: 209.9 MB (209919762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:trixie-curl`

```console
$ docker pull buildpack-deps@sha256:e23b3798e79c0cea4f4b6f51364aa68a70db6b9e03c6204d8ff820469b71d4ce
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

### `buildpack-deps:trixie-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:b3748cda7b913aacef884543e86a9509f7b67b5573ad6b7d7fd1f46ed6c11097
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69808579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f2619a9a35cd4544f71519954bc9a964c5e4bb775a0af8292af79b8d260c331`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:37:30 GMT
ADD file:3c195cef0a6014fed28aeda30d2b0d0be58874ffbe451542fe4e63c3eedc06fc in / 
# Wed, 11 Oct 2023 18:37:31 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:26:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:af8900f491294a73f9d7586b4543b5c4231f20bf6977df5d89b7834baefa83db`  
		Last Modified: Wed, 11 Oct 2023 18:44:07 GMT  
		Size: 49.5 MB (49502119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9860fefe1e6f4f965e383c52355a47c3ede6024b0d14e721534d67d8e2f60c`  
		Last Modified: Thu, 12 Oct 2023 03:33:01 GMT  
		Size: 20.3 MB (20306460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:031cbfec3788de366368b6700cf07f976ca32f81b5388f71e97a642ceaf17d99
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66536022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfeb4d63e6a42cebf132eda2fade400016c56515b7ccc382acb28f0ffaf96207`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:39:06 GMT
ADD file:a7de42b73a4591d75c2ea2f44cdd15d34ce24fa78ca8e57ac62e4fd3ffe2019d in / 
# Wed, 11 Oct 2023 17:39:07 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:12:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5a100e11229dc40f9cdcd25e779cd1f10bb500c44c5b9ae24abec0b01f4b26b1`  
		Last Modified: Wed, 11 Oct 2023 17:44:09 GMT  
		Size: 47.2 MB (47166046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13f41504078ef3db4155843c88e3eb49d76721ce77692685bb502799200ff810`  
		Last Modified: Wed, 11 Oct 2023 18:18:08 GMT  
		Size: 19.4 MB (19369976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:0341d48d95c3e5a4d2c5a756bf9c02be5ac68c3f91d4d25430cb7e2b39f87798
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.6 MB (63592453 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec3154dd1baa055cc85e3cde172b24a55a63577750ffcf2919f520810dfa4bc8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:44:26 GMT
ADD file:69ac67070b211f2a7980ec82da00c1d97d41dc6fe979f892e741ce9b7c566a85 in / 
# Wed, 11 Oct 2023 17:44:26 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:53:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:53634a2dc8fdfb2e0bde3647302a9fd6183101ae18e9a9c89ec4d54909761e25`  
		Last Modified: Wed, 11 Oct 2023 17:50:55 GMT  
		Size: 45.0 MB (44954093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2152d48e2ff44fb8710e1613ee9c264a844d0354cce2b66cb656364b0908e2`  
		Last Modified: Thu, 12 Oct 2023 04:00:35 GMT  
		Size: 18.6 MB (18638360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:9fbda31bfbc609c550daf14bef5f22d3f176104c0821d8ddfe4582837d5a85ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69615576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab0b60c14a1ee8b098f27d569ee70427ec60d1436140bb21e61e1e3ce0735f75`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:26:37 GMT
ADD file:ae967b7faba93d8a00f97f28b4d720835a90a27fe53b2f278072893f4cdaa8e7 in / 
# Wed, 11 Oct 2023 18:26:38 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:51:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ddf19dd473b427de200cf2b123540cd1dce2dcb51aeeb4a1359b7f954dc951ba`  
		Last Modified: Wed, 11 Oct 2023 18:32:45 GMT  
		Size: 49.5 MB (49505530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3234e169293a5a7c5d4630e4d414fffc649556678901730a692ba3b43cd5e618`  
		Last Modified: Wed, 11 Oct 2023 19:57:45 GMT  
		Size: 20.1 MB (20110046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:805dd0cb6d20f9293082e2731dee26c4189ba2e05e33a9f191a996164477f318
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.4 MB (71372123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92b67991ebfd3a67bfb234e83a7242703653494aeefd5471beb24c4e239b52a8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:43:20 GMT
ADD file:ad97acda5f74778001aece2a9e280f0e58d2953cf8fdbd4740a049c4a595a225 in / 
# Wed, 11 Oct 2023 17:43:20 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:19:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce8ed34eaeffdeb7ac49225c6093f421b0005558aedb2b9c429731032d156621`  
		Last Modified: Wed, 11 Oct 2023 17:50:59 GMT  
		Size: 50.5 MB (50485846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f94c813421107d5ab710ec3329c2cd90f1b42da6b64e3d4ea8428fc7802b293`  
		Last Modified: Wed, 11 Oct 2023 18:27:57 GMT  
		Size: 20.9 MB (20886277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:2f51f1238b9640b9e5ee718926672d0df20e00b0acbf2c2b311248148673bbc6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68895374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5db4384cd0f6fbbde63af84a9a7aba48e7ca88a8045c743733eb4c43414eed70`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:56:15 GMT
ADD file:29bed270e296c5a95f2141f114580e0f25c1040c03609fa632757a8e48ec43fd in / 
# Wed, 11 Oct 2023 17:56:22 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:46:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f0d54eafe706e7144ea10a18a0abaa975cb4f7f92fd40e292f388c2b1321a794`  
		Last Modified: Wed, 11 Oct 2023 18:07:41 GMT  
		Size: 49.3 MB (49301729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5204f5199336e47ca287487c83b254ad7b0260c5bf568e92c8927077786ee91c`  
		Last Modified: Thu, 12 Oct 2023 00:05:30 GMT  
		Size: 19.6 MB (19593645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:591e2f9c3b9c350ed8dba9ca0614e4c7b44b3610c178f9e4448c57ad5e3133b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75062217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdae9eab9b095c3c61aa347d6635f9ce2117099144c8bea9931d276e481f2711`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:47:23 GMT
ADD file:24d4df221ce118a8059e0559a8bb2d715512fa6f5b15cd1397dbc177ceaa1bfd in / 
# Wed, 11 Oct 2023 17:47:26 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:30:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:93b578febbe769059c90eaa91e9dc027d172e6088856c2c52dc3e26dfdf01d4c`  
		Last Modified: Wed, 11 Oct 2023 17:54:24 GMT  
		Size: 53.4 MB (53418134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:576f9c6569231cdc2bf492ed27ab8c980261301252c26c4d6fcf8dec4fa4de9b`  
		Last Modified: Wed, 11 Oct 2023 18:41:22 GMT  
		Size: 21.6 MB (21644083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:dce98873fc650b5ee64351ca6ac11454fe20bca0ec37aeca46e3f5eaebabcafd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (68965809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3887383a692e4e80043fe7ea299b03d5845a16f8d443c12d78177cdea73045e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:53:11 GMT
ADD file:7f7d0fe596110ed400f2bbc2fe6edf5716a5a62332062c86009df0df0cc0a257 in / 
# Wed, 11 Oct 2023 17:53:14 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 00:25:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3f47ccc9a5d62eac06dcd9bcbdf51b3bf5f494156a2c21d58d93d11f5261baf4`  
		Last Modified: Wed, 11 Oct 2023 18:01:45 GMT  
		Size: 48.9 MB (48924346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:659ce526b11a7e72319632cba55fb2631fe06f2d042501bcb6fd357be98825e4`  
		Last Modified: Thu, 12 Oct 2023 00:38:24 GMT  
		Size: 20.0 MB (20041463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:trixie-scm`

```console
$ docker pull buildpack-deps@sha256:44ba27103cdeb4abe69f7e404555306ce5248a4f51d16a72418af0bfdd537a12
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

### `buildpack-deps:trixie-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:bd7500ebabf1abc10b5af503dad44aa3b05f3f6eca4ef72caeeb8fda16485a94
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.1 MB (135128328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f347a88d4cc94ea5906a30d6318baef6923feaf2317fb5b5750ae55348560d52`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:37:30 GMT
ADD file:3c195cef0a6014fed28aeda30d2b0d0be58874ffbe451542fe4e63c3eedc06fc in / 
# Wed, 11 Oct 2023 18:37:31 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:26:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:26:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:af8900f491294a73f9d7586b4543b5c4231f20bf6977df5d89b7834baefa83db`  
		Last Modified: Wed, 11 Oct 2023 18:44:07 GMT  
		Size: 49.5 MB (49502119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9860fefe1e6f4f965e383c52355a47c3ede6024b0d14e721534d67d8e2f60c`  
		Last Modified: Thu, 12 Oct 2023 03:33:01 GMT  
		Size: 20.3 MB (20306460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c363cc8f9e708c06b320264321cf82790bbb5c5a0bcb7a2086eb0ad55100b76a`  
		Last Modified: Thu, 12 Oct 2023 03:33:19 GMT  
		Size: 65.3 MB (65319749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:0ebff169c1476a3a84b0ddec9c0d87c66ee5c9c7c790880727c23c2e387be6f8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.4 MB (129374712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bed6de9127d38f8a91bb4e3baec0e807c69c85ec95b3eb85617c79e5dfc8b6b2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:39:06 GMT
ADD file:a7de42b73a4591d75c2ea2f44cdd15d34ce24fa78ca8e57ac62e4fd3ffe2019d in / 
# Wed, 11 Oct 2023 17:39:07 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:12:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:12:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5a100e11229dc40f9cdcd25e779cd1f10bb500c44c5b9ae24abec0b01f4b26b1`  
		Last Modified: Wed, 11 Oct 2023 17:44:09 GMT  
		Size: 47.2 MB (47166046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13f41504078ef3db4155843c88e3eb49d76721ce77692685bb502799200ff810`  
		Last Modified: Wed, 11 Oct 2023 18:18:08 GMT  
		Size: 19.4 MB (19369976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262dceb7106ef55dcd198f1f5e689fd8eb7e9ed58de15831f3c0c75dfd041123`  
		Last Modified: Wed, 11 Oct 2023 18:18:28 GMT  
		Size: 62.8 MB (62838690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:85b21ba969054c1b0ab1fc5db729f54a2b8ef9e62258344568f916698d9947a8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.0 MB (124028817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89fe0a557548aa01429458a69c202a28e1d3771485ab683b5452453f2ecca967`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:44:26 GMT
ADD file:69ac67070b211f2a7980ec82da00c1d97d41dc6fe979f892e741ce9b7c566a85 in / 
# Wed, 11 Oct 2023 17:44:26 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:53:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:53:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:53634a2dc8fdfb2e0bde3647302a9fd6183101ae18e9a9c89ec4d54909761e25`  
		Last Modified: Wed, 11 Oct 2023 17:50:55 GMT  
		Size: 45.0 MB (44954093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2152d48e2ff44fb8710e1613ee9c264a844d0354cce2b66cb656364b0908e2`  
		Last Modified: Thu, 12 Oct 2023 04:00:35 GMT  
		Size: 18.6 MB (18638360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f80ce051fa36ff87ccad2188b21b904002f911e804126f90381e2bfe700e56`  
		Last Modified: Thu, 12 Oct 2023 04:00:54 GMT  
		Size: 60.4 MB (60436364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:5d9bcecf36028c9169e4f22dcfb0789845cf6523bd944dd55eab22dd5d4ba9aa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.0 MB (135021557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82b7c1249c50f4b3449269dc5abe7ee5c404db73aead5b7fe4b25aff61f441f6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:26:37 GMT
ADD file:ae967b7faba93d8a00f97f28b4d720835a90a27fe53b2f278072893f4cdaa8e7 in / 
# Wed, 11 Oct 2023 18:26:38 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:51:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 19:51:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ddf19dd473b427de200cf2b123540cd1dce2dcb51aeeb4a1359b7f954dc951ba`  
		Last Modified: Wed, 11 Oct 2023 18:32:45 GMT  
		Size: 49.5 MB (49505530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3234e169293a5a7c5d4630e4d414fffc649556678901730a692ba3b43cd5e618`  
		Last Modified: Wed, 11 Oct 2023 19:57:45 GMT  
		Size: 20.1 MB (20110046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71bac299e7b4e42a2756046d77fc625e1dc632615808cd1ec6bbcc2d48bf4f5`  
		Last Modified: Wed, 11 Oct 2023 19:58:01 GMT  
		Size: 65.4 MB (65405981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:c68a447d1f8f8a57fc43e7455aaaabda87e8fe5f7bb01f584d260efac38c75b0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.5 MB (138461262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e178f98ad66d50e8c497cf5503dcda5d92cae0a761c41df1e7a2d0905b93549e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:43:20 GMT
ADD file:ad97acda5f74778001aece2a9e280f0e58d2953cf8fdbd4740a049c4a595a225 in / 
# Wed, 11 Oct 2023 17:43:20 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:19:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:19:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce8ed34eaeffdeb7ac49225c6093f421b0005558aedb2b9c429731032d156621`  
		Last Modified: Wed, 11 Oct 2023 17:50:59 GMT  
		Size: 50.5 MB (50485846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f94c813421107d5ab710ec3329c2cd90f1b42da6b64e3d4ea8428fc7802b293`  
		Last Modified: Wed, 11 Oct 2023 18:27:57 GMT  
		Size: 20.9 MB (20886277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f264142306efbcccd3638b5a3b7788249da917c198eab1e97f89a7fb7178050`  
		Last Modified: Wed, 11 Oct 2023 18:28:21 GMT  
		Size: 67.1 MB (67089139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:30a2cdeea3d62c9dd4c0e562792d7aa77f1039eed2ee98069e6905a96ca15261
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.0 MB (133031060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36fb20dd0a09ce4ea2be6a3e98e09f84f36053e6646b0f5e76821b4998265f5c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:56:15 GMT
ADD file:29bed270e296c5a95f2141f114580e0f25c1040c03609fa632757a8e48ec43fd in / 
# Wed, 11 Oct 2023 17:56:22 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:46:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 23:48:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f0d54eafe706e7144ea10a18a0abaa975cb4f7f92fd40e292f388c2b1321a794`  
		Last Modified: Wed, 11 Oct 2023 18:07:41 GMT  
		Size: 49.3 MB (49301729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5204f5199336e47ca287487c83b254ad7b0260c5bf568e92c8927077786ee91c`  
		Last Modified: Thu, 12 Oct 2023 00:05:30 GMT  
		Size: 19.6 MB (19593645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf370881cf98cc9a8acbbacf482b90a7a2d7f3a1d96216bd4d6b824f2814f5c`  
		Last Modified: Thu, 12 Oct 2023 00:06:22 GMT  
		Size: 64.1 MB (64135686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d2b8ff9957833a55d2e2a2acb81c8ded45ed8f7cfdf2e9256ef9a8a8e4b699c5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.8 MB (145831200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f52eb015b31afb09fcb86b0b390e24b827066a43b906b3574e645b2a65406697`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:47:23 GMT
ADD file:24d4df221ce118a8059e0559a8bb2d715512fa6f5b15cd1397dbc177ceaa1bfd in / 
# Wed, 11 Oct 2023 17:47:26 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:30:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Oct 2023 18:31:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:93b578febbe769059c90eaa91e9dc027d172e6088856c2c52dc3e26dfdf01d4c`  
		Last Modified: Wed, 11 Oct 2023 17:54:24 GMT  
		Size: 53.4 MB (53418134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:576f9c6569231cdc2bf492ed27ab8c980261301252c26c4d6fcf8dec4fa4de9b`  
		Last Modified: Wed, 11 Oct 2023 18:41:22 GMT  
		Size: 21.6 MB (21644083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86429c6121c1cef63b4087b6359567a0aa3be523db5603dc673793266a48e8c4`  
		Last Modified: Wed, 11 Oct 2023 18:41:50 GMT  
		Size: 70.8 MB (70768983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:d56b43941a28de4537dd79f70f50cdf39dd28ebab1806ed5a4fddf6ffabcbe5e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.2 MB (135174700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5db68d1b36c00eab98e91d36cd34783d7f739259d8c82262bada484ee4590aa9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:53:11 GMT
ADD file:7f7d0fe596110ed400f2bbc2fe6edf5716a5a62332062c86009df0df0cc0a257 in / 
# Wed, 11 Oct 2023 17:53:14 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 00:25:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 00:26:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3f47ccc9a5d62eac06dcd9bcbdf51b3bf5f494156a2c21d58d93d11f5261baf4`  
		Last Modified: Wed, 11 Oct 2023 18:01:45 GMT  
		Size: 48.9 MB (48924346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:659ce526b11a7e72319632cba55fb2631fe06f2d042501bcb6fd357be98825e4`  
		Last Modified: Thu, 12 Oct 2023 00:38:24 GMT  
		Size: 20.0 MB (20041463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb87df3b4ff93b8ee1589ac6dee47871cab5b94a7b2b411694cada1830b9793`  
		Last Modified: Thu, 12 Oct 2023 00:38:56 GMT  
		Size: 66.2 MB (66208891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:unstable`

```console
$ docker pull buildpack-deps@sha256:8815033d9170f0e05af5c2cd68e7f754eb3aa01c893f5d61a2396a59e668a5bb
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
$ docker pull buildpack-deps@sha256:2d20963c232d6971a6a39af931571eb1d5e7fba7c4bcdaf0088977bfc6844a83
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **379.9 MB (379943549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59354cbe9e3cad45620c2a2218d362d004025667786b9e7ebfa732437af1daef`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:36:29 GMT
ADD file:0301a32b2b2f0af81dd4277b61ab0069818663e8ad39e59dec42f2a74e027eda in / 
# Wed, 11 Oct 2023 18:36:29 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:24:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:24:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:25:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3997a52aa0dcbfc5a01686dece23fdbb32f74ea998359451f16034544761414c`  
		Last Modified: Wed, 11 Oct 2023 18:42:29 GMT  
		Size: 49.5 MB (49503645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0b8297fd30d70e6a01a348e7e07badb169eb034e4f609afaa217cab587d8b9`  
		Last Modified: Thu, 12 Oct 2023 03:31:53 GMT  
		Size: 24.3 MB (24334751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6e5521f78eb644a7a00e353d6c3a5f1799c951272b0b5ec79a44243d51a462`  
		Last Modified: Thu, 12 Oct 2023 03:32:12 GMT  
		Size: 65.5 MB (65492596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af279c69b25af9b0d882b06462ffef0299fb0aa7628e001b6b2607baca6c6b94`  
		Last Modified: Thu, 12 Oct 2023 03:32:50 GMT  
		Size: 240.6 MB (240612557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v5

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

### `buildpack-deps:unstable` - linux; arm variant v7

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

### `buildpack-deps:unstable` - linux; arm64 variant v8

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

### `buildpack-deps:unstable` - linux; 386

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

### `buildpack-deps:unstable` - linux; mips64le

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

### `buildpack-deps:unstable` - linux; ppc64le

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

### `buildpack-deps:unstable` - linux; riscv64

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

### `buildpack-deps:unstable` - linux; s390x

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

## `buildpack-deps:unstable-curl`

```console
$ docker pull buildpack-deps@sha256:e9e3226aca93195d4f816612bce1cd5fb77e540c1269e6a3629c11235c9d9859
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
$ docker pull buildpack-deps@sha256:93d69ad7c2dba69a9f03d997bc80b11965a717a955bad0dbc9e73930c0fec227
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.8 MB (73838396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0aead4e0ede50e21f0bb6b06b316d7bf4b26320273def7c2d20529ceb8d60a57`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:36:29 GMT
ADD file:0301a32b2b2f0af81dd4277b61ab0069818663e8ad39e59dec42f2a74e027eda in / 
# Wed, 11 Oct 2023 18:36:29 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:24:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3997a52aa0dcbfc5a01686dece23fdbb32f74ea998359451f16034544761414c`  
		Last Modified: Wed, 11 Oct 2023 18:42:29 GMT  
		Size: 49.5 MB (49503645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0b8297fd30d70e6a01a348e7e07badb169eb034e4f609afaa217cab587d8b9`  
		Last Modified: Thu, 12 Oct 2023 03:31:53 GMT  
		Size: 24.3 MB (24334751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:2facb29855ce778449935650ad0bf8f05285f5bc037e27c0abc545731ade43e0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70157877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e3ce55c97d64bebc6d52e5b52a1e5ec90df23921d54256da45d2978fabdcf44`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:38:22 GMT
ADD file:32bc859b55e9b4aada411b379418b1cd95da1e1f72e89ade7698d0132f8edafd in / 
# Wed, 11 Oct 2023 17:38:22 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:09:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
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

### `buildpack-deps:unstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:2a3ac98b13e5c0b84e8a96c479d489b7281c2542c75032fdcd02dda6af1de78e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67168379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d21e5bc073011f98455f4bb3cf2cf376f08857422f623a0610bbb271406d9f9c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:43:32 GMT
ADD file:e83473ecad5aa9a153d02c535c6e40e22679b973268fdd74a0f5bd86b004222a in / 
# Wed, 11 Oct 2023 17:43:33 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:50:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
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

### `buildpack-deps:unstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:fce215ecb937435e92000bf5dfe52f3717f5dca30b710c5064233ef875426f43
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.4 MB (73391816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2d378acba0577367ce6a31afd366988b2b397f9537de3a47b965ec3899cb758`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:56 GMT
ADD file:c18e09bd64c99d045a504c333efaa05322c76b488039b206edcf75aa2a1a3812 in / 
# Wed, 11 Oct 2023 18:25:57 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 19:49:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
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

### `buildpack-deps:unstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:6c5a3c841432a3311b27c5d3b9ab74fbfd33f1fc8c9c5570adcbd1a3449f301c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75645770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b139468ba853f4e64f72ad3a626476ad17acf6b17286e5b697e458ab16986cd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:42:19 GMT
ADD file:e8e1c13db04ddce5a6b3f4e29283e75eeecf85f213c2433ccb342a253457abc1 in / 
# Wed, 11 Oct 2023 17:42:20 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:16:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
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

### `buildpack-deps:unstable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:630fa9a87431d5ef63ba0403e35b1d13078e44716350c2f7f626b79644299959
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73189227 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4f8b088028ae199b72c712652c50ff8948c76437c673b92447dcdf542c35ff8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:52:38 GMT
ADD file:b80f07fa17341655abce58a1824ae94b2623d66b3f37a58194b8a738cf645945 in / 
# Wed, 11 Oct 2023 17:52:44 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 23:36:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
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

### `buildpack-deps:unstable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:cd232f49802d24b109a6845c69de40da722b1c48414c6b7198c904425c111923
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.4 MB (79394432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dff07d1542982f90245cadfde4cf3d10fe51356a3b06794d5b5de4fb83cb01e2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:45:44 GMT
ADD file:5f062baf648f8cba61d84347ebedbe11eca129a318a8146b4c7c30586cbf0436 in / 
# Wed, 11 Oct 2023 17:45:47 GMT
CMD ["bash"]
# Wed, 11 Oct 2023 18:25:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
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

### `buildpack-deps:unstable-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:463277650cb87ff963c4f3e246c78101c2bf595bfdcfda04fb4db350e9dc1592
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69007846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a46d4dea6048745e0f58711f73e97cfebd76971edb90fbbf0cf7dc14a24ec144`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:09:51 GMT
ADD file:fdcff160dcad587bb28b0cba721c24193be4ab5de90a2d503cba3d329b78797b in / 
# Thu, 27 Jul 2023 23:09:54 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:32:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
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

### `buildpack-deps:unstable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:43c6868e1269e7652a2de8a9524ef2cfdc486ebee9b841c762abc68d593b7c7b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.5 MB (73502003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cbc0b99dfdb875d8a7fc97b0162f802cadba9a8045b9077107c5592300b2f65`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 17:51:43 GMT
ADD file:66653f97d007e397b8dbcdca1bbb32bd8039456ae5b2cae3e049382489afb265 in / 
# Wed, 11 Oct 2023 17:51:47 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 00:05:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
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

## `buildpack-deps:unstable-scm`

```console
$ docker pull buildpack-deps@sha256:718fec922b4a6871329a1bbf1c6d9da309a17f8aac5af9743fdda459d5fb3a85
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
$ docker pull buildpack-deps@sha256:0b2f3bd1cc4c7815a7e596fb753fc38a233e70c90ecf2bed32ecdcf28e5a74a2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.3 MB (139330992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6908eca674268f2a8c937287486ca0fb7661d00ec8e725e0ede07b0970b7ee1b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:36:29 GMT
ADD file:0301a32b2b2f0af81dd4277b61ab0069818663e8ad39e59dec42f2a74e027eda in / 
# Wed, 11 Oct 2023 18:36:29 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:24:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:24:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3997a52aa0dcbfc5a01686dece23fdbb32f74ea998359451f16034544761414c`  
		Last Modified: Wed, 11 Oct 2023 18:42:29 GMT  
		Size: 49.5 MB (49503645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0b8297fd30d70e6a01a348e7e07badb169eb034e4f609afaa217cab587d8b9`  
		Last Modified: Thu, 12 Oct 2023 03:31:53 GMT  
		Size: 24.3 MB (24334751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6e5521f78eb644a7a00e353d6c3a5f1799c951272b0b5ec79a44243d51a462`  
		Last Modified: Thu, 12 Oct 2023 03:32:12 GMT  
		Size: 65.5 MB (65492596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:6e5665d5853aa13b18e4bc33e2e74ccd3fd4299bbee0d5638a8edfd8811fd31d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.2 MB (133155810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82733bdae381c5738d0e28f4d4a7b2e23a488cf237028a2f9d7340ed42a2de6a`
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

### `buildpack-deps:unstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:0241422c180b52449cebfb843511a622b3db62b876adcb35f83687d33338ebd0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127780532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e47cd5dfc4c910b811a8be1f25b280a059fbcfd20276ea41ecb9d61a43415c5`
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

### `buildpack-deps:unstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:944bdc970d6ca598d11e588a54f084da0fb8a9ba812e762a9214eabe87384929
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.0 MB (138977761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1834be5b56b00292a42bceb02448a4a30da604bc1654bd80098dd463aa4b5e12`
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

### `buildpack-deps:unstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:db6becb86617eec873cc1f2cbc1f8c0abd30edc8936fe15da22884a7c262b25f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.9 MB (142912216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5170e1fe625abd2d29e37453c2b4b9ba4255f5b27a6f1e529629d4b96d54a95`
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

### `buildpack-deps:unstable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:89df672a2eae0669920f05fcd19c0581e1dece33f0bb2a1d319e25e9d2537059
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.5 MB (137502013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e3b055ef2c6b884b963271c3f7fbb51f1913f3ac0ad28460eb6d5a0d022fb30`
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

### `buildpack-deps:unstable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:bfd905fe06deae4a397b28f46fa0b93ebc6e0f31d8de7f7d64f20a01c3510614
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.3 MB (150311356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc0c94e86ebe4c6d3673f604832571ce2c2f31974dc5f67beeb360a926f3aa03`
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

### `buildpack-deps:unstable-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:82b54224e16141b3d128a2c7213a413e390b1216abe389f923a2eaf497c751af
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.4 MB (129394231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4d1a4d2d9108164c640ce2247e18e16b8a958c777fd7a7181f424ddb829d083`
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

### `buildpack-deps:unstable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:60c63e0e0ad978fcf73dd18012240127fcb631a7993d05b3f9d3ddabab132675
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.9 MB (139893138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f3debda305b48b4c96aeca9c4076cb44864a7a588e3041b287ddf0f78757147`
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
