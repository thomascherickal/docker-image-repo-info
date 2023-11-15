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
$ docker pull buildpack-deps@sha256:0ce585b92f5ec1586823ded83ae124239bc3596b06c19f436320bd0788a4c9b7
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
$ docker pull buildpack-deps@sha256:2d8c4194fb7309c82c42c5e72f9eb63bd2a91a53b563d1477bb145b5bab8a964
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.5 MB (226549744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3075cf4fa6991f63d4d84b9f17dca444f018d69cca3039b157ec2ecceb038a0c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 Oct 2023 11:03:23 GMT
ARG RELEASE
# Tue, 03 Oct 2023 11:03:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 11:03:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 11:03:23 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 11:03:25 GMT
ADD file:1d9be1bf43c126d53bda18c06d12757c021da97c0c9d3a9c9f56df17312095b8 in / 
# Tue, 03 Oct 2023 11:03:25 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 11:01:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 11:02:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 11:04:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2f51ce1532d2fc433720a55b8851134d5051381dedc2ef6109fb7ebb7a0edb92`  
		Last Modified: Fri, 13 Oct 2023 10:16:26 GMT  
		Size: 27.0 MB (27014102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c5cede6167f4e42b7f5e8cf8fb25ba8e103554c1d3afce502fb3e1f7e24b43`  
		Last Modified: Fri, 13 Oct 2023 11:13:32 GMT  
		Size: 10.7 MB (10687808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af317778e55c85e39b6ea37b448d46e0197947b603250dea5a4ac60cc8a53d8`  
		Last Modified: Fri, 13 Oct 2023 11:13:47 GMT  
		Size: 60.3 MB (60311494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c74bf94f4dabe59299e4f79fa6db52ecd3d45cced8c8f2a7268a73dc893e07`  
		Last Modified: Fri, 13 Oct 2023 11:14:11 GMT  
		Size: 128.5 MB (128536340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:20.04-curl`

```console
$ docker pull buildpack-deps@sha256:d4947847a090a83bc604b03f063b6c3581a512d8d7540cee339d4f804dc3e5f4
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
$ docker pull buildpack-deps@sha256:02cd3122d24058fbd1b8e50757076b598990a16b09c533afe912ec749e661f93
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37701910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23b5ed0a418136ce71335a277e0b38f1285bb432922fe1fc0572dc210936d4ad`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 Oct 2023 11:03:23 GMT
ARG RELEASE
# Tue, 03 Oct 2023 11:03:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 11:03:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 11:03:23 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 11:03:25 GMT
ADD file:1d9be1bf43c126d53bda18c06d12757c021da97c0c9d3a9c9f56df17312095b8 in / 
# Tue, 03 Oct 2023 11:03:25 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 11:01:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2f51ce1532d2fc433720a55b8851134d5051381dedc2ef6109fb7ebb7a0edb92`  
		Last Modified: Fri, 13 Oct 2023 10:16:26 GMT  
		Size: 27.0 MB (27014102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c5cede6167f4e42b7f5e8cf8fb25ba8e103554c1d3afce502fb3e1f7e24b43`  
		Last Modified: Fri, 13 Oct 2023 11:13:32 GMT  
		Size: 10.7 MB (10687808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:20.04-scm`

```console
$ docker pull buildpack-deps@sha256:4d7f93ed85af3446f7ec8598f188eab65156a6514197672620844a56f9b9f2fa
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
$ docker pull buildpack-deps@sha256:05b5108d044759d54f2f80eb3a45210f2b631e49fcf67cd333b46b13111a155c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.0 MB (98013404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8f52f13ce965b8eb5ebf01d5353ccde18fb00da4df1e00f8427a9966f2d6a17`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 Oct 2023 11:03:23 GMT
ARG RELEASE
# Tue, 03 Oct 2023 11:03:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 11:03:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 11:03:23 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 11:03:25 GMT
ADD file:1d9be1bf43c126d53bda18c06d12757c021da97c0c9d3a9c9f56df17312095b8 in / 
# Tue, 03 Oct 2023 11:03:25 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 11:01:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 11:02:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2f51ce1532d2fc433720a55b8851134d5051381dedc2ef6109fb7ebb7a0edb92`  
		Last Modified: Fri, 13 Oct 2023 10:16:26 GMT  
		Size: 27.0 MB (27014102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c5cede6167f4e42b7f5e8cf8fb25ba8e103554c1d3afce502fb3e1f7e24b43`  
		Last Modified: Fri, 13 Oct 2023 11:13:32 GMT  
		Size: 10.7 MB (10687808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af317778e55c85e39b6ea37b448d46e0197947b603250dea5a4ac60cc8a53d8`  
		Last Modified: Fri, 13 Oct 2023 11:13:47 GMT  
		Size: 60.3 MB (60311494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.04`

```console
$ docker pull buildpack-deps@sha256:4a33447a13decae8d0e6fe2b6444168aa358c260a758d775cae0676c125f5698
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
$ docker pull buildpack-deps@sha256:224fda92a290ee7dce3b93f8ef46090b274c54e6c85125025c20b13569a84ad9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.8 MB (223838717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e1c00dab04ed667278bb299d0cd64a72c6aac1bf6dea472b34db49d75e79740`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:29:34 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:29:34 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:29:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:29:34 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:29:36 GMT
ADD file:d165475f8f027ab758a463da57c8c29f5d302f0a87a475ac68fdfae30005c7ac in / 
# Thu, 05 Oct 2023 07:29:36 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 11:05:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 11:05:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 11:07:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:818e4e246beb9ab026d2b95bf051fe9610b92dbc0a35b45d09b0cf237b6f3c2e`  
		Last Modified: Fri, 13 Oct 2023 10:16:45 GMT  
		Size: 28.7 MB (28650497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e533f7ce965854f8f4cdc647d000c54a4925b3b180750298427b9235afa18e51`  
		Last Modified: Fri, 13 Oct 2023 11:14:18 GMT  
		Size: 7.0 MB (7033617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c01525ba07c29d70d75e5ad0aa553d3b9ab93b48dbf3368a2e637f0d4d225d0`  
		Last Modified: Fri, 13 Oct 2023 11:14:30 GMT  
		Size: 39.4 MB (39414564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef34b85cef45adc613db3947199161e633e7076231b6a41ef4854ca8e3ceabbc`  
		Last Modified: Fri, 13 Oct 2023 11:14:56 GMT  
		Size: 148.7 MB (148740039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.04-curl`

```console
$ docker pull buildpack-deps@sha256:b6d4d85cb1727a557a2a10db192be5aa79af3b05092a96d7a6f293d7242487d6
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
$ docker pull buildpack-deps@sha256:2de035e63fc2a4e0bcb3c141b59f3918f2388a91db1280bbbc45b732c8196739
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35684114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1ef128f78a0b9d9f64497c39fbe68d730dd357868b4f101d7a0feec3b20645e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:29:34 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:29:34 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:29:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:29:34 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:29:36 GMT
ADD file:d165475f8f027ab758a463da57c8c29f5d302f0a87a475ac68fdfae30005c7ac in / 
# Thu, 05 Oct 2023 07:29:36 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 11:05:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:818e4e246beb9ab026d2b95bf051fe9610b92dbc0a35b45d09b0cf237b6f3c2e`  
		Last Modified: Fri, 13 Oct 2023 10:16:45 GMT  
		Size: 28.7 MB (28650497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e533f7ce965854f8f4cdc647d000c54a4925b3b180750298427b9235afa18e51`  
		Last Modified: Fri, 13 Oct 2023 11:14:18 GMT  
		Size: 7.0 MB (7033617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.04-scm`

```console
$ docker pull buildpack-deps@sha256:f205acc8dc8abd31d431089175b0f6f366261875e18e4055432a0e49659a80b0
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
$ docker pull buildpack-deps@sha256:c0da1ea44cc5848bd53fb6e94390685144a6a15b9440e02f9acc6ee3c6f192a8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75098678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a9c666b9c8b0954dade1579aed2a7d9b57345535d874545267e8c4ea50d4ecd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:29:34 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:29:34 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:29:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:29:34 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:29:36 GMT
ADD file:d165475f8f027ab758a463da57c8c29f5d302f0a87a475ac68fdfae30005c7ac in / 
# Thu, 05 Oct 2023 07:29:36 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 11:05:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 11:05:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:818e4e246beb9ab026d2b95bf051fe9610b92dbc0a35b45d09b0cf237b6f3c2e`  
		Last Modified: Fri, 13 Oct 2023 10:16:45 GMT  
		Size: 28.7 MB (28650497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e533f7ce965854f8f4cdc647d000c54a4925b3b180750298427b9235afa18e51`  
		Last Modified: Fri, 13 Oct 2023 11:14:18 GMT  
		Size: 7.0 MB (7033617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c01525ba07c29d70d75e5ad0aa553d3b9ab93b48dbf3368a2e637f0d4d225d0`  
		Last Modified: Fri, 13 Oct 2023 11:14:30 GMT  
		Size: 39.4 MB (39414564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:23.04`

```console
$ docker pull buildpack-deps@sha256:9d3347dff07c65b321044655161d08f18441853c906686fc726318ca72c41a25
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
$ docker pull buildpack-deps@sha256:a0851ce95bf9247c04db9bf58ce62db350f36adf2937da6b0e8ec31eb69993dd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.2 MB (240192288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:223926587c6bf995caec15c7e535b8415b6bde18631d04c2527f6138d6b213a2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:26:55 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:26:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:26:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:26:55 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:26:57 GMT
ADD file:553d1c48ed98fa8bd575a7a645019079304c101dd6e06e82591a25440fe1a9b8 in / 
# Wed, 04 Oct 2023 12:26:57 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 11:08:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 11:09:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 11:11:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d713c3685e42819275f0fd629c394d4cc0cb20ebedd41e0c903afea19652cda9`  
		Last Modified: Fri, 13 Oct 2023 11:15:09 GMT  
		Size: 26.2 MB (26227299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10986e1aade9beaffef4018fdb444b55730350800aadabb7852a08f52b4e62fb`  
		Last Modified: Fri, 13 Oct 2023 11:15:06 GMT  
		Size: 14.0 MB (14006392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a2b5e38d0d2baf19e26862b6913dbfd77f4a4a48316294650cf07405115b38`  
		Last Modified: Fri, 13 Oct 2023 11:15:22 GMT  
		Size: 44.3 MB (44276364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c850916986260e8d643a72fb43633da561be89db5f3dfca9538eef8ce5175a1`  
		Last Modified: Fri, 13 Oct 2023 11:15:50 GMT  
		Size: 155.7 MB (155682233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:23.04-curl`

```console
$ docker pull buildpack-deps@sha256:4580a8a315197a8e4aa6953328d97401177416efc796a21a526f0eef3d184c95
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
$ docker pull buildpack-deps@sha256:4238b02664305627674ca2c52080ae3df742aaac231ebd9eb6b703501d4733d2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40233691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b6c03fa308ad0e9faa468a0f88ccb79519aecef58256d45189f7f748d9d9c04`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:26:55 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:26:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:26:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:26:55 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:26:57 GMT
ADD file:553d1c48ed98fa8bd575a7a645019079304c101dd6e06e82591a25440fe1a9b8 in / 
# Wed, 04 Oct 2023 12:26:57 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 11:08:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d713c3685e42819275f0fd629c394d4cc0cb20ebedd41e0c903afea19652cda9`  
		Last Modified: Fri, 13 Oct 2023 11:15:09 GMT  
		Size: 26.2 MB (26227299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10986e1aade9beaffef4018fdb444b55730350800aadabb7852a08f52b4e62fb`  
		Last Modified: Fri, 13 Oct 2023 11:15:06 GMT  
		Size: 14.0 MB (14006392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:23.04-scm`

```console
$ docker pull buildpack-deps@sha256:28f0686151e36942ee57461782428b02ae03d89b2c284474e804bb1fa5296202
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
$ docker pull buildpack-deps@sha256:312fb14d7e1c8447dc941245fdf9000d5a021a9f0f69b6b5a0efc49e859e46a6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84510055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:950a90c7fe2432bea9c867925cf0529090d9e75843d2a055960535aef8a866e9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:26:55 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:26:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:26:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:26:55 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:26:57 GMT
ADD file:553d1c48ed98fa8bd575a7a645019079304c101dd6e06e82591a25440fe1a9b8 in / 
# Wed, 04 Oct 2023 12:26:57 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 11:08:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 11:09:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d713c3685e42819275f0fd629c394d4cc0cb20ebedd41e0c903afea19652cda9`  
		Last Modified: Fri, 13 Oct 2023 11:15:09 GMT  
		Size: 26.2 MB (26227299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10986e1aade9beaffef4018fdb444b55730350800aadabb7852a08f52b4e62fb`  
		Last Modified: Fri, 13 Oct 2023 11:15:06 GMT  
		Size: 14.0 MB (14006392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a2b5e38d0d2baf19e26862b6913dbfd77f4a4a48316294650cf07405115b38`  
		Last Modified: Fri, 13 Oct 2023 11:15:22 GMT  
		Size: 44.3 MB (44276364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:23.10`

```console
$ docker pull buildpack-deps@sha256:7a2d476ae163cde92e9c4b8ef2906d865ccfc52fb63c465166aac7cef534ab80
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
$ docker pull buildpack-deps@sha256:46a4bc226b23e753406055137a46fe3c7fe73db1967c597eb2c08ac8d5aee8b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.0 MB (246981399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31561ec40607a691d299c442e8b44dfb1cb951ac72c779e6afbdb8b2aa082143`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:02:33 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:02:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:02:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:02:34 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:02:39 GMT
ADD file:1be1311acbd557f7769fb5c1913ef56305431e7547f96c20ac36284fdd926223 in / 
# Wed, 11 Oct 2023 18:02:39 GMT
CMD ["/bin/bash"]
# Wed, 15 Nov 2023 02:04:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 02:05:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 02:09:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:917b6666fb3ef51da1fc4435b7ebc2e973f8582d1321861d37d40dd0864b8927`  
		Last Modified: Wed, 15 Nov 2023 02:12:00 GMT  
		Size: 26.0 MB (26018438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179cd7cba3839185a2e0560fddb5800f6454b72d5acf3d485458ee26f6fef69f`  
		Last Modified: Wed, 15 Nov 2023 02:11:56 GMT  
		Size: 9.1 MB (9144906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d43664e3e871d40780214b000e38e04e3e840e99201a63699c325b0f02b0e5c`  
		Last Modified: Wed, 15 Nov 2023 02:12:19 GMT  
		Size: 49.2 MB (49223065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a4ff86544066b3c295e5fcd8ff907e64e35463f7b0911a6b709c5c52a28625`  
		Last Modified: Wed, 15 Nov 2023 02:12:57 GMT  
		Size: 162.6 MB (162594990 bytes)  
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
$ docker pull buildpack-deps@sha256:390630061f7241d7a3a338d8c1a2b285ebe1fff641bff92948cd16d604fedb96
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.9 MB (293947200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd0ab4387549ce1201adde944fda71531759b742627a5e12f382d3316893aea6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:06:00 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:06:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:06:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:06:00 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:06:03 GMT
ADD file:a18be8add7eb60493b13d2aac8d624230297bd15be033756795582dc07cb04bb in / 
# Wed, 11 Oct 2023 18:06:03 GMT
CMD ["/bin/bash"]
# Wed, 15 Nov 2023 02:22:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 02:23:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 02:27:21 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cffa8c08adf985954e82a5191220c2cac943e97ffd91acc2baa5d2cf0f8d4f44`  
		Last Modified: Wed, 15 Nov 2023 02:29:45 GMT  
		Size: 32.3 MB (32331370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5791ffbc3c4fdf8ff7e22c644078ce798cd8033f9d2e244eca8aec0a44ac5ce7`  
		Last Modified: Wed, 15 Nov 2023 02:29:40 GMT  
		Size: 11.6 MB (11573378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6331f990f21c8548212ac022cb9047ae9a7b4ac314bf49338f47926ca887eb14`  
		Last Modified: Wed, 15 Nov 2023 02:30:03 GMT  
		Size: 49.9 MB (49917559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c87fb10926a50da16bbd6eccc10a2b838b8368f36be454459fb19bc65df426`  
		Last Modified: Wed, 15 Nov 2023 02:30:42 GMT  
		Size: 200.1 MB (200124893 bytes)  
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
$ docker pull buildpack-deps@sha256:cd4d41ae6132051a907e3cfd0d9fddcfcd6b582033f9ab9291a2fcfde4976171
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
$ docker pull buildpack-deps@sha256:921a763a77cd772742a6ae544a5bd71b4411f92a999be5d1d7fed1684ddac2e3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (37974507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:287d7639ff0677fdfe2b1eadc6efdd695a529748505a9cbdc44b29355b92125b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:04:48 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:04:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:04:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:04:49 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:04:50 GMT
ADD file:492ae1940ef5a9a4d7af92b9120b5b7c7d3bfd8107ce94d28eab844ace024981 in / 
# Wed, 11 Oct 2023 18:04:50 GMT
CMD ["/bin/bash"]
# Wed, 15 Nov 2023 05:11:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2e92ecfee06656d1e7ef085e24769afe12ea1e14f3acdbdaf9d5cb922da5d97b`  
		Last Modified: Sat, 14 Oct 2023 00:22:39 GMT  
		Size: 28.1 MB (28067323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a6e6c1f13a01a9a83ddb22794e5e9998c28232b9695a11941b9c2fad7dfcc9`  
		Last Modified: Wed, 15 Nov 2023 05:19:05 GMT  
		Size: 9.9 MB (9907184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.10-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:2913f2f84d97ff1be7ca139b43ce4e8d05cfaf7ed3248b39aa9e6a70b154ea91
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.2 MB (35163344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59cd33ac4877ec60e73bfb24bb572ad8088801b2acdcc70314770203d15b6c91`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:02:33 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:02:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:02:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:02:34 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:02:39 GMT
ADD file:1be1311acbd557f7769fb5c1913ef56305431e7547f96c20ac36284fdd926223 in / 
# Wed, 11 Oct 2023 18:02:39 GMT
CMD ["/bin/bash"]
# Wed, 15 Nov 2023 02:04:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:917b6666fb3ef51da1fc4435b7ebc2e973f8582d1321861d37d40dd0864b8927`  
		Last Modified: Wed, 15 Nov 2023 02:12:00 GMT  
		Size: 26.0 MB (26018438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179cd7cba3839185a2e0560fddb5800f6454b72d5acf3d485458ee26f6fef69f`  
		Last Modified: Wed, 15 Nov 2023 02:11:56 GMT  
		Size: 9.1 MB (9144906 bytes)  
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
$ docker pull buildpack-deps@sha256:bcab01774044541e169e955e9d52762f736b27fb6c76d029381b6162dedbfee9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43904748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbce8aeac751517d845efadce6fb839eff255b2c00e279e01eeb686343d3d0d8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:06:00 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:06:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:06:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:06:00 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:06:03 GMT
ADD file:a18be8add7eb60493b13d2aac8d624230297bd15be033756795582dc07cb04bb in / 
# Wed, 11 Oct 2023 18:06:03 GMT
CMD ["/bin/bash"]
# Wed, 15 Nov 2023 02:22:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cffa8c08adf985954e82a5191220c2cac943e97ffd91acc2baa5d2cf0f8d4f44`  
		Last Modified: Wed, 15 Nov 2023 02:29:45 GMT  
		Size: 32.3 MB (32331370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5791ffbc3c4fdf8ff7e22c644078ce798cd8033f9d2e244eca8aec0a44ac5ce7`  
		Last Modified: Wed, 15 Nov 2023 02:29:40 GMT  
		Size: 11.6 MB (11573378 bytes)  
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
$ docker pull buildpack-deps@sha256:c04969aa1a89a875915b3c8f7a54f60fca8979f802161c1acf9c9b9eae984578
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
$ docker pull buildpack-deps@sha256:405d376e0a44215dd53d9e4cea3ff098d03cae9e0aeeb846816f17d396321b18
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.1 MB (83062814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b3aba9e6064055dae56a062bcb092f50cffe5887b49242fdff98a4ea0eb3aa4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:04:48 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:04:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:04:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:04:49 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:04:50 GMT
ADD file:492ae1940ef5a9a4d7af92b9120b5b7c7d3bfd8107ce94d28eab844ace024981 in / 
# Wed, 11 Oct 2023 18:04:50 GMT
CMD ["/bin/bash"]
# Wed, 15 Nov 2023 05:11:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 05:12:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2e92ecfee06656d1e7ef085e24769afe12ea1e14f3acdbdaf9d5cb922da5d97b`  
		Last Modified: Sat, 14 Oct 2023 00:22:39 GMT  
		Size: 28.1 MB (28067323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a6e6c1f13a01a9a83ddb22794e5e9998c28232b9695a11941b9c2fad7dfcc9`  
		Last Modified: Wed, 15 Nov 2023 05:19:05 GMT  
		Size: 9.9 MB (9907184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7fdbffee3006b2f392267c0bb2881b445fa2d9a6a932b40496bf246d26ed245`  
		Last Modified: Wed, 15 Nov 2023 05:19:22 GMT  
		Size: 45.1 MB (45088307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.10-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:afca6c528e9a02dffda09b471ae45eb3c1cd24ff62f025ec89877622c62fca52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.4 MB (84386409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cfd5fac42f464b6ae54e8ee27cba67ca6befadd81810a15993572f7fbd736e1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:02:33 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:02:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:02:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:02:34 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:02:39 GMT
ADD file:1be1311acbd557f7769fb5c1913ef56305431e7547f96c20ac36284fdd926223 in / 
# Wed, 11 Oct 2023 18:02:39 GMT
CMD ["/bin/bash"]
# Wed, 15 Nov 2023 02:04:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 02:05:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:917b6666fb3ef51da1fc4435b7ebc2e973f8582d1321861d37d40dd0864b8927`  
		Last Modified: Wed, 15 Nov 2023 02:12:00 GMT  
		Size: 26.0 MB (26018438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179cd7cba3839185a2e0560fddb5800f6454b72d5acf3d485458ee26f6fef69f`  
		Last Modified: Wed, 15 Nov 2023 02:11:56 GMT  
		Size: 9.1 MB (9144906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d43664e3e871d40780214b000e38e04e3e840e99201a63699c325b0f02b0e5c`  
		Last Modified: Wed, 15 Nov 2023 02:12:19 GMT  
		Size: 49.2 MB (49223065 bytes)  
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
$ docker pull buildpack-deps@sha256:710b61b098eb5d89e1e90686bd2c18ab1114706836bec26a133f94735ca05450
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.8 MB (93822307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9e385101b300162a4d39d603be56508551348b1b4e836cf511396429cdcd345`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:06:00 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:06:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:06:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:06:00 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:06:03 GMT
ADD file:a18be8add7eb60493b13d2aac8d624230297bd15be033756795582dc07cb04bb in / 
# Wed, 11 Oct 2023 18:06:03 GMT
CMD ["/bin/bash"]
# Wed, 15 Nov 2023 02:22:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 02:23:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cffa8c08adf985954e82a5191220c2cac943e97ffd91acc2baa5d2cf0f8d4f44`  
		Last Modified: Wed, 15 Nov 2023 02:29:45 GMT  
		Size: 32.3 MB (32331370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5791ffbc3c4fdf8ff7e22c644078ce798cd8033f9d2e244eca8aec0a44ac5ce7`  
		Last Modified: Wed, 15 Nov 2023 02:29:40 GMT  
		Size: 11.6 MB (11573378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6331f990f21c8548212ac022cb9047ae9a7b4ac314bf49338f47926ca887eb14`  
		Last Modified: Wed, 15 Nov 2023 02:30:03 GMT  
		Size: 49.9 MB (49917559 bytes)  
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
$ docker pull buildpack-deps@sha256:8465175ca53f8f2e756d069658b3f353bb3732926b1f33f34332cfbf597ad0c0
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
$ docker pull buildpack-deps@sha256:c281372d752c50bd925a7ef863ad65222d68d37028b97ae6378f38fe3ead7b15
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.8 MB (348825839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6672223876e40fadb1dac262c5e01bdaefbffd0107862c58d80b4df910d55414`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:37 GMT
ADD file:3e9b6405f11dd24ce62105c033f1d8b931d9409298553f63b03af1b6dd1dda35 in / 
# Wed, 01 Nov 2023 00:20:38 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:52:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 00:52:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 00:53:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8457fd5474e70835e4482983a5662355d892d5f6f0f90a27a8e9f009997e8196`  
		Last Modified: Wed, 01 Nov 2023 00:25:05 GMT  
		Size: 49.6 MB (49582024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13baa2029dde87a21b87127168a0fb50a007c07da6b5adc8864e1fe1376c86ff`  
		Last Modified: Wed, 01 Nov 2023 01:02:01 GMT  
		Size: 24.0 MB (24049147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:325c5bf4c2f26c11380501bec4b6eef8a3ea35b554aa1b222cbcd1e1fe11ae1d`  
		Last Modified: Wed, 01 Nov 2023 01:02:20 GMT  
		Size: 64.1 MB (64130415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e18a660069fd7f87a7a6c49ddb701449bfb929c066811777601d36916c7f674`  
		Last Modified: Wed, 01 Nov 2023 01:02:55 GMT  
		Size: 211.1 MB (211064253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:f8310b73e4ca74a8a62aa3a60614bce0092e656117d95d96abf6efa958f10f39
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.0 MB (316028995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1bbae5789c5511aa21a7f8cac7ff0966d933f3cba2914e0630044c3d3d9a171`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:48:23 GMT
ADD file:963e26decfc65419428098047df29dcbf7865e13bcdd67abeb9849f99a7815e7 in / 
# Wed, 01 Nov 2023 00:48:23 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:56:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:53c5547a993a8adb09a632a8ae34fbc336b27a456c6b3a670865cd8bedb5e6a9`  
		Last Modified: Wed, 01 Nov 2023 00:51:04 GMT  
		Size: 47.4 MB (47355649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752979e12aac8f84972cea68e4f8d9bb1b645e71b3fc64047af1ba792dd338d9`  
		Last Modified: Wed, 01 Nov 2023 03:04:53 GMT  
		Size: 22.7 MB (22727584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bad2403917aecfddc5d239a343aacd942aeb9c9e6d76c027cfdbb0d5479bcaa`  
		Last Modified: Wed, 01 Nov 2023 03:05:15 GMT  
		Size: 61.6 MB (61561816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f0dda98bbf4b74a7919e20bcc31a0ecda8fd013c63ef827f0316369707e6af`  
		Last Modified: Wed, 01 Nov 2023 03:05:53 GMT  
		Size: 184.4 MB (184383946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1d6a60f9f2f559b189af01218c17dcda727d852c6c6d4a004b3a18dffdba281b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.4 MB (301446629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:576fdf6667f95f602d6807ecabd5c0e4f0643440a9c83b60e388dc8614f59f15`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:57:42 GMT
ADD file:3b2b4eda35d794b39d6b5567e81651625af51da3deb3f63b3ffdffa07720646e in / 
# Wed, 01 Nov 2023 00:57:42 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:30:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:30:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:31:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9bf855396a6f46c1cbac4e188af10f2c38474f989707b0b1b406b48c4b7284ef`  
		Last Modified: Wed, 01 Nov 2023 01:01:41 GMT  
		Size: 45.2 MB (45179410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6e59eca644b227cb755978679a3031e7b3f9a5c707057c293f2ba8732d8ef2`  
		Last Modified: Wed, 01 Nov 2023 02:41:40 GMT  
		Size: 22.0 MB (21951880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aefa016475f9e4925fd893a9d8cfcf375937aa4e637d337806176426509dfcd`  
		Last Modified: Wed, 01 Nov 2023 02:42:04 GMT  
		Size: 59.3 MB (59266468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d2c477968e94d61a34b16e774d58519d5e26175f92fbd0dfb90938103fab68`  
		Last Modified: Wed, 01 Nov 2023 02:42:47 GMT  
		Size: 175.0 MB (175048871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a8b07b41b675910dbc20eaf720c7716422cb5d1f0ddac9fbbdf56f6211f2a34e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.6 MB (339641684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08254bfa9a67c2c123e58e5c10e5e73f9c4aa1eee30e14a41e6c78b513d6e36d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:32 GMT
ADD file:c934ceb4c53a1cce6779198f1ea73d5c8aad9a035e750b343d49826120ecd0eb in / 
# Wed, 01 Nov 2023 00:39:33 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:04:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:04:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:05:48 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8024d4fb53b2455f66d49b7ee72eb3cad5074043578238b796a9879955946a88`  
		Last Modified: Wed, 01 Nov 2023 00:42:44 GMT  
		Size: 49.6 MB (49612653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d826ee8aa65e56e167f0e27fa65cfc065687a7ac6c360787d5940d8b51f0cf1`  
		Last Modified: Wed, 01 Nov 2023 02:13:39 GMT  
		Size: 23.6 MB (23584896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198068495d09b6865e75ce28d5d5d5de39897b8325ada63ba80eca884ad5666b`  
		Last Modified: Wed, 01 Nov 2023 02:13:57 GMT  
		Size: 64.0 MB (63994018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509db9a897ae5a94cad05bcf48605637fbf3f79733e8bf8c317b6babe3de1dbd`  
		Last Modified: Wed, 01 Nov 2023 02:14:29 GMT  
		Size: 202.5 MB (202450117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:06f4072db6e5dfbd8c8a3f60ac4b15f0852ba0216c33198a58e8da312fb8beda
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.5 MB (351464296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa96e3b9058ae71c8b65439bf05b32b30c99e3b7b9e4f07e1692eefc747c08c8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:38:46 GMT
ADD file:4043d711d8d7d1a995aed0a6998c96230765f55d4449167107955fe4af2a31db in / 
# Wed, 01 Nov 2023 00:38:47 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 13:44:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:44:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:45:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be8d77e28ff21732ba73253b6226e47e4e07ec2cedc803ffd62148df5d7a165b`  
		Last Modified: Wed, 01 Nov 2023 00:43:00 GMT  
		Size: 50.6 MB (50600049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cef920c8d790c11b84fa21c2204cca8ac6a84ec43e4a60bca3670e828748583`  
		Last Modified: Wed, 01 Nov 2023 13:55:45 GMT  
		Size: 24.9 MB (24885575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fee1ec8688f07e43b49247f3490035da93288449034600daee26c8ce0150a8c`  
		Last Modified: Wed, 01 Nov 2023 13:56:13 GMT  
		Size: 66.0 MB (65984300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6a893690e210e75c1236dc74079509b9f860409954240df3b2276364c416f8`  
		Last Modified: Wed, 01 Nov 2023 13:57:04 GMT  
		Size: 210.0 MB (209994372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:34b5b299169edc7c1281954a26f710d3d5d9c2101b510ae89ba1ca136df9b03c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.6 MB (325622171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0dc2b58709b67c5f83e2571566693513ad91a3ec9cd7626f14d8e210d8f7925`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:08:17 GMT
ADD file:b181441dc28bc6879e29cd086c569c653171c681525c124ffb6277bd71732bb1 in / 
# Wed, 01 Nov 2023 01:08:24 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 21:17:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 21:19:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 21:25:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0bfbf01892d22dd14fb9536e8675cc932ff41f415a415fbf8c6199106b01240d`  
		Last Modified: Wed, 01 Nov 2023 01:19:01 GMT  
		Size: 49.6 MB (49568811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9310598b7549f388c445368ea2a0a4077c57ddd45436efddb37e089d293f87fe`  
		Last Modified: Wed, 01 Nov 2023 21:53:41 GMT  
		Size: 23.4 MB (23438019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af2206444fab218d319700cbfcd93423bf4622bb8085adee11b684b7d3fd245`  
		Last Modified: Wed, 01 Nov 2023 21:54:35 GMT  
		Size: 63.0 MB (62962363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41601926009dec498023c4d0a7e1c4877fc9fe8372d6497206d1de026aeb215d`  
		Last Modified: Wed, 01 Nov 2023 21:57:00 GMT  
		Size: 189.7 MB (189652978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:0cd2296657f87dc9875b44afde1718960b7c982dea8b3128a2c2e9f0ad987be2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **363.0 MB (362952137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96ec2f6ad64fe7094e57094fb3436d0709d2e3f0d3a1ec0f6ed4cc91ef594b34`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:25 GMT
ADD file:31b995b44eb1f532fd265be3fc0c3d3b55e28db0911c86a06c83de621418db94 in / 
# Wed, 01 Nov 2023 00:21:28 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:24:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:24:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:27:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:071872f8f8cb44e883168d06195f8fbb330e259b415d1ab108c27bda84d6c060`  
		Last Modified: Wed, 01 Nov 2023 00:25:41 GMT  
		Size: 53.6 MB (53575361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9986fe7e71120fd78fcaad86d3a1d827f54f56f266364834bcb7c13eccf9ca0`  
		Last Modified: Wed, 01 Nov 2023 01:40:25 GMT  
		Size: 25.7 MB (25698676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7316c6cea433a21258a8af8686d8a74e964c21c6c563afd63f274e9346f8f7`  
		Last Modified: Wed, 01 Nov 2023 01:40:48 GMT  
		Size: 69.6 MB (69584512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d43d4f467d09dbebbdbbe77e08bdef659a411541528d2d0542c5a201a1e3953`  
		Last Modified: Wed, 01 Nov 2023 01:41:31 GMT  
		Size: 214.1 MB (214093588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:2592737d5c14c9cd628b8b622a4a8d02a213a6b6a91a832feb16b338c44c95ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.2 MB (318220170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97ece825d20df85062f7e8dc9e143e2cd80da86d6928f1260cee829c756fa6c9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:42:15 GMT
ADD file:6d8ee60b2fe4604969d8feeeb7e0dc8b9619a778d1a905c8bfdde5ede5e1eb54 in / 
# Wed, 01 Nov 2023 00:42:19 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:54:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:55:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:56:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bca95e393f709ba301b35c2439a815fd4fe8134d7a466bd528563bc32fd754d8`  
		Last Modified: Wed, 01 Nov 2023 00:47:43 GMT  
		Size: 47.9 MB (47943171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e744d1ef2c8405f6352136656080d7e244e1a97362c21069b734a55b86c8d0a`  
		Last Modified: Wed, 01 Nov 2023 02:05:09 GMT  
		Size: 24.0 MB (24045096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de40af46a5373d0a49892fa9000736be09090b477719517fcec84887d847f94b`  
		Last Modified: Wed, 01 Nov 2023 02:05:25 GMT  
		Size: 63.1 MB (63132485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5d582ecd4430347fbaa4df40283ca084e7bf9c17c0ce600484712c9f61dbe3`  
		Last Modified: Wed, 01 Nov 2023 02:05:57 GMT  
		Size: 183.1 MB (183099418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bookworm-curl`

```console
$ docker pull buildpack-deps@sha256:57892e6ad71a863f2ac7fb2bb00901d96d41a257e1ef9d10c44639f1dc795ab3
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
$ docker pull buildpack-deps@sha256:81138c0eec1922d626830b19f73fea9792c263880367cde9b37fc4c021aec989
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73631171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7937fdd23222e4c8dcf166fc96dcc583d6d66bb47ac9af8d666d0e1bbace30d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:37 GMT
ADD file:3e9b6405f11dd24ce62105c033f1d8b931d9409298553f63b03af1b6dd1dda35 in / 
# Wed, 01 Nov 2023 00:20:38 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:52:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8457fd5474e70835e4482983a5662355d892d5f6f0f90a27a8e9f009997e8196`  
		Last Modified: Wed, 01 Nov 2023 00:25:05 GMT  
		Size: 49.6 MB (49582024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13baa2029dde87a21b87127168a0fb50a007c07da6b5adc8864e1fe1376c86ff`  
		Last Modified: Wed, 01 Nov 2023 01:02:01 GMT  
		Size: 24.0 MB (24049147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:ed09164fc4880f94c58fa72329b74e2deb0e9c4c49c4c89bbd311dfbec5a7108
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.1 MB (70083233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:992836c8887553b50c3a23f1fe3a3755bcd7acd42fce7ad4b6ad8137282b3ebb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:48:23 GMT
ADD file:963e26decfc65419428098047df29dcbf7865e13bcdd67abeb9849f99a7815e7 in / 
# Wed, 01 Nov 2023 00:48:23 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:53c5547a993a8adb09a632a8ae34fbc336b27a456c6b3a670865cd8bedb5e6a9`  
		Last Modified: Wed, 01 Nov 2023 00:51:04 GMT  
		Size: 47.4 MB (47355649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752979e12aac8f84972cea68e4f8d9bb1b645e71b3fc64047af1ba792dd338d9`  
		Last Modified: Wed, 01 Nov 2023 03:04:53 GMT  
		Size: 22.7 MB (22727584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1171fe398f6788003f5bacbadd2a89ea2013fff55c0f14da9e106bbcbe024a7a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67131290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a88861f4a437ff5c87eec39e153ae95413a03c4172c7e8751b0cc2825002d218`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:57:42 GMT
ADD file:3b2b4eda35d794b39d6b5567e81651625af51da3deb3f63b3ffdffa07720646e in / 
# Wed, 01 Nov 2023 00:57:42 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:30:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9bf855396a6f46c1cbac4e188af10f2c38474f989707b0b1b406b48c4b7284ef`  
		Last Modified: Wed, 01 Nov 2023 01:01:41 GMT  
		Size: 45.2 MB (45179410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6e59eca644b227cb755978679a3031e7b3f9a5c707057c293f2ba8732d8ef2`  
		Last Modified: Wed, 01 Nov 2023 02:41:40 GMT  
		Size: 22.0 MB (21951880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f82a3141ca386a79076c0ba0418c8782a361c8bb51e75deaa8866db1b2bed5ea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73197549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a409f55570736a6c820237e1f60fad4f8bb18dfc77870b144516ef2fe8e2ff11`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:32 GMT
ADD file:c934ceb4c53a1cce6779198f1ea73d5c8aad9a035e750b343d49826120ecd0eb in / 
# Wed, 01 Nov 2023 00:39:33 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:04:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8024d4fb53b2455f66d49b7ee72eb3cad5074043578238b796a9879955946a88`  
		Last Modified: Wed, 01 Nov 2023 00:42:44 GMT  
		Size: 49.6 MB (49612653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d826ee8aa65e56e167f0e27fa65cfc065687a7ac6c360787d5940d8b51f0cf1`  
		Last Modified: Wed, 01 Nov 2023 02:13:39 GMT  
		Size: 23.6 MB (23584896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:e583e18e995680fcec2033ed1ec977f42c6a379c165cc1770dc0ccef1f48ab1e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.5 MB (75485624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05e2aefc926d6cb666936937674be7f6a97c7ed0b53b7f469e95897450b1e705`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:38:46 GMT
ADD file:4043d711d8d7d1a995aed0a6998c96230765f55d4449167107955fe4af2a31db in / 
# Wed, 01 Nov 2023 00:38:47 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 13:44:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be8d77e28ff21732ba73253b6226e47e4e07ec2cedc803ffd62148df5d7a165b`  
		Last Modified: Wed, 01 Nov 2023 00:43:00 GMT  
		Size: 50.6 MB (50600049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cef920c8d790c11b84fa21c2204cca8ac6a84ec43e4a60bca3670e828748583`  
		Last Modified: Wed, 01 Nov 2023 13:55:45 GMT  
		Size: 24.9 MB (24885575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:c86473381513b077b2b848a187217476731ef8648b6efa00e40b3b540d28c8cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (73006830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5305c7a9d52eb2df81294cd30b305c75ce3a58c6c2f14ffd4fc4015d09853ad9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:08:17 GMT
ADD file:b181441dc28bc6879e29cd086c569c653171c681525c124ffb6277bd71732bb1 in / 
# Wed, 01 Nov 2023 01:08:24 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 21:17:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0bfbf01892d22dd14fb9536e8675cc932ff41f415a415fbf8c6199106b01240d`  
		Last Modified: Wed, 01 Nov 2023 01:19:01 GMT  
		Size: 49.6 MB (49568811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9310598b7549f388c445368ea2a0a4077c57ddd45436efddb37e089d293f87fe`  
		Last Modified: Wed, 01 Nov 2023 21:53:41 GMT  
		Size: 23.4 MB (23438019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:8fef9d5a3be088dbbfed19de3a7a624448239421641b6dba8621c6400edd7f06
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.3 MB (79274037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39d499c3ba7b3bc05ab676e65cd1d1351b56d80a02752dfd5053677641ce5b37`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:25 GMT
ADD file:31b995b44eb1f532fd265be3fc0c3d3b55e28db0911c86a06c83de621418db94 in / 
# Wed, 01 Nov 2023 00:21:28 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:24:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:071872f8f8cb44e883168d06195f8fbb330e259b415d1ab108c27bda84d6c060`  
		Last Modified: Wed, 01 Nov 2023 00:25:41 GMT  
		Size: 53.6 MB (53575361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9986fe7e71120fd78fcaad86d3a1d827f54f56f266364834bcb7c13eccf9ca0`  
		Last Modified: Wed, 01 Nov 2023 01:40:25 GMT  
		Size: 25.7 MB (25698676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:5f7c17a38a04a8eccaa364dd9860f483d4d838929e9817e888412ab607f0ebe1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.0 MB (71988267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:098bd7234fbac6dbe5ad9b2b1184781e15d3c49ddbd180c6247dff18efda87f8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:42:15 GMT
ADD file:6d8ee60b2fe4604969d8feeeb7e0dc8b9619a778d1a905c8bfdde5ede5e1eb54 in / 
# Wed, 01 Nov 2023 00:42:19 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:54:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bca95e393f709ba301b35c2439a815fd4fe8134d7a466bd528563bc32fd754d8`  
		Last Modified: Wed, 01 Nov 2023 00:47:43 GMT  
		Size: 47.9 MB (47943171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e744d1ef2c8405f6352136656080d7e244e1a97362c21069b734a55b86c8d0a`  
		Last Modified: Wed, 01 Nov 2023 02:05:09 GMT  
		Size: 24.0 MB (24045096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bookworm-scm`

```console
$ docker pull buildpack-deps@sha256:c128f8e680e8bfc06477d452a567975cc58188cddefc68cec3c72c1d8a15a4b2
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
$ docker pull buildpack-deps@sha256:93590f9f25a12437d9d01f7ac4309b83af5532680e36bbc01181f61e19ae7135
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.8 MB (137761586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:941f9c887621d4fee5936ccc92b35b887f74ed81aac7b90fcedc1fcb5d65741b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:37 GMT
ADD file:3e9b6405f11dd24ce62105c033f1d8b931d9409298553f63b03af1b6dd1dda35 in / 
# Wed, 01 Nov 2023 00:20:38 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:52:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 00:52:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8457fd5474e70835e4482983a5662355d892d5f6f0f90a27a8e9f009997e8196`  
		Last Modified: Wed, 01 Nov 2023 00:25:05 GMT  
		Size: 49.6 MB (49582024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13baa2029dde87a21b87127168a0fb50a007c07da6b5adc8864e1fe1376c86ff`  
		Last Modified: Wed, 01 Nov 2023 01:02:01 GMT  
		Size: 24.0 MB (24049147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:325c5bf4c2f26c11380501bec4b6eef8a3ea35b554aa1b222cbcd1e1fe11ae1d`  
		Last Modified: Wed, 01 Nov 2023 01:02:20 GMT  
		Size: 64.1 MB (64130415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:9a1d134fc9b0926e5316223c1622334e19ab18d8c110ded139188fe219084032
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.6 MB (131645049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58e29752e0aab3ef315e59c15de2796ae467eea85f7d51848bbd963d7cdcf627`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:48:23 GMT
ADD file:963e26decfc65419428098047df29dcbf7865e13bcdd67abeb9849f99a7815e7 in / 
# Wed, 01 Nov 2023 00:48:23 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:53c5547a993a8adb09a632a8ae34fbc336b27a456c6b3a670865cd8bedb5e6a9`  
		Last Modified: Wed, 01 Nov 2023 00:51:04 GMT  
		Size: 47.4 MB (47355649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752979e12aac8f84972cea68e4f8d9bb1b645e71b3fc64047af1ba792dd338d9`  
		Last Modified: Wed, 01 Nov 2023 03:04:53 GMT  
		Size: 22.7 MB (22727584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bad2403917aecfddc5d239a343aacd942aeb9c9e6d76c027cfdbb0d5479bcaa`  
		Last Modified: Wed, 01 Nov 2023 03:05:15 GMT  
		Size: 61.6 MB (61561816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:d0accba6d4ea1e12f6ab955a70a96005bac84d284fa4ca006ed0a4b165b38db4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.4 MB (126397758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8322db01431af3b3bc3e5d7ca0be48f5ea14663ef8678973003e7aef9e95fbc3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:57:42 GMT
ADD file:3b2b4eda35d794b39d6b5567e81651625af51da3deb3f63b3ffdffa07720646e in / 
# Wed, 01 Nov 2023 00:57:42 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:30:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:30:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9bf855396a6f46c1cbac4e188af10f2c38474f989707b0b1b406b48c4b7284ef`  
		Last Modified: Wed, 01 Nov 2023 01:01:41 GMT  
		Size: 45.2 MB (45179410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6e59eca644b227cb755978679a3031e7b3f9a5c707057c293f2ba8732d8ef2`  
		Last Modified: Wed, 01 Nov 2023 02:41:40 GMT  
		Size: 22.0 MB (21951880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aefa016475f9e4925fd893a9d8cfcf375937aa4e637d337806176426509dfcd`  
		Last Modified: Wed, 01 Nov 2023 02:42:04 GMT  
		Size: 59.3 MB (59266468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3cec78f7e6894f6dd48b42e66476bad2daa2533d5b6d12b2cb243c765752e854
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.2 MB (137191567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d91cf57cfc88561be3a3af9dc95f31e6740e086c0a3db3dc1bd42da9ef6313ce`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:32 GMT
ADD file:c934ceb4c53a1cce6779198f1ea73d5c8aad9a035e750b343d49826120ecd0eb in / 
# Wed, 01 Nov 2023 00:39:33 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:04:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:04:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8024d4fb53b2455f66d49b7ee72eb3cad5074043578238b796a9879955946a88`  
		Last Modified: Wed, 01 Nov 2023 00:42:44 GMT  
		Size: 49.6 MB (49612653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d826ee8aa65e56e167f0e27fa65cfc065687a7ac6c360787d5940d8b51f0cf1`  
		Last Modified: Wed, 01 Nov 2023 02:13:39 GMT  
		Size: 23.6 MB (23584896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198068495d09b6865e75ce28d5d5d5de39897b8325ada63ba80eca884ad5666b`  
		Last Modified: Wed, 01 Nov 2023 02:13:57 GMT  
		Size: 64.0 MB (63994018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:4904b1a13827dfb9dc0294607ef88a92eb6d9fb5af266f3b436b6e747de5bbc9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.5 MB (141469924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c9c6e32dc86d819a813b06b60a98e41499c7cc87049b7acf4e87c5b4c52cb05`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:38:46 GMT
ADD file:4043d711d8d7d1a995aed0a6998c96230765f55d4449167107955fe4af2a31db in / 
# Wed, 01 Nov 2023 00:38:47 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 13:44:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:44:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be8d77e28ff21732ba73253b6226e47e4e07ec2cedc803ffd62148df5d7a165b`  
		Last Modified: Wed, 01 Nov 2023 00:43:00 GMT  
		Size: 50.6 MB (50600049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cef920c8d790c11b84fa21c2204cca8ac6a84ec43e4a60bca3670e828748583`  
		Last Modified: Wed, 01 Nov 2023 13:55:45 GMT  
		Size: 24.9 MB (24885575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fee1ec8688f07e43b49247f3490035da93288449034600daee26c8ce0150a8c`  
		Last Modified: Wed, 01 Nov 2023 13:56:13 GMT  
		Size: 66.0 MB (65984300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:7512d5d9e16a66d343238bf97e5b6d176e537b37e99b90b662154d61c082523b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.0 MB (135969193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ddc1f3c73e907d5ace49797cc746b10a794acc32d29af85c665e901745196ea`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:08:17 GMT
ADD file:b181441dc28bc6879e29cd086c569c653171c681525c124ffb6277bd71732bb1 in / 
# Wed, 01 Nov 2023 01:08:24 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 21:17:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 21:19:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0bfbf01892d22dd14fb9536e8675cc932ff41f415a415fbf8c6199106b01240d`  
		Last Modified: Wed, 01 Nov 2023 01:19:01 GMT  
		Size: 49.6 MB (49568811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9310598b7549f388c445368ea2a0a4077c57ddd45436efddb37e089d293f87fe`  
		Last Modified: Wed, 01 Nov 2023 21:53:41 GMT  
		Size: 23.4 MB (23438019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af2206444fab218d319700cbfcd93423bf4622bb8085adee11b684b7d3fd245`  
		Last Modified: Wed, 01 Nov 2023 21:54:35 GMT  
		Size: 63.0 MB (62962363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:e720e0531751cf77d1933f62e84bc5d4d2d63c0da3d890797548ca4e0192e571
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.9 MB (148858549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffb46a21911fb664a3630a45e7195ee955092521b2066322ec031cd4dd405ff3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:25 GMT
ADD file:31b995b44eb1f532fd265be3fc0c3d3b55e28db0911c86a06c83de621418db94 in / 
# Wed, 01 Nov 2023 00:21:28 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:24:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:24:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:071872f8f8cb44e883168d06195f8fbb330e259b415d1ab108c27bda84d6c060`  
		Last Modified: Wed, 01 Nov 2023 00:25:41 GMT  
		Size: 53.6 MB (53575361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9986fe7e71120fd78fcaad86d3a1d827f54f56f266364834bcb7c13eccf9ca0`  
		Last Modified: Wed, 01 Nov 2023 01:40:25 GMT  
		Size: 25.7 MB (25698676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7316c6cea433a21258a8af8686d8a74e964c21c6c563afd63f274e9346f8f7`  
		Last Modified: Wed, 01 Nov 2023 01:40:48 GMT  
		Size: 69.6 MB (69584512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:09520ba698b0b094ea1454bc687588fec9372d55e89e0b94e6afd1a415c1466f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.1 MB (135120752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e276550e9f3dc4f49a7d31441193c04d44abfc4220d18845eec66bdbbb473977`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:42:15 GMT
ADD file:6d8ee60b2fe4604969d8feeeb7e0dc8b9619a778d1a905c8bfdde5ede5e1eb54 in / 
# Wed, 01 Nov 2023 00:42:19 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:54:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:55:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bca95e393f709ba301b35c2439a815fd4fe8134d7a466bd528563bc32fd754d8`  
		Last Modified: Wed, 01 Nov 2023 00:47:43 GMT  
		Size: 47.9 MB (47943171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e744d1ef2c8405f6352136656080d7e244e1a97362c21069b734a55b86c8d0a`  
		Last Modified: Wed, 01 Nov 2023 02:05:09 GMT  
		Size: 24.0 MB (24045096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de40af46a5373d0a49892fa9000736be09090b477719517fcec84887d847f94b`  
		Last Modified: Wed, 01 Nov 2023 02:05:25 GMT  
		Size: 63.1 MB (63132485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bullseye`

```console
$ docker pull buildpack-deps@sha256:91d0d87bdeb73250aa8b9bc1739ab59e0df4e365dd7e459d1d453d46befd93c3
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
$ docker pull buildpack-deps@sha256:e5b39fe0f583451250fadb67733c6d8a9c946ac57311eb29e32f2ef2fe4738d8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.3 MB (322297709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:337d5c3296dbe61598d78522d56582f1893dbf23ecf8b2a563411e498bdbf0c7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:59 GMT
ADD file:da3938f00f114fa8f5948fb7182da39c43e5ce57a334ba528681cb29aff0d2f6 in / 
# Wed, 01 Nov 2023 00:21:00 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:53:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 00:54:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 00:55:16 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2f088d622efd8dbaa13d01eafd0aac8f9f33bb335edd3be897ae8059338c7bf7`  
		Last Modified: Wed, 01 Nov 2023 00:25:49 GMT  
		Size: 55.1 MB (55058052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de448b80f06437f3025dcaa9285d40c9c81e4be00df1b04bd5a26fd6b9447fc8`  
		Last Modified: Wed, 01 Nov 2023 01:03:07 GMT  
		Size: 15.8 MB (15764212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24e5da9a0e1f93fa4f1a07ca9a691e0d941bab6927f80157ffc14b478815f95b`  
		Last Modified: Wed, 01 Nov 2023 01:03:23 GMT  
		Size: 54.6 MB (54595619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d61681290435197504d4cdaa3724700bd66544d064d068e837f70e5abede255`  
		Last Modified: Wed, 01 Nov 2023 01:03:55 GMT  
		Size: 196.9 MB (196879826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:e498b9b502d1ca1acfa852d25bfce183b268515664ebfcc3a4e87c68e4725e1d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.4 MB (295371150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f3c22a828484005d7d76c4c66e1b944be8c68f20bcc8ecd02ac88b1b12ca17a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:48:39 GMT
ADD file:6fcdedd346da0744f7f45d0e7df77336a37ce87345bd414bd4e198804980781e in / 
# Wed, 01 Nov 2023 00:48:40 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:57:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:57:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:59:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e0adb3cac2906548cd3544bf3c384be3e3bdca9d41c37e11c160813af74301b9`  
		Last Modified: Wed, 01 Nov 2023 00:51:49 GMT  
		Size: 52.6 MB (52563334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f1ac168a113a53eb04058318b3d7cb7470e780e76570d1454453907e7a8707`  
		Last Modified: Wed, 01 Nov 2023 03:06:05 GMT  
		Size: 15.4 MB (15374711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17505c8dbffa755d9815a1b1f2a760d22100354db441079cb21283d37a0f5cae`  
		Last Modified: Wed, 01 Nov 2023 03:06:23 GMT  
		Size: 52.3 MB (52331088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af45e26d5b203d7ce4ea96b10a3e560243b596a031d560011445a0febbf5983`  
		Last Modified: Wed, 01 Nov 2023 03:06:58 GMT  
		Size: 175.1 MB (175102017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:0ec89f8bc6a95decbf549e0463c9560d0705af1099c8c4e66dc388810624ab4a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.8 MB (282800617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b7746f40355811236974bb35f0f769d9275f70b839f97e18e010fdff459f6dd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:58:01 GMT
ADD file:5e11ff51eeca3d0b7e760186b5792864fee2bfe7e8a1fa531a89870abaebfc89 in / 
# Wed, 01 Nov 2023 00:58:02 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:31:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:32:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:33:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:17b69ad2612f8fffb539ede3765dcc1fbd121518fd38fe89720482d622dbc960`  
		Last Modified: Wed, 01 Nov 2023 01:02:32 GMT  
		Size: 50.2 MB (50215350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0803d90cd63c47dea677f156a9802a95d09886d9a3b07415dd94b2ac199f25`  
		Last Modified: Wed, 01 Nov 2023 02:43:01 GMT  
		Size: 14.9 MB (14879723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524b9dc19e6fd54f3a85453a84bc99da2ca6e508d91ce084872e33c6c60d774c`  
		Last Modified: Wed, 01 Nov 2023 02:43:18 GMT  
		Size: 50.4 MB (50353285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b091dd2c95f61d367ee00244a69ce9fbbbe3b5cf82c05e675bfeb00a2d248480`  
		Last Modified: Wed, 01 Nov 2023 02:43:48 GMT  
		Size: 167.4 MB (167352259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:507681f36e1adb6d525f95c0a2d182fc847c2d74bb04e84db4fe41a55b1a6ccf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.0 MB (313958442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8f1530a08d0a05c65962560d0105156de41a165257827ced93a5c5c30c81e0a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:48 GMT
ADD file:f5677286e85ce6a345c7f5937e1ec576c37228e49c0fafe33574614c81cb7f76 in / 
# Wed, 01 Nov 2023 00:39:48 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:06:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:06:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:07:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d42ebdfc37acca5c3acbe173ac11133e691b402003a525c2b8431baf6935291e`  
		Last Modified: Wed, 01 Nov 2023 00:43:25 GMT  
		Size: 53.7 MB (53707757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098bcc814ee5bafa2842bc45ecc3974bc4f2b66d05b05a8da5ac0c9fb91be947`  
		Last Modified: Wed, 01 Nov 2023 02:14:42 GMT  
		Size: 15.7 MB (15749872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e627bbf1475bea4dce35bb2c9ee58b6eb3be5573e4efe8bd5793ae6a1555118`  
		Last Modified: Wed, 01 Nov 2023 02:14:57 GMT  
		Size: 54.7 MB (54699568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1aedf10290011154f8817dfb0b21ae189951f1bfcc41d82b3ed061ae69c6ff9`  
		Last Modified: Wed, 01 Nov 2023 02:15:24 GMT  
		Size: 189.8 MB (189801245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; 386

```console
$ docker pull buildpack-deps@sha256:e86c91c91fe62b43e8e45b32b82fa0be22969497a312e05cf39a51aaeaf67f4f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.0 MB (328046228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47bcedab4330997f14313c4b8012559714b4c4a50ae19a963576cfd318fd4659`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:06 GMT
ADD file:4095d27bc1a281dda044919be3bb570d581df169c01f22b0963b38e0dd6d9eff in / 
# Wed, 01 Nov 2023 00:39:07 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 13:46:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:46:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:47:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:95d6aa56ba74b8ed0a732c4676a2c45c84a18076696d466cd9bf0b459c600e02`  
		Last Modified: Wed, 01 Nov 2023 00:43:49 GMT  
		Size: 56.0 MB (56046261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a221a3957c157fc6091d669757aa644810547d3e3fcf1e1af9da5c23408ccfd`  
		Last Modified: Wed, 01 Nov 2023 13:57:18 GMT  
		Size: 16.3 MB (16268154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae620e9f38cdbc37cabf7785918528f2cabd2fc93a6f2df4a0536a17c985a83`  
		Last Modified: Wed, 01 Nov 2023 13:57:39 GMT  
		Size: 55.9 MB (55937130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3adf864130f60c8d2fc5630732c739bcbf96036834ad946abd62c2b01311aa01`  
		Last Modified: Wed, 01 Nov 2023 13:58:23 GMT  
		Size: 199.8 MB (199794683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:e594b6e1cfae9243fd7cbefe66cf6bc57a66bc539bdeed15fd448e150064a0fa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.1 MB (301123609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71ec146db4e94ece054208dbb3d587c01e6c09b362a2191332a29dca4e72a5ca`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:09:34 GMT
ADD file:2c9f9140e731974a497825454c08d67829f514a83742973e30454cc905ebac6c in / 
# Wed, 01 Nov 2023 01:09:39 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 21:26:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 21:27:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 21:33:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a10c6e715fcf314db953339b3e58b9e0167f6cd2d02bf633e20282058eb83331`  
		Last Modified: Wed, 01 Nov 2023 01:20:31 GMT  
		Size: 53.3 MB (53288991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe6d659051b6e411cbd9b3be6e727341a73a5b15c0c29975704b7249f84fd86`  
		Last Modified: Wed, 01 Nov 2023 21:57:24 GMT  
		Size: 15.5 MB (15529696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8566d8664b53694b0954345257a0d1054f4e6986ca39c2e219045fec1804bca9`  
		Last Modified: Wed, 01 Nov 2023 21:58:10 GMT  
		Size: 53.3 MB (53302576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9127ef70b3d7f2c8696b4631dc66ee403ee865e060aa586e35ac9ae4217dfca`  
		Last Modified: Wed, 01 Nov 2023 22:00:10 GMT  
		Size: 179.0 MB (179002346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:82bc2a3f618b2276770a5b4e66fc4eb97dc374aa4d6262bc4f8e7328416884d7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.8 MB (330808710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac93ae090ca7af9095be55d239af46ce549e519e63cef45c4c9cf11e16473ea5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:51 GMT
ADD file:68e9024f0c99fe38d7046b4ad1aee044d14b93d248ec431380a1cefcacb7dea3 in / 
# Wed, 01 Nov 2023 00:21:54 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:27:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:28:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:31:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d002f39ef040587852c73a806a7f49edd2ae7eb78b997c05ca1c5bfedad0506d`  
		Last Modified: Wed, 01 Nov 2023 00:26:33 GMT  
		Size: 58.9 MB (58929494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8932ef1d4dad602784eb2f811c1c987e261b97dfbc072a2c097836198cc588b`  
		Last Modified: Wed, 01 Nov 2023 01:41:47 GMT  
		Size: 16.8 MB (16765480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5598ff1b384ed8a267e359e36806478cf035252da4caca5d70aae48d01bcde`  
		Last Modified: Wed, 01 Nov 2023 01:42:05 GMT  
		Size: 58.9 MB (58865922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b8984065c2be285a155b4228b44b214dc7b7918b687b2c17d3e3136e5a7b03`  
		Last Modified: Wed, 01 Nov 2023 01:42:43 GMT  
		Size: 196.2 MB (196247814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:9d61cfff42a2c3154228569b2d18a12fa0110f89af96c3c01f32a15657e5fbde
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.9 MB (295893097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:899a28fa35119cbb45aec21c0d234226f5e5ea9d03d265db0ae96dda474a9660`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:42:50 GMT
ADD file:5c168741fe0b80d3b365ae703c082556326a889730963a304b218ab3361d2e8a in / 
# Wed, 01 Nov 2023 00:42:54 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:56:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:57:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:58:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a21b3124d41be76bb35d41f49b041980e640c1ea030b4099c4eaa419414f1618`  
		Last Modified: Wed, 01 Nov 2023 00:48:19 GMT  
		Size: 53.3 MB (53296572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb969a0416e6d103d044f625db373b704e7253a5661a213c76711df733f8db0`  
		Last Modified: Wed, 01 Nov 2023 02:06:09 GMT  
		Size: 15.6 MB (15640071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6df2909ff3ad376afb0b5c8415d39aa102919dfc8415cd2c3d3ab0866cb8794`  
		Last Modified: Wed, 01 Nov 2023 02:06:23 GMT  
		Size: 54.1 MB (54065848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7c416e9929ef46a9a0f52c4720975b46e23cda524123c9f33d3d9bf287a380`  
		Last Modified: Wed, 01 Nov 2023 02:06:49 GMT  
		Size: 172.9 MB (172890606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bullseye-curl`

```console
$ docker pull buildpack-deps@sha256:daee6a831682d0fef3be9af87ffa7b513a8923199f3ee75e63d787ca7a0eb445
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
$ docker pull buildpack-deps@sha256:fe96c991e03a42155f09f164fab997201cd385d51b961d79c2cee47dad3fa471
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.8 MB (70822264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9267342af80900380a694508ac882c18c81244c1790e1a82484f2b23e45b6ce5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:59 GMT
ADD file:da3938f00f114fa8f5948fb7182da39c43e5ce57a334ba528681cb29aff0d2f6 in / 
# Wed, 01 Nov 2023 00:21:00 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:53:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2f088d622efd8dbaa13d01eafd0aac8f9f33bb335edd3be897ae8059338c7bf7`  
		Last Modified: Wed, 01 Nov 2023 00:25:49 GMT  
		Size: 55.1 MB (55058052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de448b80f06437f3025dcaa9285d40c9c81e4be00df1b04bd5a26fd6b9447fc8`  
		Last Modified: Wed, 01 Nov 2023 01:03:07 GMT  
		Size: 15.8 MB (15764212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:7b311b6096eb6345ca23254eedd11cdc452439fd11a0f754602457b1cd51f5af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.9 MB (67938045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fdeee1b038c70ec83b9f0de8673d6232c0d52472bde1372852e3c01a3e7fb2d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:48:39 GMT
ADD file:6fcdedd346da0744f7f45d0e7df77336a37ce87345bd414bd4e198804980781e in / 
# Wed, 01 Nov 2023 00:48:40 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:57:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e0adb3cac2906548cd3544bf3c384be3e3bdca9d41c37e11c160813af74301b9`  
		Last Modified: Wed, 01 Nov 2023 00:51:49 GMT  
		Size: 52.6 MB (52563334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f1ac168a113a53eb04058318b3d7cb7470e780e76570d1454453907e7a8707`  
		Last Modified: Wed, 01 Nov 2023 03:06:05 GMT  
		Size: 15.4 MB (15374711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:938715a48d3af6947e95b1ba3f7d072a0383966fa35cb4e543d0df56d5f09ac7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.1 MB (65095073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de18a5e0f396c35eee7ef96ee7cf1030ac0c1aba47e9a7311dae5b771137335c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:58:01 GMT
ADD file:5e11ff51eeca3d0b7e760186b5792864fee2bfe7e8a1fa531a89870abaebfc89 in / 
# Wed, 01 Nov 2023 00:58:02 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:31:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:17b69ad2612f8fffb539ede3765dcc1fbd121518fd38fe89720482d622dbc960`  
		Last Modified: Wed, 01 Nov 2023 01:02:32 GMT  
		Size: 50.2 MB (50215350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0803d90cd63c47dea677f156a9802a95d09886d9a3b07415dd94b2ac199f25`  
		Last Modified: Wed, 01 Nov 2023 02:43:01 GMT  
		Size: 14.9 MB (14879723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a5756865ff5b689520b2adc61fe9c4e1d05fc87bc136dd6f8e4e84e7aa595583
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69457629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0307db700b406ff0f670aafedc3682ef7699b96e9b1288101822e3417b87d6ca`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:48 GMT
ADD file:f5677286e85ce6a345c7f5937e1ec576c37228e49c0fafe33574614c81cb7f76 in / 
# Wed, 01 Nov 2023 00:39:48 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:06:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d42ebdfc37acca5c3acbe173ac11133e691b402003a525c2b8431baf6935291e`  
		Last Modified: Wed, 01 Nov 2023 00:43:25 GMT  
		Size: 53.7 MB (53707757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098bcc814ee5bafa2842bc45ecc3974bc4f2b66d05b05a8da5ac0c9fb91be947`  
		Last Modified: Wed, 01 Nov 2023 02:14:42 GMT  
		Size: 15.7 MB (15749872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:3031323302eaff84a691d3ee86f673dcf58faec6ca26af36306a26264bf3fc4b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.3 MB (72314415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30e808a609f652bd8bfd97a50be155e7b8cd8f48d49c5dcca1574139b8b52ebc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:06 GMT
ADD file:4095d27bc1a281dda044919be3bb570d581df169c01f22b0963b38e0dd6d9eff in / 
# Wed, 01 Nov 2023 00:39:07 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 13:46:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:95d6aa56ba74b8ed0a732c4676a2c45c84a18076696d466cd9bf0b459c600e02`  
		Last Modified: Wed, 01 Nov 2023 00:43:49 GMT  
		Size: 56.0 MB (56046261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a221a3957c157fc6091d669757aa644810547d3e3fcf1e1af9da5c23408ccfd`  
		Last Modified: Wed, 01 Nov 2023 13:57:18 GMT  
		Size: 16.3 MB (16268154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:d8e9e7111c1ffedd6d881f3b0e23d591e549254d9769e151fd5b120c2722c378
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68818687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1dca7251f559caeddfa4e791323c9b2839014697d5e5af163f859e9a94e594c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:09:34 GMT
ADD file:2c9f9140e731974a497825454c08d67829f514a83742973e30454cc905ebac6c in / 
# Wed, 01 Nov 2023 01:09:39 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 21:26:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a10c6e715fcf314db953339b3e58b9e0167f6cd2d02bf633e20282058eb83331`  
		Last Modified: Wed, 01 Nov 2023 01:20:31 GMT  
		Size: 53.3 MB (53288991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe6d659051b6e411cbd9b3be6e727341a73a5b15c0c29975704b7249f84fd86`  
		Last Modified: Wed, 01 Nov 2023 21:57:24 GMT  
		Size: 15.5 MB (15529696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:7cc922cccb492c0a7586506eb781cfd4aca3122d5bad473bcc57f8faf10f1b9a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75694974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b4307adf590ebe3c7869b5b22159689cfaa09e73b33741d2ccb188a374ee2ac`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:51 GMT
ADD file:68e9024f0c99fe38d7046b4ad1aee044d14b93d248ec431380a1cefcacb7dea3 in / 
# Wed, 01 Nov 2023 00:21:54 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:27:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d002f39ef040587852c73a806a7f49edd2ae7eb78b997c05ca1c5bfedad0506d`  
		Last Modified: Wed, 01 Nov 2023 00:26:33 GMT  
		Size: 58.9 MB (58929494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8932ef1d4dad602784eb2f811c1c987e261b97dfbc072a2c097836198cc588b`  
		Last Modified: Wed, 01 Nov 2023 01:41:47 GMT  
		Size: 16.8 MB (16765480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:cef619c4e2fff9d2bd0e6bcc3b9254d2e33f7347143cc9124087dee5433f476f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68936643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:899170b75ff49b852db13ad9fd0b8e0b9c69f7fa9fa438bfea0bd62bddfd75bd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:42:50 GMT
ADD file:5c168741fe0b80d3b365ae703c082556326a889730963a304b218ab3361d2e8a in / 
# Wed, 01 Nov 2023 00:42:54 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:56:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a21b3124d41be76bb35d41f49b041980e640c1ea030b4099c4eaa419414f1618`  
		Last Modified: Wed, 01 Nov 2023 00:48:19 GMT  
		Size: 53.3 MB (53296572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb969a0416e6d103d044f625db373b704e7253a5661a213c76711df733f8db0`  
		Last Modified: Wed, 01 Nov 2023 02:06:09 GMT  
		Size: 15.6 MB (15640071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bullseye-scm`

```console
$ docker pull buildpack-deps@sha256:70ff4e786a57b07a66e70fc4ac621abc2f85c90c8a50c92db1004d750f1afceb
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
$ docker pull buildpack-deps@sha256:aee2844de5599ce4ea6389a884d8cd4a8de58712b6e5a02d62251f18e8696060
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.4 MB (125417883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c9ef67b38f3703597d152b6d1c032033b993b1828d68fe7495ac3768f7a967b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:59 GMT
ADD file:da3938f00f114fa8f5948fb7182da39c43e5ce57a334ba528681cb29aff0d2f6 in / 
# Wed, 01 Nov 2023 00:21:00 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:53:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 00:54:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2f088d622efd8dbaa13d01eafd0aac8f9f33bb335edd3be897ae8059338c7bf7`  
		Last Modified: Wed, 01 Nov 2023 00:25:49 GMT  
		Size: 55.1 MB (55058052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de448b80f06437f3025dcaa9285d40c9c81e4be00df1b04bd5a26fd6b9447fc8`  
		Last Modified: Wed, 01 Nov 2023 01:03:07 GMT  
		Size: 15.8 MB (15764212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24e5da9a0e1f93fa4f1a07ca9a691e0d941bab6927f80157ffc14b478815f95b`  
		Last Modified: Wed, 01 Nov 2023 01:03:23 GMT  
		Size: 54.6 MB (54595619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:dc112c6d13a25d02bc6c10da7320cf3cd72abcd6902b3d8b1daa1b435692630b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.3 MB (120269133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3eba71c7387e8a339718a365505f0baf67502bf260281df1d28565c819cf769`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:48:39 GMT
ADD file:6fcdedd346da0744f7f45d0e7df77336a37ce87345bd414bd4e198804980781e in / 
# Wed, 01 Nov 2023 00:48:40 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:57:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:57:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e0adb3cac2906548cd3544bf3c384be3e3bdca9d41c37e11c160813af74301b9`  
		Last Modified: Wed, 01 Nov 2023 00:51:49 GMT  
		Size: 52.6 MB (52563334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f1ac168a113a53eb04058318b3d7cb7470e780e76570d1454453907e7a8707`  
		Last Modified: Wed, 01 Nov 2023 03:06:05 GMT  
		Size: 15.4 MB (15374711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17505c8dbffa755d9815a1b1f2a760d22100354db441079cb21283d37a0f5cae`  
		Last Modified: Wed, 01 Nov 2023 03:06:23 GMT  
		Size: 52.3 MB (52331088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f91a8bb800cf9f7759f256b610549bab7137aa27b412e565c153877592aa25fc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115448358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7293fc0d511b0567083617d783259480fb8c6f9398173f21707a6aa45f36094`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:58:01 GMT
ADD file:5e11ff51eeca3d0b7e760186b5792864fee2bfe7e8a1fa531a89870abaebfc89 in / 
# Wed, 01 Nov 2023 00:58:02 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:31:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:32:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:17b69ad2612f8fffb539ede3765dcc1fbd121518fd38fe89720482d622dbc960`  
		Last Modified: Wed, 01 Nov 2023 01:02:32 GMT  
		Size: 50.2 MB (50215350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0803d90cd63c47dea677f156a9802a95d09886d9a3b07415dd94b2ac199f25`  
		Last Modified: Wed, 01 Nov 2023 02:43:01 GMT  
		Size: 14.9 MB (14879723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524b9dc19e6fd54f3a85453a84bc99da2ca6e508d91ce084872e33c6c60d774c`  
		Last Modified: Wed, 01 Nov 2023 02:43:18 GMT  
		Size: 50.4 MB (50353285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:4cf4511cd7836341048828afed7f6f64760851ab73b5d451014aae119afa1a8d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124157197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfed8a1aba30dc750dde56fe15716729ccb292429fe81882481c660fc3e3fc70`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:48 GMT
ADD file:f5677286e85ce6a345c7f5937e1ec576c37228e49c0fafe33574614c81cb7f76 in / 
# Wed, 01 Nov 2023 00:39:48 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:06:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:06:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d42ebdfc37acca5c3acbe173ac11133e691b402003a525c2b8431baf6935291e`  
		Last Modified: Wed, 01 Nov 2023 00:43:25 GMT  
		Size: 53.7 MB (53707757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098bcc814ee5bafa2842bc45ecc3974bc4f2b66d05b05a8da5ac0c9fb91be947`  
		Last Modified: Wed, 01 Nov 2023 02:14:42 GMT  
		Size: 15.7 MB (15749872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e627bbf1475bea4dce35bb2c9ee58b6eb3be5573e4efe8bd5793ae6a1555118`  
		Last Modified: Wed, 01 Nov 2023 02:14:57 GMT  
		Size: 54.7 MB (54699568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8d58db39b5254846274374168677310fff3253244bf5a6d2ce6260f6a954d56f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128251545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00fcd7435762272d60c82baecddc1312882335ef3b4d818cd0b3c67fecf85729`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:06 GMT
ADD file:4095d27bc1a281dda044919be3bb570d581df169c01f22b0963b38e0dd6d9eff in / 
# Wed, 01 Nov 2023 00:39:07 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 13:46:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:46:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:95d6aa56ba74b8ed0a732c4676a2c45c84a18076696d466cd9bf0b459c600e02`  
		Last Modified: Wed, 01 Nov 2023 00:43:49 GMT  
		Size: 56.0 MB (56046261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a221a3957c157fc6091d669757aa644810547d3e3fcf1e1af9da5c23408ccfd`  
		Last Modified: Wed, 01 Nov 2023 13:57:18 GMT  
		Size: 16.3 MB (16268154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae620e9f38cdbc37cabf7785918528f2cabd2fc93a6f2df4a0536a17c985a83`  
		Last Modified: Wed, 01 Nov 2023 13:57:39 GMT  
		Size: 55.9 MB (55937130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:d93ee9ee466572ddc358a190303042e8ecbc24d89865152f38eea95055e713f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122121263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db1876f7fa25cbcab884a102075bd6f8684bba0e6b6360ff846167f0de396728`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:09:34 GMT
ADD file:2c9f9140e731974a497825454c08d67829f514a83742973e30454cc905ebac6c in / 
# Wed, 01 Nov 2023 01:09:39 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 21:26:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 21:27:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a10c6e715fcf314db953339b3e58b9e0167f6cd2d02bf633e20282058eb83331`  
		Last Modified: Wed, 01 Nov 2023 01:20:31 GMT  
		Size: 53.3 MB (53288991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe6d659051b6e411cbd9b3be6e727341a73a5b15c0c29975704b7249f84fd86`  
		Last Modified: Wed, 01 Nov 2023 21:57:24 GMT  
		Size: 15.5 MB (15529696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8566d8664b53694b0954345257a0d1054f4e6986ca39c2e219045fec1804bca9`  
		Last Modified: Wed, 01 Nov 2023 21:58:10 GMT  
		Size: 53.3 MB (53302576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:8117582621ca40cd9aa664d7a8920f2829422f7c27388f12eb20f8203c6d4015
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.6 MB (134560896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec96f11e0d12047d5722fc5d69d37309a058d1ed16360cb007b03aaf3c4c034b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:51 GMT
ADD file:68e9024f0c99fe38d7046b4ad1aee044d14b93d248ec431380a1cefcacb7dea3 in / 
# Wed, 01 Nov 2023 00:21:54 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:27:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:28:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d002f39ef040587852c73a806a7f49edd2ae7eb78b997c05ca1c5bfedad0506d`  
		Last Modified: Wed, 01 Nov 2023 00:26:33 GMT  
		Size: 58.9 MB (58929494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8932ef1d4dad602784eb2f811c1c987e261b97dfbc072a2c097836198cc588b`  
		Last Modified: Wed, 01 Nov 2023 01:41:47 GMT  
		Size: 16.8 MB (16765480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5598ff1b384ed8a267e359e36806478cf035252da4caca5d70aae48d01bcde`  
		Last Modified: Wed, 01 Nov 2023 01:42:05 GMT  
		Size: 58.9 MB (58865922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:87a81ace16049e3a81cb4550162435a699f3d58045130f0693a7b7092b14f2d3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123002491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e97a46624fdc756523296a468935e44b34cfc5c8fa801fc0471b51842f34f960`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:42:50 GMT
ADD file:5c168741fe0b80d3b365ae703c082556326a889730963a304b218ab3361d2e8a in / 
# Wed, 01 Nov 2023 00:42:54 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:56:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:57:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a21b3124d41be76bb35d41f49b041980e640c1ea030b4099c4eaa419414f1618`  
		Last Modified: Wed, 01 Nov 2023 00:48:19 GMT  
		Size: 53.3 MB (53296572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb969a0416e6d103d044f625db373b704e7253a5661a213c76711df733f8db0`  
		Last Modified: Wed, 01 Nov 2023 02:06:09 GMT  
		Size: 15.6 MB (15640071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6df2909ff3ad376afb0b5c8415d39aa102919dfc8415cd2c3d3ab0866cb8794`  
		Last Modified: Wed, 01 Nov 2023 02:06:23 GMT  
		Size: 54.1 MB (54065848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:buster`

```console
$ docker pull buildpack-deps@sha256:994c0590e60c01834f0b716a12087fa53cdc8751260c9924a698e38e9548e12a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:buster` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:ad93c92a1a49a84211028e913750883a2f28de561fde391a39714867ba406d36
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.9 MB (311867207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cbe55f5e882a696ded59f2a4da88985cff31ead69b6e59a7690a13e9fc6434d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:21 GMT
ADD file:e12306e266f3e237ff7df5ea95bd339c3eb4a539f31be801afd63a76e116f522 in / 
# Wed, 01 Nov 2023 00:21:22 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:55:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 00:56:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 00:57:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:711706b827bb26857b90ceb32b653a05be0e06459342cc05124da0f97f9b6ad9`  
		Last Modified: Wed, 01 Nov 2023 00:26:31 GMT  
		Size: 50.5 MB (50499123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465ae13a022e930633aeb58ebf812a0350a4ec43803e013187863d358e62f15f`  
		Last Modified: Wed, 01 Nov 2023 01:04:06 GMT  
		Size: 17.6 MB (17583932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac648dffba596ed8d982778472e34b8ba1ad650a3ea934c0c1b202e63e338860`  
		Last Modified: Wed, 01 Nov 2023 01:04:21 GMT  
		Size: 51.9 MB (51873954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1729d430e574c53c4882a063283bce8773703ecdcd1c010c604c04bcb85340f`  
		Last Modified: Wed, 01 Nov 2023 01:04:52 GMT  
		Size: 191.9 MB (191910198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:23e96132f6b9dd83ade53635f26ad7a584f1ff76e6fb6a6c4dbaeaa32fa9daf0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.7 MB (277696007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f06d6e26d9616bddfad69e554ee321e043cb2568e5064592ac36f28b66bfd3e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:58:20 GMT
ADD file:ff8efe260318f1cfb8bfc8aaaa6d6bb15c878689f7edea37d776cf111c30fefb in / 
# Wed, 01 Nov 2023 00:58:20 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:33:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:34:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:35:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:608341ab24b1ec00c021d73e16dbb8ca54b2437a4a3f5ae09ca58578603a32bf`  
		Last Modified: Wed, 01 Nov 2023 01:03:18 GMT  
		Size: 46.0 MB (45966058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d69be9a283bc43e8f0b0d0da1bb41aaf159446bc58f5d8f73cd7c86fd9d3cc`  
		Last Modified: Wed, 01 Nov 2023 02:44:00 GMT  
		Size: 16.2 MB (16215741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0b6d0aa1dff66e917c4bbec58a8d82c3bf1380c7772452e657e0e4ad5c190e`  
		Last Modified: Wed, 01 Nov 2023 02:44:16 GMT  
		Size: 47.4 MB (47411022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ef6c73d3c316731b1f2a4a1e12f29f955579feed16f8ddb603886d76efef32`  
		Last Modified: Wed, 01 Nov 2023 02:44:46 GMT  
		Size: 168.1 MB (168103186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:1a8d69bac6a059b10a24162a21252d8a3c9494d8290277547234d54872ae3daf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.4 MB (302430569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a503fe9299e3ee1608bed8a555b831e6f4e3de9b36c05c0a1590d3a4b266b812`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:40:02 GMT
ADD file:e3f63671dca138b2b525b60f1471241941cdf4dab7f0c17cd91124978716bd93 in / 
# Wed, 01 Nov 2023 00:40:02 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:07:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:07:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:08:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d3db7215fb502c5873a81db7c6fd3214f199f6a1d8034da9d90918ac3220b20b`  
		Last Modified: Wed, 01 Nov 2023 00:44:04 GMT  
		Size: 49.3 MB (49291092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273f65b8dba688a4aab84c27f594891edb3518fd96d226c06ca7667c8c2a5b06`  
		Last Modified: Wed, 01 Nov 2023 02:15:35 GMT  
		Size: 17.5 MB (17454091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c150f07b6a196359013d5fe6373a86fec69409163977b1cd213268cd033d320c`  
		Last Modified: Wed, 01 Nov 2023 02:15:49 GMT  
		Size: 52.2 MB (52208340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e75642759fbcf85e98624fae6727771f0e966a4debdef80548654cb137d1609`  
		Last Modified: Wed, 01 Nov 2023 02:16:15 GMT  
		Size: 183.5 MB (183477046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; 386

```console
$ docker pull buildpack-deps@sha256:4a2c1f92814c3a19ccbc81bc64a1b343bf0c601559c1e742946c3c14e1234d14
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.3 MB (321284071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccd929b52893acac0a10a782e89423a5ceff76790faf025f06a885343b371517`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:28 GMT
ADD file:65beb9bd9a5ca258316260fb802c65d9c3cc4a9137e0a09a873d4404d5b24fcc in / 
# Wed, 01 Nov 2023 00:39:29 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 13:48:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:48:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:50:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2e1a1831feefb5bd8f0a9fbc43f06ac287e16d9dd672e28d11eb17f3df2c71cd`  
		Last Modified: Wed, 01 Nov 2023 00:44:36 GMT  
		Size: 51.3 MB (51255735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4efeebbb8917115755445da9fb58c99b67f18a2552b83c24eb9b3a6b280700de`  
		Last Modified: Wed, 01 Nov 2023 13:58:36 GMT  
		Size: 18.1 MB (18099490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52765542e10643f266bb59e790311fa685b420f7ddf55344e27da30b0e98fb64`  
		Last Modified: Wed, 01 Nov 2023 13:58:57 GMT  
		Size: 53.5 MB (53488289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edccb9c788dcbf10ac8a2c7dea85d9116e0b0bb24b034ce8a03e4e00cb5820b2`  
		Last Modified: Wed, 01 Nov 2023 13:59:40 GMT  
		Size: 198.4 MB (198440557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:buster-curl`

```console
$ docker pull buildpack-deps@sha256:6f247f6bed7b6840e5c67f0438cddaec352488db0748e6f1d8a712f493d11802
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:buster-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:8c5b0be8284f3ffad21b631a565d95b206ad13fd7fab4860bed8ae57dbec5bd3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68083055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffa032cdabe4be1922293729cab49304bdbfc5bb0a7ecf88d15b26752bcd58a6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:21 GMT
ADD file:e12306e266f3e237ff7df5ea95bd339c3eb4a539f31be801afd63a76e116f522 in / 
# Wed, 01 Nov 2023 00:21:22 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:55:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:711706b827bb26857b90ceb32b653a05be0e06459342cc05124da0f97f9b6ad9`  
		Last Modified: Wed, 01 Nov 2023 00:26:31 GMT  
		Size: 50.5 MB (50499123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465ae13a022e930633aeb58ebf812a0350a4ec43803e013187863d358e62f15f`  
		Last Modified: Wed, 01 Nov 2023 01:04:06 GMT  
		Size: 17.6 MB (17583932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:547c920f8106c64ef8fef69ea98bbb06f3f5db4cb6e6ce5e702a3d48326dbbac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62181799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:842dffaf721877ed8fd91016937a055c084b9f96228d966abacc70503596ee76`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:58:20 GMT
ADD file:ff8efe260318f1cfb8bfc8aaaa6d6bb15c878689f7edea37d776cf111c30fefb in / 
# Wed, 01 Nov 2023 00:58:20 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:33:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:608341ab24b1ec00c021d73e16dbb8ca54b2437a4a3f5ae09ca58578603a32bf`  
		Last Modified: Wed, 01 Nov 2023 01:03:18 GMT  
		Size: 46.0 MB (45966058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d69be9a283bc43e8f0b0d0da1bb41aaf159446bc58f5d8f73cd7c86fd9d3cc`  
		Last Modified: Wed, 01 Nov 2023 02:44:00 GMT  
		Size: 16.2 MB (16215741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3187ad722182d5ffc423d3c4e25669ca3060f6b403232da1593133503aaa5311
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66745183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99607d7258254818c503a77cfe1d852a45c168e4c07cde3dfaa3210ace0def66`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:40:02 GMT
ADD file:e3f63671dca138b2b525b60f1471241941cdf4dab7f0c17cd91124978716bd93 in / 
# Wed, 01 Nov 2023 00:40:02 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:07:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d3db7215fb502c5873a81db7c6fd3214f199f6a1d8034da9d90918ac3220b20b`  
		Last Modified: Wed, 01 Nov 2023 00:44:04 GMT  
		Size: 49.3 MB (49291092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273f65b8dba688a4aab84c27f594891edb3518fd96d226c06ca7667c8c2a5b06`  
		Last Modified: Wed, 01 Nov 2023 02:15:35 GMT  
		Size: 17.5 MB (17454091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:860907a7a7afe3f516a398c4bc4fcd433e291cbf564587b42f7818462dd571c6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.4 MB (69355225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67647118a2406cfa85155bb8a01a813c5d19b67a81364505935d344f41d7d932`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:28 GMT
ADD file:65beb9bd9a5ca258316260fb802c65d9c3cc4a9137e0a09a873d4404d5b24fcc in / 
# Wed, 01 Nov 2023 00:39:29 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 13:48:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2e1a1831feefb5bd8f0a9fbc43f06ac287e16d9dd672e28d11eb17f3df2c71cd`  
		Last Modified: Wed, 01 Nov 2023 00:44:36 GMT  
		Size: 51.3 MB (51255735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4efeebbb8917115755445da9fb58c99b67f18a2552b83c24eb9b3a6b280700de`  
		Last Modified: Wed, 01 Nov 2023 13:58:36 GMT  
		Size: 18.1 MB (18099490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:buster-scm`

```console
$ docker pull buildpack-deps@sha256:fd691cd5b0c388046d1240a0668d65b62d77574d933a323bd30d909a37121960
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:buster-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:4e63e1919e1281065996f42681e6b2f5962e28fb15610d02cbb8cad12a395cfa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.0 MB (119957009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b0f4e232802bdb79ecad162dc2170c54cd789211d8b17c6fdbbe34502eebfd9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:21 GMT
ADD file:e12306e266f3e237ff7df5ea95bd339c3eb4a539f31be801afd63a76e116f522 in / 
# Wed, 01 Nov 2023 00:21:22 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:55:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 00:56:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:711706b827bb26857b90ceb32b653a05be0e06459342cc05124da0f97f9b6ad9`  
		Last Modified: Wed, 01 Nov 2023 00:26:31 GMT  
		Size: 50.5 MB (50499123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465ae13a022e930633aeb58ebf812a0350a4ec43803e013187863d358e62f15f`  
		Last Modified: Wed, 01 Nov 2023 01:04:06 GMT  
		Size: 17.6 MB (17583932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac648dffba596ed8d982778472e34b8ba1ad650a3ea934c0c1b202e63e338860`  
		Last Modified: Wed, 01 Nov 2023 01:04:21 GMT  
		Size: 51.9 MB (51873954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:dbeda7c5cd3b5023e84fd8111f8691ab1c4d0448e93f288091ad74479c344d51
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109592821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8056131f6b34799617afef5be94af84f6c0140b7610b218f084a4597e00df1d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:58:20 GMT
ADD file:ff8efe260318f1cfb8bfc8aaaa6d6bb15c878689f7edea37d776cf111c30fefb in / 
# Wed, 01 Nov 2023 00:58:20 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:33:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:34:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:608341ab24b1ec00c021d73e16dbb8ca54b2437a4a3f5ae09ca58578603a32bf`  
		Last Modified: Wed, 01 Nov 2023 01:03:18 GMT  
		Size: 46.0 MB (45966058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d69be9a283bc43e8f0b0d0da1bb41aaf159446bc58f5d8f73cd7c86fd9d3cc`  
		Last Modified: Wed, 01 Nov 2023 02:44:00 GMT  
		Size: 16.2 MB (16215741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0b6d0aa1dff66e917c4bbec58a8d82c3bf1380c7772452e657e0e4ad5c190e`  
		Last Modified: Wed, 01 Nov 2023 02:44:16 GMT  
		Size: 47.4 MB (47411022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:440f4f9f9e36fe1c7aa17c2a75d5764603f4dc8afb7924b71c83fb73405d82ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.0 MB (118953523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bffb0b1dca0833986cd2d5c52f34da17dc8b5cad2d118f4e5775db45049ff8f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:40:02 GMT
ADD file:e3f63671dca138b2b525b60f1471241941cdf4dab7f0c17cd91124978716bd93 in / 
# Wed, 01 Nov 2023 00:40:02 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:07:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:07:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d3db7215fb502c5873a81db7c6fd3214f199f6a1d8034da9d90918ac3220b20b`  
		Last Modified: Wed, 01 Nov 2023 00:44:04 GMT  
		Size: 49.3 MB (49291092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273f65b8dba688a4aab84c27f594891edb3518fd96d226c06ca7667c8c2a5b06`  
		Last Modified: Wed, 01 Nov 2023 02:15:35 GMT  
		Size: 17.5 MB (17454091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c150f07b6a196359013d5fe6373a86fec69409163977b1cd213268cd033d320c`  
		Last Modified: Wed, 01 Nov 2023 02:15:49 GMT  
		Size: 52.2 MB (52208340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:e721e5812cb11d6b77990dffebc194b4663f5848d6f439c87920d67d95635b98
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.8 MB (122843514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e56a96c2faf3f6388c9337058992884b3dcaeec74a26a10a8801695fe84458fa`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:28 GMT
ADD file:65beb9bd9a5ca258316260fb802c65d9c3cc4a9137e0a09a873d4404d5b24fcc in / 
# Wed, 01 Nov 2023 00:39:29 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 13:48:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:48:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2e1a1831feefb5bd8f0a9fbc43f06ac287e16d9dd672e28d11eb17f3df2c71cd`  
		Last Modified: Wed, 01 Nov 2023 00:44:36 GMT  
		Size: 51.3 MB (51255735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4efeebbb8917115755445da9fb58c99b67f18a2552b83c24eb9b3a6b280700de`  
		Last Modified: Wed, 01 Nov 2023 13:58:36 GMT  
		Size: 18.1 MB (18099490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52765542e10643f266bb59e790311fa685b420f7ddf55344e27da30b0e98fb64`  
		Last Modified: Wed, 01 Nov 2023 13:58:57 GMT  
		Size: 53.5 MB (53488289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:curl`

```console
$ docker pull buildpack-deps@sha256:57892e6ad71a863f2ac7fb2bb00901d96d41a257e1ef9d10c44639f1dc795ab3
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
$ docker pull buildpack-deps@sha256:81138c0eec1922d626830b19f73fea9792c263880367cde9b37fc4c021aec989
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73631171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7937fdd23222e4c8dcf166fc96dcc583d6d66bb47ac9af8d666d0e1bbace30d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:37 GMT
ADD file:3e9b6405f11dd24ce62105c033f1d8b931d9409298553f63b03af1b6dd1dda35 in / 
# Wed, 01 Nov 2023 00:20:38 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:52:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8457fd5474e70835e4482983a5662355d892d5f6f0f90a27a8e9f009997e8196`  
		Last Modified: Wed, 01 Nov 2023 00:25:05 GMT  
		Size: 49.6 MB (49582024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13baa2029dde87a21b87127168a0fb50a007c07da6b5adc8864e1fe1376c86ff`  
		Last Modified: Wed, 01 Nov 2023 01:02:01 GMT  
		Size: 24.0 MB (24049147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:ed09164fc4880f94c58fa72329b74e2deb0e9c4c49c4c89bbd311dfbec5a7108
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.1 MB (70083233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:992836c8887553b50c3a23f1fe3a3755bcd7acd42fce7ad4b6ad8137282b3ebb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:48:23 GMT
ADD file:963e26decfc65419428098047df29dcbf7865e13bcdd67abeb9849f99a7815e7 in / 
# Wed, 01 Nov 2023 00:48:23 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:53c5547a993a8adb09a632a8ae34fbc336b27a456c6b3a670865cd8bedb5e6a9`  
		Last Modified: Wed, 01 Nov 2023 00:51:04 GMT  
		Size: 47.4 MB (47355649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752979e12aac8f84972cea68e4f8d9bb1b645e71b3fc64047af1ba792dd338d9`  
		Last Modified: Wed, 01 Nov 2023 03:04:53 GMT  
		Size: 22.7 MB (22727584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1171fe398f6788003f5bacbadd2a89ea2013fff55c0f14da9e106bbcbe024a7a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67131290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a88861f4a437ff5c87eec39e153ae95413a03c4172c7e8751b0cc2825002d218`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:57:42 GMT
ADD file:3b2b4eda35d794b39d6b5567e81651625af51da3deb3f63b3ffdffa07720646e in / 
# Wed, 01 Nov 2023 00:57:42 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:30:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9bf855396a6f46c1cbac4e188af10f2c38474f989707b0b1b406b48c4b7284ef`  
		Last Modified: Wed, 01 Nov 2023 01:01:41 GMT  
		Size: 45.2 MB (45179410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6e59eca644b227cb755978679a3031e7b3f9a5c707057c293f2ba8732d8ef2`  
		Last Modified: Wed, 01 Nov 2023 02:41:40 GMT  
		Size: 22.0 MB (21951880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f82a3141ca386a79076c0ba0418c8782a361c8bb51e75deaa8866db1b2bed5ea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73197549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a409f55570736a6c820237e1f60fad4f8bb18dfc77870b144516ef2fe8e2ff11`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:32 GMT
ADD file:c934ceb4c53a1cce6779198f1ea73d5c8aad9a035e750b343d49826120ecd0eb in / 
# Wed, 01 Nov 2023 00:39:33 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:04:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8024d4fb53b2455f66d49b7ee72eb3cad5074043578238b796a9879955946a88`  
		Last Modified: Wed, 01 Nov 2023 00:42:44 GMT  
		Size: 49.6 MB (49612653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d826ee8aa65e56e167f0e27fa65cfc065687a7ac6c360787d5940d8b51f0cf1`  
		Last Modified: Wed, 01 Nov 2023 02:13:39 GMT  
		Size: 23.6 MB (23584896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:e583e18e995680fcec2033ed1ec977f42c6a379c165cc1770dc0ccef1f48ab1e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.5 MB (75485624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05e2aefc926d6cb666936937674be7f6a97c7ed0b53b7f469e95897450b1e705`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:38:46 GMT
ADD file:4043d711d8d7d1a995aed0a6998c96230765f55d4449167107955fe4af2a31db in / 
# Wed, 01 Nov 2023 00:38:47 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 13:44:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be8d77e28ff21732ba73253b6226e47e4e07ec2cedc803ffd62148df5d7a165b`  
		Last Modified: Wed, 01 Nov 2023 00:43:00 GMT  
		Size: 50.6 MB (50600049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cef920c8d790c11b84fa21c2204cca8ac6a84ec43e4a60bca3670e828748583`  
		Last Modified: Wed, 01 Nov 2023 13:55:45 GMT  
		Size: 24.9 MB (24885575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:c86473381513b077b2b848a187217476731ef8648b6efa00e40b3b540d28c8cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (73006830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5305c7a9d52eb2df81294cd30b305c75ce3a58c6c2f14ffd4fc4015d09853ad9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:08:17 GMT
ADD file:b181441dc28bc6879e29cd086c569c653171c681525c124ffb6277bd71732bb1 in / 
# Wed, 01 Nov 2023 01:08:24 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 21:17:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0bfbf01892d22dd14fb9536e8675cc932ff41f415a415fbf8c6199106b01240d`  
		Last Modified: Wed, 01 Nov 2023 01:19:01 GMT  
		Size: 49.6 MB (49568811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9310598b7549f388c445368ea2a0a4077c57ddd45436efddb37e089d293f87fe`  
		Last Modified: Wed, 01 Nov 2023 21:53:41 GMT  
		Size: 23.4 MB (23438019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:8fef9d5a3be088dbbfed19de3a7a624448239421641b6dba8621c6400edd7f06
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.3 MB (79274037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39d499c3ba7b3bc05ab676e65cd1d1351b56d80a02752dfd5053677641ce5b37`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:25 GMT
ADD file:31b995b44eb1f532fd265be3fc0c3d3b55e28db0911c86a06c83de621418db94 in / 
# Wed, 01 Nov 2023 00:21:28 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:24:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:071872f8f8cb44e883168d06195f8fbb330e259b415d1ab108c27bda84d6c060`  
		Last Modified: Wed, 01 Nov 2023 00:25:41 GMT  
		Size: 53.6 MB (53575361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9986fe7e71120fd78fcaad86d3a1d827f54f56f266364834bcb7c13eccf9ca0`  
		Last Modified: Wed, 01 Nov 2023 01:40:25 GMT  
		Size: 25.7 MB (25698676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:5f7c17a38a04a8eccaa364dd9860f483d4d838929e9817e888412ab607f0ebe1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.0 MB (71988267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:098bd7234fbac6dbe5ad9b2b1184781e15d3c49ddbd180c6247dff18efda87f8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:42:15 GMT
ADD file:6d8ee60b2fe4604969d8feeeb7e0dc8b9619a778d1a905c8bfdde5ede5e1eb54 in / 
# Wed, 01 Nov 2023 00:42:19 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:54:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bca95e393f709ba301b35c2439a815fd4fe8134d7a466bd528563bc32fd754d8`  
		Last Modified: Wed, 01 Nov 2023 00:47:43 GMT  
		Size: 47.9 MB (47943171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e744d1ef2c8405f6352136656080d7e244e1a97362c21069b734a55b86c8d0a`  
		Last Modified: Wed, 01 Nov 2023 02:05:09 GMT  
		Size: 24.0 MB (24045096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:focal`

```console
$ docker pull buildpack-deps@sha256:0ce585b92f5ec1586823ded83ae124239bc3596b06c19f436320bd0788a4c9b7
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
$ docker pull buildpack-deps@sha256:2d8c4194fb7309c82c42c5e72f9eb63bd2a91a53b563d1477bb145b5bab8a964
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.5 MB (226549744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3075cf4fa6991f63d4d84b9f17dca444f018d69cca3039b157ec2ecceb038a0c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 Oct 2023 11:03:23 GMT
ARG RELEASE
# Tue, 03 Oct 2023 11:03:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 11:03:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 11:03:23 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 11:03:25 GMT
ADD file:1d9be1bf43c126d53bda18c06d12757c021da97c0c9d3a9c9f56df17312095b8 in / 
# Tue, 03 Oct 2023 11:03:25 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 11:01:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 11:02:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 11:04:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2f51ce1532d2fc433720a55b8851134d5051381dedc2ef6109fb7ebb7a0edb92`  
		Last Modified: Fri, 13 Oct 2023 10:16:26 GMT  
		Size: 27.0 MB (27014102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c5cede6167f4e42b7f5e8cf8fb25ba8e103554c1d3afce502fb3e1f7e24b43`  
		Last Modified: Fri, 13 Oct 2023 11:13:32 GMT  
		Size: 10.7 MB (10687808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af317778e55c85e39b6ea37b448d46e0197947b603250dea5a4ac60cc8a53d8`  
		Last Modified: Fri, 13 Oct 2023 11:13:47 GMT  
		Size: 60.3 MB (60311494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c74bf94f4dabe59299e4f79fa6db52ecd3d45cced8c8f2a7268a73dc893e07`  
		Last Modified: Fri, 13 Oct 2023 11:14:11 GMT  
		Size: 128.5 MB (128536340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:focal-curl`

```console
$ docker pull buildpack-deps@sha256:d4947847a090a83bc604b03f063b6c3581a512d8d7540cee339d4f804dc3e5f4
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
$ docker pull buildpack-deps@sha256:02cd3122d24058fbd1b8e50757076b598990a16b09c533afe912ec749e661f93
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37701910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23b5ed0a418136ce71335a277e0b38f1285bb432922fe1fc0572dc210936d4ad`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 Oct 2023 11:03:23 GMT
ARG RELEASE
# Tue, 03 Oct 2023 11:03:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 11:03:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 11:03:23 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 11:03:25 GMT
ADD file:1d9be1bf43c126d53bda18c06d12757c021da97c0c9d3a9c9f56df17312095b8 in / 
# Tue, 03 Oct 2023 11:03:25 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 11:01:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2f51ce1532d2fc433720a55b8851134d5051381dedc2ef6109fb7ebb7a0edb92`  
		Last Modified: Fri, 13 Oct 2023 10:16:26 GMT  
		Size: 27.0 MB (27014102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c5cede6167f4e42b7f5e8cf8fb25ba8e103554c1d3afce502fb3e1f7e24b43`  
		Last Modified: Fri, 13 Oct 2023 11:13:32 GMT  
		Size: 10.7 MB (10687808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:focal-scm`

```console
$ docker pull buildpack-deps@sha256:4d7f93ed85af3446f7ec8598f188eab65156a6514197672620844a56f9b9f2fa
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
$ docker pull buildpack-deps@sha256:05b5108d044759d54f2f80eb3a45210f2b631e49fcf67cd333b46b13111a155c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.0 MB (98013404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8f52f13ce965b8eb5ebf01d5353ccde18fb00da4df1e00f8427a9966f2d6a17`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 03 Oct 2023 11:03:23 GMT
ARG RELEASE
# Tue, 03 Oct 2023 11:03:23 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 03 Oct 2023 11:03:23 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 03 Oct 2023 11:03:23 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 03 Oct 2023 11:03:25 GMT
ADD file:1d9be1bf43c126d53bda18c06d12757c021da97c0c9d3a9c9f56df17312095b8 in / 
# Tue, 03 Oct 2023 11:03:25 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 11:01:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 11:02:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2f51ce1532d2fc433720a55b8851134d5051381dedc2ef6109fb7ebb7a0edb92`  
		Last Modified: Fri, 13 Oct 2023 10:16:26 GMT  
		Size: 27.0 MB (27014102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c5cede6167f4e42b7f5e8cf8fb25ba8e103554c1d3afce502fb3e1f7e24b43`  
		Last Modified: Fri, 13 Oct 2023 11:13:32 GMT  
		Size: 10.7 MB (10687808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af317778e55c85e39b6ea37b448d46e0197947b603250dea5a4ac60cc8a53d8`  
		Last Modified: Fri, 13 Oct 2023 11:13:47 GMT  
		Size: 60.3 MB (60311494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:jammy`

```console
$ docker pull buildpack-deps@sha256:4a33447a13decae8d0e6fe2b6444168aa358c260a758d775cae0676c125f5698
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
$ docker pull buildpack-deps@sha256:224fda92a290ee7dce3b93f8ef46090b274c54e6c85125025c20b13569a84ad9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.8 MB (223838717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e1c00dab04ed667278bb299d0cd64a72c6aac1bf6dea472b34db49d75e79740`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:29:34 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:29:34 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:29:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:29:34 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:29:36 GMT
ADD file:d165475f8f027ab758a463da57c8c29f5d302f0a87a475ac68fdfae30005c7ac in / 
# Thu, 05 Oct 2023 07:29:36 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 11:05:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 11:05:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 11:07:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:818e4e246beb9ab026d2b95bf051fe9610b92dbc0a35b45d09b0cf237b6f3c2e`  
		Last Modified: Fri, 13 Oct 2023 10:16:45 GMT  
		Size: 28.7 MB (28650497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e533f7ce965854f8f4cdc647d000c54a4925b3b180750298427b9235afa18e51`  
		Last Modified: Fri, 13 Oct 2023 11:14:18 GMT  
		Size: 7.0 MB (7033617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c01525ba07c29d70d75e5ad0aa553d3b9ab93b48dbf3368a2e637f0d4d225d0`  
		Last Modified: Fri, 13 Oct 2023 11:14:30 GMT  
		Size: 39.4 MB (39414564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef34b85cef45adc613db3947199161e633e7076231b6a41ef4854ca8e3ceabbc`  
		Last Modified: Fri, 13 Oct 2023 11:14:56 GMT  
		Size: 148.7 MB (148740039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:jammy-curl`

```console
$ docker pull buildpack-deps@sha256:b6d4d85cb1727a557a2a10db192be5aa79af3b05092a96d7a6f293d7242487d6
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
$ docker pull buildpack-deps@sha256:2de035e63fc2a4e0bcb3c141b59f3918f2388a91db1280bbbc45b732c8196739
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35684114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1ef128f78a0b9d9f64497c39fbe68d730dd357868b4f101d7a0feec3b20645e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:29:34 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:29:34 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:29:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:29:34 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:29:36 GMT
ADD file:d165475f8f027ab758a463da57c8c29f5d302f0a87a475ac68fdfae30005c7ac in / 
# Thu, 05 Oct 2023 07:29:36 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 11:05:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:818e4e246beb9ab026d2b95bf051fe9610b92dbc0a35b45d09b0cf237b6f3c2e`  
		Last Modified: Fri, 13 Oct 2023 10:16:45 GMT  
		Size: 28.7 MB (28650497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e533f7ce965854f8f4cdc647d000c54a4925b3b180750298427b9235afa18e51`  
		Last Modified: Fri, 13 Oct 2023 11:14:18 GMT  
		Size: 7.0 MB (7033617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:jammy-scm`

```console
$ docker pull buildpack-deps@sha256:f205acc8dc8abd31d431089175b0f6f366261875e18e4055432a0e49659a80b0
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
$ docker pull buildpack-deps@sha256:c0da1ea44cc5848bd53fb6e94390685144a6a15b9440e02f9acc6ee3c6f192a8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75098678 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a9c666b9c8b0954dade1579aed2a7d9b57345535d874545267e8c4ea50d4ecd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 05 Oct 2023 07:29:34 GMT
ARG RELEASE
# Thu, 05 Oct 2023 07:29:34 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 05 Oct 2023 07:29:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 05 Oct 2023 07:29:34 GMT
LABEL org.opencontainers.image.version=22.04
# Thu, 05 Oct 2023 07:29:36 GMT
ADD file:d165475f8f027ab758a463da57c8c29f5d302f0a87a475ac68fdfae30005c7ac in / 
# Thu, 05 Oct 2023 07:29:36 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 11:05:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 11:05:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:818e4e246beb9ab026d2b95bf051fe9610b92dbc0a35b45d09b0cf237b6f3c2e`  
		Last Modified: Fri, 13 Oct 2023 10:16:45 GMT  
		Size: 28.7 MB (28650497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e533f7ce965854f8f4cdc647d000c54a4925b3b180750298427b9235afa18e51`  
		Last Modified: Fri, 13 Oct 2023 11:14:18 GMT  
		Size: 7.0 MB (7033617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c01525ba07c29d70d75e5ad0aa553d3b9ab93b48dbf3368a2e637f0d4d225d0`  
		Last Modified: Fri, 13 Oct 2023 11:14:30 GMT  
		Size: 39.4 MB (39414564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:latest`

```console
$ docker pull buildpack-deps@sha256:8465175ca53f8f2e756d069658b3f353bb3732926b1f33f34332cfbf597ad0c0
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
$ docker pull buildpack-deps@sha256:c281372d752c50bd925a7ef863ad65222d68d37028b97ae6378f38fe3ead7b15
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.8 MB (348825839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6672223876e40fadb1dac262c5e01bdaefbffd0107862c58d80b4df910d55414`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:37 GMT
ADD file:3e9b6405f11dd24ce62105c033f1d8b931d9409298553f63b03af1b6dd1dda35 in / 
# Wed, 01 Nov 2023 00:20:38 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:52:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 00:52:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 00:53:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8457fd5474e70835e4482983a5662355d892d5f6f0f90a27a8e9f009997e8196`  
		Last Modified: Wed, 01 Nov 2023 00:25:05 GMT  
		Size: 49.6 MB (49582024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13baa2029dde87a21b87127168a0fb50a007c07da6b5adc8864e1fe1376c86ff`  
		Last Modified: Wed, 01 Nov 2023 01:02:01 GMT  
		Size: 24.0 MB (24049147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:325c5bf4c2f26c11380501bec4b6eef8a3ea35b554aa1b222cbcd1e1fe11ae1d`  
		Last Modified: Wed, 01 Nov 2023 01:02:20 GMT  
		Size: 64.1 MB (64130415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e18a660069fd7f87a7a6c49ddb701449bfb929c066811777601d36916c7f674`  
		Last Modified: Wed, 01 Nov 2023 01:02:55 GMT  
		Size: 211.1 MB (211064253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:f8310b73e4ca74a8a62aa3a60614bce0092e656117d95d96abf6efa958f10f39
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.0 MB (316028995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1bbae5789c5511aa21a7f8cac7ff0966d933f3cba2914e0630044c3d3d9a171`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:48:23 GMT
ADD file:963e26decfc65419428098047df29dcbf7865e13bcdd67abeb9849f99a7815e7 in / 
# Wed, 01 Nov 2023 00:48:23 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:56:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:53c5547a993a8adb09a632a8ae34fbc336b27a456c6b3a670865cd8bedb5e6a9`  
		Last Modified: Wed, 01 Nov 2023 00:51:04 GMT  
		Size: 47.4 MB (47355649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752979e12aac8f84972cea68e4f8d9bb1b645e71b3fc64047af1ba792dd338d9`  
		Last Modified: Wed, 01 Nov 2023 03:04:53 GMT  
		Size: 22.7 MB (22727584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bad2403917aecfddc5d239a343aacd942aeb9c9e6d76c027cfdbb0d5479bcaa`  
		Last Modified: Wed, 01 Nov 2023 03:05:15 GMT  
		Size: 61.6 MB (61561816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f0dda98bbf4b74a7919e20bcc31a0ecda8fd013c63ef827f0316369707e6af`  
		Last Modified: Wed, 01 Nov 2023 03:05:53 GMT  
		Size: 184.4 MB (184383946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1d6a60f9f2f559b189af01218c17dcda727d852c6c6d4a004b3a18dffdba281b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.4 MB (301446629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:576fdf6667f95f602d6807ecabd5c0e4f0643440a9c83b60e388dc8614f59f15`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:57:42 GMT
ADD file:3b2b4eda35d794b39d6b5567e81651625af51da3deb3f63b3ffdffa07720646e in / 
# Wed, 01 Nov 2023 00:57:42 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:30:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:30:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:31:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9bf855396a6f46c1cbac4e188af10f2c38474f989707b0b1b406b48c4b7284ef`  
		Last Modified: Wed, 01 Nov 2023 01:01:41 GMT  
		Size: 45.2 MB (45179410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6e59eca644b227cb755978679a3031e7b3f9a5c707057c293f2ba8732d8ef2`  
		Last Modified: Wed, 01 Nov 2023 02:41:40 GMT  
		Size: 22.0 MB (21951880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aefa016475f9e4925fd893a9d8cfcf375937aa4e637d337806176426509dfcd`  
		Last Modified: Wed, 01 Nov 2023 02:42:04 GMT  
		Size: 59.3 MB (59266468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d2c477968e94d61a34b16e774d58519d5e26175f92fbd0dfb90938103fab68`  
		Last Modified: Wed, 01 Nov 2023 02:42:47 GMT  
		Size: 175.0 MB (175048871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a8b07b41b675910dbc20eaf720c7716422cb5d1f0ddac9fbbdf56f6211f2a34e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.6 MB (339641684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08254bfa9a67c2c123e58e5c10e5e73f9c4aa1eee30e14a41e6c78b513d6e36d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:32 GMT
ADD file:c934ceb4c53a1cce6779198f1ea73d5c8aad9a035e750b343d49826120ecd0eb in / 
# Wed, 01 Nov 2023 00:39:33 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:04:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:04:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:05:48 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8024d4fb53b2455f66d49b7ee72eb3cad5074043578238b796a9879955946a88`  
		Last Modified: Wed, 01 Nov 2023 00:42:44 GMT  
		Size: 49.6 MB (49612653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d826ee8aa65e56e167f0e27fa65cfc065687a7ac6c360787d5940d8b51f0cf1`  
		Last Modified: Wed, 01 Nov 2023 02:13:39 GMT  
		Size: 23.6 MB (23584896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198068495d09b6865e75ce28d5d5d5de39897b8325ada63ba80eca884ad5666b`  
		Last Modified: Wed, 01 Nov 2023 02:13:57 GMT  
		Size: 64.0 MB (63994018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509db9a897ae5a94cad05bcf48605637fbf3f79733e8bf8c317b6babe3de1dbd`  
		Last Modified: Wed, 01 Nov 2023 02:14:29 GMT  
		Size: 202.5 MB (202450117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; 386

```console
$ docker pull buildpack-deps@sha256:06f4072db6e5dfbd8c8a3f60ac4b15f0852ba0216c33198a58e8da312fb8beda
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.5 MB (351464296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa96e3b9058ae71c8b65439bf05b32b30c99e3b7b9e4f07e1692eefc747c08c8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:38:46 GMT
ADD file:4043d711d8d7d1a995aed0a6998c96230765f55d4449167107955fe4af2a31db in / 
# Wed, 01 Nov 2023 00:38:47 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 13:44:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:44:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:45:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be8d77e28ff21732ba73253b6226e47e4e07ec2cedc803ffd62148df5d7a165b`  
		Last Modified: Wed, 01 Nov 2023 00:43:00 GMT  
		Size: 50.6 MB (50600049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cef920c8d790c11b84fa21c2204cca8ac6a84ec43e4a60bca3670e828748583`  
		Last Modified: Wed, 01 Nov 2023 13:55:45 GMT  
		Size: 24.9 MB (24885575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fee1ec8688f07e43b49247f3490035da93288449034600daee26c8ce0150a8c`  
		Last Modified: Wed, 01 Nov 2023 13:56:13 GMT  
		Size: 66.0 MB (65984300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6a893690e210e75c1236dc74079509b9f860409954240df3b2276364c416f8`  
		Last Modified: Wed, 01 Nov 2023 13:57:04 GMT  
		Size: 210.0 MB (209994372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:34b5b299169edc7c1281954a26f710d3d5d9c2101b510ae89ba1ca136df9b03c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.6 MB (325622171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0dc2b58709b67c5f83e2571566693513ad91a3ec9cd7626f14d8e210d8f7925`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:08:17 GMT
ADD file:b181441dc28bc6879e29cd086c569c653171c681525c124ffb6277bd71732bb1 in / 
# Wed, 01 Nov 2023 01:08:24 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 21:17:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 21:19:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 21:25:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0bfbf01892d22dd14fb9536e8675cc932ff41f415a415fbf8c6199106b01240d`  
		Last Modified: Wed, 01 Nov 2023 01:19:01 GMT  
		Size: 49.6 MB (49568811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9310598b7549f388c445368ea2a0a4077c57ddd45436efddb37e089d293f87fe`  
		Last Modified: Wed, 01 Nov 2023 21:53:41 GMT  
		Size: 23.4 MB (23438019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af2206444fab218d319700cbfcd93423bf4622bb8085adee11b684b7d3fd245`  
		Last Modified: Wed, 01 Nov 2023 21:54:35 GMT  
		Size: 63.0 MB (62962363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41601926009dec498023c4d0a7e1c4877fc9fe8372d6497206d1de026aeb215d`  
		Last Modified: Wed, 01 Nov 2023 21:57:00 GMT  
		Size: 189.7 MB (189652978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:0cd2296657f87dc9875b44afde1718960b7c982dea8b3128a2c2e9f0ad987be2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **363.0 MB (362952137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96ec2f6ad64fe7094e57094fb3436d0709d2e3f0d3a1ec0f6ed4cc91ef594b34`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:25 GMT
ADD file:31b995b44eb1f532fd265be3fc0c3d3b55e28db0911c86a06c83de621418db94 in / 
# Wed, 01 Nov 2023 00:21:28 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:24:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:24:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:27:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:071872f8f8cb44e883168d06195f8fbb330e259b415d1ab108c27bda84d6c060`  
		Last Modified: Wed, 01 Nov 2023 00:25:41 GMT  
		Size: 53.6 MB (53575361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9986fe7e71120fd78fcaad86d3a1d827f54f56f266364834bcb7c13eccf9ca0`  
		Last Modified: Wed, 01 Nov 2023 01:40:25 GMT  
		Size: 25.7 MB (25698676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7316c6cea433a21258a8af8686d8a74e964c21c6c563afd63f274e9346f8f7`  
		Last Modified: Wed, 01 Nov 2023 01:40:48 GMT  
		Size: 69.6 MB (69584512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d43d4f467d09dbebbdbbe77e08bdef659a411541528d2d0542c5a201a1e3953`  
		Last Modified: Wed, 01 Nov 2023 01:41:31 GMT  
		Size: 214.1 MB (214093588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:2592737d5c14c9cd628b8b622a4a8d02a213a6b6a91a832feb16b338c44c95ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.2 MB (318220170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97ece825d20df85062f7e8dc9e143e2cd80da86d6928f1260cee829c756fa6c9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:42:15 GMT
ADD file:6d8ee60b2fe4604969d8feeeb7e0dc8b9619a778d1a905c8bfdde5ede5e1eb54 in / 
# Wed, 01 Nov 2023 00:42:19 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:54:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:55:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:56:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bca95e393f709ba301b35c2439a815fd4fe8134d7a466bd528563bc32fd754d8`  
		Last Modified: Wed, 01 Nov 2023 00:47:43 GMT  
		Size: 47.9 MB (47943171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e744d1ef2c8405f6352136656080d7e244e1a97362c21069b734a55b86c8d0a`  
		Last Modified: Wed, 01 Nov 2023 02:05:09 GMT  
		Size: 24.0 MB (24045096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de40af46a5373d0a49892fa9000736be09090b477719517fcec84887d847f94b`  
		Last Modified: Wed, 01 Nov 2023 02:05:25 GMT  
		Size: 63.1 MB (63132485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5d582ecd4430347fbaa4df40283ca084e7bf9c17c0ce600484712c9f61dbe3`  
		Last Modified: Wed, 01 Nov 2023 02:05:57 GMT  
		Size: 183.1 MB (183099418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:lunar`

```console
$ docker pull buildpack-deps@sha256:9d3347dff07c65b321044655161d08f18441853c906686fc726318ca72c41a25
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
$ docker pull buildpack-deps@sha256:a0851ce95bf9247c04db9bf58ce62db350f36adf2937da6b0e8ec31eb69993dd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.2 MB (240192288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:223926587c6bf995caec15c7e535b8415b6bde18631d04c2527f6138d6b213a2`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:26:55 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:26:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:26:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:26:55 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:26:57 GMT
ADD file:553d1c48ed98fa8bd575a7a645019079304c101dd6e06e82591a25440fe1a9b8 in / 
# Wed, 04 Oct 2023 12:26:57 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 11:08:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 11:09:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 11:11:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d713c3685e42819275f0fd629c394d4cc0cb20ebedd41e0c903afea19652cda9`  
		Last Modified: Fri, 13 Oct 2023 11:15:09 GMT  
		Size: 26.2 MB (26227299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10986e1aade9beaffef4018fdb444b55730350800aadabb7852a08f52b4e62fb`  
		Last Modified: Fri, 13 Oct 2023 11:15:06 GMT  
		Size: 14.0 MB (14006392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a2b5e38d0d2baf19e26862b6913dbfd77f4a4a48316294650cf07405115b38`  
		Last Modified: Fri, 13 Oct 2023 11:15:22 GMT  
		Size: 44.3 MB (44276364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c850916986260e8d643a72fb43633da561be89db5f3dfca9538eef8ce5175a1`  
		Last Modified: Fri, 13 Oct 2023 11:15:50 GMT  
		Size: 155.7 MB (155682233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:lunar-curl`

```console
$ docker pull buildpack-deps@sha256:4580a8a315197a8e4aa6953328d97401177416efc796a21a526f0eef3d184c95
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
$ docker pull buildpack-deps@sha256:4238b02664305627674ca2c52080ae3df742aaac231ebd9eb6b703501d4733d2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40233691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b6c03fa308ad0e9faa468a0f88ccb79519aecef58256d45189f7f748d9d9c04`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:26:55 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:26:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:26:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:26:55 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:26:57 GMT
ADD file:553d1c48ed98fa8bd575a7a645019079304c101dd6e06e82591a25440fe1a9b8 in / 
# Wed, 04 Oct 2023 12:26:57 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 11:08:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d713c3685e42819275f0fd629c394d4cc0cb20ebedd41e0c903afea19652cda9`  
		Last Modified: Fri, 13 Oct 2023 11:15:09 GMT  
		Size: 26.2 MB (26227299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10986e1aade9beaffef4018fdb444b55730350800aadabb7852a08f52b4e62fb`  
		Last Modified: Fri, 13 Oct 2023 11:15:06 GMT  
		Size: 14.0 MB (14006392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:lunar-scm`

```console
$ docker pull buildpack-deps@sha256:28f0686151e36942ee57461782428b02ae03d89b2c284474e804bb1fa5296202
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
$ docker pull buildpack-deps@sha256:312fb14d7e1c8447dc941245fdf9000d5a021a9f0f69b6b5a0efc49e859e46a6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84510055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:950a90c7fe2432bea9c867925cf0529090d9e75843d2a055960535aef8a866e9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 04 Oct 2023 12:26:55 GMT
ARG RELEASE
# Wed, 04 Oct 2023 12:26:55 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 04 Oct 2023 12:26:55 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 04 Oct 2023 12:26:55 GMT
LABEL org.opencontainers.image.version=23.04
# Wed, 04 Oct 2023 12:26:57 GMT
ADD file:553d1c48ed98fa8bd575a7a645019079304c101dd6e06e82591a25440fe1a9b8 in / 
# Wed, 04 Oct 2023 12:26:57 GMT
CMD ["/bin/bash"]
# Fri, 13 Oct 2023 11:08:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 Oct 2023 11:09:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d713c3685e42819275f0fd629c394d4cc0cb20ebedd41e0c903afea19652cda9`  
		Last Modified: Fri, 13 Oct 2023 11:15:09 GMT  
		Size: 26.2 MB (26227299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10986e1aade9beaffef4018fdb444b55730350800aadabb7852a08f52b4e62fb`  
		Last Modified: Fri, 13 Oct 2023 11:15:06 GMT  
		Size: 14.0 MB (14006392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a2b5e38d0d2baf19e26862b6913dbfd77f4a4a48316294650cf07405115b38`  
		Last Modified: Fri, 13 Oct 2023 11:15:22 GMT  
		Size: 44.3 MB (44276364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:mantic`

```console
$ docker pull buildpack-deps@sha256:73b2fe4c16b501c6faced6ae66568f7811fb7f9851c37dd883150de1b37cd988
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
$ docker pull buildpack-deps@sha256:5d033eccd30235895c02a2691efd3630128f77e40b483f005b4df76b7c244447
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.1 MB (280089512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48546e409c323ebe47eda00f7fdc3413d76e86f117df3fd0594b8a26df12af38`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:04:48 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:04:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:04:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:04:49 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:04:50 GMT
ADD file:492ae1940ef5a9a4d7af92b9120b5b7c7d3bfd8107ce94d28eab844ace024981 in / 
# Wed, 11 Oct 2023 18:04:50 GMT
CMD ["/bin/bash"]
# Wed, 15 Nov 2023 05:11:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 05:12:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 05:16:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2e92ecfee06656d1e7ef085e24769afe12ea1e14f3acdbdaf9d5cb922da5d97b`  
		Last Modified: Sat, 14 Oct 2023 00:22:39 GMT  
		Size: 28.1 MB (28067323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a6e6c1f13a01a9a83ddb22794e5e9998c28232b9695a11941b9c2fad7dfcc9`  
		Last Modified: Wed, 15 Nov 2023 05:19:05 GMT  
		Size: 9.9 MB (9907184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7fdbffee3006b2f392267c0bb2881b445fa2d9a6a932b40496bf246d26ed245`  
		Last Modified: Wed, 15 Nov 2023 05:19:22 GMT  
		Size: 45.1 MB (45088307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b169796f390a9ac9d50293b54e6c3c107ce2ef5569fb2c7d63831cd5ab1706`  
		Last Modified: Wed, 15 Nov 2023 05:19:54 GMT  
		Size: 197.0 MB (197026698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:46a4bc226b23e753406055137a46fe3c7fe73db1967c597eb2c08ac8d5aee8b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.0 MB (246981399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31561ec40607a691d299c442e8b44dfb1cb951ac72c779e6afbdb8b2aa082143`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:02:33 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:02:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:02:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:02:34 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:02:39 GMT
ADD file:1be1311acbd557f7769fb5c1913ef56305431e7547f96c20ac36284fdd926223 in / 
# Wed, 11 Oct 2023 18:02:39 GMT
CMD ["/bin/bash"]
# Wed, 15 Nov 2023 02:04:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 02:05:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 02:09:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:917b6666fb3ef51da1fc4435b7ebc2e973f8582d1321861d37d40dd0864b8927`  
		Last Modified: Wed, 15 Nov 2023 02:12:00 GMT  
		Size: 26.0 MB (26018438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179cd7cba3839185a2e0560fddb5800f6454b72d5acf3d485458ee26f6fef69f`  
		Last Modified: Wed, 15 Nov 2023 02:11:56 GMT  
		Size: 9.1 MB (9144906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d43664e3e871d40780214b000e38e04e3e840e99201a63699c325b0f02b0e5c`  
		Last Modified: Wed, 15 Nov 2023 02:12:19 GMT  
		Size: 49.2 MB (49223065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a4ff86544066b3c295e5fcd8ff907e64e35463f7b0911a6b709c5c52a28625`  
		Last Modified: Wed, 15 Nov 2023 02:12:57 GMT  
		Size: 162.6 MB (162594990 bytes)  
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
$ docker pull buildpack-deps@sha256:390630061f7241d7a3a338d8c1a2b285ebe1fff641bff92948cd16d604fedb96
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.9 MB (293947200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd0ab4387549ce1201adde944fda71531759b742627a5e12f382d3316893aea6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:06:00 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:06:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:06:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:06:00 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:06:03 GMT
ADD file:a18be8add7eb60493b13d2aac8d624230297bd15be033756795582dc07cb04bb in / 
# Wed, 11 Oct 2023 18:06:03 GMT
CMD ["/bin/bash"]
# Wed, 15 Nov 2023 02:22:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 02:23:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 02:27:21 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cffa8c08adf985954e82a5191220c2cac943e97ffd91acc2baa5d2cf0f8d4f44`  
		Last Modified: Wed, 15 Nov 2023 02:29:45 GMT  
		Size: 32.3 MB (32331370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5791ffbc3c4fdf8ff7e22c644078ce798cd8033f9d2e244eca8aec0a44ac5ce7`  
		Last Modified: Wed, 15 Nov 2023 02:29:40 GMT  
		Size: 11.6 MB (11573378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6331f990f21c8548212ac022cb9047ae9a7b4ac314bf49338f47926ca887eb14`  
		Last Modified: Wed, 15 Nov 2023 02:30:03 GMT  
		Size: 49.9 MB (49917559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c87fb10926a50da16bbd6eccc10a2b838b8368f36be454459fb19bc65df426`  
		Last Modified: Wed, 15 Nov 2023 02:30:42 GMT  
		Size: 200.1 MB (200124893 bytes)  
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
$ docker pull buildpack-deps@sha256:cd4d41ae6132051a907e3cfd0d9fddcfcd6b582033f9ab9291a2fcfde4976171
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
$ docker pull buildpack-deps@sha256:921a763a77cd772742a6ae544a5bd71b4411f92a999be5d1d7fed1684ddac2e3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (37974507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:287d7639ff0677fdfe2b1eadc6efdd695a529748505a9cbdc44b29355b92125b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:04:48 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:04:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:04:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:04:49 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:04:50 GMT
ADD file:492ae1940ef5a9a4d7af92b9120b5b7c7d3bfd8107ce94d28eab844ace024981 in / 
# Wed, 11 Oct 2023 18:04:50 GMT
CMD ["/bin/bash"]
# Wed, 15 Nov 2023 05:11:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2e92ecfee06656d1e7ef085e24769afe12ea1e14f3acdbdaf9d5cb922da5d97b`  
		Last Modified: Sat, 14 Oct 2023 00:22:39 GMT  
		Size: 28.1 MB (28067323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a6e6c1f13a01a9a83ddb22794e5e9998c28232b9695a11941b9c2fad7dfcc9`  
		Last Modified: Wed, 15 Nov 2023 05:19:05 GMT  
		Size: 9.9 MB (9907184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:2913f2f84d97ff1be7ca139b43ce4e8d05cfaf7ed3248b39aa9e6a70b154ea91
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.2 MB (35163344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59cd33ac4877ec60e73bfb24bb572ad8088801b2acdcc70314770203d15b6c91`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:02:33 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:02:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:02:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:02:34 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:02:39 GMT
ADD file:1be1311acbd557f7769fb5c1913ef56305431e7547f96c20ac36284fdd926223 in / 
# Wed, 11 Oct 2023 18:02:39 GMT
CMD ["/bin/bash"]
# Wed, 15 Nov 2023 02:04:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:917b6666fb3ef51da1fc4435b7ebc2e973f8582d1321861d37d40dd0864b8927`  
		Last Modified: Wed, 15 Nov 2023 02:12:00 GMT  
		Size: 26.0 MB (26018438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179cd7cba3839185a2e0560fddb5800f6454b72d5acf3d485458ee26f6fef69f`  
		Last Modified: Wed, 15 Nov 2023 02:11:56 GMT  
		Size: 9.1 MB (9144906 bytes)  
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
$ docker pull buildpack-deps@sha256:bcab01774044541e169e955e9d52762f736b27fb6c76d029381b6162dedbfee9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43904748 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbce8aeac751517d845efadce6fb839eff255b2c00e279e01eeb686343d3d0d8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:06:00 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:06:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:06:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:06:00 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:06:03 GMT
ADD file:a18be8add7eb60493b13d2aac8d624230297bd15be033756795582dc07cb04bb in / 
# Wed, 11 Oct 2023 18:06:03 GMT
CMD ["/bin/bash"]
# Wed, 15 Nov 2023 02:22:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cffa8c08adf985954e82a5191220c2cac943e97ffd91acc2baa5d2cf0f8d4f44`  
		Last Modified: Wed, 15 Nov 2023 02:29:45 GMT  
		Size: 32.3 MB (32331370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5791ffbc3c4fdf8ff7e22c644078ce798cd8033f9d2e244eca8aec0a44ac5ce7`  
		Last Modified: Wed, 15 Nov 2023 02:29:40 GMT  
		Size: 11.6 MB (11573378 bytes)  
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
$ docker pull buildpack-deps@sha256:c04969aa1a89a875915b3c8f7a54f60fca8979f802161c1acf9c9b9eae984578
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
$ docker pull buildpack-deps@sha256:405d376e0a44215dd53d9e4cea3ff098d03cae9e0aeeb846816f17d396321b18
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.1 MB (83062814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b3aba9e6064055dae56a062bcb092f50cffe5887b49242fdff98a4ea0eb3aa4`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:04:48 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:04:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:04:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:04:49 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:04:50 GMT
ADD file:492ae1940ef5a9a4d7af92b9120b5b7c7d3bfd8107ce94d28eab844ace024981 in / 
# Wed, 11 Oct 2023 18:04:50 GMT
CMD ["/bin/bash"]
# Wed, 15 Nov 2023 05:11:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 05:12:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2e92ecfee06656d1e7ef085e24769afe12ea1e14f3acdbdaf9d5cb922da5d97b`  
		Last Modified: Sat, 14 Oct 2023 00:22:39 GMT  
		Size: 28.1 MB (28067323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a6e6c1f13a01a9a83ddb22794e5e9998c28232b9695a11941b9c2fad7dfcc9`  
		Last Modified: Wed, 15 Nov 2023 05:19:05 GMT  
		Size: 9.9 MB (9907184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7fdbffee3006b2f392267c0bb2881b445fa2d9a6a932b40496bf246d26ed245`  
		Last Modified: Wed, 15 Nov 2023 05:19:22 GMT  
		Size: 45.1 MB (45088307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:afca6c528e9a02dffda09b471ae45eb3c1cd24ff62f025ec89877622c62fca52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.4 MB (84386409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cfd5fac42f464b6ae54e8ee27cba67ca6befadd81810a15993572f7fbd736e1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:02:33 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:02:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:02:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:02:34 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:02:39 GMT
ADD file:1be1311acbd557f7769fb5c1913ef56305431e7547f96c20ac36284fdd926223 in / 
# Wed, 11 Oct 2023 18:02:39 GMT
CMD ["/bin/bash"]
# Wed, 15 Nov 2023 02:04:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 02:05:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:917b6666fb3ef51da1fc4435b7ebc2e973f8582d1321861d37d40dd0864b8927`  
		Last Modified: Wed, 15 Nov 2023 02:12:00 GMT  
		Size: 26.0 MB (26018438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179cd7cba3839185a2e0560fddb5800f6454b72d5acf3d485458ee26f6fef69f`  
		Last Modified: Wed, 15 Nov 2023 02:11:56 GMT  
		Size: 9.1 MB (9144906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d43664e3e871d40780214b000e38e04e3e840e99201a63699c325b0f02b0e5c`  
		Last Modified: Wed, 15 Nov 2023 02:12:19 GMT  
		Size: 49.2 MB (49223065 bytes)  
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
$ docker pull buildpack-deps@sha256:710b61b098eb5d89e1e90686bd2c18ab1114706836bec26a133f94735ca05450
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.8 MB (93822307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9e385101b300162a4d39d603be56508551348b1b4e836cf511396429cdcd345`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 11 Oct 2023 18:06:00 GMT
ARG RELEASE
# Wed, 11 Oct 2023 18:06:00 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 11 Oct 2023 18:06:00 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 11 Oct 2023 18:06:00 GMT
LABEL org.opencontainers.image.version=23.10
# Wed, 11 Oct 2023 18:06:03 GMT
ADD file:a18be8add7eb60493b13d2aac8d624230297bd15be033756795582dc07cb04bb in / 
# Wed, 11 Oct 2023 18:06:03 GMT
CMD ["/bin/bash"]
# Wed, 15 Nov 2023 02:22:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 02:23:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cffa8c08adf985954e82a5191220c2cac943e97ffd91acc2baa5d2cf0f8d4f44`  
		Last Modified: Wed, 15 Nov 2023 02:29:45 GMT  
		Size: 32.3 MB (32331370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5791ffbc3c4fdf8ff7e22c644078ce798cd8033f9d2e244eca8aec0a44ac5ce7`  
		Last Modified: Wed, 15 Nov 2023 02:29:40 GMT  
		Size: 11.6 MB (11573378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6331f990f21c8548212ac022cb9047ae9a7b4ac314bf49338f47926ca887eb14`  
		Last Modified: Wed, 15 Nov 2023 02:30:03 GMT  
		Size: 49.9 MB (49917559 bytes)  
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
$ docker pull buildpack-deps@sha256:994c0590e60c01834f0b716a12087fa53cdc8751260c9924a698e38e9548e12a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:oldoldstable` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:ad93c92a1a49a84211028e913750883a2f28de561fde391a39714867ba406d36
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.9 MB (311867207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cbe55f5e882a696ded59f2a4da88985cff31ead69b6e59a7690a13e9fc6434d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:21 GMT
ADD file:e12306e266f3e237ff7df5ea95bd339c3eb4a539f31be801afd63a76e116f522 in / 
# Wed, 01 Nov 2023 00:21:22 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:55:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 00:56:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 00:57:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:711706b827bb26857b90ceb32b653a05be0e06459342cc05124da0f97f9b6ad9`  
		Last Modified: Wed, 01 Nov 2023 00:26:31 GMT  
		Size: 50.5 MB (50499123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465ae13a022e930633aeb58ebf812a0350a4ec43803e013187863d358e62f15f`  
		Last Modified: Wed, 01 Nov 2023 01:04:06 GMT  
		Size: 17.6 MB (17583932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac648dffba596ed8d982778472e34b8ba1ad650a3ea934c0c1b202e63e338860`  
		Last Modified: Wed, 01 Nov 2023 01:04:21 GMT  
		Size: 51.9 MB (51873954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1729d430e574c53c4882a063283bce8773703ecdcd1c010c604c04bcb85340f`  
		Last Modified: Wed, 01 Nov 2023 01:04:52 GMT  
		Size: 191.9 MB (191910198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:23e96132f6b9dd83ade53635f26ad7a584f1ff76e6fb6a6c4dbaeaa32fa9daf0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.7 MB (277696007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f06d6e26d9616bddfad69e554ee321e043cb2568e5064592ac36f28b66bfd3e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:58:20 GMT
ADD file:ff8efe260318f1cfb8bfc8aaaa6d6bb15c878689f7edea37d776cf111c30fefb in / 
# Wed, 01 Nov 2023 00:58:20 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:33:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:34:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:35:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:608341ab24b1ec00c021d73e16dbb8ca54b2437a4a3f5ae09ca58578603a32bf`  
		Last Modified: Wed, 01 Nov 2023 01:03:18 GMT  
		Size: 46.0 MB (45966058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d69be9a283bc43e8f0b0d0da1bb41aaf159446bc58f5d8f73cd7c86fd9d3cc`  
		Last Modified: Wed, 01 Nov 2023 02:44:00 GMT  
		Size: 16.2 MB (16215741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0b6d0aa1dff66e917c4bbec58a8d82c3bf1380c7772452e657e0e4ad5c190e`  
		Last Modified: Wed, 01 Nov 2023 02:44:16 GMT  
		Size: 47.4 MB (47411022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ef6c73d3c316731b1f2a4a1e12f29f955579feed16f8ddb603886d76efef32`  
		Last Modified: Wed, 01 Nov 2023 02:44:46 GMT  
		Size: 168.1 MB (168103186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:1a8d69bac6a059b10a24162a21252d8a3c9494d8290277547234d54872ae3daf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.4 MB (302430569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a503fe9299e3ee1608bed8a555b831e6f4e3de9b36c05c0a1590d3a4b266b812`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:40:02 GMT
ADD file:e3f63671dca138b2b525b60f1471241941cdf4dab7f0c17cd91124978716bd93 in / 
# Wed, 01 Nov 2023 00:40:02 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:07:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:07:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:08:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d3db7215fb502c5873a81db7c6fd3214f199f6a1d8034da9d90918ac3220b20b`  
		Last Modified: Wed, 01 Nov 2023 00:44:04 GMT  
		Size: 49.3 MB (49291092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273f65b8dba688a4aab84c27f594891edb3518fd96d226c06ca7667c8c2a5b06`  
		Last Modified: Wed, 01 Nov 2023 02:15:35 GMT  
		Size: 17.5 MB (17454091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c150f07b6a196359013d5fe6373a86fec69409163977b1cd213268cd033d320c`  
		Last Modified: Wed, 01 Nov 2023 02:15:49 GMT  
		Size: 52.2 MB (52208340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e75642759fbcf85e98624fae6727771f0e966a4debdef80548654cb137d1609`  
		Last Modified: Wed, 01 Nov 2023 02:16:15 GMT  
		Size: 183.5 MB (183477046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:4a2c1f92814c3a19ccbc81bc64a1b343bf0c601559c1e742946c3c14e1234d14
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.3 MB (321284071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccd929b52893acac0a10a782e89423a5ceff76790faf025f06a885343b371517`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:28 GMT
ADD file:65beb9bd9a5ca258316260fb802c65d9c3cc4a9137e0a09a873d4404d5b24fcc in / 
# Wed, 01 Nov 2023 00:39:29 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 13:48:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:48:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:50:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2e1a1831feefb5bd8f0a9fbc43f06ac287e16d9dd672e28d11eb17f3df2c71cd`  
		Last Modified: Wed, 01 Nov 2023 00:44:36 GMT  
		Size: 51.3 MB (51255735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4efeebbb8917115755445da9fb58c99b67f18a2552b83c24eb9b3a6b280700de`  
		Last Modified: Wed, 01 Nov 2023 13:58:36 GMT  
		Size: 18.1 MB (18099490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52765542e10643f266bb59e790311fa685b420f7ddf55344e27da30b0e98fb64`  
		Last Modified: Wed, 01 Nov 2023 13:58:57 GMT  
		Size: 53.5 MB (53488289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edccb9c788dcbf10ac8a2c7dea85d9116e0b0bb24b034ce8a03e4e00cb5820b2`  
		Last Modified: Wed, 01 Nov 2023 13:59:40 GMT  
		Size: 198.4 MB (198440557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldoldstable-curl`

```console
$ docker pull buildpack-deps@sha256:6f247f6bed7b6840e5c67f0438cddaec352488db0748e6f1d8a712f493d11802
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:oldoldstable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:8c5b0be8284f3ffad21b631a565d95b206ad13fd7fab4860bed8ae57dbec5bd3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68083055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffa032cdabe4be1922293729cab49304bdbfc5bb0a7ecf88d15b26752bcd58a6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:21 GMT
ADD file:e12306e266f3e237ff7df5ea95bd339c3eb4a539f31be801afd63a76e116f522 in / 
# Wed, 01 Nov 2023 00:21:22 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:55:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:711706b827bb26857b90ceb32b653a05be0e06459342cc05124da0f97f9b6ad9`  
		Last Modified: Wed, 01 Nov 2023 00:26:31 GMT  
		Size: 50.5 MB (50499123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465ae13a022e930633aeb58ebf812a0350a4ec43803e013187863d358e62f15f`  
		Last Modified: Wed, 01 Nov 2023 01:04:06 GMT  
		Size: 17.6 MB (17583932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:547c920f8106c64ef8fef69ea98bbb06f3f5db4cb6e6ce5e702a3d48326dbbac
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62181799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:842dffaf721877ed8fd91016937a055c084b9f96228d966abacc70503596ee76`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:58:20 GMT
ADD file:ff8efe260318f1cfb8bfc8aaaa6d6bb15c878689f7edea37d776cf111c30fefb in / 
# Wed, 01 Nov 2023 00:58:20 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:33:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:608341ab24b1ec00c021d73e16dbb8ca54b2437a4a3f5ae09ca58578603a32bf`  
		Last Modified: Wed, 01 Nov 2023 01:03:18 GMT  
		Size: 46.0 MB (45966058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d69be9a283bc43e8f0b0d0da1bb41aaf159446bc58f5d8f73cd7c86fd9d3cc`  
		Last Modified: Wed, 01 Nov 2023 02:44:00 GMT  
		Size: 16.2 MB (16215741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3187ad722182d5ffc423d3c4e25669ca3060f6b403232da1593133503aaa5311
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66745183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99607d7258254818c503a77cfe1d852a45c168e4c07cde3dfaa3210ace0def66`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:40:02 GMT
ADD file:e3f63671dca138b2b525b60f1471241941cdf4dab7f0c17cd91124978716bd93 in / 
# Wed, 01 Nov 2023 00:40:02 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:07:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d3db7215fb502c5873a81db7c6fd3214f199f6a1d8034da9d90918ac3220b20b`  
		Last Modified: Wed, 01 Nov 2023 00:44:04 GMT  
		Size: 49.3 MB (49291092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273f65b8dba688a4aab84c27f594891edb3518fd96d226c06ca7667c8c2a5b06`  
		Last Modified: Wed, 01 Nov 2023 02:15:35 GMT  
		Size: 17.5 MB (17454091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:860907a7a7afe3f516a398c4bc4fcd433e291cbf564587b42f7818462dd571c6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.4 MB (69355225 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67647118a2406cfa85155bb8a01a813c5d19b67a81364505935d344f41d7d932`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:28 GMT
ADD file:65beb9bd9a5ca258316260fb802c65d9c3cc4a9137e0a09a873d4404d5b24fcc in / 
# Wed, 01 Nov 2023 00:39:29 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 13:48:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2e1a1831feefb5bd8f0a9fbc43f06ac287e16d9dd672e28d11eb17f3df2c71cd`  
		Last Modified: Wed, 01 Nov 2023 00:44:36 GMT  
		Size: 51.3 MB (51255735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4efeebbb8917115755445da9fb58c99b67f18a2552b83c24eb9b3a6b280700de`  
		Last Modified: Wed, 01 Nov 2023 13:58:36 GMT  
		Size: 18.1 MB (18099490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldoldstable-scm`

```console
$ docker pull buildpack-deps@sha256:fd691cd5b0c388046d1240a0668d65b62d77574d933a323bd30d909a37121960
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:oldoldstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:4e63e1919e1281065996f42681e6b2f5962e28fb15610d02cbb8cad12a395cfa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.0 MB (119957009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b0f4e232802bdb79ecad162dc2170c54cd789211d8b17c6fdbbe34502eebfd9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:21 GMT
ADD file:e12306e266f3e237ff7df5ea95bd339c3eb4a539f31be801afd63a76e116f522 in / 
# Wed, 01 Nov 2023 00:21:22 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:55:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 00:56:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:711706b827bb26857b90ceb32b653a05be0e06459342cc05124da0f97f9b6ad9`  
		Last Modified: Wed, 01 Nov 2023 00:26:31 GMT  
		Size: 50.5 MB (50499123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465ae13a022e930633aeb58ebf812a0350a4ec43803e013187863d358e62f15f`  
		Last Modified: Wed, 01 Nov 2023 01:04:06 GMT  
		Size: 17.6 MB (17583932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac648dffba596ed8d982778472e34b8ba1ad650a3ea934c0c1b202e63e338860`  
		Last Modified: Wed, 01 Nov 2023 01:04:21 GMT  
		Size: 51.9 MB (51873954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:dbeda7c5cd3b5023e84fd8111f8691ab1c4d0448e93f288091ad74479c344d51
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.6 MB (109592821 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8056131f6b34799617afef5be94af84f6c0140b7610b218f084a4597e00df1d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:58:20 GMT
ADD file:ff8efe260318f1cfb8bfc8aaaa6d6bb15c878689f7edea37d776cf111c30fefb in / 
# Wed, 01 Nov 2023 00:58:20 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:33:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:34:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:608341ab24b1ec00c021d73e16dbb8ca54b2437a4a3f5ae09ca58578603a32bf`  
		Last Modified: Wed, 01 Nov 2023 01:03:18 GMT  
		Size: 46.0 MB (45966058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2d69be9a283bc43e8f0b0d0da1bb41aaf159446bc58f5d8f73cd7c86fd9d3cc`  
		Last Modified: Wed, 01 Nov 2023 02:44:00 GMT  
		Size: 16.2 MB (16215741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0b6d0aa1dff66e917c4bbec58a8d82c3bf1380c7772452e657e0e4ad5c190e`  
		Last Modified: Wed, 01 Nov 2023 02:44:16 GMT  
		Size: 47.4 MB (47411022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:440f4f9f9e36fe1c7aa17c2a75d5764603f4dc8afb7924b71c83fb73405d82ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.0 MB (118953523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bffb0b1dca0833986cd2d5c52f34da17dc8b5cad2d118f4e5775db45049ff8f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:40:02 GMT
ADD file:e3f63671dca138b2b525b60f1471241941cdf4dab7f0c17cd91124978716bd93 in / 
# Wed, 01 Nov 2023 00:40:02 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:07:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:07:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d3db7215fb502c5873a81db7c6fd3214f199f6a1d8034da9d90918ac3220b20b`  
		Last Modified: Wed, 01 Nov 2023 00:44:04 GMT  
		Size: 49.3 MB (49291092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273f65b8dba688a4aab84c27f594891edb3518fd96d226c06ca7667c8c2a5b06`  
		Last Modified: Wed, 01 Nov 2023 02:15:35 GMT  
		Size: 17.5 MB (17454091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c150f07b6a196359013d5fe6373a86fec69409163977b1cd213268cd033d320c`  
		Last Modified: Wed, 01 Nov 2023 02:15:49 GMT  
		Size: 52.2 MB (52208340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:e721e5812cb11d6b77990dffebc194b4663f5848d6f439c87920d67d95635b98
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.8 MB (122843514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e56a96c2faf3f6388c9337058992884b3dcaeec74a26a10a8801695fe84458fa`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:28 GMT
ADD file:65beb9bd9a5ca258316260fb802c65d9c3cc4a9137e0a09a873d4404d5b24fcc in / 
# Wed, 01 Nov 2023 00:39:29 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 13:48:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:48:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2e1a1831feefb5bd8f0a9fbc43f06ac287e16d9dd672e28d11eb17f3df2c71cd`  
		Last Modified: Wed, 01 Nov 2023 00:44:36 GMT  
		Size: 51.3 MB (51255735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4efeebbb8917115755445da9fb58c99b67f18a2552b83c24eb9b3a6b280700de`  
		Last Modified: Wed, 01 Nov 2023 13:58:36 GMT  
		Size: 18.1 MB (18099490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52765542e10643f266bb59e790311fa685b420f7ddf55344e27da30b0e98fb64`  
		Last Modified: Wed, 01 Nov 2023 13:58:57 GMT  
		Size: 53.5 MB (53488289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldstable`

```console
$ docker pull buildpack-deps@sha256:91d0d87bdeb73250aa8b9bc1739ab59e0df4e365dd7e459d1d453d46befd93c3
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
$ docker pull buildpack-deps@sha256:e5b39fe0f583451250fadb67733c6d8a9c946ac57311eb29e32f2ef2fe4738d8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.3 MB (322297709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:337d5c3296dbe61598d78522d56582f1893dbf23ecf8b2a563411e498bdbf0c7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:59 GMT
ADD file:da3938f00f114fa8f5948fb7182da39c43e5ce57a334ba528681cb29aff0d2f6 in / 
# Wed, 01 Nov 2023 00:21:00 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:53:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 00:54:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 00:55:16 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2f088d622efd8dbaa13d01eafd0aac8f9f33bb335edd3be897ae8059338c7bf7`  
		Last Modified: Wed, 01 Nov 2023 00:25:49 GMT  
		Size: 55.1 MB (55058052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de448b80f06437f3025dcaa9285d40c9c81e4be00df1b04bd5a26fd6b9447fc8`  
		Last Modified: Wed, 01 Nov 2023 01:03:07 GMT  
		Size: 15.8 MB (15764212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24e5da9a0e1f93fa4f1a07ca9a691e0d941bab6927f80157ffc14b478815f95b`  
		Last Modified: Wed, 01 Nov 2023 01:03:23 GMT  
		Size: 54.6 MB (54595619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d61681290435197504d4cdaa3724700bd66544d064d068e837f70e5abede255`  
		Last Modified: Wed, 01 Nov 2023 01:03:55 GMT  
		Size: 196.9 MB (196879826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:e498b9b502d1ca1acfa852d25bfce183b268515664ebfcc3a4e87c68e4725e1d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.4 MB (295371150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f3c22a828484005d7d76c4c66e1b944be8c68f20bcc8ecd02ac88b1b12ca17a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:48:39 GMT
ADD file:6fcdedd346da0744f7f45d0e7df77336a37ce87345bd414bd4e198804980781e in / 
# Wed, 01 Nov 2023 00:48:40 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:57:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:57:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:59:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e0adb3cac2906548cd3544bf3c384be3e3bdca9d41c37e11c160813af74301b9`  
		Last Modified: Wed, 01 Nov 2023 00:51:49 GMT  
		Size: 52.6 MB (52563334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f1ac168a113a53eb04058318b3d7cb7470e780e76570d1454453907e7a8707`  
		Last Modified: Wed, 01 Nov 2023 03:06:05 GMT  
		Size: 15.4 MB (15374711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17505c8dbffa755d9815a1b1f2a760d22100354db441079cb21283d37a0f5cae`  
		Last Modified: Wed, 01 Nov 2023 03:06:23 GMT  
		Size: 52.3 MB (52331088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af45e26d5b203d7ce4ea96b10a3e560243b596a031d560011445a0febbf5983`  
		Last Modified: Wed, 01 Nov 2023 03:06:58 GMT  
		Size: 175.1 MB (175102017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:0ec89f8bc6a95decbf549e0463c9560d0705af1099c8c4e66dc388810624ab4a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.8 MB (282800617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b7746f40355811236974bb35f0f769d9275f70b839f97e18e010fdff459f6dd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:58:01 GMT
ADD file:5e11ff51eeca3d0b7e760186b5792864fee2bfe7e8a1fa531a89870abaebfc89 in / 
# Wed, 01 Nov 2023 00:58:02 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:31:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:32:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:33:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:17b69ad2612f8fffb539ede3765dcc1fbd121518fd38fe89720482d622dbc960`  
		Last Modified: Wed, 01 Nov 2023 01:02:32 GMT  
		Size: 50.2 MB (50215350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0803d90cd63c47dea677f156a9802a95d09886d9a3b07415dd94b2ac199f25`  
		Last Modified: Wed, 01 Nov 2023 02:43:01 GMT  
		Size: 14.9 MB (14879723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524b9dc19e6fd54f3a85453a84bc99da2ca6e508d91ce084872e33c6c60d774c`  
		Last Modified: Wed, 01 Nov 2023 02:43:18 GMT  
		Size: 50.4 MB (50353285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b091dd2c95f61d367ee00244a69ce9fbbbe3b5cf82c05e675bfeb00a2d248480`  
		Last Modified: Wed, 01 Nov 2023 02:43:48 GMT  
		Size: 167.4 MB (167352259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:507681f36e1adb6d525f95c0a2d182fc847c2d74bb04e84db4fe41a55b1a6ccf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.0 MB (313958442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8f1530a08d0a05c65962560d0105156de41a165257827ced93a5c5c30c81e0a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:48 GMT
ADD file:f5677286e85ce6a345c7f5937e1ec576c37228e49c0fafe33574614c81cb7f76 in / 
# Wed, 01 Nov 2023 00:39:48 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:06:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:06:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:07:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d42ebdfc37acca5c3acbe173ac11133e691b402003a525c2b8431baf6935291e`  
		Last Modified: Wed, 01 Nov 2023 00:43:25 GMT  
		Size: 53.7 MB (53707757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098bcc814ee5bafa2842bc45ecc3974bc4f2b66d05b05a8da5ac0c9fb91be947`  
		Last Modified: Wed, 01 Nov 2023 02:14:42 GMT  
		Size: 15.7 MB (15749872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e627bbf1475bea4dce35bb2c9ee58b6eb3be5573e4efe8bd5793ae6a1555118`  
		Last Modified: Wed, 01 Nov 2023 02:14:57 GMT  
		Size: 54.7 MB (54699568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1aedf10290011154f8817dfb0b21ae189951f1bfcc41d82b3ed061ae69c6ff9`  
		Last Modified: Wed, 01 Nov 2023 02:15:24 GMT  
		Size: 189.8 MB (189801245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:e86c91c91fe62b43e8e45b32b82fa0be22969497a312e05cf39a51aaeaf67f4f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.0 MB (328046228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47bcedab4330997f14313c4b8012559714b4c4a50ae19a963576cfd318fd4659`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:06 GMT
ADD file:4095d27bc1a281dda044919be3bb570d581df169c01f22b0963b38e0dd6d9eff in / 
# Wed, 01 Nov 2023 00:39:07 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 13:46:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:46:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:47:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:95d6aa56ba74b8ed0a732c4676a2c45c84a18076696d466cd9bf0b459c600e02`  
		Last Modified: Wed, 01 Nov 2023 00:43:49 GMT  
		Size: 56.0 MB (56046261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a221a3957c157fc6091d669757aa644810547d3e3fcf1e1af9da5c23408ccfd`  
		Last Modified: Wed, 01 Nov 2023 13:57:18 GMT  
		Size: 16.3 MB (16268154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae620e9f38cdbc37cabf7785918528f2cabd2fc93a6f2df4a0536a17c985a83`  
		Last Modified: Wed, 01 Nov 2023 13:57:39 GMT  
		Size: 55.9 MB (55937130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3adf864130f60c8d2fc5630732c739bcbf96036834ad946abd62c2b01311aa01`  
		Last Modified: Wed, 01 Nov 2023 13:58:23 GMT  
		Size: 199.8 MB (199794683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:e594b6e1cfae9243fd7cbefe66cf6bc57a66bc539bdeed15fd448e150064a0fa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.1 MB (301123609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71ec146db4e94ece054208dbb3d587c01e6c09b362a2191332a29dca4e72a5ca`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:09:34 GMT
ADD file:2c9f9140e731974a497825454c08d67829f514a83742973e30454cc905ebac6c in / 
# Wed, 01 Nov 2023 01:09:39 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 21:26:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 21:27:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 21:33:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a10c6e715fcf314db953339b3e58b9e0167f6cd2d02bf633e20282058eb83331`  
		Last Modified: Wed, 01 Nov 2023 01:20:31 GMT  
		Size: 53.3 MB (53288991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe6d659051b6e411cbd9b3be6e727341a73a5b15c0c29975704b7249f84fd86`  
		Last Modified: Wed, 01 Nov 2023 21:57:24 GMT  
		Size: 15.5 MB (15529696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8566d8664b53694b0954345257a0d1054f4e6986ca39c2e219045fec1804bca9`  
		Last Modified: Wed, 01 Nov 2023 21:58:10 GMT  
		Size: 53.3 MB (53302576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9127ef70b3d7f2c8696b4631dc66ee403ee865e060aa586e35ac9ae4217dfca`  
		Last Modified: Wed, 01 Nov 2023 22:00:10 GMT  
		Size: 179.0 MB (179002346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:82bc2a3f618b2276770a5b4e66fc4eb97dc374aa4d6262bc4f8e7328416884d7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.8 MB (330808710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac93ae090ca7af9095be55d239af46ce549e519e63cef45c4c9cf11e16473ea5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:51 GMT
ADD file:68e9024f0c99fe38d7046b4ad1aee044d14b93d248ec431380a1cefcacb7dea3 in / 
# Wed, 01 Nov 2023 00:21:54 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:27:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:28:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:31:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d002f39ef040587852c73a806a7f49edd2ae7eb78b997c05ca1c5bfedad0506d`  
		Last Modified: Wed, 01 Nov 2023 00:26:33 GMT  
		Size: 58.9 MB (58929494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8932ef1d4dad602784eb2f811c1c987e261b97dfbc072a2c097836198cc588b`  
		Last Modified: Wed, 01 Nov 2023 01:41:47 GMT  
		Size: 16.8 MB (16765480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5598ff1b384ed8a267e359e36806478cf035252da4caca5d70aae48d01bcde`  
		Last Modified: Wed, 01 Nov 2023 01:42:05 GMT  
		Size: 58.9 MB (58865922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b8984065c2be285a155b4228b44b214dc7b7918b687b2c17d3e3136e5a7b03`  
		Last Modified: Wed, 01 Nov 2023 01:42:43 GMT  
		Size: 196.2 MB (196247814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:9d61cfff42a2c3154228569b2d18a12fa0110f89af96c3c01f32a15657e5fbde
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.9 MB (295893097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:899a28fa35119cbb45aec21c0d234226f5e5ea9d03d265db0ae96dda474a9660`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:42:50 GMT
ADD file:5c168741fe0b80d3b365ae703c082556326a889730963a304b218ab3361d2e8a in / 
# Wed, 01 Nov 2023 00:42:54 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:56:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:57:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:58:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a21b3124d41be76bb35d41f49b041980e640c1ea030b4099c4eaa419414f1618`  
		Last Modified: Wed, 01 Nov 2023 00:48:19 GMT  
		Size: 53.3 MB (53296572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb969a0416e6d103d044f625db373b704e7253a5661a213c76711df733f8db0`  
		Last Modified: Wed, 01 Nov 2023 02:06:09 GMT  
		Size: 15.6 MB (15640071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6df2909ff3ad376afb0b5c8415d39aa102919dfc8415cd2c3d3ab0866cb8794`  
		Last Modified: Wed, 01 Nov 2023 02:06:23 GMT  
		Size: 54.1 MB (54065848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7c416e9929ef46a9a0f52c4720975b46e23cda524123c9f33d3d9bf287a380`  
		Last Modified: Wed, 01 Nov 2023 02:06:49 GMT  
		Size: 172.9 MB (172890606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldstable-curl`

```console
$ docker pull buildpack-deps@sha256:daee6a831682d0fef3be9af87ffa7b513a8923199f3ee75e63d787ca7a0eb445
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
$ docker pull buildpack-deps@sha256:fe96c991e03a42155f09f164fab997201cd385d51b961d79c2cee47dad3fa471
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.8 MB (70822264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9267342af80900380a694508ac882c18c81244c1790e1a82484f2b23e45b6ce5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:59 GMT
ADD file:da3938f00f114fa8f5948fb7182da39c43e5ce57a334ba528681cb29aff0d2f6 in / 
# Wed, 01 Nov 2023 00:21:00 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:53:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2f088d622efd8dbaa13d01eafd0aac8f9f33bb335edd3be897ae8059338c7bf7`  
		Last Modified: Wed, 01 Nov 2023 00:25:49 GMT  
		Size: 55.1 MB (55058052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de448b80f06437f3025dcaa9285d40c9c81e4be00df1b04bd5a26fd6b9447fc8`  
		Last Modified: Wed, 01 Nov 2023 01:03:07 GMT  
		Size: 15.8 MB (15764212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:7b311b6096eb6345ca23254eedd11cdc452439fd11a0f754602457b1cd51f5af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.9 MB (67938045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fdeee1b038c70ec83b9f0de8673d6232c0d52472bde1372852e3c01a3e7fb2d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:48:39 GMT
ADD file:6fcdedd346da0744f7f45d0e7df77336a37ce87345bd414bd4e198804980781e in / 
# Wed, 01 Nov 2023 00:48:40 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:57:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e0adb3cac2906548cd3544bf3c384be3e3bdca9d41c37e11c160813af74301b9`  
		Last Modified: Wed, 01 Nov 2023 00:51:49 GMT  
		Size: 52.6 MB (52563334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f1ac168a113a53eb04058318b3d7cb7470e780e76570d1454453907e7a8707`  
		Last Modified: Wed, 01 Nov 2023 03:06:05 GMT  
		Size: 15.4 MB (15374711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:938715a48d3af6947e95b1ba3f7d072a0383966fa35cb4e543d0df56d5f09ac7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.1 MB (65095073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de18a5e0f396c35eee7ef96ee7cf1030ac0c1aba47e9a7311dae5b771137335c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:58:01 GMT
ADD file:5e11ff51eeca3d0b7e760186b5792864fee2bfe7e8a1fa531a89870abaebfc89 in / 
# Wed, 01 Nov 2023 00:58:02 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:31:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:17b69ad2612f8fffb539ede3765dcc1fbd121518fd38fe89720482d622dbc960`  
		Last Modified: Wed, 01 Nov 2023 01:02:32 GMT  
		Size: 50.2 MB (50215350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0803d90cd63c47dea677f156a9802a95d09886d9a3b07415dd94b2ac199f25`  
		Last Modified: Wed, 01 Nov 2023 02:43:01 GMT  
		Size: 14.9 MB (14879723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a5756865ff5b689520b2adc61fe9c4e1d05fc87bc136dd6f8e4e84e7aa595583
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69457629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0307db700b406ff0f670aafedc3682ef7699b96e9b1288101822e3417b87d6ca`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:48 GMT
ADD file:f5677286e85ce6a345c7f5937e1ec576c37228e49c0fafe33574614c81cb7f76 in / 
# Wed, 01 Nov 2023 00:39:48 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:06:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d42ebdfc37acca5c3acbe173ac11133e691b402003a525c2b8431baf6935291e`  
		Last Modified: Wed, 01 Nov 2023 00:43:25 GMT  
		Size: 53.7 MB (53707757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098bcc814ee5bafa2842bc45ecc3974bc4f2b66d05b05a8da5ac0c9fb91be947`  
		Last Modified: Wed, 01 Nov 2023 02:14:42 GMT  
		Size: 15.7 MB (15749872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:3031323302eaff84a691d3ee86f673dcf58faec6ca26af36306a26264bf3fc4b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.3 MB (72314415 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30e808a609f652bd8bfd97a50be155e7b8cd8f48d49c5dcca1574139b8b52ebc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:06 GMT
ADD file:4095d27bc1a281dda044919be3bb570d581df169c01f22b0963b38e0dd6d9eff in / 
# Wed, 01 Nov 2023 00:39:07 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 13:46:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:95d6aa56ba74b8ed0a732c4676a2c45c84a18076696d466cd9bf0b459c600e02`  
		Last Modified: Wed, 01 Nov 2023 00:43:49 GMT  
		Size: 56.0 MB (56046261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a221a3957c157fc6091d669757aa644810547d3e3fcf1e1af9da5c23408ccfd`  
		Last Modified: Wed, 01 Nov 2023 13:57:18 GMT  
		Size: 16.3 MB (16268154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:d8e9e7111c1ffedd6d881f3b0e23d591e549254d9769e151fd5b120c2722c378
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68818687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1dca7251f559caeddfa4e791323c9b2839014697d5e5af163f859e9a94e594c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:09:34 GMT
ADD file:2c9f9140e731974a497825454c08d67829f514a83742973e30454cc905ebac6c in / 
# Wed, 01 Nov 2023 01:09:39 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 21:26:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a10c6e715fcf314db953339b3e58b9e0167f6cd2d02bf633e20282058eb83331`  
		Last Modified: Wed, 01 Nov 2023 01:20:31 GMT  
		Size: 53.3 MB (53288991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe6d659051b6e411cbd9b3be6e727341a73a5b15c0c29975704b7249f84fd86`  
		Last Modified: Wed, 01 Nov 2023 21:57:24 GMT  
		Size: 15.5 MB (15529696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:7cc922cccb492c0a7586506eb781cfd4aca3122d5bad473bcc57f8faf10f1b9a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75694974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b4307adf590ebe3c7869b5b22159689cfaa09e73b33741d2ccb188a374ee2ac`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:51 GMT
ADD file:68e9024f0c99fe38d7046b4ad1aee044d14b93d248ec431380a1cefcacb7dea3 in / 
# Wed, 01 Nov 2023 00:21:54 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:27:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d002f39ef040587852c73a806a7f49edd2ae7eb78b997c05ca1c5bfedad0506d`  
		Last Modified: Wed, 01 Nov 2023 00:26:33 GMT  
		Size: 58.9 MB (58929494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8932ef1d4dad602784eb2f811c1c987e261b97dfbc072a2c097836198cc588b`  
		Last Modified: Wed, 01 Nov 2023 01:41:47 GMT  
		Size: 16.8 MB (16765480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:cef619c4e2fff9d2bd0e6bcc3b9254d2e33f7347143cc9124087dee5433f476f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68936643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:899170b75ff49b852db13ad9fd0b8e0b9c69f7fa9fa438bfea0bd62bddfd75bd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:42:50 GMT
ADD file:5c168741fe0b80d3b365ae703c082556326a889730963a304b218ab3361d2e8a in / 
# Wed, 01 Nov 2023 00:42:54 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:56:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a21b3124d41be76bb35d41f49b041980e640c1ea030b4099c4eaa419414f1618`  
		Last Modified: Wed, 01 Nov 2023 00:48:19 GMT  
		Size: 53.3 MB (53296572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb969a0416e6d103d044f625db373b704e7253a5661a213c76711df733f8db0`  
		Last Modified: Wed, 01 Nov 2023 02:06:09 GMT  
		Size: 15.6 MB (15640071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldstable-scm`

```console
$ docker pull buildpack-deps@sha256:70ff4e786a57b07a66e70fc4ac621abc2f85c90c8a50c92db1004d750f1afceb
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
$ docker pull buildpack-deps@sha256:aee2844de5599ce4ea6389a884d8cd4a8de58712b6e5a02d62251f18e8696060
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.4 MB (125417883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c9ef67b38f3703597d152b6d1c032033b993b1828d68fe7495ac3768f7a967b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:59 GMT
ADD file:da3938f00f114fa8f5948fb7182da39c43e5ce57a334ba528681cb29aff0d2f6 in / 
# Wed, 01 Nov 2023 00:21:00 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:53:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 00:54:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2f088d622efd8dbaa13d01eafd0aac8f9f33bb335edd3be897ae8059338c7bf7`  
		Last Modified: Wed, 01 Nov 2023 00:25:49 GMT  
		Size: 55.1 MB (55058052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de448b80f06437f3025dcaa9285d40c9c81e4be00df1b04bd5a26fd6b9447fc8`  
		Last Modified: Wed, 01 Nov 2023 01:03:07 GMT  
		Size: 15.8 MB (15764212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24e5da9a0e1f93fa4f1a07ca9a691e0d941bab6927f80157ffc14b478815f95b`  
		Last Modified: Wed, 01 Nov 2023 01:03:23 GMT  
		Size: 54.6 MB (54595619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:dc112c6d13a25d02bc6c10da7320cf3cd72abcd6902b3d8b1daa1b435692630b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.3 MB (120269133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3eba71c7387e8a339718a365505f0baf67502bf260281df1d28565c819cf769`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:48:39 GMT
ADD file:6fcdedd346da0744f7f45d0e7df77336a37ce87345bd414bd4e198804980781e in / 
# Wed, 01 Nov 2023 00:48:40 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:57:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:57:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e0adb3cac2906548cd3544bf3c384be3e3bdca9d41c37e11c160813af74301b9`  
		Last Modified: Wed, 01 Nov 2023 00:51:49 GMT  
		Size: 52.6 MB (52563334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f1ac168a113a53eb04058318b3d7cb7470e780e76570d1454453907e7a8707`  
		Last Modified: Wed, 01 Nov 2023 03:06:05 GMT  
		Size: 15.4 MB (15374711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17505c8dbffa755d9815a1b1f2a760d22100354db441079cb21283d37a0f5cae`  
		Last Modified: Wed, 01 Nov 2023 03:06:23 GMT  
		Size: 52.3 MB (52331088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f91a8bb800cf9f7759f256b610549bab7137aa27b412e565c153877592aa25fc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115448358 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7293fc0d511b0567083617d783259480fb8c6f9398173f21707a6aa45f36094`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:58:01 GMT
ADD file:5e11ff51eeca3d0b7e760186b5792864fee2bfe7e8a1fa531a89870abaebfc89 in / 
# Wed, 01 Nov 2023 00:58:02 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:31:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:32:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:17b69ad2612f8fffb539ede3765dcc1fbd121518fd38fe89720482d622dbc960`  
		Last Modified: Wed, 01 Nov 2023 01:02:32 GMT  
		Size: 50.2 MB (50215350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0803d90cd63c47dea677f156a9802a95d09886d9a3b07415dd94b2ac199f25`  
		Last Modified: Wed, 01 Nov 2023 02:43:01 GMT  
		Size: 14.9 MB (14879723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524b9dc19e6fd54f3a85453a84bc99da2ca6e508d91ce084872e33c6c60d774c`  
		Last Modified: Wed, 01 Nov 2023 02:43:18 GMT  
		Size: 50.4 MB (50353285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:4cf4511cd7836341048828afed7f6f64760851ab73b5d451014aae119afa1a8d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.2 MB (124157197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfed8a1aba30dc750dde56fe15716729ccb292429fe81882481c660fc3e3fc70`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:48 GMT
ADD file:f5677286e85ce6a345c7f5937e1ec576c37228e49c0fafe33574614c81cb7f76 in / 
# Wed, 01 Nov 2023 00:39:48 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:06:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:06:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d42ebdfc37acca5c3acbe173ac11133e691b402003a525c2b8431baf6935291e`  
		Last Modified: Wed, 01 Nov 2023 00:43:25 GMT  
		Size: 53.7 MB (53707757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098bcc814ee5bafa2842bc45ecc3974bc4f2b66d05b05a8da5ac0c9fb91be947`  
		Last Modified: Wed, 01 Nov 2023 02:14:42 GMT  
		Size: 15.7 MB (15749872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e627bbf1475bea4dce35bb2c9ee58b6eb3be5573e4efe8bd5793ae6a1555118`  
		Last Modified: Wed, 01 Nov 2023 02:14:57 GMT  
		Size: 54.7 MB (54699568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8d58db39b5254846274374168677310fff3253244bf5a6d2ce6260f6a954d56f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128251545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00fcd7435762272d60c82baecddc1312882335ef3b4d818cd0b3c67fecf85729`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:06 GMT
ADD file:4095d27bc1a281dda044919be3bb570d581df169c01f22b0963b38e0dd6d9eff in / 
# Wed, 01 Nov 2023 00:39:07 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 13:46:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:46:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:95d6aa56ba74b8ed0a732c4676a2c45c84a18076696d466cd9bf0b459c600e02`  
		Last Modified: Wed, 01 Nov 2023 00:43:49 GMT  
		Size: 56.0 MB (56046261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a221a3957c157fc6091d669757aa644810547d3e3fcf1e1af9da5c23408ccfd`  
		Last Modified: Wed, 01 Nov 2023 13:57:18 GMT  
		Size: 16.3 MB (16268154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae620e9f38cdbc37cabf7785918528f2cabd2fc93a6f2df4a0536a17c985a83`  
		Last Modified: Wed, 01 Nov 2023 13:57:39 GMT  
		Size: 55.9 MB (55937130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:d93ee9ee466572ddc358a190303042e8ecbc24d89865152f38eea95055e713f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122121263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db1876f7fa25cbcab884a102075bd6f8684bba0e6b6360ff846167f0de396728`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:09:34 GMT
ADD file:2c9f9140e731974a497825454c08d67829f514a83742973e30454cc905ebac6c in / 
# Wed, 01 Nov 2023 01:09:39 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 21:26:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 21:27:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a10c6e715fcf314db953339b3e58b9e0167f6cd2d02bf633e20282058eb83331`  
		Last Modified: Wed, 01 Nov 2023 01:20:31 GMT  
		Size: 53.3 MB (53288991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe6d659051b6e411cbd9b3be6e727341a73a5b15c0c29975704b7249f84fd86`  
		Last Modified: Wed, 01 Nov 2023 21:57:24 GMT  
		Size: 15.5 MB (15529696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8566d8664b53694b0954345257a0d1054f4e6986ca39c2e219045fec1804bca9`  
		Last Modified: Wed, 01 Nov 2023 21:58:10 GMT  
		Size: 53.3 MB (53302576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:8117582621ca40cd9aa664d7a8920f2829422f7c27388f12eb20f8203c6d4015
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.6 MB (134560896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec96f11e0d12047d5722fc5d69d37309a058d1ed16360cb007b03aaf3c4c034b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:51 GMT
ADD file:68e9024f0c99fe38d7046b4ad1aee044d14b93d248ec431380a1cefcacb7dea3 in / 
# Wed, 01 Nov 2023 00:21:54 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:27:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:28:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d002f39ef040587852c73a806a7f49edd2ae7eb78b997c05ca1c5bfedad0506d`  
		Last Modified: Wed, 01 Nov 2023 00:26:33 GMT  
		Size: 58.9 MB (58929494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8932ef1d4dad602784eb2f811c1c987e261b97dfbc072a2c097836198cc588b`  
		Last Modified: Wed, 01 Nov 2023 01:41:47 GMT  
		Size: 16.8 MB (16765480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5598ff1b384ed8a267e359e36806478cf035252da4caca5d70aae48d01bcde`  
		Last Modified: Wed, 01 Nov 2023 01:42:05 GMT  
		Size: 58.9 MB (58865922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:87a81ace16049e3a81cb4550162435a699f3d58045130f0693a7b7092b14f2d3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (123002491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e97a46624fdc756523296a468935e44b34cfc5c8fa801fc0471b51842f34f960`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:42:50 GMT
ADD file:5c168741fe0b80d3b365ae703c082556326a889730963a304b218ab3361d2e8a in / 
# Wed, 01 Nov 2023 00:42:54 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:56:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:57:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a21b3124d41be76bb35d41f49b041980e640c1ea030b4099c4eaa419414f1618`  
		Last Modified: Wed, 01 Nov 2023 00:48:19 GMT  
		Size: 53.3 MB (53296572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb969a0416e6d103d044f625db373b704e7253a5661a213c76711df733f8db0`  
		Last Modified: Wed, 01 Nov 2023 02:06:09 GMT  
		Size: 15.6 MB (15640071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6df2909ff3ad376afb0b5c8415d39aa102919dfc8415cd2c3d3ab0866cb8794`  
		Last Modified: Wed, 01 Nov 2023 02:06:23 GMT  
		Size: 54.1 MB (54065848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:scm`

```console
$ docker pull buildpack-deps@sha256:c128f8e680e8bfc06477d452a567975cc58188cddefc68cec3c72c1d8a15a4b2
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
$ docker pull buildpack-deps@sha256:93590f9f25a12437d9d01f7ac4309b83af5532680e36bbc01181f61e19ae7135
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.8 MB (137761586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:941f9c887621d4fee5936ccc92b35b887f74ed81aac7b90fcedc1fcb5d65741b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:37 GMT
ADD file:3e9b6405f11dd24ce62105c033f1d8b931d9409298553f63b03af1b6dd1dda35 in / 
# Wed, 01 Nov 2023 00:20:38 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:52:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 00:52:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8457fd5474e70835e4482983a5662355d892d5f6f0f90a27a8e9f009997e8196`  
		Last Modified: Wed, 01 Nov 2023 00:25:05 GMT  
		Size: 49.6 MB (49582024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13baa2029dde87a21b87127168a0fb50a007c07da6b5adc8864e1fe1376c86ff`  
		Last Modified: Wed, 01 Nov 2023 01:02:01 GMT  
		Size: 24.0 MB (24049147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:325c5bf4c2f26c11380501bec4b6eef8a3ea35b554aa1b222cbcd1e1fe11ae1d`  
		Last Modified: Wed, 01 Nov 2023 01:02:20 GMT  
		Size: 64.1 MB (64130415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:9a1d134fc9b0926e5316223c1622334e19ab18d8c110ded139188fe219084032
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.6 MB (131645049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58e29752e0aab3ef315e59c15de2796ae467eea85f7d51848bbd963d7cdcf627`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:48:23 GMT
ADD file:963e26decfc65419428098047df29dcbf7865e13bcdd67abeb9849f99a7815e7 in / 
# Wed, 01 Nov 2023 00:48:23 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:53c5547a993a8adb09a632a8ae34fbc336b27a456c6b3a670865cd8bedb5e6a9`  
		Last Modified: Wed, 01 Nov 2023 00:51:04 GMT  
		Size: 47.4 MB (47355649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752979e12aac8f84972cea68e4f8d9bb1b645e71b3fc64047af1ba792dd338d9`  
		Last Modified: Wed, 01 Nov 2023 03:04:53 GMT  
		Size: 22.7 MB (22727584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bad2403917aecfddc5d239a343aacd942aeb9c9e6d76c027cfdbb0d5479bcaa`  
		Last Modified: Wed, 01 Nov 2023 03:05:15 GMT  
		Size: 61.6 MB (61561816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:d0accba6d4ea1e12f6ab955a70a96005bac84d284fa4ca006ed0a4b165b38db4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.4 MB (126397758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8322db01431af3b3bc3e5d7ca0be48f5ea14663ef8678973003e7aef9e95fbc3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:57:42 GMT
ADD file:3b2b4eda35d794b39d6b5567e81651625af51da3deb3f63b3ffdffa07720646e in / 
# Wed, 01 Nov 2023 00:57:42 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:30:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:30:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9bf855396a6f46c1cbac4e188af10f2c38474f989707b0b1b406b48c4b7284ef`  
		Last Modified: Wed, 01 Nov 2023 01:01:41 GMT  
		Size: 45.2 MB (45179410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6e59eca644b227cb755978679a3031e7b3f9a5c707057c293f2ba8732d8ef2`  
		Last Modified: Wed, 01 Nov 2023 02:41:40 GMT  
		Size: 22.0 MB (21951880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aefa016475f9e4925fd893a9d8cfcf375937aa4e637d337806176426509dfcd`  
		Last Modified: Wed, 01 Nov 2023 02:42:04 GMT  
		Size: 59.3 MB (59266468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3cec78f7e6894f6dd48b42e66476bad2daa2533d5b6d12b2cb243c765752e854
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.2 MB (137191567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d91cf57cfc88561be3a3af9dc95f31e6740e086c0a3db3dc1bd42da9ef6313ce`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:32 GMT
ADD file:c934ceb4c53a1cce6779198f1ea73d5c8aad9a035e750b343d49826120ecd0eb in / 
# Wed, 01 Nov 2023 00:39:33 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:04:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:04:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8024d4fb53b2455f66d49b7ee72eb3cad5074043578238b796a9879955946a88`  
		Last Modified: Wed, 01 Nov 2023 00:42:44 GMT  
		Size: 49.6 MB (49612653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d826ee8aa65e56e167f0e27fa65cfc065687a7ac6c360787d5940d8b51f0cf1`  
		Last Modified: Wed, 01 Nov 2023 02:13:39 GMT  
		Size: 23.6 MB (23584896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198068495d09b6865e75ce28d5d5d5de39897b8325ada63ba80eca884ad5666b`  
		Last Modified: Wed, 01 Nov 2023 02:13:57 GMT  
		Size: 64.0 MB (63994018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:4904b1a13827dfb9dc0294607ef88a92eb6d9fb5af266f3b436b6e747de5bbc9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.5 MB (141469924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c9c6e32dc86d819a813b06b60a98e41499c7cc87049b7acf4e87c5b4c52cb05`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:38:46 GMT
ADD file:4043d711d8d7d1a995aed0a6998c96230765f55d4449167107955fe4af2a31db in / 
# Wed, 01 Nov 2023 00:38:47 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 13:44:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:44:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be8d77e28ff21732ba73253b6226e47e4e07ec2cedc803ffd62148df5d7a165b`  
		Last Modified: Wed, 01 Nov 2023 00:43:00 GMT  
		Size: 50.6 MB (50600049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cef920c8d790c11b84fa21c2204cca8ac6a84ec43e4a60bca3670e828748583`  
		Last Modified: Wed, 01 Nov 2023 13:55:45 GMT  
		Size: 24.9 MB (24885575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fee1ec8688f07e43b49247f3490035da93288449034600daee26c8ce0150a8c`  
		Last Modified: Wed, 01 Nov 2023 13:56:13 GMT  
		Size: 66.0 MB (65984300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:7512d5d9e16a66d343238bf97e5b6d176e537b37e99b90b662154d61c082523b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.0 MB (135969193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ddc1f3c73e907d5ace49797cc746b10a794acc32d29af85c665e901745196ea`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:08:17 GMT
ADD file:b181441dc28bc6879e29cd086c569c653171c681525c124ffb6277bd71732bb1 in / 
# Wed, 01 Nov 2023 01:08:24 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 21:17:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 21:19:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0bfbf01892d22dd14fb9536e8675cc932ff41f415a415fbf8c6199106b01240d`  
		Last Modified: Wed, 01 Nov 2023 01:19:01 GMT  
		Size: 49.6 MB (49568811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9310598b7549f388c445368ea2a0a4077c57ddd45436efddb37e089d293f87fe`  
		Last Modified: Wed, 01 Nov 2023 21:53:41 GMT  
		Size: 23.4 MB (23438019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af2206444fab218d319700cbfcd93423bf4622bb8085adee11b684b7d3fd245`  
		Last Modified: Wed, 01 Nov 2023 21:54:35 GMT  
		Size: 63.0 MB (62962363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:e720e0531751cf77d1933f62e84bc5d4d2d63c0da3d890797548ca4e0192e571
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.9 MB (148858549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffb46a21911fb664a3630a45e7195ee955092521b2066322ec031cd4dd405ff3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:25 GMT
ADD file:31b995b44eb1f532fd265be3fc0c3d3b55e28db0911c86a06c83de621418db94 in / 
# Wed, 01 Nov 2023 00:21:28 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:24:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:24:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:071872f8f8cb44e883168d06195f8fbb330e259b415d1ab108c27bda84d6c060`  
		Last Modified: Wed, 01 Nov 2023 00:25:41 GMT  
		Size: 53.6 MB (53575361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9986fe7e71120fd78fcaad86d3a1d827f54f56f266364834bcb7c13eccf9ca0`  
		Last Modified: Wed, 01 Nov 2023 01:40:25 GMT  
		Size: 25.7 MB (25698676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7316c6cea433a21258a8af8686d8a74e964c21c6c563afd63f274e9346f8f7`  
		Last Modified: Wed, 01 Nov 2023 01:40:48 GMT  
		Size: 69.6 MB (69584512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:09520ba698b0b094ea1454bc687588fec9372d55e89e0b94e6afd1a415c1466f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.1 MB (135120752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e276550e9f3dc4f49a7d31441193c04d44abfc4220d18845eec66bdbbb473977`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:42:15 GMT
ADD file:6d8ee60b2fe4604969d8feeeb7e0dc8b9619a778d1a905c8bfdde5ede5e1eb54 in / 
# Wed, 01 Nov 2023 00:42:19 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:54:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:55:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bca95e393f709ba301b35c2439a815fd4fe8134d7a466bd528563bc32fd754d8`  
		Last Modified: Wed, 01 Nov 2023 00:47:43 GMT  
		Size: 47.9 MB (47943171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e744d1ef2c8405f6352136656080d7e244e1a97362c21069b734a55b86c8d0a`  
		Last Modified: Wed, 01 Nov 2023 02:05:09 GMT  
		Size: 24.0 MB (24045096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de40af46a5373d0a49892fa9000736be09090b477719517fcec84887d847f94b`  
		Last Modified: Wed, 01 Nov 2023 02:05:25 GMT  
		Size: 63.1 MB (63132485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:sid`

```console
$ docker pull buildpack-deps@sha256:f84df4a563092acda4fed5202298f0b6bfa78cb77cb7cbfd9d6ce293d83e8bd5
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
$ docker pull buildpack-deps@sha256:e7cc569fa46f03c3b37e2eb8a2e07f21c7e5b0e30cf67b785ebca55c8338b12e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.6 MB (351621495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e98f8ea8863e64d24c9f40759a43604de07e2ea088eee61d4a1f1f536226f449`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:49:10 GMT
ADD file:3dfec265d80292cf14629bdbd49822be7a5672ab8299d43e9ec734f6e032c8df in / 
# Wed, 01 Nov 2023 00:49:10 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:59:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 03:00:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 03:02:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0609920749c8743a3627a0a7a377598014123518f5e0ed7f1443c78c8c9f3446`  
		Last Modified: Wed, 01 Nov 2023 00:53:10 GMT  
		Size: 47.2 MB (47192458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3b7ab88084f4d09eb30fe75dbc159cd99b0692cea6232d2f457c292a62968c`  
		Last Modified: Wed, 01 Nov 2023 03:07:10 GMT  
		Size: 23.0 MB (23016482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3ff5e12103a446acf43b661291fc30a67ca5851b7c1f67906ac39a5a609ef1c`  
		Last Modified: Wed, 01 Nov 2023 03:07:30 GMT  
		Size: 63.0 MB (63010355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cefdf6db1915fab2d33c8090895aeecc671cb90ef4527f9b4ca1ae99fd45870d`  
		Last Modified: Wed, 01 Nov 2023 03:08:09 GMT  
		Size: 218.4 MB (218402200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:0b69a293dbe1e851613427c41b98e1ac973abf0ffd16ae00e87e83287cc0114a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.3 MB (332315093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bc1f83378e6ca85f13dee6672ad2ab008d5efd04b8307d9899c3b0cf1b87ff1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:59:14 GMT
ADD file:a72fe3de4b178dd8b7c48a1dc98d4c14520570e5edb66049dfe2cd6bb0a5dd6c in / 
# Wed, 01 Nov 2023 00:59:15 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:36:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:36:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:38:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f6e9a66eb905933433a5a2a8c16e480468f3731f107d5854bac12ef9a79bc271`  
		Last Modified: Wed, 01 Nov 2023 01:05:19 GMT  
		Size: 45.0 MB (44981409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c61548fabf75545be26d57a05800e5dbcd765a1c5c804a7671c92c59e15834d8`  
		Last Modified: Wed, 01 Nov 2023 02:44:58 GMT  
		Size: 22.2 MB (22234767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa95d6d6902734ac1af894edaf67096b114b4935d12a40bf35b44bca0f33e21`  
		Last Modified: Wed, 01 Nov 2023 02:45:16 GMT  
		Size: 60.6 MB (60610186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8828360bbf372d14fe88491ee679919df8f916259a40637ce6044d862916ccb`  
		Last Modified: Wed, 01 Nov 2023 02:45:51 GMT  
		Size: 204.5 MB (204488731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:4e0722b3b91c70dc433459035eb7504e1e3e4ace8334cf061672453cac0548b3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **374.4 MB (374367609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:703487ba0762e6be168e40b4bb8cd5297bd509bb84e88e953bdbc0cba3660726`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:40:45 GMT
ADD file:1a4ef85bba464538c4f87a65a055d954fc8edc51f26efd06b43d8ae9f7e54f7a in / 
# Wed, 01 Nov 2023 00:40:46 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:09:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:09:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:10:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ba6956ade110f0fe56bbad19a8d10b1eb0ae1b1006ccba5fadff0026a00dbc20`  
		Last Modified: Wed, 01 Nov 2023 00:45:46 GMT  
		Size: 49.6 MB (49552835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516c292c0ab5612a524438779924b5cc187f530a208c71056c8b9994656ef043`  
		Last Modified: Wed, 01 Nov 2023 02:16:27 GMT  
		Size: 23.9 MB (23916545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8977dd4a34d5416619317940446894bcaf8bc0c5f832e562683f4aa703db7f`  
		Last Modified: Wed, 01 Nov 2023 02:16:44 GMT  
		Size: 65.6 MB (65605231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f03a9258674c4a8e3c26a670786d3af44115d865542a8ca88ddb82d3056bee`  
		Last Modified: Wed, 01 Nov 2023 02:17:17 GMT  
		Size: 235.3 MB (235292998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; 386

```console
$ docker pull buildpack-deps@sha256:ae76f8ad80b82b6fdffaa4931dc6daa3ca2c972c3b5b05f2cb4991fb4720e31c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **388.7 MB (388669349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96527636c4addf379e53b4ec348c7fe3db44767d72e6489bb2c45db3f96f34b2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:40:31 GMT
ADD file:0aa90abbd80c68d937903de7ac8fdcce0f516fdd70f080b677af1e2322c000b9 in / 
# Wed, 01 Nov 2023 00:40:32 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 13:50:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:51:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:53:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:96660bac4658b1bffb27e96ac8ecc86753a1844f042ede32c4f1faef702dc202`  
		Last Modified: Wed, 01 Nov 2023 00:46:42 GMT  
		Size: 50.5 MB (50516486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7af088639fa61079db294f16f91145938a488365f2aec8cef7a85da80c4b13b`  
		Last Modified: Wed, 01 Nov 2023 13:59:54 GMT  
		Size: 25.2 MB (25185750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34a1138df818473932216f10a656452bbeead89efc81870811003208908e138`  
		Last Modified: Wed, 01 Nov 2023 14:00:17 GMT  
		Size: 67.3 MB (67267247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4105a9010ad6b6eb2295fe9bd43b392d6a4b2314d5c52c4020f7645fcd5b3c26`  
		Last Modified: Wed, 01 Nov 2023 14:01:10 GMT  
		Size: 245.7 MB (245699866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:41945b8dac854a10d2da3ff6944d8b39a59fb2e080101c9cb5583a0bd726fccd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.8 MB (359784858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2973da056cdad1602f11a8f10c07c22423951a38bd52b7024eae7189a700bbad`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:12:08 GMT
ADD file:e27a157c42d1aedcb0f6cf695f1f5c31d442488e049826c940509e2288537427 in / 
# Wed, 01 Nov 2023 01:12:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 21:35:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 21:36:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 21:43:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0eacf4d958160d2729e1bb31fbb12227afa7536ce6304928b13c2c65d297f9b9`  
		Last Modified: Wed, 01 Nov 2023 01:23:11 GMT  
		Size: 49.3 MB (49326735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76fea98d048b05ee3313ca45517a641b11637c7f8dc3ec543480fe6111a66fc0`  
		Last Modified: Wed, 01 Nov 2023 22:00:34 GMT  
		Size: 23.9 MB (23910243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde7d59b79a44cf2fd6509592cd5ffa2ac26dd4a37fb70dbe72408010c4a2926`  
		Last Modified: Wed, 01 Nov 2023 22:01:27 GMT  
		Size: 64.3 MB (64323488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:812e226799f37d4cc00732c97925157577a5924147f47974ea2e38bf5b013bf2`  
		Last Modified: Wed, 01 Nov 2023 22:03:55 GMT  
		Size: 222.2 MB (222224392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:a294a5485974dcc719539acaa65612e53c0633d687c14a93eb2fffc89c32c068
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **395.9 MB (395889008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:053444952bbb99335c24da95e60652c8bf13fdf4d34ca8258e433d137e2187b0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:22:46 GMT
ADD file:b4e182cbec02f1d3bb7c8ff0ef09924ac255ba6717bdd73f24d0a6114ff305d6 in / 
# Wed, 01 Nov 2023 00:22:49 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:31:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:32:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:35:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:46cca77d78176c861335b7b91e20d7b4cb2b3a75a124c300124de5818b724a9d`  
		Last Modified: Wed, 01 Nov 2023 00:27:59 GMT  
		Size: 53.4 MB (53438164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c27d7acaf849316ba11ccd36c024abe28c48180ca4ed48c1d645cdbac13d42`  
		Last Modified: Wed, 01 Nov 2023 01:42:56 GMT  
		Size: 26.0 MB (26000762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1f87f5498621b44bb593666a49a2167487d185ef2ba48d24ee657724f9e1b8`  
		Last Modified: Wed, 01 Nov 2023 01:43:17 GMT  
		Size: 70.9 MB (70933174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293d32682820b51e6038052ac32c5615a7e362a951c538e2e7dfcd2260f9bf08`  
		Last Modified: Wed, 01 Nov 2023 01:44:03 GMT  
		Size: 245.5 MB (245516908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:8cdef13f992928b7ced89bd24774f889b46a4ba3c167a501a32629523efafecb
```

-	Docker Version: 20.10.25
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.5 MB (422517112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d6a14901feb9be459b29b2ec05a91f16169520c614043d74824ef29f5ef68fc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:10:39 GMT
ADD file:10aac34e5379cbca42071631c10447895ece01063babea5769d7a1ca12c1d5e1 in / 
# Wed, 01 Nov 2023 01:10:41 GMT
CMD ["bash"]
# Fri, 10 Nov 2023 15:09:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 10 Nov 2023 15:11:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 10 Nov 2023 15:18:43 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8b987d803641183eb947c3e5f17a8a822be136b9081a3e13a881ea93c5b5c153`  
		Last Modified: Wed, 01 Nov 2023 01:13:28 GMT  
		Size: 47.9 MB (47903676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e686018657ba2f600a983c566c04aa87a7d470e15735c7687c3f08ad9fc14c6`  
		Last Modified: Fri, 10 Nov 2023 15:19:24 GMT  
		Size: 25.7 MB (25689738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e367241f870c7b27facfdeed51bb1705e06e838663a27ed4411063a890b5d9`  
		Last Modified: Fri, 10 Nov 2023 15:20:39 GMT  
		Size: 64.7 MB (64712965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7608d7ee7a6e227d7e1ffd0c22faa80adf546d9105155ee8e590b239746a8e`  
		Last Modified: Fri, 10 Nov 2023 15:26:16 GMT  
		Size: 284.2 MB (284210733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:94c1320e61a65661393d39cd613dad56ade7b9114794ea363c35cd1d98bf1472
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.1 MB (357129350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd53476e97fafeffd02c74a4b92a8131082486dfaf6e18124bce5faa8fe8ed79`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:44:04 GMT
ADD file:e94f75ffd7aa648bb85fefcceb02afa58747273f05e89c473c1ad438c3ba2345 in / 
# Wed, 01 Nov 2023 00:44:07 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:59:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:59:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:00:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:43e2d693d4cc2a3e58c2344ef771699434d5f0e6ffb98ac8bdb822ee0e2534fa`  
		Last Modified: Wed, 01 Nov 2023 00:49:25 GMT  
		Size: 49.0 MB (48966976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17216a40a3f2f28f99307df60faffa863e423de83464990e34dd5854b1206c45`  
		Last Modified: Wed, 01 Nov 2023 02:07:00 GMT  
		Size: 24.6 MB (24596949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa15755375f48461c5f3dcfc8b172b68b06d99c8b37bacff592046619c269ff5`  
		Last Modified: Wed, 01 Nov 2023 02:07:15 GMT  
		Size: 66.5 MB (66478150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee715cf843b2c30de31308613798cb1286cc46aace75a30b5454885808889c6a`  
		Last Modified: Wed, 01 Nov 2023 02:07:47 GMT  
		Size: 217.1 MB (217087275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:77c7980908342e34e20c6dded2d582be454afc3b1cacb6b3f51afcdafc207e75
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
$ docker pull buildpack-deps@sha256:55d3c9a086b1f3e2bf2efc43a3facd9259debb301bc36d744d399b9f9183baab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.9 MB (73888718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ca5ff02ac501d48c546df140a835f2ebdb2306a1a564dd635fc72f385dd9659`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:22:27 GMT
ADD file:69815228666696b3cd3b2799492e3d9cdf4f513ccca5c1cc9282f6c569cc8730 in / 
# Wed, 01 Nov 2023 00:22:28 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:57:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
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

### `buildpack-deps:sid-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:8fd71e79ed7adb4eabd5ab187c04681bd8d7225ad23f383b19e2983aafe7dca9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70208940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d62ceb7c735018d913dc495afa525a353cb6e5196e0df330873dac97ea2527f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:49:10 GMT
ADD file:3dfec265d80292cf14629bdbd49822be7a5672ab8299d43e9ec734f6e032c8df in / 
# Wed, 01 Nov 2023 00:49:10 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:59:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0609920749c8743a3627a0a7a377598014123518f5e0ed7f1443c78c8c9f3446`  
		Last Modified: Wed, 01 Nov 2023 00:53:10 GMT  
		Size: 47.2 MB (47192458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3b7ab88084f4d09eb30fe75dbc159cd99b0692cea6232d2f457c292a62968c`  
		Last Modified: Wed, 01 Nov 2023 03:07:10 GMT  
		Size: 23.0 MB (23016482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:51146f13fdb6437822863cfb091ce22dd810970f7bf2062d9a989c5b98b20ad3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67216176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:441627c1997be627df062cc68f9e0305629e418cd85ef184060f05d45e2ca94a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:59:14 GMT
ADD file:a72fe3de4b178dd8b7c48a1dc98d4c14520570e5edb66049dfe2cd6bb0a5dd6c in / 
# Wed, 01 Nov 2023 00:59:15 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:36:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f6e9a66eb905933433a5a2a8c16e480468f3731f107d5854bac12ef9a79bc271`  
		Last Modified: Wed, 01 Nov 2023 01:05:19 GMT  
		Size: 45.0 MB (44981409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c61548fabf75545be26d57a05800e5dbcd765a1c5c804a7671c92c59e15834d8`  
		Last Modified: Wed, 01 Nov 2023 02:44:58 GMT  
		Size: 22.2 MB (22234767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:37eb53a80fd102fcb5f14a4d0dc9bd7732ec1c734a422e4b427b175555c575a5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.5 MB (73469380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0be9b3ee789a657aea7026023fad3bfad1ddd7a5e725b324dd61f03508c0130d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:40:45 GMT
ADD file:1a4ef85bba464538c4f87a65a055d954fc8edc51f26efd06b43d8ae9f7e54f7a in / 
# Wed, 01 Nov 2023 00:40:46 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:09:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ba6956ade110f0fe56bbad19a8d10b1eb0ae1b1006ccba5fadff0026a00dbc20`  
		Last Modified: Wed, 01 Nov 2023 00:45:46 GMT  
		Size: 49.6 MB (49552835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516c292c0ab5612a524438779924b5cc187f530a208c71056c8b9994656ef043`  
		Last Modified: Wed, 01 Nov 2023 02:16:27 GMT  
		Size: 23.9 MB (23916545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8988d06749683ea585cf137051dfe9710e79a4dd694e684d3de84c6bf3757d32
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75702236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:830e36b2a276fddf3fa83594c87499d590059eb10e73ca22fcc5a827bbbda7c4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:40:31 GMT
ADD file:0aa90abbd80c68d937903de7ac8fdcce0f516fdd70f080b677af1e2322c000b9 in / 
# Wed, 01 Nov 2023 00:40:32 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 13:50:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:96660bac4658b1bffb27e96ac8ecc86753a1844f042ede32c4f1faef702dc202`  
		Last Modified: Wed, 01 Nov 2023 00:46:42 GMT  
		Size: 50.5 MB (50516486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7af088639fa61079db294f16f91145938a488365f2aec8cef7a85da80c4b13b`  
		Last Modified: Wed, 01 Nov 2023 13:59:54 GMT  
		Size: 25.2 MB (25185750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:3d072782b869915c68ce21a8a78370274e3aad0379c863c87bed0513c371bf28
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73236978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48d581d8a17daaf6df47819c5605bf4a8542057b4a50efa28345f4f2918775db`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:12:08 GMT
ADD file:e27a157c42d1aedcb0f6cf695f1f5c31d442488e049826c940509e2288537427 in / 
# Wed, 01 Nov 2023 01:12:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 21:35:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0eacf4d958160d2729e1bb31fbb12227afa7536ce6304928b13c2c65d297f9b9`  
		Last Modified: Wed, 01 Nov 2023 01:23:11 GMT  
		Size: 49.3 MB (49326735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76fea98d048b05ee3313ca45517a641b11637c7f8dc3ec543480fe6111a66fc0`  
		Last Modified: Wed, 01 Nov 2023 22:00:34 GMT  
		Size: 23.9 MB (23910243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:e3fe6632a18f418e4435cc7a8063378cec3d6e7e86eda522d299f55d99caeb06
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.4 MB (79438926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f3939720778f56545dbb5f838729141ef56732c086b66a0537faf6460e0937f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:22:46 GMT
ADD file:b4e182cbec02f1d3bb7c8ff0ef09924ac255ba6717bdd73f24d0a6114ff305d6 in / 
# Wed, 01 Nov 2023 00:22:49 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:31:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:46cca77d78176c861335b7b91e20d7b4cb2b3a75a124c300124de5818b724a9d`  
		Last Modified: Wed, 01 Nov 2023 00:27:59 GMT  
		Size: 53.4 MB (53438164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c27d7acaf849316ba11ccd36c024abe28c48180ca4ed48c1d645cdbac13d42`  
		Last Modified: Wed, 01 Nov 2023 01:42:56 GMT  
		Size: 26.0 MB (26000762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:7502e4d219b556bf0e1c723558e81fc25bec41051d62b6d01fe6ee8594649131
```

-	Docker Version: 20.10.25
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73593414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fed54f446cc8c45b1b49a470ff94f7e04623b8690749725aab0ecf7751eb268`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:10:39 GMT
ADD file:10aac34e5379cbca42071631c10447895ece01063babea5769d7a1ca12c1d5e1 in / 
# Wed, 01 Nov 2023 01:10:41 GMT
CMD ["bash"]
# Fri, 10 Nov 2023 15:09:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8b987d803641183eb947c3e5f17a8a822be136b9081a3e13a881ea93c5b5c153`  
		Last Modified: Wed, 01 Nov 2023 01:13:28 GMT  
		Size: 47.9 MB (47903676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e686018657ba2f600a983c566c04aa87a7d470e15735c7687c3f08ad9fc14c6`  
		Last Modified: Fri, 10 Nov 2023 15:19:24 GMT  
		Size: 25.7 MB (25689738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:c4b64ed3c6f7849da4bf232ee9b0346c8375234ae05e858fdaab19159c92be3b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73563925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fb6298a353936cc00a02214b0172e7ebcb8439494257afc18435c9ae46f6ac3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:44:04 GMT
ADD file:e94f75ffd7aa648bb85fefcceb02afa58747273f05e89c473c1ad438c3ba2345 in / 
# Wed, 01 Nov 2023 00:44:07 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:59:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:43e2d693d4cc2a3e58c2344ef771699434d5f0e6ffb98ac8bdb822ee0e2534fa`  
		Last Modified: Wed, 01 Nov 2023 00:49:25 GMT  
		Size: 49.0 MB (48966976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17216a40a3f2f28f99307df60faffa863e423de83464990e34dd5854b1206c45`  
		Last Modified: Wed, 01 Nov 2023 02:07:00 GMT  
		Size: 24.6 MB (24596949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:sid-scm`

```console
$ docker pull buildpack-deps@sha256:7b4a1e2323631a5a20efc067593b78128e3cc6c7793ca6d8029761e4a5971ff5
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
$ docker pull buildpack-deps@sha256:69b4c504c9caa677158b04a5dffa59425c7649f735a7b8728d6537f55e5bbf1b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.4 MB (139405504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ea95fd684a079be0c5deeb96861c07b4992a71e7818a9c7960f6a1baee07c8f`
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

### `buildpack-deps:sid-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:9417cb6ff8564c4d3bf1b82efb889976197dc0cb69f9ef179d844ff4c5a47a07
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.2 MB (133219295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:791053f347823ad45507927ca12fc46992f6485bb6ded865460b387df1861d71`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:49:10 GMT
ADD file:3dfec265d80292cf14629bdbd49822be7a5672ab8299d43e9ec734f6e032c8df in / 
# Wed, 01 Nov 2023 00:49:10 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:59:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 03:00:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0609920749c8743a3627a0a7a377598014123518f5e0ed7f1443c78c8c9f3446`  
		Last Modified: Wed, 01 Nov 2023 00:53:10 GMT  
		Size: 47.2 MB (47192458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3b7ab88084f4d09eb30fe75dbc159cd99b0692cea6232d2f457c292a62968c`  
		Last Modified: Wed, 01 Nov 2023 03:07:10 GMT  
		Size: 23.0 MB (23016482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3ff5e12103a446acf43b661291fc30a67ca5851b7c1f67906ac39a5a609ef1c`  
		Last Modified: Wed, 01 Nov 2023 03:07:30 GMT  
		Size: 63.0 MB (63010355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:dd781c833a3b0edcfcd2d86a091e60c74feac13e09a04d42ecf30ed1992d57c3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127826362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82080f96e7a0b68c7bc49369001f13514e2d0bb7da42e22f391c832020ee4beb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:59:14 GMT
ADD file:a72fe3de4b178dd8b7c48a1dc98d4c14520570e5edb66049dfe2cd6bb0a5dd6c in / 
# Wed, 01 Nov 2023 00:59:15 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:36:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:36:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f6e9a66eb905933433a5a2a8c16e480468f3731f107d5854bac12ef9a79bc271`  
		Last Modified: Wed, 01 Nov 2023 01:05:19 GMT  
		Size: 45.0 MB (44981409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c61548fabf75545be26d57a05800e5dbcd765a1c5c804a7671c92c59e15834d8`  
		Last Modified: Wed, 01 Nov 2023 02:44:58 GMT  
		Size: 22.2 MB (22234767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa95d6d6902734ac1af894edaf67096b114b4935d12a40bf35b44bca0f33e21`  
		Last Modified: Wed, 01 Nov 2023 02:45:16 GMT  
		Size: 60.6 MB (60610186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:24a9674f7ee955af54b2ff9dff74e3a3a5ab908c092ef87046b36185bba90552
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.1 MB (139074611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49432ff4faca7e8f8e7e1c0674996ca4a6b2a93bdec8b6cf4059353c81e1a6eb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:40:45 GMT
ADD file:1a4ef85bba464538c4f87a65a055d954fc8edc51f26efd06b43d8ae9f7e54f7a in / 
# Wed, 01 Nov 2023 00:40:46 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:09:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:09:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ba6956ade110f0fe56bbad19a8d10b1eb0ae1b1006ccba5fadff0026a00dbc20`  
		Last Modified: Wed, 01 Nov 2023 00:45:46 GMT  
		Size: 49.6 MB (49552835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516c292c0ab5612a524438779924b5cc187f530a208c71056c8b9994656ef043`  
		Last Modified: Wed, 01 Nov 2023 02:16:27 GMT  
		Size: 23.9 MB (23916545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8977dd4a34d5416619317940446894bcaf8bc0c5f832e562683f4aa703db7f`  
		Last Modified: Wed, 01 Nov 2023 02:16:44 GMT  
		Size: 65.6 MB (65605231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:bf9e365b381337f4d6b2f5562e4a5c66f62d51e107a697e2abc16c6cf3807722
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.0 MB (142969483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:890f7be8650dfbec3174b0c555ee6f84c9085c83f218e591ccd4bcd9822ca9fd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:40:31 GMT
ADD file:0aa90abbd80c68d937903de7ac8fdcce0f516fdd70f080b677af1e2322c000b9 in / 
# Wed, 01 Nov 2023 00:40:32 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 13:50:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:51:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:96660bac4658b1bffb27e96ac8ecc86753a1844f042ede32c4f1faef702dc202`  
		Last Modified: Wed, 01 Nov 2023 00:46:42 GMT  
		Size: 50.5 MB (50516486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7af088639fa61079db294f16f91145938a488365f2aec8cef7a85da80c4b13b`  
		Last Modified: Wed, 01 Nov 2023 13:59:54 GMT  
		Size: 25.2 MB (25185750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34a1138df818473932216f10a656452bbeead89efc81870811003208908e138`  
		Last Modified: Wed, 01 Nov 2023 14:00:17 GMT  
		Size: 67.3 MB (67267247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:be68bbc454236b68329461f9d169e194956bde9a85d831f12f67ffc86823332b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.6 MB (137560466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8009d8ed04a6125b5b9fefa3fad72e3a2ffe0dc6f0abd9e503ca667526d713c5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:12:08 GMT
ADD file:e27a157c42d1aedcb0f6cf695f1f5c31d442488e049826c940509e2288537427 in / 
# Wed, 01 Nov 2023 01:12:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 21:35:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 21:36:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0eacf4d958160d2729e1bb31fbb12227afa7536ce6304928b13c2c65d297f9b9`  
		Last Modified: Wed, 01 Nov 2023 01:23:11 GMT  
		Size: 49.3 MB (49326735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76fea98d048b05ee3313ca45517a641b11637c7f8dc3ec543480fe6111a66fc0`  
		Last Modified: Wed, 01 Nov 2023 22:00:34 GMT  
		Size: 23.9 MB (23910243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde7d59b79a44cf2fd6509592cd5ffa2ac26dd4a37fb70dbe72408010c4a2926`  
		Last Modified: Wed, 01 Nov 2023 22:01:27 GMT  
		Size: 64.3 MB (64323488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:353b2a9b54d029503ae0b036b97d823535850f152a54820f9faeb5adba83eb89
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.4 MB (150372100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b8e3c9ad7f10aec351582b84c48d9a4a2a4b8b4496b3fc285248982f5238995`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:22:46 GMT
ADD file:b4e182cbec02f1d3bb7c8ff0ef09924ac255ba6717bdd73f24d0a6114ff305d6 in / 
# Wed, 01 Nov 2023 00:22:49 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:31:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:32:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:46cca77d78176c861335b7b91e20d7b4cb2b3a75a124c300124de5818b724a9d`  
		Last Modified: Wed, 01 Nov 2023 00:27:59 GMT  
		Size: 53.4 MB (53438164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c27d7acaf849316ba11ccd36c024abe28c48180ca4ed48c1d645cdbac13d42`  
		Last Modified: Wed, 01 Nov 2023 01:42:56 GMT  
		Size: 26.0 MB (26000762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1f87f5498621b44bb593666a49a2167487d185ef2ba48d24ee657724f9e1b8`  
		Last Modified: Wed, 01 Nov 2023 01:43:17 GMT  
		Size: 70.9 MB (70933174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:d98851f479f5b91644eea439930f9a94b4da22e3c4d133aed85216a103b3e873
```

-	Docker Version: 20.10.25
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.3 MB (138306379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a556e968fe99b77f67556941b078d49fa94ba4ac7ebab95aa19b50fd184956fd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:10:39 GMT
ADD file:10aac34e5379cbca42071631c10447895ece01063babea5769d7a1ca12c1d5e1 in / 
# Wed, 01 Nov 2023 01:10:41 GMT
CMD ["bash"]
# Fri, 10 Nov 2023 15:09:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 10 Nov 2023 15:11:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8b987d803641183eb947c3e5f17a8a822be136b9081a3e13a881ea93c5b5c153`  
		Last Modified: Wed, 01 Nov 2023 01:13:28 GMT  
		Size: 47.9 MB (47903676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e686018657ba2f600a983c566c04aa87a7d470e15735c7687c3f08ad9fc14c6`  
		Last Modified: Fri, 10 Nov 2023 15:19:24 GMT  
		Size: 25.7 MB (25689738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e367241f870c7b27facfdeed51bb1705e06e838663a27ed4411063a890b5d9`  
		Last Modified: Fri, 10 Nov 2023 15:20:39 GMT  
		Size: 64.7 MB (64712965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:0c3580029357b03dab5202367b9675aa78ae0db89b391735b34327fa0aad12e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.0 MB (140042075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b4c6469d28f8ab0416e1b296a12c5545babdafd6352d9d73e5fab9096a5c5d5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:44:04 GMT
ADD file:e94f75ffd7aa648bb85fefcceb02afa58747273f05e89c473c1ad438c3ba2345 in / 
# Wed, 01 Nov 2023 00:44:07 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:59:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:59:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:43e2d693d4cc2a3e58c2344ef771699434d5f0e6ffb98ac8bdb822ee0e2534fa`  
		Last Modified: Wed, 01 Nov 2023 00:49:25 GMT  
		Size: 49.0 MB (48966976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17216a40a3f2f28f99307df60faffa863e423de83464990e34dd5854b1206c45`  
		Last Modified: Wed, 01 Nov 2023 02:07:00 GMT  
		Size: 24.6 MB (24596949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa15755375f48461c5f3dcfc8b172b68b06d99c8b37bacff592046619c269ff5`  
		Last Modified: Wed, 01 Nov 2023 02:07:15 GMT  
		Size: 66.5 MB (66478150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stable`

```console
$ docker pull buildpack-deps@sha256:8465175ca53f8f2e756d069658b3f353bb3732926b1f33f34332cfbf597ad0c0
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
$ docker pull buildpack-deps@sha256:c281372d752c50bd925a7ef863ad65222d68d37028b97ae6378f38fe3ead7b15
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.8 MB (348825839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6672223876e40fadb1dac262c5e01bdaefbffd0107862c58d80b4df910d55414`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:37 GMT
ADD file:3e9b6405f11dd24ce62105c033f1d8b931d9409298553f63b03af1b6dd1dda35 in / 
# Wed, 01 Nov 2023 00:20:38 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:52:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 00:52:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 00:53:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8457fd5474e70835e4482983a5662355d892d5f6f0f90a27a8e9f009997e8196`  
		Last Modified: Wed, 01 Nov 2023 00:25:05 GMT  
		Size: 49.6 MB (49582024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13baa2029dde87a21b87127168a0fb50a007c07da6b5adc8864e1fe1376c86ff`  
		Last Modified: Wed, 01 Nov 2023 01:02:01 GMT  
		Size: 24.0 MB (24049147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:325c5bf4c2f26c11380501bec4b6eef8a3ea35b554aa1b222cbcd1e1fe11ae1d`  
		Last Modified: Wed, 01 Nov 2023 01:02:20 GMT  
		Size: 64.1 MB (64130415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e18a660069fd7f87a7a6c49ddb701449bfb929c066811777601d36916c7f674`  
		Last Modified: Wed, 01 Nov 2023 01:02:55 GMT  
		Size: 211.1 MB (211064253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:f8310b73e4ca74a8a62aa3a60614bce0092e656117d95d96abf6efa958f10f39
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.0 MB (316028995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1bbae5789c5511aa21a7f8cac7ff0966d933f3cba2914e0630044c3d3d9a171`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:48:23 GMT
ADD file:963e26decfc65419428098047df29dcbf7865e13bcdd67abeb9849f99a7815e7 in / 
# Wed, 01 Nov 2023 00:48:23 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:56:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:53c5547a993a8adb09a632a8ae34fbc336b27a456c6b3a670865cd8bedb5e6a9`  
		Last Modified: Wed, 01 Nov 2023 00:51:04 GMT  
		Size: 47.4 MB (47355649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752979e12aac8f84972cea68e4f8d9bb1b645e71b3fc64047af1ba792dd338d9`  
		Last Modified: Wed, 01 Nov 2023 03:04:53 GMT  
		Size: 22.7 MB (22727584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bad2403917aecfddc5d239a343aacd942aeb9c9e6d76c027cfdbb0d5479bcaa`  
		Last Modified: Wed, 01 Nov 2023 03:05:15 GMT  
		Size: 61.6 MB (61561816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f0dda98bbf4b74a7919e20bcc31a0ecda8fd013c63ef827f0316369707e6af`  
		Last Modified: Wed, 01 Nov 2023 03:05:53 GMT  
		Size: 184.4 MB (184383946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1d6a60f9f2f559b189af01218c17dcda727d852c6c6d4a004b3a18dffdba281b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.4 MB (301446629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:576fdf6667f95f602d6807ecabd5c0e4f0643440a9c83b60e388dc8614f59f15`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:57:42 GMT
ADD file:3b2b4eda35d794b39d6b5567e81651625af51da3deb3f63b3ffdffa07720646e in / 
# Wed, 01 Nov 2023 00:57:42 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:30:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:30:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:31:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9bf855396a6f46c1cbac4e188af10f2c38474f989707b0b1b406b48c4b7284ef`  
		Last Modified: Wed, 01 Nov 2023 01:01:41 GMT  
		Size: 45.2 MB (45179410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6e59eca644b227cb755978679a3031e7b3f9a5c707057c293f2ba8732d8ef2`  
		Last Modified: Wed, 01 Nov 2023 02:41:40 GMT  
		Size: 22.0 MB (21951880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aefa016475f9e4925fd893a9d8cfcf375937aa4e637d337806176426509dfcd`  
		Last Modified: Wed, 01 Nov 2023 02:42:04 GMT  
		Size: 59.3 MB (59266468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d2c477968e94d61a34b16e774d58519d5e26175f92fbd0dfb90938103fab68`  
		Last Modified: Wed, 01 Nov 2023 02:42:47 GMT  
		Size: 175.0 MB (175048871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a8b07b41b675910dbc20eaf720c7716422cb5d1f0ddac9fbbdf56f6211f2a34e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.6 MB (339641684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08254bfa9a67c2c123e58e5c10e5e73f9c4aa1eee30e14a41e6c78b513d6e36d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:32 GMT
ADD file:c934ceb4c53a1cce6779198f1ea73d5c8aad9a035e750b343d49826120ecd0eb in / 
# Wed, 01 Nov 2023 00:39:33 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:04:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:04:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:05:48 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8024d4fb53b2455f66d49b7ee72eb3cad5074043578238b796a9879955946a88`  
		Last Modified: Wed, 01 Nov 2023 00:42:44 GMT  
		Size: 49.6 MB (49612653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d826ee8aa65e56e167f0e27fa65cfc065687a7ac6c360787d5940d8b51f0cf1`  
		Last Modified: Wed, 01 Nov 2023 02:13:39 GMT  
		Size: 23.6 MB (23584896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198068495d09b6865e75ce28d5d5d5de39897b8325ada63ba80eca884ad5666b`  
		Last Modified: Wed, 01 Nov 2023 02:13:57 GMT  
		Size: 64.0 MB (63994018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509db9a897ae5a94cad05bcf48605637fbf3f79733e8bf8c317b6babe3de1dbd`  
		Last Modified: Wed, 01 Nov 2023 02:14:29 GMT  
		Size: 202.5 MB (202450117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:06f4072db6e5dfbd8c8a3f60ac4b15f0852ba0216c33198a58e8da312fb8beda
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.5 MB (351464296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa96e3b9058ae71c8b65439bf05b32b30c99e3b7b9e4f07e1692eefc747c08c8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:38:46 GMT
ADD file:4043d711d8d7d1a995aed0a6998c96230765f55d4449167107955fe4af2a31db in / 
# Wed, 01 Nov 2023 00:38:47 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 13:44:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:44:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:45:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be8d77e28ff21732ba73253b6226e47e4e07ec2cedc803ffd62148df5d7a165b`  
		Last Modified: Wed, 01 Nov 2023 00:43:00 GMT  
		Size: 50.6 MB (50600049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cef920c8d790c11b84fa21c2204cca8ac6a84ec43e4a60bca3670e828748583`  
		Last Modified: Wed, 01 Nov 2023 13:55:45 GMT  
		Size: 24.9 MB (24885575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fee1ec8688f07e43b49247f3490035da93288449034600daee26c8ce0150a8c`  
		Last Modified: Wed, 01 Nov 2023 13:56:13 GMT  
		Size: 66.0 MB (65984300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6a893690e210e75c1236dc74079509b9f860409954240df3b2276364c416f8`  
		Last Modified: Wed, 01 Nov 2023 13:57:04 GMT  
		Size: 210.0 MB (209994372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:34b5b299169edc7c1281954a26f710d3d5d9c2101b510ae89ba1ca136df9b03c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.6 MB (325622171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0dc2b58709b67c5f83e2571566693513ad91a3ec9cd7626f14d8e210d8f7925`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:08:17 GMT
ADD file:b181441dc28bc6879e29cd086c569c653171c681525c124ffb6277bd71732bb1 in / 
# Wed, 01 Nov 2023 01:08:24 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 21:17:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 21:19:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 21:25:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0bfbf01892d22dd14fb9536e8675cc932ff41f415a415fbf8c6199106b01240d`  
		Last Modified: Wed, 01 Nov 2023 01:19:01 GMT  
		Size: 49.6 MB (49568811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9310598b7549f388c445368ea2a0a4077c57ddd45436efddb37e089d293f87fe`  
		Last Modified: Wed, 01 Nov 2023 21:53:41 GMT  
		Size: 23.4 MB (23438019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af2206444fab218d319700cbfcd93423bf4622bb8085adee11b684b7d3fd245`  
		Last Modified: Wed, 01 Nov 2023 21:54:35 GMT  
		Size: 63.0 MB (62962363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41601926009dec498023c4d0a7e1c4877fc9fe8372d6497206d1de026aeb215d`  
		Last Modified: Wed, 01 Nov 2023 21:57:00 GMT  
		Size: 189.7 MB (189652978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:0cd2296657f87dc9875b44afde1718960b7c982dea8b3128a2c2e9f0ad987be2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **363.0 MB (362952137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96ec2f6ad64fe7094e57094fb3436d0709d2e3f0d3a1ec0f6ed4cc91ef594b34`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:25 GMT
ADD file:31b995b44eb1f532fd265be3fc0c3d3b55e28db0911c86a06c83de621418db94 in / 
# Wed, 01 Nov 2023 00:21:28 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:24:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:24:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:27:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:071872f8f8cb44e883168d06195f8fbb330e259b415d1ab108c27bda84d6c060`  
		Last Modified: Wed, 01 Nov 2023 00:25:41 GMT  
		Size: 53.6 MB (53575361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9986fe7e71120fd78fcaad86d3a1d827f54f56f266364834bcb7c13eccf9ca0`  
		Last Modified: Wed, 01 Nov 2023 01:40:25 GMT  
		Size: 25.7 MB (25698676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7316c6cea433a21258a8af8686d8a74e964c21c6c563afd63f274e9346f8f7`  
		Last Modified: Wed, 01 Nov 2023 01:40:48 GMT  
		Size: 69.6 MB (69584512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d43d4f467d09dbebbdbbe77e08bdef659a411541528d2d0542c5a201a1e3953`  
		Last Modified: Wed, 01 Nov 2023 01:41:31 GMT  
		Size: 214.1 MB (214093588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:2592737d5c14c9cd628b8b622a4a8d02a213a6b6a91a832feb16b338c44c95ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.2 MB (318220170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97ece825d20df85062f7e8dc9e143e2cd80da86d6928f1260cee829c756fa6c9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:42:15 GMT
ADD file:6d8ee60b2fe4604969d8feeeb7e0dc8b9619a778d1a905c8bfdde5ede5e1eb54 in / 
# Wed, 01 Nov 2023 00:42:19 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:54:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:55:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:56:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bca95e393f709ba301b35c2439a815fd4fe8134d7a466bd528563bc32fd754d8`  
		Last Modified: Wed, 01 Nov 2023 00:47:43 GMT  
		Size: 47.9 MB (47943171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e744d1ef2c8405f6352136656080d7e244e1a97362c21069b734a55b86c8d0a`  
		Last Modified: Wed, 01 Nov 2023 02:05:09 GMT  
		Size: 24.0 MB (24045096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de40af46a5373d0a49892fa9000736be09090b477719517fcec84887d847f94b`  
		Last Modified: Wed, 01 Nov 2023 02:05:25 GMT  
		Size: 63.1 MB (63132485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5d582ecd4430347fbaa4df40283ca084e7bf9c17c0ce600484712c9f61dbe3`  
		Last Modified: Wed, 01 Nov 2023 02:05:57 GMT  
		Size: 183.1 MB (183099418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stable-curl`

```console
$ docker pull buildpack-deps@sha256:57892e6ad71a863f2ac7fb2bb00901d96d41a257e1ef9d10c44639f1dc795ab3
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
$ docker pull buildpack-deps@sha256:81138c0eec1922d626830b19f73fea9792c263880367cde9b37fc4c021aec989
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73631171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7937fdd23222e4c8dcf166fc96dcc583d6d66bb47ac9af8d666d0e1bbace30d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:37 GMT
ADD file:3e9b6405f11dd24ce62105c033f1d8b931d9409298553f63b03af1b6dd1dda35 in / 
# Wed, 01 Nov 2023 00:20:38 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:52:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8457fd5474e70835e4482983a5662355d892d5f6f0f90a27a8e9f009997e8196`  
		Last Modified: Wed, 01 Nov 2023 00:25:05 GMT  
		Size: 49.6 MB (49582024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13baa2029dde87a21b87127168a0fb50a007c07da6b5adc8864e1fe1376c86ff`  
		Last Modified: Wed, 01 Nov 2023 01:02:01 GMT  
		Size: 24.0 MB (24049147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:ed09164fc4880f94c58fa72329b74e2deb0e9c4c49c4c89bbd311dfbec5a7108
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.1 MB (70083233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:992836c8887553b50c3a23f1fe3a3755bcd7acd42fce7ad4b6ad8137282b3ebb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:48:23 GMT
ADD file:963e26decfc65419428098047df29dcbf7865e13bcdd67abeb9849f99a7815e7 in / 
# Wed, 01 Nov 2023 00:48:23 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:53c5547a993a8adb09a632a8ae34fbc336b27a456c6b3a670865cd8bedb5e6a9`  
		Last Modified: Wed, 01 Nov 2023 00:51:04 GMT  
		Size: 47.4 MB (47355649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752979e12aac8f84972cea68e4f8d9bb1b645e71b3fc64047af1ba792dd338d9`  
		Last Modified: Wed, 01 Nov 2023 03:04:53 GMT  
		Size: 22.7 MB (22727584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1171fe398f6788003f5bacbadd2a89ea2013fff55c0f14da9e106bbcbe024a7a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67131290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a88861f4a437ff5c87eec39e153ae95413a03c4172c7e8751b0cc2825002d218`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:57:42 GMT
ADD file:3b2b4eda35d794b39d6b5567e81651625af51da3deb3f63b3ffdffa07720646e in / 
# Wed, 01 Nov 2023 00:57:42 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:30:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9bf855396a6f46c1cbac4e188af10f2c38474f989707b0b1b406b48c4b7284ef`  
		Last Modified: Wed, 01 Nov 2023 01:01:41 GMT  
		Size: 45.2 MB (45179410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6e59eca644b227cb755978679a3031e7b3f9a5c707057c293f2ba8732d8ef2`  
		Last Modified: Wed, 01 Nov 2023 02:41:40 GMT  
		Size: 22.0 MB (21951880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f82a3141ca386a79076c0ba0418c8782a361c8bb51e75deaa8866db1b2bed5ea
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73197549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a409f55570736a6c820237e1f60fad4f8bb18dfc77870b144516ef2fe8e2ff11`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:32 GMT
ADD file:c934ceb4c53a1cce6779198f1ea73d5c8aad9a035e750b343d49826120ecd0eb in / 
# Wed, 01 Nov 2023 00:39:33 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:04:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8024d4fb53b2455f66d49b7ee72eb3cad5074043578238b796a9879955946a88`  
		Last Modified: Wed, 01 Nov 2023 00:42:44 GMT  
		Size: 49.6 MB (49612653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d826ee8aa65e56e167f0e27fa65cfc065687a7ac6c360787d5940d8b51f0cf1`  
		Last Modified: Wed, 01 Nov 2023 02:13:39 GMT  
		Size: 23.6 MB (23584896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:e583e18e995680fcec2033ed1ec977f42c6a379c165cc1770dc0ccef1f48ab1e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.5 MB (75485624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05e2aefc926d6cb666936937674be7f6a97c7ed0b53b7f469e95897450b1e705`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:38:46 GMT
ADD file:4043d711d8d7d1a995aed0a6998c96230765f55d4449167107955fe4af2a31db in / 
# Wed, 01 Nov 2023 00:38:47 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 13:44:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be8d77e28ff21732ba73253b6226e47e4e07ec2cedc803ffd62148df5d7a165b`  
		Last Modified: Wed, 01 Nov 2023 00:43:00 GMT  
		Size: 50.6 MB (50600049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cef920c8d790c11b84fa21c2204cca8ac6a84ec43e4a60bca3670e828748583`  
		Last Modified: Wed, 01 Nov 2023 13:55:45 GMT  
		Size: 24.9 MB (24885575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:c86473381513b077b2b848a187217476731ef8648b6efa00e40b3b540d28c8cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.0 MB (73006830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5305c7a9d52eb2df81294cd30b305c75ce3a58c6c2f14ffd4fc4015d09853ad9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:08:17 GMT
ADD file:b181441dc28bc6879e29cd086c569c653171c681525c124ffb6277bd71732bb1 in / 
# Wed, 01 Nov 2023 01:08:24 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 21:17:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0bfbf01892d22dd14fb9536e8675cc932ff41f415a415fbf8c6199106b01240d`  
		Last Modified: Wed, 01 Nov 2023 01:19:01 GMT  
		Size: 49.6 MB (49568811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9310598b7549f388c445368ea2a0a4077c57ddd45436efddb37e089d293f87fe`  
		Last Modified: Wed, 01 Nov 2023 21:53:41 GMT  
		Size: 23.4 MB (23438019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:8fef9d5a3be088dbbfed19de3a7a624448239421641b6dba8621c6400edd7f06
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.3 MB (79274037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39d499c3ba7b3bc05ab676e65cd1d1351b56d80a02752dfd5053677641ce5b37`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:25 GMT
ADD file:31b995b44eb1f532fd265be3fc0c3d3b55e28db0911c86a06c83de621418db94 in / 
# Wed, 01 Nov 2023 00:21:28 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:24:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:071872f8f8cb44e883168d06195f8fbb330e259b415d1ab108c27bda84d6c060`  
		Last Modified: Wed, 01 Nov 2023 00:25:41 GMT  
		Size: 53.6 MB (53575361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9986fe7e71120fd78fcaad86d3a1d827f54f56f266364834bcb7c13eccf9ca0`  
		Last Modified: Wed, 01 Nov 2023 01:40:25 GMT  
		Size: 25.7 MB (25698676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:5f7c17a38a04a8eccaa364dd9860f483d4d838929e9817e888412ab607f0ebe1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.0 MB (71988267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:098bd7234fbac6dbe5ad9b2b1184781e15d3c49ddbd180c6247dff18efda87f8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:42:15 GMT
ADD file:6d8ee60b2fe4604969d8feeeb7e0dc8b9619a778d1a905c8bfdde5ede5e1eb54 in / 
# Wed, 01 Nov 2023 00:42:19 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:54:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bca95e393f709ba301b35c2439a815fd4fe8134d7a466bd528563bc32fd754d8`  
		Last Modified: Wed, 01 Nov 2023 00:47:43 GMT  
		Size: 47.9 MB (47943171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e744d1ef2c8405f6352136656080d7e244e1a97362c21069b734a55b86c8d0a`  
		Last Modified: Wed, 01 Nov 2023 02:05:09 GMT  
		Size: 24.0 MB (24045096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stable-scm`

```console
$ docker pull buildpack-deps@sha256:c128f8e680e8bfc06477d452a567975cc58188cddefc68cec3c72c1d8a15a4b2
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
$ docker pull buildpack-deps@sha256:93590f9f25a12437d9d01f7ac4309b83af5532680e36bbc01181f61e19ae7135
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.8 MB (137761586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:941f9c887621d4fee5936ccc92b35b887f74ed81aac7b90fcedc1fcb5d65741b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:37 GMT
ADD file:3e9b6405f11dd24ce62105c033f1d8b931d9409298553f63b03af1b6dd1dda35 in / 
# Wed, 01 Nov 2023 00:20:38 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:52:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 00:52:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8457fd5474e70835e4482983a5662355d892d5f6f0f90a27a8e9f009997e8196`  
		Last Modified: Wed, 01 Nov 2023 00:25:05 GMT  
		Size: 49.6 MB (49582024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13baa2029dde87a21b87127168a0fb50a007c07da6b5adc8864e1fe1376c86ff`  
		Last Modified: Wed, 01 Nov 2023 01:02:01 GMT  
		Size: 24.0 MB (24049147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:325c5bf4c2f26c11380501bec4b6eef8a3ea35b554aa1b222cbcd1e1fe11ae1d`  
		Last Modified: Wed, 01 Nov 2023 01:02:20 GMT  
		Size: 64.1 MB (64130415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:9a1d134fc9b0926e5316223c1622334e19ab18d8c110ded139188fe219084032
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.6 MB (131645049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58e29752e0aab3ef315e59c15de2796ae467eea85f7d51848bbd963d7cdcf627`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:48:23 GMT
ADD file:963e26decfc65419428098047df29dcbf7865e13bcdd67abeb9849f99a7815e7 in / 
# Wed, 01 Nov 2023 00:48:23 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:54:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:55:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:53c5547a993a8adb09a632a8ae34fbc336b27a456c6b3a670865cd8bedb5e6a9`  
		Last Modified: Wed, 01 Nov 2023 00:51:04 GMT  
		Size: 47.4 MB (47355649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752979e12aac8f84972cea68e4f8d9bb1b645e71b3fc64047af1ba792dd338d9`  
		Last Modified: Wed, 01 Nov 2023 03:04:53 GMT  
		Size: 22.7 MB (22727584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bad2403917aecfddc5d239a343aacd942aeb9c9e6d76c027cfdbb0d5479bcaa`  
		Last Modified: Wed, 01 Nov 2023 03:05:15 GMT  
		Size: 61.6 MB (61561816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:d0accba6d4ea1e12f6ab955a70a96005bac84d284fa4ca006ed0a4b165b38db4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.4 MB (126397758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8322db01431af3b3bc3e5d7ca0be48f5ea14663ef8678973003e7aef9e95fbc3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:57:42 GMT
ADD file:3b2b4eda35d794b39d6b5567e81651625af51da3deb3f63b3ffdffa07720646e in / 
# Wed, 01 Nov 2023 00:57:42 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:30:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:30:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9bf855396a6f46c1cbac4e188af10f2c38474f989707b0b1b406b48c4b7284ef`  
		Last Modified: Wed, 01 Nov 2023 01:01:41 GMT  
		Size: 45.2 MB (45179410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6e59eca644b227cb755978679a3031e7b3f9a5c707057c293f2ba8732d8ef2`  
		Last Modified: Wed, 01 Nov 2023 02:41:40 GMT  
		Size: 22.0 MB (21951880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aefa016475f9e4925fd893a9d8cfcf375937aa4e637d337806176426509dfcd`  
		Last Modified: Wed, 01 Nov 2023 02:42:04 GMT  
		Size: 59.3 MB (59266468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3cec78f7e6894f6dd48b42e66476bad2daa2533d5b6d12b2cb243c765752e854
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.2 MB (137191567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d91cf57cfc88561be3a3af9dc95f31e6740e086c0a3db3dc1bd42da9ef6313ce`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:32 GMT
ADD file:c934ceb4c53a1cce6779198f1ea73d5c8aad9a035e750b343d49826120ecd0eb in / 
# Wed, 01 Nov 2023 00:39:33 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:04:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:04:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8024d4fb53b2455f66d49b7ee72eb3cad5074043578238b796a9879955946a88`  
		Last Modified: Wed, 01 Nov 2023 00:42:44 GMT  
		Size: 49.6 MB (49612653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d826ee8aa65e56e167f0e27fa65cfc065687a7ac6c360787d5940d8b51f0cf1`  
		Last Modified: Wed, 01 Nov 2023 02:13:39 GMT  
		Size: 23.6 MB (23584896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198068495d09b6865e75ce28d5d5d5de39897b8325ada63ba80eca884ad5666b`  
		Last Modified: Wed, 01 Nov 2023 02:13:57 GMT  
		Size: 64.0 MB (63994018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:4904b1a13827dfb9dc0294607ef88a92eb6d9fb5af266f3b436b6e747de5bbc9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.5 MB (141469924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c9c6e32dc86d819a813b06b60a98e41499c7cc87049b7acf4e87c5b4c52cb05`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:38:46 GMT
ADD file:4043d711d8d7d1a995aed0a6998c96230765f55d4449167107955fe4af2a31db in / 
# Wed, 01 Nov 2023 00:38:47 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 13:44:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:44:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be8d77e28ff21732ba73253b6226e47e4e07ec2cedc803ffd62148df5d7a165b`  
		Last Modified: Wed, 01 Nov 2023 00:43:00 GMT  
		Size: 50.6 MB (50600049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cef920c8d790c11b84fa21c2204cca8ac6a84ec43e4a60bca3670e828748583`  
		Last Modified: Wed, 01 Nov 2023 13:55:45 GMT  
		Size: 24.9 MB (24885575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fee1ec8688f07e43b49247f3490035da93288449034600daee26c8ce0150a8c`  
		Last Modified: Wed, 01 Nov 2023 13:56:13 GMT  
		Size: 66.0 MB (65984300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:7512d5d9e16a66d343238bf97e5b6d176e537b37e99b90b662154d61c082523b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.0 MB (135969193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ddc1f3c73e907d5ace49797cc746b10a794acc32d29af85c665e901745196ea`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:08:17 GMT
ADD file:b181441dc28bc6879e29cd086c569c653171c681525c124ffb6277bd71732bb1 in / 
# Wed, 01 Nov 2023 01:08:24 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 21:17:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 21:19:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0bfbf01892d22dd14fb9536e8675cc932ff41f415a415fbf8c6199106b01240d`  
		Last Modified: Wed, 01 Nov 2023 01:19:01 GMT  
		Size: 49.6 MB (49568811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9310598b7549f388c445368ea2a0a4077c57ddd45436efddb37e089d293f87fe`  
		Last Modified: Wed, 01 Nov 2023 21:53:41 GMT  
		Size: 23.4 MB (23438019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af2206444fab218d319700cbfcd93423bf4622bb8085adee11b684b7d3fd245`  
		Last Modified: Wed, 01 Nov 2023 21:54:35 GMT  
		Size: 63.0 MB (62962363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:e720e0531751cf77d1933f62e84bc5d4d2d63c0da3d890797548ca4e0192e571
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.9 MB (148858549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffb46a21911fb664a3630a45e7195ee955092521b2066322ec031cd4dd405ff3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:21:25 GMT
ADD file:31b995b44eb1f532fd265be3fc0c3d3b55e28db0911c86a06c83de621418db94 in / 
# Wed, 01 Nov 2023 00:21:28 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:24:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:24:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:071872f8f8cb44e883168d06195f8fbb330e259b415d1ab108c27bda84d6c060`  
		Last Modified: Wed, 01 Nov 2023 00:25:41 GMT  
		Size: 53.6 MB (53575361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9986fe7e71120fd78fcaad86d3a1d827f54f56f266364834bcb7c13eccf9ca0`  
		Last Modified: Wed, 01 Nov 2023 01:40:25 GMT  
		Size: 25.7 MB (25698676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7316c6cea433a21258a8af8686d8a74e964c21c6c563afd63f274e9346f8f7`  
		Last Modified: Wed, 01 Nov 2023 01:40:48 GMT  
		Size: 69.6 MB (69584512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:09520ba698b0b094ea1454bc687588fec9372d55e89e0b94e6afd1a415c1466f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.1 MB (135120752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e276550e9f3dc4f49a7d31441193c04d44abfc4220d18845eec66bdbbb473977`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:42:15 GMT
ADD file:6d8ee60b2fe4604969d8feeeb7e0dc8b9619a778d1a905c8bfdde5ede5e1eb54 in / 
# Wed, 01 Nov 2023 00:42:19 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:54:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:55:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bca95e393f709ba301b35c2439a815fd4fe8134d7a466bd528563bc32fd754d8`  
		Last Modified: Wed, 01 Nov 2023 00:47:43 GMT  
		Size: 47.9 MB (47943171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e744d1ef2c8405f6352136656080d7e244e1a97362c21069b734a55b86c8d0a`  
		Last Modified: Wed, 01 Nov 2023 02:05:09 GMT  
		Size: 24.0 MB (24045096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de40af46a5373d0a49892fa9000736be09090b477719517fcec84887d847f94b`  
		Last Modified: Wed, 01 Nov 2023 02:05:25 GMT  
		Size: 63.1 MB (63132485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:testing`

```console
$ docker pull buildpack-deps@sha256:e1a1af9997b0a0b3209f6efdd1ac32967e59abb80b8f121269b5afd4423b18f1
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
$ docker pull buildpack-deps@sha256:76eb5e32172570da1b6bda61e11f0cbee6572c35b8a7eeabe5b484ea2d802352
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.6 MB (385631216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3c533569935244fa74af768bb5f93b0f8da2205a8ad7d9f42536d17e9af7086`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:23:31 GMT
ADD file:00d06a447c9580e05c2514d623a6906f35419629a74e8f29f8627b620df970f3 in / 
# Wed, 01 Nov 2023 00:23:32 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 05:08:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 05:09:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 05:10:21 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9f30dcdc5629f1d2f740d6a704db5e6f29ed782df4486ef49cdbddb30250312f`  
		Last Modified: Wed, 01 Nov 2023 00:30:07 GMT  
		Size: 49.5 MB (49486885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b00fcc62737a4287ca8fcd27724545f3a9669ead301dbede869f8af73f94159`  
		Last Modified: Wed, 15 Nov 2023 05:17:53 GMT  
		Size: 26.3 MB (26255430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ccab398df14d3fc8ad70c0ac91181d737fba7720072d703f9b4cd4776dd5a54`  
		Last Modified: Wed, 15 Nov 2023 05:18:10 GMT  
		Size: 65.5 MB (65508665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d8e7265592a80bc6680099d6e4ebc6438f12eb4409b2ba9c29c9e1cd6192615`  
		Last Modified: Wed, 15 Nov 2023 05:18:47 GMT  
		Size: 244.4 MB (244380236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:c4dd02b720a78446828274ab2cc6528fa2c312793ed7452b372b8bd885afc039
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **354.2 MB (354181507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd6c57d4fbb357e2da385c326cf859f23bcbb94acf5c4d2a75da642ad8a76c3e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:49:55 GMT
ADD file:c8135c4f5f4b7815dc29bb93d73adb514649c5dfb72bfc1c072a7a9ae53653f1 in / 
# Wed, 01 Nov 2023 00:49:55 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 04:19:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 04:19:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 04:22:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:136f2fd3e12dd347dbdab54d5a79402eda3c65de7050120b6c1d86345bcc99da`  
		Last Modified: Wed, 01 Nov 2023 00:54:48 GMT  
		Size: 47.1 MB (47142117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76630daa19e4462e67c7427306ed19109a580c7c1d8e740a83a167e409d9cabc`  
		Last Modified: Wed, 15 Nov 2023 04:22:58 GMT  
		Size: 24.8 MB (24757320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20938e88d9c5a89a0f108e782b84fd782c481cd62c2b806cf84d1ec9e42be3fb`  
		Last Modified: Wed, 15 Nov 2023 04:23:17 GMT  
		Size: 63.0 MB (63026865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b34524d0ae9b6222d63fb5f12bcd3ba14069504b977deaddf1ff76f5e2f5add3`  
		Last Modified: Wed, 15 Nov 2023 04:24:00 GMT  
		Size: 219.3 MB (219255205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1fd4efca28447d364730072aaf05453d9dbce242854e327d14f86a31410de3e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.0 MB (334031743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ac2ec93c94487daa3001f353568b804e94ad3dafadb27880a05040daad71603`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:00:07 GMT
ADD file:035b362840f9210e5a7bfde4a95079958d9f57f5b5a556d22b48ad6abcdf2134 in / 
# Wed, 01 Nov 2023 01:00:07 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 02:00:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 02:01:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 02:03:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b403287e0cd0f39bef349bb68bed383fd0582cc2ae9137aac1969a41c84e30db`  
		Last Modified: Wed, 01 Nov 2023 01:06:58 GMT  
		Size: 44.9 MB (44936197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d95ccb30a9e3ceec487ec02756f65216d24abc33ca03c71393ac6e54f4e82b2`  
		Last Modified: Wed, 15 Nov 2023 02:10:23 GMT  
		Size: 23.9 MB (23949923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a902151f0ab2df8ae45f89c290b155db85a2180a36075c89127fdbbdbccb5431`  
		Last Modified: Wed, 15 Nov 2023 02:10:46 GMT  
		Size: 60.6 MB (60620862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15cd9a864ac37ceaebcb654bdbe09fa0bf0e29cb8d0748ee7f70f1dee480df63`  
		Last Modified: Wed, 15 Nov 2023 02:11:29 GMT  
		Size: 204.5 MB (204524761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3688319b9c516e88d24c8592d6f88fa17216ed884e10e81f6fb8c67ab2266bc8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **364.1 MB (364078462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ebd82260ec2e6d7eaf8c5e1a4fe85b1b86ad077d536c2d55d19661bc0babff5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:41:27 GMT
ADD file:d0c94454bffd347b60b86607fe3aea27f4afc57648c812d80575bc9d7d71a1fc in / 
# Wed, 01 Nov 2023 00:41:28 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:11:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:11:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:12:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6bbd151733a83c3c4e1747562a07b8dc0d6b9a1a38140e050fec86a0e73e1f0e`  
		Last Modified: Wed, 01 Nov 2023 00:47:15 GMT  
		Size: 49.5 MB (49495227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aaa14e94a2e8ffb5faf3100c888245cbc9a4eaaf9d6edea6ed3aef228b6b1f1`  
		Last Modified: Wed, 01 Nov 2023 02:17:28 GMT  
		Size: 20.1 MB (20141380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94bd9c6d088804a732d5962844e6cf83a29d1b30528f3b5ec7ff6e67e742a132`  
		Last Modified: Wed, 01 Nov 2023 02:17:45 GMT  
		Size: 65.6 MB (65600134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c397bd2bdea2862ea763227f6eda962a2798527c478e64bd500bdad5239cdbd9`  
		Last Modified: Wed, 01 Nov 2023 02:18:16 GMT  
		Size: 228.8 MB (228841721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; 386

```console
$ docker pull buildpack-deps@sha256:1255020c439389d597eaa2b16dee9c7aa1536b2b4aa224dfbc210a3756402d3e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **378.1 MB (378083228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27c3defb0da7e8349b162012f087f54867d2c18aad1f3b129d672e18ae6a787f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:41:31 GMT
ADD file:99d6a1f205a46734ffc61c992b3c9029eb83aceaab7b9777a94552ae226a209f in / 
# Wed, 01 Nov 2023 00:41:32 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 13:53:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:53:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:54:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7778791eeb3e7444e84c2d682795ca0f756d9e1d87e924e2739660a8ed9134ad`  
		Last Modified: Wed, 01 Nov 2023 00:48:34 GMT  
		Size: 50.5 MB (50466373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d80422353ec8a9a13b994d878c456b9feb2c3711191dccf08d7957979acd368`  
		Last Modified: Wed, 01 Nov 2023 14:01:24 GMT  
		Size: 20.9 MB (20909176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be46fd0a3e04a3c48fa349f6b3baa84f402e8ec4ed841491191fa80991567c8`  
		Last Modified: Wed, 01 Nov 2023 14:01:50 GMT  
		Size: 67.3 MB (67264025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f58267d46c1a5f0b0d20f45e86d4a01dbce5ad96ec0ea36ee8de24679e7fc63`  
		Last Modified: Wed, 01 Nov 2023 14:02:44 GMT  
		Size: 239.4 MB (239443654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:d9a456d77bdcd7c232974a87886dd2bbb590b9cf95313c9f1f0fdffa407dfca2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **361.9 MB (361931070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6647c63058a006d3eb26ee45646b020d6a4bd9871013d88648b3668a910bd6bb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:15:37 GMT
ADD file:fcddbc3f0c0456097a49c255590801b884727d47f9ceac6afe8463117d63a70e in / 
# Wed, 01 Nov 2023 01:15:43 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 02:09:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 02:11:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 02:18:52 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:434392845279581746e8cecd769b536845c39fb214d29012afa566896853392c`  
		Last Modified: Wed, 01 Nov 2023 01:26:47 GMT  
		Size: 49.3 MB (49278627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ede9f97c171cbb8a558528bdc51f6a5dd9e805644cae6cc9891cb76258eb9d`  
		Last Modified: Wed, 15 Nov 2023 02:19:46 GMT  
		Size: 26.1 MB (26073841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7717e39a49a836fc0908b857bdee9522fd3c967c00400172afac7d1498f8b2`  
		Last Modified: Wed, 15 Nov 2023 02:20:37 GMT  
		Size: 64.3 MB (64324993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6b9044ec2fd759757a7d3da51aebd64910bbea1f92e2ab8c2074ed1c4023fb`  
		Last Modified: Wed, 15 Nov 2023 02:23:00 GMT  
		Size: 222.3 MB (222253609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:6f399110e0e0cf3dcce653b18ab632e351a9b0b44822bda406fb7ec996027af3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **398.7 MB (398685762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6faa4d627a08f8d90cb01d865c1011c663ea79b5a68f992797a5e15914ff8fae`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:24:06 GMT
ADD file:d45c9f62cb1fd4297a5ee2026bc6abb62f25a456f3a44a8ab6d115eb1d59ce39 in / 
# Wed, 01 Nov 2023 00:24:09 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 02:17:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 02:17:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 02:20:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a86485f1d263f9f0955a85f3d3707fcc2bc7bb4d598df11d02b766bd3da90ad3`  
		Last Modified: Wed, 01 Nov 2023 00:29:48 GMT  
		Size: 53.4 MB (53390698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4809c26c5fbcf46e724e97753b831c03c2021ac2def13026b528fb114d6989f`  
		Last Modified: Wed, 15 Nov 2023 02:28:19 GMT  
		Size: 28.8 MB (28814600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01dd59a7c5494927ca7f0a3267579f63aea083a036ffa58f2bdba9773f3f058`  
		Last Modified: Wed, 15 Nov 2023 02:28:39 GMT  
		Size: 70.9 MB (70934394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187103a4b58ffe18a1ab1eb4ebd7272365c8a7b0c6d3c3a47de357e5293439b8`  
		Last Modified: Wed, 15 Nov 2023 02:29:23 GMT  
		Size: 245.5 MB (245546070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:0aea1b61a3cc9258f80eb9afd15b4d43a1fec3dc78a985dcee84a17ffb7d8abc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.5 MB (346493962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8528bad8c02e35e6fc9861a3f1e072a52eae0d62f97c014affc16af978eb160a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:45:36 GMT
ADD file:b451624b6214da7e4871235da21071d55a6c21b9ed56fe301e78beebaa9c034d in / 
# Wed, 01 Nov 2023 00:45:40 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:01:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:01:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:02:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:37319c2577b55a62447a947186364b13c616c3448bd2c4aeb444733fc58dfb64`  
		Last Modified: Wed, 01 Nov 2023 00:50:43 GMT  
		Size: 48.9 MB (48900178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10e593352eeadc1fa34f624da16ec4d5ffc03e962de8e47f9fd30d101863f83`  
		Last Modified: Wed, 01 Nov 2023 02:07:56 GMT  
		Size: 20.1 MB (20059774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b780353fcf3645d3b82950a80a107c5134cb03e7e2514a5a84924d066df64f80`  
		Last Modified: Wed, 01 Nov 2023 02:08:13 GMT  
		Size: 66.5 MB (66470254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfd3c0b27e6f490c7f70213d49854c77842e63e87abe059666a4a45282b64bf`  
		Last Modified: Wed, 01 Nov 2023 02:08:45 GMT  
		Size: 211.1 MB (211063756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:testing-curl`

```console
$ docker pull buildpack-deps@sha256:9c5d9dc31c46e42857fe71925e7bb7777399aaeb18ed91ad1f76e1deda549703
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
$ docker pull buildpack-deps@sha256:16d76495ee528187f25d63a08b40e77e5331d2d813b678c1bd4b2874cb4958f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75742315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08129f3119f282d801ddd2495b0ce1a0ff7da19d113e7643294c273eefee0517`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:23:31 GMT
ADD file:00d06a447c9580e05c2514d623a6906f35419629a74e8f29f8627b620df970f3 in / 
# Wed, 01 Nov 2023 00:23:32 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 05:08:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9f30dcdc5629f1d2f740d6a704db5e6f29ed782df4486ef49cdbddb30250312f`  
		Last Modified: Wed, 01 Nov 2023 00:30:07 GMT  
		Size: 49.5 MB (49486885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b00fcc62737a4287ca8fcd27724545f3a9669ead301dbede869f8af73f94159`  
		Last Modified: Wed, 15 Nov 2023 05:17:53 GMT  
		Size: 26.3 MB (26255430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:183b0d8da52453026ea622f8c7c995c1081c5ae8a3f6862372f63e7b7919e8eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.9 MB (71899437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e2b5a8f8d6c6dac8255764c07b7f9820742d18652d355b4c770aa79586d64d0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:49:55 GMT
ADD file:c8135c4f5f4b7815dc29bb93d73adb514649c5dfb72bfc1c072a7a9ae53653f1 in / 
# Wed, 01 Nov 2023 00:49:55 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 04:19:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:136f2fd3e12dd347dbdab54d5a79402eda3c65de7050120b6c1d86345bcc99da`  
		Last Modified: Wed, 01 Nov 2023 00:54:48 GMT  
		Size: 47.1 MB (47142117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76630daa19e4462e67c7427306ed19109a580c7c1d8e740a83a167e409d9cabc`  
		Last Modified: Wed, 15 Nov 2023 04:22:58 GMT  
		Size: 24.8 MB (24757320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:e31302afdcfe501a4c29c36c0a87773fff9d16438b1671c9029e28df9d629a51
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68886120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6c65f518912c504507ebe9ed5400c06cba43acf501dfe7b266a37735559d3f3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:00:07 GMT
ADD file:035b362840f9210e5a7bfde4a95079958d9f57f5b5a556d22b48ad6abcdf2134 in / 
# Wed, 01 Nov 2023 01:00:07 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 02:00:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b403287e0cd0f39bef349bb68bed383fd0582cc2ae9137aac1969a41c84e30db`  
		Last Modified: Wed, 01 Nov 2023 01:06:58 GMT  
		Size: 44.9 MB (44936197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d95ccb30a9e3ceec487ec02756f65216d24abc33ca03c71393ac6e54f4e82b2`  
		Last Modified: Wed, 15 Nov 2023 02:10:23 GMT  
		Size: 23.9 MB (23949923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:5c597fc3f240d9ec58bc7a8bb6eac544d7f91bc95c583c0dea4a8c5343d2cd6f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69636607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:799b9d80cfbf3d254cc2d8e1ba2618aeab9932ba566919d1c5b40598e8817518`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:41:27 GMT
ADD file:d0c94454bffd347b60b86607fe3aea27f4afc57648c812d80575bc9d7d71a1fc in / 
# Wed, 01 Nov 2023 00:41:28 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:11:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6bbd151733a83c3c4e1747562a07b8dc0d6b9a1a38140e050fec86a0e73e1f0e`  
		Last Modified: Wed, 01 Nov 2023 00:47:15 GMT  
		Size: 49.5 MB (49495227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aaa14e94a2e8ffb5faf3100c888245cbc9a4eaaf9d6edea6ed3aef228b6b1f1`  
		Last Modified: Wed, 01 Nov 2023 02:17:28 GMT  
		Size: 20.1 MB (20141380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:fda33c228a37bc721c34159128f4b6f92a8612f6ff05cb52658d80550ce009c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.4 MB (71375549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35b7cb6002b21caeea5999881a72aa5b1ca27460c4602a3328892064928b5dc6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:41:31 GMT
ADD file:99d6a1f205a46734ffc61c992b3c9029eb83aceaab7b9777a94552ae226a209f in / 
# Wed, 01 Nov 2023 00:41:32 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 13:53:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7778791eeb3e7444e84c2d682795ca0f756d9e1d87e924e2739660a8ed9134ad`  
		Last Modified: Wed, 01 Nov 2023 00:48:34 GMT  
		Size: 50.5 MB (50466373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d80422353ec8a9a13b994d878c456b9feb2c3711191dccf08d7957979acd368`  
		Last Modified: Wed, 01 Nov 2023 14:01:24 GMT  
		Size: 20.9 MB (20909176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:4912dd6e6037dde41e039e3f907c9a89a70a4cb4b47eb68958c1d742b35e0a8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75352468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4ffb34227c79ce599b62d0355af9d7910bd374bc71278835a773cbc85704dea`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:15:37 GMT
ADD file:fcddbc3f0c0456097a49c255590801b884727d47f9ceac6afe8463117d63a70e in / 
# Wed, 01 Nov 2023 01:15:43 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 02:09:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:434392845279581746e8cecd769b536845c39fb214d29012afa566896853392c`  
		Last Modified: Wed, 01 Nov 2023 01:26:47 GMT  
		Size: 49.3 MB (49278627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ede9f97c171cbb8a558528bdc51f6a5dd9e805644cae6cc9891cb76258eb9d`  
		Last Modified: Wed, 15 Nov 2023 02:19:46 GMT  
		Size: 26.1 MB (26073841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:a025ed6b3c26a7fbaeb80a232f467b2b87e5075ffbf6a43ed4dfc3f122c22f88
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.2 MB (82205298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04223e52eef897909d667acd82f3d25674d39d08063ec943bee425cb270c6ab7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:24:06 GMT
ADD file:d45c9f62cb1fd4297a5ee2026bc6abb62f25a456f3a44a8ab6d115eb1d59ce39 in / 
# Wed, 01 Nov 2023 00:24:09 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 02:17:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a86485f1d263f9f0955a85f3d3707fcc2bc7bb4d598df11d02b766bd3da90ad3`  
		Last Modified: Wed, 01 Nov 2023 00:29:48 GMT  
		Size: 53.4 MB (53390698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4809c26c5fbcf46e724e97753b831c03c2021ac2def13026b528fb114d6989f`  
		Last Modified: Wed, 15 Nov 2023 02:28:19 GMT  
		Size: 28.8 MB (28814600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:69f5a6be863cb69c5e8fbf9fb8eaf91c2994ca992b4db4df61c766a3dc512c80
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (68959952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c167457a1683a82fde1556d548ac9344db2d2d3e22530763b33801be31261264`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:45:36 GMT
ADD file:b451624b6214da7e4871235da21071d55a6c21b9ed56fe301e78beebaa9c034d in / 
# Wed, 01 Nov 2023 00:45:40 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:01:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:37319c2577b55a62447a947186364b13c616c3448bd2c4aeb444733fc58dfb64`  
		Last Modified: Wed, 01 Nov 2023 00:50:43 GMT  
		Size: 48.9 MB (48900178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10e593352eeadc1fa34f624da16ec4d5ffc03e962de8e47f9fd30d101863f83`  
		Last Modified: Wed, 01 Nov 2023 02:07:56 GMT  
		Size: 20.1 MB (20059774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:testing-scm`

```console
$ docker pull buildpack-deps@sha256:edeaaf37b0c2d2152e4472af4581152e1302658eb6f695a9e4b755089c7f6413
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
$ docker pull buildpack-deps@sha256:462e243f20451b99d0d4631d40e08f3aba91c7940a658745d7943320c2f05060
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.3 MB (141250980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d619a60defd797722d81ef2e28e8daee71fad5dc46f5b42a61ed8e4addadf451`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:23:31 GMT
ADD file:00d06a447c9580e05c2514d623a6906f35419629a74e8f29f8627b620df970f3 in / 
# Wed, 01 Nov 2023 00:23:32 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 05:08:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 05:09:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9f30dcdc5629f1d2f740d6a704db5e6f29ed782df4486ef49cdbddb30250312f`  
		Last Modified: Wed, 01 Nov 2023 00:30:07 GMT  
		Size: 49.5 MB (49486885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b00fcc62737a4287ca8fcd27724545f3a9669ead301dbede869f8af73f94159`  
		Last Modified: Wed, 15 Nov 2023 05:17:53 GMT  
		Size: 26.3 MB (26255430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ccab398df14d3fc8ad70c0ac91181d737fba7720072d703f9b4cd4776dd5a54`  
		Last Modified: Wed, 15 Nov 2023 05:18:10 GMT  
		Size: 65.5 MB (65508665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:e98e275298640ac337d66d1e8b2daff0b1fa47059063cc5cf730d09153ea11f7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.9 MB (134926302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:591879d8e8fe078a1d376f8f02273465613a192e6ae1d6f30d60bd1012d7552f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:49:55 GMT
ADD file:c8135c4f5f4b7815dc29bb93d73adb514649c5dfb72bfc1c072a7a9ae53653f1 in / 
# Wed, 01 Nov 2023 00:49:55 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 04:19:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 04:19:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:136f2fd3e12dd347dbdab54d5a79402eda3c65de7050120b6c1d86345bcc99da`  
		Last Modified: Wed, 01 Nov 2023 00:54:48 GMT  
		Size: 47.1 MB (47142117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76630daa19e4462e67c7427306ed19109a580c7c1d8e740a83a167e409d9cabc`  
		Last Modified: Wed, 15 Nov 2023 04:22:58 GMT  
		Size: 24.8 MB (24757320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20938e88d9c5a89a0f108e782b84fd782c481cd62c2b806cf84d1ec9e42be3fb`  
		Last Modified: Wed, 15 Nov 2023 04:23:17 GMT  
		Size: 63.0 MB (63026865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:75dea238cd526afe7ce7b9513ca46dbf1cc6dadc22fe16aa542aabad67481013
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129506982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:361deb5742958e94144bd2fcf2dca7450743abbd022702c2dcbb5df03bf5b48f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:00:07 GMT
ADD file:035b362840f9210e5a7bfde4a95079958d9f57f5b5a556d22b48ad6abcdf2134 in / 
# Wed, 01 Nov 2023 01:00:07 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 02:00:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 02:01:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b403287e0cd0f39bef349bb68bed383fd0582cc2ae9137aac1969a41c84e30db`  
		Last Modified: Wed, 01 Nov 2023 01:06:58 GMT  
		Size: 44.9 MB (44936197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d95ccb30a9e3ceec487ec02756f65216d24abc33ca03c71393ac6e54f4e82b2`  
		Last Modified: Wed, 15 Nov 2023 02:10:23 GMT  
		Size: 23.9 MB (23949923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a902151f0ab2df8ae45f89c290b155db85a2180a36075c89127fdbbdbccb5431`  
		Last Modified: Wed, 15 Nov 2023 02:10:46 GMT  
		Size: 60.6 MB (60620862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f4ecc23cf3593d792eccac10de6f65402681509d9c2e2121c4f5fc696291e245
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.2 MB (135236741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:511a2b90c89c51a56cd6d51c5f1fcd9b7b1901c5c794c3d3d7967fa1b226b629`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:41:27 GMT
ADD file:d0c94454bffd347b60b86607fe3aea27f4afc57648c812d80575bc9d7d71a1fc in / 
# Wed, 01 Nov 2023 00:41:28 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:11:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:11:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6bbd151733a83c3c4e1747562a07b8dc0d6b9a1a38140e050fec86a0e73e1f0e`  
		Last Modified: Wed, 01 Nov 2023 00:47:15 GMT  
		Size: 49.5 MB (49495227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aaa14e94a2e8ffb5faf3100c888245cbc9a4eaaf9d6edea6ed3aef228b6b1f1`  
		Last Modified: Wed, 01 Nov 2023 02:17:28 GMT  
		Size: 20.1 MB (20141380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94bd9c6d088804a732d5962844e6cf83a29d1b30528f3b5ec7ff6e67e742a132`  
		Last Modified: Wed, 01 Nov 2023 02:17:45 GMT  
		Size: 65.6 MB (65600134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:369a5742bedd7592b08d2ba7e7c53deedacf83dcf67f1610298c4d302e96504f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.6 MB (138639574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1715791f3ccb5695b0269a0a7a09b417f3354ebcb9c4022a0a20136e58c7fb82`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:41:31 GMT
ADD file:99d6a1f205a46734ffc61c992b3c9029eb83aceaab7b9777a94552ae226a209f in / 
# Wed, 01 Nov 2023 00:41:32 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 13:53:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:53:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7778791eeb3e7444e84c2d682795ca0f756d9e1d87e924e2739660a8ed9134ad`  
		Last Modified: Wed, 01 Nov 2023 00:48:34 GMT  
		Size: 50.5 MB (50466373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d80422353ec8a9a13b994d878c456b9feb2c3711191dccf08d7957979acd368`  
		Last Modified: Wed, 01 Nov 2023 14:01:24 GMT  
		Size: 20.9 MB (20909176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be46fd0a3e04a3c48fa349f6b3baa84f402e8ec4ed841491191fa80991567c8`  
		Last Modified: Wed, 01 Nov 2023 14:01:50 GMT  
		Size: 67.3 MB (67264025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:018e682c1fa14ae9daeebeb7f90363910e3dbeb3a6c031b7d8c7079e35211784
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.7 MB (139677461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0dc06258e7ec131a3593eb9cdd566566727a64176af57e747bbbca3bee96d6d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:15:37 GMT
ADD file:fcddbc3f0c0456097a49c255590801b884727d47f9ceac6afe8463117d63a70e in / 
# Wed, 01 Nov 2023 01:15:43 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 02:09:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 02:11:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:434392845279581746e8cecd769b536845c39fb214d29012afa566896853392c`  
		Last Modified: Wed, 01 Nov 2023 01:26:47 GMT  
		Size: 49.3 MB (49278627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ede9f97c171cbb8a558528bdc51f6a5dd9e805644cae6cc9891cb76258eb9d`  
		Last Modified: Wed, 15 Nov 2023 02:19:46 GMT  
		Size: 26.1 MB (26073841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7717e39a49a836fc0908b857bdee9522fd3c967c00400172afac7d1498f8b2`  
		Last Modified: Wed, 15 Nov 2023 02:20:37 GMT  
		Size: 64.3 MB (64324993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:6d6dbff7260cc7e234001f7f9ed2e110a4bb9e164d381614d3e257f52b4d43d6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.1 MB (153139692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f24f72538a7400a19c9b0300cb9383805393e690e5c2f5aecade97749ca15e8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:24:06 GMT
ADD file:d45c9f62cb1fd4297a5ee2026bc6abb62f25a456f3a44a8ab6d115eb1d59ce39 in / 
# Wed, 01 Nov 2023 00:24:09 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 02:17:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 02:17:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a86485f1d263f9f0955a85f3d3707fcc2bc7bb4d598df11d02b766bd3da90ad3`  
		Last Modified: Wed, 01 Nov 2023 00:29:48 GMT  
		Size: 53.4 MB (53390698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4809c26c5fbcf46e724e97753b831c03c2021ac2def13026b528fb114d6989f`  
		Last Modified: Wed, 15 Nov 2023 02:28:19 GMT  
		Size: 28.8 MB (28814600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01dd59a7c5494927ca7f0a3267579f63aea083a036ffa58f2bdba9773f3f058`  
		Last Modified: Wed, 15 Nov 2023 02:28:39 GMT  
		Size: 70.9 MB (70934394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:3244855b69745d2237dff0ee5e5caff6d4f2a6a66ec03c531ea9f8ef87b75e04
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.4 MB (135430206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70939a2063f13adf3e74bb8cf060f2ddead45dbf2bcf0890fa8dc94a65c68026`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:45:36 GMT
ADD file:b451624b6214da7e4871235da21071d55a6c21b9ed56fe301e78beebaa9c034d in / 
# Wed, 01 Nov 2023 00:45:40 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:01:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:01:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:37319c2577b55a62447a947186364b13c616c3448bd2c4aeb444733fc58dfb64`  
		Last Modified: Wed, 01 Nov 2023 00:50:43 GMT  
		Size: 48.9 MB (48900178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10e593352eeadc1fa34f624da16ec4d5ffc03e962de8e47f9fd30d101863f83`  
		Last Modified: Wed, 01 Nov 2023 02:07:56 GMT  
		Size: 20.1 MB (20059774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b780353fcf3645d3b82950a80a107c5134cb03e7e2514a5a84924d066df64f80`  
		Last Modified: Wed, 01 Nov 2023 02:08:13 GMT  
		Size: 66.5 MB (66470254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:trixie`

```console
$ docker pull buildpack-deps@sha256:e1a1af9997b0a0b3209f6efdd1ac32967e59abb80b8f121269b5afd4423b18f1
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
$ docker pull buildpack-deps@sha256:76eb5e32172570da1b6bda61e11f0cbee6572c35b8a7eeabe5b484ea2d802352
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **385.6 MB (385631216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3c533569935244fa74af768bb5f93b0f8da2205a8ad7d9f42536d17e9af7086`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:23:31 GMT
ADD file:00d06a447c9580e05c2514d623a6906f35419629a74e8f29f8627b620df970f3 in / 
# Wed, 01 Nov 2023 00:23:32 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 05:08:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 05:09:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 05:10:21 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9f30dcdc5629f1d2f740d6a704db5e6f29ed782df4486ef49cdbddb30250312f`  
		Last Modified: Wed, 01 Nov 2023 00:30:07 GMT  
		Size: 49.5 MB (49486885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b00fcc62737a4287ca8fcd27724545f3a9669ead301dbede869f8af73f94159`  
		Last Modified: Wed, 15 Nov 2023 05:17:53 GMT  
		Size: 26.3 MB (26255430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ccab398df14d3fc8ad70c0ac91181d737fba7720072d703f9b4cd4776dd5a54`  
		Last Modified: Wed, 15 Nov 2023 05:18:10 GMT  
		Size: 65.5 MB (65508665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d8e7265592a80bc6680099d6e4ebc6438f12eb4409b2ba9c29c9e1cd6192615`  
		Last Modified: Wed, 15 Nov 2023 05:18:47 GMT  
		Size: 244.4 MB (244380236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:c4dd02b720a78446828274ab2cc6528fa2c312793ed7452b372b8bd885afc039
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **354.2 MB (354181507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd6c57d4fbb357e2da385c326cf859f23bcbb94acf5c4d2a75da642ad8a76c3e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:49:55 GMT
ADD file:c8135c4f5f4b7815dc29bb93d73adb514649c5dfb72bfc1c072a7a9ae53653f1 in / 
# Wed, 01 Nov 2023 00:49:55 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 04:19:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 04:19:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 04:22:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:136f2fd3e12dd347dbdab54d5a79402eda3c65de7050120b6c1d86345bcc99da`  
		Last Modified: Wed, 01 Nov 2023 00:54:48 GMT  
		Size: 47.1 MB (47142117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76630daa19e4462e67c7427306ed19109a580c7c1d8e740a83a167e409d9cabc`  
		Last Modified: Wed, 15 Nov 2023 04:22:58 GMT  
		Size: 24.8 MB (24757320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20938e88d9c5a89a0f108e782b84fd782c481cd62c2b806cf84d1ec9e42be3fb`  
		Last Modified: Wed, 15 Nov 2023 04:23:17 GMT  
		Size: 63.0 MB (63026865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b34524d0ae9b6222d63fb5f12bcd3ba14069504b977deaddf1ff76f5e2f5add3`  
		Last Modified: Wed, 15 Nov 2023 04:24:00 GMT  
		Size: 219.3 MB (219255205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1fd4efca28447d364730072aaf05453d9dbce242854e327d14f86a31410de3e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.0 MB (334031743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ac2ec93c94487daa3001f353568b804e94ad3dafadb27880a05040daad71603`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:00:07 GMT
ADD file:035b362840f9210e5a7bfde4a95079958d9f57f5b5a556d22b48ad6abcdf2134 in / 
# Wed, 01 Nov 2023 01:00:07 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 02:00:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 02:01:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 02:03:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b403287e0cd0f39bef349bb68bed383fd0582cc2ae9137aac1969a41c84e30db`  
		Last Modified: Wed, 01 Nov 2023 01:06:58 GMT  
		Size: 44.9 MB (44936197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d95ccb30a9e3ceec487ec02756f65216d24abc33ca03c71393ac6e54f4e82b2`  
		Last Modified: Wed, 15 Nov 2023 02:10:23 GMT  
		Size: 23.9 MB (23949923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a902151f0ab2df8ae45f89c290b155db85a2180a36075c89127fdbbdbccb5431`  
		Last Modified: Wed, 15 Nov 2023 02:10:46 GMT  
		Size: 60.6 MB (60620862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15cd9a864ac37ceaebcb654bdbe09fa0bf0e29cb8d0748ee7f70f1dee480df63`  
		Last Modified: Wed, 15 Nov 2023 02:11:29 GMT  
		Size: 204.5 MB (204524761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3688319b9c516e88d24c8592d6f88fa17216ed884e10e81f6fb8c67ab2266bc8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **364.1 MB (364078462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ebd82260ec2e6d7eaf8c5e1a4fe85b1b86ad077d536c2d55d19661bc0babff5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:41:27 GMT
ADD file:d0c94454bffd347b60b86607fe3aea27f4afc57648c812d80575bc9d7d71a1fc in / 
# Wed, 01 Nov 2023 00:41:28 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:11:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:11:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:12:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6bbd151733a83c3c4e1747562a07b8dc0d6b9a1a38140e050fec86a0e73e1f0e`  
		Last Modified: Wed, 01 Nov 2023 00:47:15 GMT  
		Size: 49.5 MB (49495227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aaa14e94a2e8ffb5faf3100c888245cbc9a4eaaf9d6edea6ed3aef228b6b1f1`  
		Last Modified: Wed, 01 Nov 2023 02:17:28 GMT  
		Size: 20.1 MB (20141380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94bd9c6d088804a732d5962844e6cf83a29d1b30528f3b5ec7ff6e67e742a132`  
		Last Modified: Wed, 01 Nov 2023 02:17:45 GMT  
		Size: 65.6 MB (65600134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c397bd2bdea2862ea763227f6eda962a2798527c478e64bd500bdad5239cdbd9`  
		Last Modified: Wed, 01 Nov 2023 02:18:16 GMT  
		Size: 228.8 MB (228841721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie` - linux; 386

```console
$ docker pull buildpack-deps@sha256:1255020c439389d597eaa2b16dee9c7aa1536b2b4aa224dfbc210a3756402d3e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **378.1 MB (378083228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27c3defb0da7e8349b162012f087f54867d2c18aad1f3b129d672e18ae6a787f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:41:31 GMT
ADD file:99d6a1f205a46734ffc61c992b3c9029eb83aceaab7b9777a94552ae226a209f in / 
# Wed, 01 Nov 2023 00:41:32 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 13:53:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:53:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:54:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7778791eeb3e7444e84c2d682795ca0f756d9e1d87e924e2739660a8ed9134ad`  
		Last Modified: Wed, 01 Nov 2023 00:48:34 GMT  
		Size: 50.5 MB (50466373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d80422353ec8a9a13b994d878c456b9feb2c3711191dccf08d7957979acd368`  
		Last Modified: Wed, 01 Nov 2023 14:01:24 GMT  
		Size: 20.9 MB (20909176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be46fd0a3e04a3c48fa349f6b3baa84f402e8ec4ed841491191fa80991567c8`  
		Last Modified: Wed, 01 Nov 2023 14:01:50 GMT  
		Size: 67.3 MB (67264025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f58267d46c1a5f0b0d20f45e86d4a01dbce5ad96ec0ea36ee8de24679e7fc63`  
		Last Modified: Wed, 01 Nov 2023 14:02:44 GMT  
		Size: 239.4 MB (239443654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:d9a456d77bdcd7c232974a87886dd2bbb590b9cf95313c9f1f0fdffa407dfca2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **361.9 MB (361931070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6647c63058a006d3eb26ee45646b020d6a4bd9871013d88648b3668a910bd6bb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:15:37 GMT
ADD file:fcddbc3f0c0456097a49c255590801b884727d47f9ceac6afe8463117d63a70e in / 
# Wed, 01 Nov 2023 01:15:43 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 02:09:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 02:11:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 02:18:52 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:434392845279581746e8cecd769b536845c39fb214d29012afa566896853392c`  
		Last Modified: Wed, 01 Nov 2023 01:26:47 GMT  
		Size: 49.3 MB (49278627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ede9f97c171cbb8a558528bdc51f6a5dd9e805644cae6cc9891cb76258eb9d`  
		Last Modified: Wed, 15 Nov 2023 02:19:46 GMT  
		Size: 26.1 MB (26073841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7717e39a49a836fc0908b857bdee9522fd3c967c00400172afac7d1498f8b2`  
		Last Modified: Wed, 15 Nov 2023 02:20:37 GMT  
		Size: 64.3 MB (64324993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6b9044ec2fd759757a7d3da51aebd64910bbea1f92e2ab8c2074ed1c4023fb`  
		Last Modified: Wed, 15 Nov 2023 02:23:00 GMT  
		Size: 222.3 MB (222253609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:6f399110e0e0cf3dcce653b18ab632e351a9b0b44822bda406fb7ec996027af3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **398.7 MB (398685762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6faa4d627a08f8d90cb01d865c1011c663ea79b5a68f992797a5e15914ff8fae`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:24:06 GMT
ADD file:d45c9f62cb1fd4297a5ee2026bc6abb62f25a456f3a44a8ab6d115eb1d59ce39 in / 
# Wed, 01 Nov 2023 00:24:09 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 02:17:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 02:17:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 02:20:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a86485f1d263f9f0955a85f3d3707fcc2bc7bb4d598df11d02b766bd3da90ad3`  
		Last Modified: Wed, 01 Nov 2023 00:29:48 GMT  
		Size: 53.4 MB (53390698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4809c26c5fbcf46e724e97753b831c03c2021ac2def13026b528fb114d6989f`  
		Last Modified: Wed, 15 Nov 2023 02:28:19 GMT  
		Size: 28.8 MB (28814600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01dd59a7c5494927ca7f0a3267579f63aea083a036ffa58f2bdba9773f3f058`  
		Last Modified: Wed, 15 Nov 2023 02:28:39 GMT  
		Size: 70.9 MB (70934394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187103a4b58ffe18a1ab1eb4ebd7272365c8a7b0c6d3c3a47de357e5293439b8`  
		Last Modified: Wed, 15 Nov 2023 02:29:23 GMT  
		Size: 245.5 MB (245546070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:0aea1b61a3cc9258f80eb9afd15b4d43a1fec3dc78a985dcee84a17ffb7d8abc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.5 MB (346493962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8528bad8c02e35e6fc9861a3f1e072a52eae0d62f97c014affc16af978eb160a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:45:36 GMT
ADD file:b451624b6214da7e4871235da21071d55a6c21b9ed56fe301e78beebaa9c034d in / 
# Wed, 01 Nov 2023 00:45:40 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:01:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:01:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:02:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:37319c2577b55a62447a947186364b13c616c3448bd2c4aeb444733fc58dfb64`  
		Last Modified: Wed, 01 Nov 2023 00:50:43 GMT  
		Size: 48.9 MB (48900178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10e593352eeadc1fa34f624da16ec4d5ffc03e962de8e47f9fd30d101863f83`  
		Last Modified: Wed, 01 Nov 2023 02:07:56 GMT  
		Size: 20.1 MB (20059774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b780353fcf3645d3b82950a80a107c5134cb03e7e2514a5a84924d066df64f80`  
		Last Modified: Wed, 01 Nov 2023 02:08:13 GMT  
		Size: 66.5 MB (66470254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfd3c0b27e6f490c7f70213d49854c77842e63e87abe059666a4a45282b64bf`  
		Last Modified: Wed, 01 Nov 2023 02:08:45 GMT  
		Size: 211.1 MB (211063756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:trixie-curl`

```console
$ docker pull buildpack-deps@sha256:9c5d9dc31c46e42857fe71925e7bb7777399aaeb18ed91ad1f76e1deda549703
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
$ docker pull buildpack-deps@sha256:16d76495ee528187f25d63a08b40e77e5331d2d813b678c1bd4b2874cb4958f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75742315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08129f3119f282d801ddd2495b0ce1a0ff7da19d113e7643294c273eefee0517`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:23:31 GMT
ADD file:00d06a447c9580e05c2514d623a6906f35419629a74e8f29f8627b620df970f3 in / 
# Wed, 01 Nov 2023 00:23:32 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 05:08:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9f30dcdc5629f1d2f740d6a704db5e6f29ed782df4486ef49cdbddb30250312f`  
		Last Modified: Wed, 01 Nov 2023 00:30:07 GMT  
		Size: 49.5 MB (49486885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b00fcc62737a4287ca8fcd27724545f3a9669ead301dbede869f8af73f94159`  
		Last Modified: Wed, 15 Nov 2023 05:17:53 GMT  
		Size: 26.3 MB (26255430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:183b0d8da52453026ea622f8c7c995c1081c5ae8a3f6862372f63e7b7919e8eb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.9 MB (71899437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e2b5a8f8d6c6dac8255764c07b7f9820742d18652d355b4c770aa79586d64d0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:49:55 GMT
ADD file:c8135c4f5f4b7815dc29bb93d73adb514649c5dfb72bfc1c072a7a9ae53653f1 in / 
# Wed, 01 Nov 2023 00:49:55 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 04:19:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:136f2fd3e12dd347dbdab54d5a79402eda3c65de7050120b6c1d86345bcc99da`  
		Last Modified: Wed, 01 Nov 2023 00:54:48 GMT  
		Size: 47.1 MB (47142117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76630daa19e4462e67c7427306ed19109a580c7c1d8e740a83a167e409d9cabc`  
		Last Modified: Wed, 15 Nov 2023 04:22:58 GMT  
		Size: 24.8 MB (24757320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:e31302afdcfe501a4c29c36c0a87773fff9d16438b1671c9029e28df9d629a51
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68886120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6c65f518912c504507ebe9ed5400c06cba43acf501dfe7b266a37735559d3f3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:00:07 GMT
ADD file:035b362840f9210e5a7bfde4a95079958d9f57f5b5a556d22b48ad6abcdf2134 in / 
# Wed, 01 Nov 2023 01:00:07 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 02:00:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b403287e0cd0f39bef349bb68bed383fd0582cc2ae9137aac1969a41c84e30db`  
		Last Modified: Wed, 01 Nov 2023 01:06:58 GMT  
		Size: 44.9 MB (44936197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d95ccb30a9e3ceec487ec02756f65216d24abc33ca03c71393ac6e54f4e82b2`  
		Last Modified: Wed, 15 Nov 2023 02:10:23 GMT  
		Size: 23.9 MB (23949923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:5c597fc3f240d9ec58bc7a8bb6eac544d7f91bc95c583c0dea4a8c5343d2cd6f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69636607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:799b9d80cfbf3d254cc2d8e1ba2618aeab9932ba566919d1c5b40598e8817518`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:41:27 GMT
ADD file:d0c94454bffd347b60b86607fe3aea27f4afc57648c812d80575bc9d7d71a1fc in / 
# Wed, 01 Nov 2023 00:41:28 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:11:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6bbd151733a83c3c4e1747562a07b8dc0d6b9a1a38140e050fec86a0e73e1f0e`  
		Last Modified: Wed, 01 Nov 2023 00:47:15 GMT  
		Size: 49.5 MB (49495227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aaa14e94a2e8ffb5faf3100c888245cbc9a4eaaf9d6edea6ed3aef228b6b1f1`  
		Last Modified: Wed, 01 Nov 2023 02:17:28 GMT  
		Size: 20.1 MB (20141380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:fda33c228a37bc721c34159128f4b6f92a8612f6ff05cb52658d80550ce009c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.4 MB (71375549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35b7cb6002b21caeea5999881a72aa5b1ca27460c4602a3328892064928b5dc6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:41:31 GMT
ADD file:99d6a1f205a46734ffc61c992b3c9029eb83aceaab7b9777a94552ae226a209f in / 
# Wed, 01 Nov 2023 00:41:32 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 13:53:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7778791eeb3e7444e84c2d682795ca0f756d9e1d87e924e2739660a8ed9134ad`  
		Last Modified: Wed, 01 Nov 2023 00:48:34 GMT  
		Size: 50.5 MB (50466373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d80422353ec8a9a13b994d878c456b9feb2c3711191dccf08d7957979acd368`  
		Last Modified: Wed, 01 Nov 2023 14:01:24 GMT  
		Size: 20.9 MB (20909176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:4912dd6e6037dde41e039e3f907c9a89a70a4cb4b47eb68958c1d742b35e0a8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75352468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4ffb34227c79ce599b62d0355af9d7910bd374bc71278835a773cbc85704dea`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:15:37 GMT
ADD file:fcddbc3f0c0456097a49c255590801b884727d47f9ceac6afe8463117d63a70e in / 
# Wed, 01 Nov 2023 01:15:43 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 02:09:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:434392845279581746e8cecd769b536845c39fb214d29012afa566896853392c`  
		Last Modified: Wed, 01 Nov 2023 01:26:47 GMT  
		Size: 49.3 MB (49278627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ede9f97c171cbb8a558528bdc51f6a5dd9e805644cae6cc9891cb76258eb9d`  
		Last Modified: Wed, 15 Nov 2023 02:19:46 GMT  
		Size: 26.1 MB (26073841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:a025ed6b3c26a7fbaeb80a232f467b2b87e5075ffbf6a43ed4dfc3f122c22f88
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.2 MB (82205298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04223e52eef897909d667acd82f3d25674d39d08063ec943bee425cb270c6ab7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:24:06 GMT
ADD file:d45c9f62cb1fd4297a5ee2026bc6abb62f25a456f3a44a8ab6d115eb1d59ce39 in / 
# Wed, 01 Nov 2023 00:24:09 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 02:17:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a86485f1d263f9f0955a85f3d3707fcc2bc7bb4d598df11d02b766bd3da90ad3`  
		Last Modified: Wed, 01 Nov 2023 00:29:48 GMT  
		Size: 53.4 MB (53390698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4809c26c5fbcf46e724e97753b831c03c2021ac2def13026b528fb114d6989f`  
		Last Modified: Wed, 15 Nov 2023 02:28:19 GMT  
		Size: 28.8 MB (28814600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:69f5a6be863cb69c5e8fbf9fb8eaf91c2994ca992b4db4df61c766a3dc512c80
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (68959952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c167457a1683a82fde1556d548ac9344db2d2d3e22530763b33801be31261264`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:45:36 GMT
ADD file:b451624b6214da7e4871235da21071d55a6c21b9ed56fe301e78beebaa9c034d in / 
# Wed, 01 Nov 2023 00:45:40 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:01:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:37319c2577b55a62447a947186364b13c616c3448bd2c4aeb444733fc58dfb64`  
		Last Modified: Wed, 01 Nov 2023 00:50:43 GMT  
		Size: 48.9 MB (48900178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10e593352eeadc1fa34f624da16ec4d5ffc03e962de8e47f9fd30d101863f83`  
		Last Modified: Wed, 01 Nov 2023 02:07:56 GMT  
		Size: 20.1 MB (20059774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:trixie-scm`

```console
$ docker pull buildpack-deps@sha256:edeaaf37b0c2d2152e4472af4581152e1302658eb6f695a9e4b755089c7f6413
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
$ docker pull buildpack-deps@sha256:462e243f20451b99d0d4631d40e08f3aba91c7940a658745d7943320c2f05060
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.3 MB (141250980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d619a60defd797722d81ef2e28e8daee71fad5dc46f5b42a61ed8e4addadf451`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:23:31 GMT
ADD file:00d06a447c9580e05c2514d623a6906f35419629a74e8f29f8627b620df970f3 in / 
# Wed, 01 Nov 2023 00:23:32 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 05:08:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 05:09:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9f30dcdc5629f1d2f740d6a704db5e6f29ed782df4486ef49cdbddb30250312f`  
		Last Modified: Wed, 01 Nov 2023 00:30:07 GMT  
		Size: 49.5 MB (49486885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b00fcc62737a4287ca8fcd27724545f3a9669ead301dbede869f8af73f94159`  
		Last Modified: Wed, 15 Nov 2023 05:17:53 GMT  
		Size: 26.3 MB (26255430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ccab398df14d3fc8ad70c0ac91181d737fba7720072d703f9b4cd4776dd5a54`  
		Last Modified: Wed, 15 Nov 2023 05:18:10 GMT  
		Size: 65.5 MB (65508665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:e98e275298640ac337d66d1e8b2daff0b1fa47059063cc5cf730d09153ea11f7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.9 MB (134926302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:591879d8e8fe078a1d376f8f02273465613a192e6ae1d6f30d60bd1012d7552f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:49:55 GMT
ADD file:c8135c4f5f4b7815dc29bb93d73adb514649c5dfb72bfc1c072a7a9ae53653f1 in / 
# Wed, 01 Nov 2023 00:49:55 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 04:19:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 04:19:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:136f2fd3e12dd347dbdab54d5a79402eda3c65de7050120b6c1d86345bcc99da`  
		Last Modified: Wed, 01 Nov 2023 00:54:48 GMT  
		Size: 47.1 MB (47142117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76630daa19e4462e67c7427306ed19109a580c7c1d8e740a83a167e409d9cabc`  
		Last Modified: Wed, 15 Nov 2023 04:22:58 GMT  
		Size: 24.8 MB (24757320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20938e88d9c5a89a0f108e782b84fd782c481cd62c2b806cf84d1ec9e42be3fb`  
		Last Modified: Wed, 15 Nov 2023 04:23:17 GMT  
		Size: 63.0 MB (63026865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:75dea238cd526afe7ce7b9513ca46dbf1cc6dadc22fe16aa542aabad67481013
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129506982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:361deb5742958e94144bd2fcf2dca7450743abbd022702c2dcbb5df03bf5b48f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:00:07 GMT
ADD file:035b362840f9210e5a7bfde4a95079958d9f57f5b5a556d22b48ad6abcdf2134 in / 
# Wed, 01 Nov 2023 01:00:07 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 02:00:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 02:01:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b403287e0cd0f39bef349bb68bed383fd0582cc2ae9137aac1969a41c84e30db`  
		Last Modified: Wed, 01 Nov 2023 01:06:58 GMT  
		Size: 44.9 MB (44936197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d95ccb30a9e3ceec487ec02756f65216d24abc33ca03c71393ac6e54f4e82b2`  
		Last Modified: Wed, 15 Nov 2023 02:10:23 GMT  
		Size: 23.9 MB (23949923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a902151f0ab2df8ae45f89c290b155db85a2180a36075c89127fdbbdbccb5431`  
		Last Modified: Wed, 15 Nov 2023 02:10:46 GMT  
		Size: 60.6 MB (60620862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f4ecc23cf3593d792eccac10de6f65402681509d9c2e2121c4f5fc696291e245
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.2 MB (135236741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:511a2b90c89c51a56cd6d51c5f1fcd9b7b1901c5c794c3d3d7967fa1b226b629`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:41:27 GMT
ADD file:d0c94454bffd347b60b86607fe3aea27f4afc57648c812d80575bc9d7d71a1fc in / 
# Wed, 01 Nov 2023 00:41:28 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:11:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:11:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6bbd151733a83c3c4e1747562a07b8dc0d6b9a1a38140e050fec86a0e73e1f0e`  
		Last Modified: Wed, 01 Nov 2023 00:47:15 GMT  
		Size: 49.5 MB (49495227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aaa14e94a2e8ffb5faf3100c888245cbc9a4eaaf9d6edea6ed3aef228b6b1f1`  
		Last Modified: Wed, 01 Nov 2023 02:17:28 GMT  
		Size: 20.1 MB (20141380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94bd9c6d088804a732d5962844e6cf83a29d1b30528f3b5ec7ff6e67e742a132`  
		Last Modified: Wed, 01 Nov 2023 02:17:45 GMT  
		Size: 65.6 MB (65600134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:369a5742bedd7592b08d2ba7e7c53deedacf83dcf67f1610298c4d302e96504f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.6 MB (138639574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1715791f3ccb5695b0269a0a7a09b417f3354ebcb9c4022a0a20136e58c7fb82`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:41:31 GMT
ADD file:99d6a1f205a46734ffc61c992b3c9029eb83aceaab7b9777a94552ae226a209f in / 
# Wed, 01 Nov 2023 00:41:32 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 13:53:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:53:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7778791eeb3e7444e84c2d682795ca0f756d9e1d87e924e2739660a8ed9134ad`  
		Last Modified: Wed, 01 Nov 2023 00:48:34 GMT  
		Size: 50.5 MB (50466373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d80422353ec8a9a13b994d878c456b9feb2c3711191dccf08d7957979acd368`  
		Last Modified: Wed, 01 Nov 2023 14:01:24 GMT  
		Size: 20.9 MB (20909176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be46fd0a3e04a3c48fa349f6b3baa84f402e8ec4ed841491191fa80991567c8`  
		Last Modified: Wed, 01 Nov 2023 14:01:50 GMT  
		Size: 67.3 MB (67264025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:018e682c1fa14ae9daeebeb7f90363910e3dbeb3a6c031b7d8c7079e35211784
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.7 MB (139677461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0dc06258e7ec131a3593eb9cdd566566727a64176af57e747bbbca3bee96d6d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:15:37 GMT
ADD file:fcddbc3f0c0456097a49c255590801b884727d47f9ceac6afe8463117d63a70e in / 
# Wed, 01 Nov 2023 01:15:43 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 02:09:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 02:11:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:434392845279581746e8cecd769b536845c39fb214d29012afa566896853392c`  
		Last Modified: Wed, 01 Nov 2023 01:26:47 GMT  
		Size: 49.3 MB (49278627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18ede9f97c171cbb8a558528bdc51f6a5dd9e805644cae6cc9891cb76258eb9d`  
		Last Modified: Wed, 15 Nov 2023 02:19:46 GMT  
		Size: 26.1 MB (26073841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7717e39a49a836fc0908b857bdee9522fd3c967c00400172afac7d1498f8b2`  
		Last Modified: Wed, 15 Nov 2023 02:20:37 GMT  
		Size: 64.3 MB (64324993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:6d6dbff7260cc7e234001f7f9ed2e110a4bb9e164d381614d3e257f52b4d43d6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.1 MB (153139692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f24f72538a7400a19c9b0300cb9383805393e690e5c2f5aecade97749ca15e8`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:24:06 GMT
ADD file:d45c9f62cb1fd4297a5ee2026bc6abb62f25a456f3a44a8ab6d115eb1d59ce39 in / 
# Wed, 01 Nov 2023 00:24:09 GMT
CMD ["bash"]
# Wed, 15 Nov 2023 02:17:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 15 Nov 2023 02:17:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a86485f1d263f9f0955a85f3d3707fcc2bc7bb4d598df11d02b766bd3da90ad3`  
		Last Modified: Wed, 01 Nov 2023 00:29:48 GMT  
		Size: 53.4 MB (53390698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4809c26c5fbcf46e724e97753b831c03c2021ac2def13026b528fb114d6989f`  
		Last Modified: Wed, 15 Nov 2023 02:28:19 GMT  
		Size: 28.8 MB (28814600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01dd59a7c5494927ca7f0a3267579f63aea083a036ffa58f2bdba9773f3f058`  
		Last Modified: Wed, 15 Nov 2023 02:28:39 GMT  
		Size: 70.9 MB (70934394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:3244855b69745d2237dff0ee5e5caff6d4f2a6a66ec03c531ea9f8ef87b75e04
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.4 MB (135430206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70939a2063f13adf3e74bb8cf060f2ddead45dbf2bcf0890fa8dc94a65c68026`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:45:36 GMT
ADD file:b451624b6214da7e4871235da21071d55a6c21b9ed56fe301e78beebaa9c034d in / 
# Wed, 01 Nov 2023 00:45:40 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:01:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:01:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:37319c2577b55a62447a947186364b13c616c3448bd2c4aeb444733fc58dfb64`  
		Last Modified: Wed, 01 Nov 2023 00:50:43 GMT  
		Size: 48.9 MB (48900178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10e593352eeadc1fa34f624da16ec4d5ffc03e962de8e47f9fd30d101863f83`  
		Last Modified: Wed, 01 Nov 2023 02:07:56 GMT  
		Size: 20.1 MB (20059774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b780353fcf3645d3b82950a80a107c5134cb03e7e2514a5a84924d066df64f80`  
		Last Modified: Wed, 01 Nov 2023 02:08:13 GMT  
		Size: 66.5 MB (66470254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:unstable`

```console
$ docker pull buildpack-deps@sha256:f84df4a563092acda4fed5202298f0b6bfa78cb77cb7cbfd9d6ce293d83e8bd5
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

### `buildpack-deps:unstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:e7cc569fa46f03c3b37e2eb8a2e07f21c7e5b0e30cf67b785ebca55c8338b12e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.6 MB (351621495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e98f8ea8863e64d24c9f40759a43604de07e2ea088eee61d4a1f1f536226f449`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:49:10 GMT
ADD file:3dfec265d80292cf14629bdbd49822be7a5672ab8299d43e9ec734f6e032c8df in / 
# Wed, 01 Nov 2023 00:49:10 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:59:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 03:00:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 03:02:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0609920749c8743a3627a0a7a377598014123518f5e0ed7f1443c78c8c9f3446`  
		Last Modified: Wed, 01 Nov 2023 00:53:10 GMT  
		Size: 47.2 MB (47192458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3b7ab88084f4d09eb30fe75dbc159cd99b0692cea6232d2f457c292a62968c`  
		Last Modified: Wed, 01 Nov 2023 03:07:10 GMT  
		Size: 23.0 MB (23016482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3ff5e12103a446acf43b661291fc30a67ca5851b7c1f67906ac39a5a609ef1c`  
		Last Modified: Wed, 01 Nov 2023 03:07:30 GMT  
		Size: 63.0 MB (63010355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cefdf6db1915fab2d33c8090895aeecc671cb90ef4527f9b4ca1ae99fd45870d`  
		Last Modified: Wed, 01 Nov 2023 03:08:09 GMT  
		Size: 218.4 MB (218402200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:0b69a293dbe1e851613427c41b98e1ac973abf0ffd16ae00e87e83287cc0114a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.3 MB (332315093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bc1f83378e6ca85f13dee6672ad2ab008d5efd04b8307d9899c3b0cf1b87ff1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:59:14 GMT
ADD file:a72fe3de4b178dd8b7c48a1dc98d4c14520570e5edb66049dfe2cd6bb0a5dd6c in / 
# Wed, 01 Nov 2023 00:59:15 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:36:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:36:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:38:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f6e9a66eb905933433a5a2a8c16e480468f3731f107d5854bac12ef9a79bc271`  
		Last Modified: Wed, 01 Nov 2023 01:05:19 GMT  
		Size: 45.0 MB (44981409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c61548fabf75545be26d57a05800e5dbcd765a1c5c804a7671c92c59e15834d8`  
		Last Modified: Wed, 01 Nov 2023 02:44:58 GMT  
		Size: 22.2 MB (22234767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa95d6d6902734ac1af894edaf67096b114b4935d12a40bf35b44bca0f33e21`  
		Last Modified: Wed, 01 Nov 2023 02:45:16 GMT  
		Size: 60.6 MB (60610186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8828360bbf372d14fe88491ee679919df8f916259a40637ce6044d862916ccb`  
		Last Modified: Wed, 01 Nov 2023 02:45:51 GMT  
		Size: 204.5 MB (204488731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:4e0722b3b91c70dc433459035eb7504e1e3e4ace8334cf061672453cac0548b3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **374.4 MB (374367609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:703487ba0762e6be168e40b4bb8cd5297bd509bb84e88e953bdbc0cba3660726`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:40:45 GMT
ADD file:1a4ef85bba464538c4f87a65a055d954fc8edc51f26efd06b43d8ae9f7e54f7a in / 
# Wed, 01 Nov 2023 00:40:46 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:09:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:09:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:10:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ba6956ade110f0fe56bbad19a8d10b1eb0ae1b1006ccba5fadff0026a00dbc20`  
		Last Modified: Wed, 01 Nov 2023 00:45:46 GMT  
		Size: 49.6 MB (49552835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516c292c0ab5612a524438779924b5cc187f530a208c71056c8b9994656ef043`  
		Last Modified: Wed, 01 Nov 2023 02:16:27 GMT  
		Size: 23.9 MB (23916545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8977dd4a34d5416619317940446894bcaf8bc0c5f832e562683f4aa703db7f`  
		Last Modified: Wed, 01 Nov 2023 02:16:44 GMT  
		Size: 65.6 MB (65605231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f03a9258674c4a8e3c26a670786d3af44115d865542a8ca88ddb82d3056bee`  
		Last Modified: Wed, 01 Nov 2023 02:17:17 GMT  
		Size: 235.3 MB (235292998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:ae76f8ad80b82b6fdffaa4931dc6daa3ca2c972c3b5b05f2cb4991fb4720e31c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **388.7 MB (388669349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96527636c4addf379e53b4ec348c7fe3db44767d72e6489bb2c45db3f96f34b2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:40:31 GMT
ADD file:0aa90abbd80c68d937903de7ac8fdcce0f516fdd70f080b677af1e2322c000b9 in / 
# Wed, 01 Nov 2023 00:40:32 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 13:50:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:51:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:53:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:96660bac4658b1bffb27e96ac8ecc86753a1844f042ede32c4f1faef702dc202`  
		Last Modified: Wed, 01 Nov 2023 00:46:42 GMT  
		Size: 50.5 MB (50516486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7af088639fa61079db294f16f91145938a488365f2aec8cef7a85da80c4b13b`  
		Last Modified: Wed, 01 Nov 2023 13:59:54 GMT  
		Size: 25.2 MB (25185750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34a1138df818473932216f10a656452bbeead89efc81870811003208908e138`  
		Last Modified: Wed, 01 Nov 2023 14:00:17 GMT  
		Size: 67.3 MB (67267247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4105a9010ad6b6eb2295fe9bd43b392d6a4b2314d5c52c4020f7645fcd5b3c26`  
		Last Modified: Wed, 01 Nov 2023 14:01:10 GMT  
		Size: 245.7 MB (245699866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:41945b8dac854a10d2da3ff6944d8b39a59fb2e080101c9cb5583a0bd726fccd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **359.8 MB (359784858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2973da056cdad1602f11a8f10c07c22423951a38bd52b7024eae7189a700bbad`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:12:08 GMT
ADD file:e27a157c42d1aedcb0f6cf695f1f5c31d442488e049826c940509e2288537427 in / 
# Wed, 01 Nov 2023 01:12:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 21:35:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 21:36:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 21:43:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0eacf4d958160d2729e1bb31fbb12227afa7536ce6304928b13c2c65d297f9b9`  
		Last Modified: Wed, 01 Nov 2023 01:23:11 GMT  
		Size: 49.3 MB (49326735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76fea98d048b05ee3313ca45517a641b11637c7f8dc3ec543480fe6111a66fc0`  
		Last Modified: Wed, 01 Nov 2023 22:00:34 GMT  
		Size: 23.9 MB (23910243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde7d59b79a44cf2fd6509592cd5ffa2ac26dd4a37fb70dbe72408010c4a2926`  
		Last Modified: Wed, 01 Nov 2023 22:01:27 GMT  
		Size: 64.3 MB (64323488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:812e226799f37d4cc00732c97925157577a5924147f47974ea2e38bf5b013bf2`  
		Last Modified: Wed, 01 Nov 2023 22:03:55 GMT  
		Size: 222.2 MB (222224392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:a294a5485974dcc719539acaa65612e53c0633d687c14a93eb2fffc89c32c068
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **395.9 MB (395889008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:053444952bbb99335c24da95e60652c8bf13fdf4d34ca8258e433d137e2187b0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:22:46 GMT
ADD file:b4e182cbec02f1d3bb7c8ff0ef09924ac255ba6717bdd73f24d0a6114ff305d6 in / 
# Wed, 01 Nov 2023 00:22:49 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:31:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:32:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:35:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:46cca77d78176c861335b7b91e20d7b4cb2b3a75a124c300124de5818b724a9d`  
		Last Modified: Wed, 01 Nov 2023 00:27:59 GMT  
		Size: 53.4 MB (53438164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c27d7acaf849316ba11ccd36c024abe28c48180ca4ed48c1d645cdbac13d42`  
		Last Modified: Wed, 01 Nov 2023 01:42:56 GMT  
		Size: 26.0 MB (26000762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1f87f5498621b44bb593666a49a2167487d185ef2ba48d24ee657724f9e1b8`  
		Last Modified: Wed, 01 Nov 2023 01:43:17 GMT  
		Size: 70.9 MB (70933174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293d32682820b51e6038052ac32c5615a7e362a951c538e2e7dfcd2260f9bf08`  
		Last Modified: Wed, 01 Nov 2023 01:44:03 GMT  
		Size: 245.5 MB (245516908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:8cdef13f992928b7ced89bd24774f889b46a4ba3c167a501a32629523efafecb
```

-	Docker Version: 20.10.25
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **422.5 MB (422517112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d6a14901feb9be459b29b2ec05a91f16169520c614043d74824ef29f5ef68fc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:10:39 GMT
ADD file:10aac34e5379cbca42071631c10447895ece01063babea5769d7a1ca12c1d5e1 in / 
# Wed, 01 Nov 2023 01:10:41 GMT
CMD ["bash"]
# Fri, 10 Nov 2023 15:09:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 10 Nov 2023 15:11:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 10 Nov 2023 15:18:43 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8b987d803641183eb947c3e5f17a8a822be136b9081a3e13a881ea93c5b5c153`  
		Last Modified: Wed, 01 Nov 2023 01:13:28 GMT  
		Size: 47.9 MB (47903676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e686018657ba2f600a983c566c04aa87a7d470e15735c7687c3f08ad9fc14c6`  
		Last Modified: Fri, 10 Nov 2023 15:19:24 GMT  
		Size: 25.7 MB (25689738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e367241f870c7b27facfdeed51bb1705e06e838663a27ed4411063a890b5d9`  
		Last Modified: Fri, 10 Nov 2023 15:20:39 GMT  
		Size: 64.7 MB (64712965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7608d7ee7a6e227d7e1ffd0c22faa80adf546d9105155ee8e590b239746a8e`  
		Last Modified: Fri, 10 Nov 2023 15:26:16 GMT  
		Size: 284.2 MB (284210733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:94c1320e61a65661393d39cd613dad56ade7b9114794ea363c35cd1d98bf1472
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **357.1 MB (357129350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd53476e97fafeffd02c74a4b92a8131082486dfaf6e18124bce5faa8fe8ed79`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:44:04 GMT
ADD file:e94f75ffd7aa648bb85fefcceb02afa58747273f05e89c473c1ad438c3ba2345 in / 
# Wed, 01 Nov 2023 00:44:07 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:59:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:59:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:00:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:43e2d693d4cc2a3e58c2344ef771699434d5f0e6ffb98ac8bdb822ee0e2534fa`  
		Last Modified: Wed, 01 Nov 2023 00:49:25 GMT  
		Size: 49.0 MB (48966976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17216a40a3f2f28f99307df60faffa863e423de83464990e34dd5854b1206c45`  
		Last Modified: Wed, 01 Nov 2023 02:07:00 GMT  
		Size: 24.6 MB (24596949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa15755375f48461c5f3dcfc8b172b68b06d99c8b37bacff592046619c269ff5`  
		Last Modified: Wed, 01 Nov 2023 02:07:15 GMT  
		Size: 66.5 MB (66478150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee715cf843b2c30de31308613798cb1286cc46aace75a30b5454885808889c6a`  
		Last Modified: Wed, 01 Nov 2023 02:07:47 GMT  
		Size: 217.1 MB (217087275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:unstable-curl`

```console
$ docker pull buildpack-deps@sha256:77c7980908342e34e20c6dded2d582be454afc3b1cacb6b3f51afcdafc207e75
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
$ docker pull buildpack-deps@sha256:55d3c9a086b1f3e2bf2efc43a3facd9259debb301bc36d744d399b9f9183baab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.9 MB (73888718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ca5ff02ac501d48c546df140a835f2ebdb2306a1a564dd635fc72f385dd9659`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:22:27 GMT
ADD file:69815228666696b3cd3b2799492e3d9cdf4f513ccca5c1cc9282f6c569cc8730 in / 
# Wed, 01 Nov 2023 00:22:28 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 00:57:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
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

### `buildpack-deps:unstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:8fd71e79ed7adb4eabd5ab187c04681bd8d7225ad23f383b19e2983aafe7dca9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70208940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d62ceb7c735018d913dc495afa525a353cb6e5196e0df330873dac97ea2527f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:49:10 GMT
ADD file:3dfec265d80292cf14629bdbd49822be7a5672ab8299d43e9ec734f6e032c8df in / 
# Wed, 01 Nov 2023 00:49:10 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:59:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0609920749c8743a3627a0a7a377598014123518f5e0ed7f1443c78c8c9f3446`  
		Last Modified: Wed, 01 Nov 2023 00:53:10 GMT  
		Size: 47.2 MB (47192458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3b7ab88084f4d09eb30fe75dbc159cd99b0692cea6232d2f457c292a62968c`  
		Last Modified: Wed, 01 Nov 2023 03:07:10 GMT  
		Size: 23.0 MB (23016482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:51146f13fdb6437822863cfb091ce22dd810970f7bf2062d9a989c5b98b20ad3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67216176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:441627c1997be627df062cc68f9e0305629e418cd85ef184060f05d45e2ca94a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:59:14 GMT
ADD file:a72fe3de4b178dd8b7c48a1dc98d4c14520570e5edb66049dfe2cd6bb0a5dd6c in / 
# Wed, 01 Nov 2023 00:59:15 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:36:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f6e9a66eb905933433a5a2a8c16e480468f3731f107d5854bac12ef9a79bc271`  
		Last Modified: Wed, 01 Nov 2023 01:05:19 GMT  
		Size: 45.0 MB (44981409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c61548fabf75545be26d57a05800e5dbcd765a1c5c804a7671c92c59e15834d8`  
		Last Modified: Wed, 01 Nov 2023 02:44:58 GMT  
		Size: 22.2 MB (22234767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:37eb53a80fd102fcb5f14a4d0dc9bd7732ec1c734a422e4b427b175555c575a5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.5 MB (73469380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0be9b3ee789a657aea7026023fad3bfad1ddd7a5e725b324dd61f03508c0130d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:40:45 GMT
ADD file:1a4ef85bba464538c4f87a65a055d954fc8edc51f26efd06b43d8ae9f7e54f7a in / 
# Wed, 01 Nov 2023 00:40:46 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:09:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ba6956ade110f0fe56bbad19a8d10b1eb0ae1b1006ccba5fadff0026a00dbc20`  
		Last Modified: Wed, 01 Nov 2023 00:45:46 GMT  
		Size: 49.6 MB (49552835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516c292c0ab5612a524438779924b5cc187f530a208c71056c8b9994656ef043`  
		Last Modified: Wed, 01 Nov 2023 02:16:27 GMT  
		Size: 23.9 MB (23916545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8988d06749683ea585cf137051dfe9710e79a4dd694e684d3de84c6bf3757d32
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75702236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:830e36b2a276fddf3fa83594c87499d590059eb10e73ca22fcc5a827bbbda7c4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:40:31 GMT
ADD file:0aa90abbd80c68d937903de7ac8fdcce0f516fdd70f080b677af1e2322c000b9 in / 
# Wed, 01 Nov 2023 00:40:32 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 13:50:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:96660bac4658b1bffb27e96ac8ecc86753a1844f042ede32c4f1faef702dc202`  
		Last Modified: Wed, 01 Nov 2023 00:46:42 GMT  
		Size: 50.5 MB (50516486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7af088639fa61079db294f16f91145938a488365f2aec8cef7a85da80c4b13b`  
		Last Modified: Wed, 01 Nov 2023 13:59:54 GMT  
		Size: 25.2 MB (25185750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:3d072782b869915c68ce21a8a78370274e3aad0379c863c87bed0513c371bf28
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73236978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48d581d8a17daaf6df47819c5605bf4a8542057b4a50efa28345f4f2918775db`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:12:08 GMT
ADD file:e27a157c42d1aedcb0f6cf695f1f5c31d442488e049826c940509e2288537427 in / 
# Wed, 01 Nov 2023 01:12:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 21:35:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0eacf4d958160d2729e1bb31fbb12227afa7536ce6304928b13c2c65d297f9b9`  
		Last Modified: Wed, 01 Nov 2023 01:23:11 GMT  
		Size: 49.3 MB (49326735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76fea98d048b05ee3313ca45517a641b11637c7f8dc3ec543480fe6111a66fc0`  
		Last Modified: Wed, 01 Nov 2023 22:00:34 GMT  
		Size: 23.9 MB (23910243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:e3fe6632a18f418e4435cc7a8063378cec3d6e7e86eda522d299f55d99caeb06
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.4 MB (79438926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f3939720778f56545dbb5f838729141ef56732c086b66a0537faf6460e0937f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:22:46 GMT
ADD file:b4e182cbec02f1d3bb7c8ff0ef09924ac255ba6717bdd73f24d0a6114ff305d6 in / 
# Wed, 01 Nov 2023 00:22:49 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:31:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:46cca77d78176c861335b7b91e20d7b4cb2b3a75a124c300124de5818b724a9d`  
		Last Modified: Wed, 01 Nov 2023 00:27:59 GMT  
		Size: 53.4 MB (53438164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c27d7acaf849316ba11ccd36c024abe28c48180ca4ed48c1d645cdbac13d42`  
		Last Modified: Wed, 01 Nov 2023 01:42:56 GMT  
		Size: 26.0 MB (26000762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:7502e4d219b556bf0e1c723558e81fc25bec41051d62b6d01fe6ee8594649131
```

-	Docker Version: 20.10.25
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73593414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7fed54f446cc8c45b1b49a470ff94f7e04623b8690749725aab0ecf7751eb268`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:10:39 GMT
ADD file:10aac34e5379cbca42071631c10447895ece01063babea5769d7a1ca12c1d5e1 in / 
# Wed, 01 Nov 2023 01:10:41 GMT
CMD ["bash"]
# Fri, 10 Nov 2023 15:09:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8b987d803641183eb947c3e5f17a8a822be136b9081a3e13a881ea93c5b5c153`  
		Last Modified: Wed, 01 Nov 2023 01:13:28 GMT  
		Size: 47.9 MB (47903676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e686018657ba2f600a983c566c04aa87a7d470e15735c7687c3f08ad9fc14c6`  
		Last Modified: Fri, 10 Nov 2023 15:19:24 GMT  
		Size: 25.7 MB (25689738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:c4b64ed3c6f7849da4bf232ee9b0346c8375234ae05e858fdaab19159c92be3b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73563925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fb6298a353936cc00a02214b0172e7ebcb8439494257afc18435c9ae46f6ac3`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:44:04 GMT
ADD file:e94f75ffd7aa648bb85fefcceb02afa58747273f05e89c473c1ad438c3ba2345 in / 
# Wed, 01 Nov 2023 00:44:07 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:59:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:43e2d693d4cc2a3e58c2344ef771699434d5f0e6ffb98ac8bdb822ee0e2534fa`  
		Last Modified: Wed, 01 Nov 2023 00:49:25 GMT  
		Size: 49.0 MB (48966976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17216a40a3f2f28f99307df60faffa863e423de83464990e34dd5854b1206c45`  
		Last Modified: Wed, 01 Nov 2023 02:07:00 GMT  
		Size: 24.6 MB (24596949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:unstable-scm`

```console
$ docker pull buildpack-deps@sha256:7b4a1e2323631a5a20efc067593b78128e3cc6c7793ca6d8029761e4a5971ff5
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
$ docker pull buildpack-deps@sha256:69b4c504c9caa677158b04a5dffa59425c7649f735a7b8728d6537f55e5bbf1b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.4 MB (139405504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ea95fd684a079be0c5deeb96861c07b4992a71e7818a9c7960f6a1baee07c8f`
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

### `buildpack-deps:unstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:9417cb6ff8564c4d3bf1b82efb889976197dc0cb69f9ef179d844ff4c5a47a07
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.2 MB (133219295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:791053f347823ad45507927ca12fc46992f6485bb6ded865460b387df1861d71`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:49:10 GMT
ADD file:3dfec265d80292cf14629bdbd49822be7a5672ab8299d43e9ec734f6e032c8df in / 
# Wed, 01 Nov 2023 00:49:10 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:59:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 03:00:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0609920749c8743a3627a0a7a377598014123518f5e0ed7f1443c78c8c9f3446`  
		Last Modified: Wed, 01 Nov 2023 00:53:10 GMT  
		Size: 47.2 MB (47192458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba3b7ab88084f4d09eb30fe75dbc159cd99b0692cea6232d2f457c292a62968c`  
		Last Modified: Wed, 01 Nov 2023 03:07:10 GMT  
		Size: 23.0 MB (23016482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3ff5e12103a446acf43b661291fc30a67ca5851b7c1f67906ac39a5a609ef1c`  
		Last Modified: Wed, 01 Nov 2023 03:07:30 GMT  
		Size: 63.0 MB (63010355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:dd781c833a3b0edcfcd2d86a091e60c74feac13e09a04d42ecf30ed1992d57c3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127826362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82080f96e7a0b68c7bc49369001f13514e2d0bb7da42e22f391c832020ee4beb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:59:14 GMT
ADD file:a72fe3de4b178dd8b7c48a1dc98d4c14520570e5edb66049dfe2cd6bb0a5dd6c in / 
# Wed, 01 Nov 2023 00:59:15 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:36:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:36:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f6e9a66eb905933433a5a2a8c16e480468f3731f107d5854bac12ef9a79bc271`  
		Last Modified: Wed, 01 Nov 2023 01:05:19 GMT  
		Size: 45.0 MB (44981409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c61548fabf75545be26d57a05800e5dbcd765a1c5c804a7671c92c59e15834d8`  
		Last Modified: Wed, 01 Nov 2023 02:44:58 GMT  
		Size: 22.2 MB (22234767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa95d6d6902734ac1af894edaf67096b114b4935d12a40bf35b44bca0f33e21`  
		Last Modified: Wed, 01 Nov 2023 02:45:16 GMT  
		Size: 60.6 MB (60610186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:24a9674f7ee955af54b2ff9dff74e3a3a5ab908c092ef87046b36185bba90552
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.1 MB (139074611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49432ff4faca7e8f8e7e1c0674996ca4a6b2a93bdec8b6cf4059353c81e1a6eb`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:40:45 GMT
ADD file:1a4ef85bba464538c4f87a65a055d954fc8edc51f26efd06b43d8ae9f7e54f7a in / 
# Wed, 01 Nov 2023 00:40:46 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:09:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:09:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ba6956ade110f0fe56bbad19a8d10b1eb0ae1b1006ccba5fadff0026a00dbc20`  
		Last Modified: Wed, 01 Nov 2023 00:45:46 GMT  
		Size: 49.6 MB (49552835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516c292c0ab5612a524438779924b5cc187f530a208c71056c8b9994656ef043`  
		Last Modified: Wed, 01 Nov 2023 02:16:27 GMT  
		Size: 23.9 MB (23916545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8977dd4a34d5416619317940446894bcaf8bc0c5f832e562683f4aa703db7f`  
		Last Modified: Wed, 01 Nov 2023 02:16:44 GMT  
		Size: 65.6 MB (65605231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:bf9e365b381337f4d6b2f5562e4a5c66f62d51e107a697e2abc16c6cf3807722
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.0 MB (142969483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:890f7be8650dfbec3174b0c555ee6f84c9085c83f218e591ccd4bcd9822ca9fd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:40:31 GMT
ADD file:0aa90abbd80c68d937903de7ac8fdcce0f516fdd70f080b677af1e2322c000b9 in / 
# Wed, 01 Nov 2023 00:40:32 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 13:50:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:51:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:96660bac4658b1bffb27e96ac8ecc86753a1844f042ede32c4f1faef702dc202`  
		Last Modified: Wed, 01 Nov 2023 00:46:42 GMT  
		Size: 50.5 MB (50516486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7af088639fa61079db294f16f91145938a488365f2aec8cef7a85da80c4b13b`  
		Last Modified: Wed, 01 Nov 2023 13:59:54 GMT  
		Size: 25.2 MB (25185750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34a1138df818473932216f10a656452bbeead89efc81870811003208908e138`  
		Last Modified: Wed, 01 Nov 2023 14:00:17 GMT  
		Size: 67.3 MB (67267247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:be68bbc454236b68329461f9d169e194956bde9a85d831f12f67ffc86823332b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.6 MB (137560466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8009d8ed04a6125b5b9fefa3fad72e3a2ffe0dc6f0abd9e503ca667526d713c5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:12:08 GMT
ADD file:e27a157c42d1aedcb0f6cf695f1f5c31d442488e049826c940509e2288537427 in / 
# Wed, 01 Nov 2023 01:12:12 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 21:35:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 21:36:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0eacf4d958160d2729e1bb31fbb12227afa7536ce6304928b13c2c65d297f9b9`  
		Last Modified: Wed, 01 Nov 2023 01:23:11 GMT  
		Size: 49.3 MB (49326735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76fea98d048b05ee3313ca45517a641b11637c7f8dc3ec543480fe6111a66fc0`  
		Last Modified: Wed, 01 Nov 2023 22:00:34 GMT  
		Size: 23.9 MB (23910243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde7d59b79a44cf2fd6509592cd5ffa2ac26dd4a37fb70dbe72408010c4a2926`  
		Last Modified: Wed, 01 Nov 2023 22:01:27 GMT  
		Size: 64.3 MB (64323488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:353b2a9b54d029503ae0b036b97d823535850f152a54820f9faeb5adba83eb89
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.4 MB (150372100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b8e3c9ad7f10aec351582b84c48d9a4a2a4b8b4496b3fc285248982f5238995`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:22:46 GMT
ADD file:b4e182cbec02f1d3bb7c8ff0ef09924ac255ba6717bdd73f24d0a6114ff305d6 in / 
# Wed, 01 Nov 2023 00:22:49 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:31:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:32:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:46cca77d78176c861335b7b91e20d7b4cb2b3a75a124c300124de5818b724a9d`  
		Last Modified: Wed, 01 Nov 2023 00:27:59 GMT  
		Size: 53.4 MB (53438164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18c27d7acaf849316ba11ccd36c024abe28c48180ca4ed48c1d645cdbac13d42`  
		Last Modified: Wed, 01 Nov 2023 01:42:56 GMT  
		Size: 26.0 MB (26000762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1f87f5498621b44bb593666a49a2167487d185ef2ba48d24ee657724f9e1b8`  
		Last Modified: Wed, 01 Nov 2023 01:43:17 GMT  
		Size: 70.9 MB (70933174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:d98851f479f5b91644eea439930f9a94b4da22e3c4d133aed85216a103b3e873
```

-	Docker Version: 20.10.25
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.3 MB (138306379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a556e968fe99b77f67556941b078d49fa94ba4ac7ebab95aa19b50fd184956fd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 01:10:39 GMT
ADD file:10aac34e5379cbca42071631c10447895ece01063babea5769d7a1ca12c1d5e1 in / 
# Wed, 01 Nov 2023 01:10:41 GMT
CMD ["bash"]
# Fri, 10 Nov 2023 15:09:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 10 Nov 2023 15:11:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8b987d803641183eb947c3e5f17a8a822be136b9081a3e13a881ea93c5b5c153`  
		Last Modified: Wed, 01 Nov 2023 01:13:28 GMT  
		Size: 47.9 MB (47903676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e686018657ba2f600a983c566c04aa87a7d470e15735c7687c3f08ad9fc14c6`  
		Last Modified: Fri, 10 Nov 2023 15:19:24 GMT  
		Size: 25.7 MB (25689738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e367241f870c7b27facfdeed51bb1705e06e838663a27ed4411063a890b5d9`  
		Last Modified: Fri, 10 Nov 2023 15:20:39 GMT  
		Size: 64.7 MB (64712965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:0c3580029357b03dab5202367b9675aa78ae0db89b391735b34327fa0aad12e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.0 MB (140042075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b4c6469d28f8ab0416e1b296a12c5545babdafd6352d9d73e5fab9096a5c5d5`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 01 Nov 2023 00:44:04 GMT
ADD file:e94f75ffd7aa648bb85fefcceb02afa58747273f05e89c473c1ad438c3ba2345 in / 
# Wed, 01 Nov 2023 00:44:07 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 01:59:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 01:59:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:43e2d693d4cc2a3e58c2344ef771699434d5f0e6ffb98ac8bdb822ee0e2534fa`  
		Last Modified: Wed, 01 Nov 2023 00:49:25 GMT  
		Size: 49.0 MB (48966976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17216a40a3f2f28f99307df60faffa863e423de83464990e34dd5854b1206c45`  
		Last Modified: Wed, 01 Nov 2023 02:07:00 GMT  
		Size: 24.6 MB (24596949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa15755375f48461c5f3dcfc8b172b68b06d99c8b37bacff592046619c269ff5`  
		Last Modified: Wed, 01 Nov 2023 02:07:15 GMT  
		Size: 66.5 MB (66478150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
